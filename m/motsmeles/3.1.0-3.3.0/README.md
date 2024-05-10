# Comparing `tmp/motsmeles-3.1.0.tar.gz` & `tmp/motsmeles-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motsmeles-3.1.0.tar", max compression
+gzip compressed data, was "motsmeles-3.3.0.tar", max compression
```

## Comparing `motsmeles-3.1.0.tar` & `motsmeles-3.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      748 2024-04-20 11:07:18.603141 motsmeles-3.1.0/README.md
--rw-r--r--   0        0        0     6325 2024-04-20 11:18:27.780754 motsmeles-3.1.0/motsmeles.py
--rw-r--r--   0        0        0      402 2024-04-20 11:20:47.688543 motsmeles-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 motsmeles-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      863 2024-05-10 14:09:25.259681 motsmeles-3.3.0/README.md
+-rw-r--r--   0        0        0     8235 2024-05-10 14:09:25.260231 motsmeles-3.3.0/motsmeles.py
+-rw-r--r--   0        0        0      402 2024-05-10 14:17:45.060221 motsmeles-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 motsmeles-3.3.0/PKG-INFO
```

### Comparing `motsmeles-3.1.0/motsmeles.py` & `motsmeles-3.3.0/motsmeles.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,217 @@
 
-import numpy
+
+import numpy as np
 import pandas as pd
 import random
 import sys
 import builtins
 
 
 ALPHABET="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 debug_mode = hasattr(sys, 'gettrace') and sys.gettrace()
 # 1TODO remplacer sensPossible par allow_inverse, allow_diagonal
 class GenerateError(Exception):
     pass
 DEFAULT_WIDTH=10
 DEFAULT_HEIGHT=10
-def generate(
-    words,
-    width=DEFAULT_WIDTH,
-    height=DEFAULT_HEIGHT,
-    #sensPossible={"b","d","h","g","bg","bd","hd","hg"}
-    no_diagonal=False,
-    no_reverse=False,
-    ):
-
-    possible_directions={"d","r","u","l","dl","dr","ur","ul"}
-    """
-    d - down
-    r - right
-    u - up
-    l - left
-    dl - down-left
-    dr - down-right
-    ur - up-right
-    ul - up-left
-    """
-    if no_diagonal:
-        possible_directions -= {"dl","dr","ur","ul"}
-    if no_reverse:
-        possible_directions = {direction for direction in possible_directions if "l" not in direction and "u" not in direction}
+DIRECTIONS=((0,1),(1,1),(1,0),(1,-1),(0,-1),(-1,-1),(-1,0),(-1,1))
+class Game:
+    def __init__(self,grid,words=None):
+        if isinstance(grid,str):
+            grid=grid.strip().split("\n")
+            if not words:
+                grid,words=grid[:-1],grid[-1]
+            grid=np.array([list(line) for line in grid],dtype="<U1")
+        assert isinstance(grid,np.ndarray)
+        self.grid=grid
         
-    grid = numpy.empty((height, width), dtype=str)
-    answers = pd.DataFrame(columns=['word', 'direction', 'x1', 'y1','x2', 'y2'])
-    
-    def _generate():
-        # 1. Placer les mots
-        for word in words:
-            #Vérification du mot
-            word = word.upper()
-            for letter in word:
-                assert letter in ALPHABET,f"Mot invalid: {word}"
-            dim = min(width, height)
-            assert len(word) <= dim, f"Mot trop long: {word}"
+        if isinstance(words,str):
+            words=words.split(" ")
+        words=[word.upper() for word in words]
+        self.words=words
+        
+    @classmethod
+    def generate(
+        cls,
+        words,
+        width=DEFAULT_WIDTH,
+        height=DEFAULT_HEIGHT,
+        #sensPossible={"b","d","h","g","bg","bd","hd","hg"}
+        no_diagonal=False,
+        no_reverse=False,
+        ):
+
+
+        """
+        d - down
+        r - right
+        u - up
+        l - left
+        dl - down-left
+        dr - down-right
+        ur - up-right
+        ul - up-left
+        """
+        possible_directions = DIRECTIONS
+        if no_diagonal:
+            possible_directions = [d for d in possible_directions if 0 in d]
+        if no_reverse:
+            possible_directions = [d for d in possible_directions if -1 not in d]
             
-            #choix de rangey, rangex, addy, addx
-            direction = random.choice(tuple(possible_directions))
-            if "d" in direction:
-
-                rangey=range((height-len(word))+1)
-                addy=1
-            elif "u" in direction:
-                rangey=range(len(word)-1,height)
-                addy=-1
-            else:
-                rangey=range(height)
-                addy=0
-            if "r" in direction:
-                rangex=range((width-len(word))+1)
-                addx=1
-            elif "l" in direction:
-                rangex=range(len(word)-1,width)
-                addx=-1
-            else:
-                rangex=range(width)
-                addx=0
-
-            choixcoordonnees=[]
-            for y1 in rangey:
-
-                for x1 in rangex:
-
-                    x2,y2=x1,y1 #create copy of x,y
-                    Break=False
-                    for letter in word:
-
-                        #Verify if it's a good emplacement mean: verify if it's blank OR filled with the right letter
-                        if grid[y2,x2]!="":
-                            if grid[y2,x2]!=letter:
-                                break
-                        x2+=addx
-                        y2+=addy
-                    else:               
-                        choixcoordonnees.append((y1,x1))
-            if not choixcoordonnees: 
+
+        
+        def _generate():
+            grid = np.empty((height, width), dtype=str)
+            answers = pd.DataFrame(index=words, columns=['direction', 'x1', 'y1','x2', 'y2'])
+            # 1. Placer les mots
+            for word in words:
+                #Vérification du mot
+                word = word.upper()
+                for letter in word:
+                    assert letter in ALPHABET,f"Mot invalid: {word}"
+                dim = min(width, height)
+                assert len(word) <= dim, f"Mot trop long: {word}"
                 
-                raise GenerateError(f"Unable to place the word {word}")
-            y1,x1=random.choice(choixcoordonnees)
-            #xh,yh=coordonnees(index)
-            x2,y2=x1,y1
-            for letter in word:
-                grid[y2,x2]=letter # a big debug: replace with yh, xh
-
-                x2+=addx
-                y2+=addy
-            answers.loc[len(answers)] = {'word': word, 'direction': direction, 'x1': x1, 'y1': y1,'x2': x2, 'y2': y2}
-
-        def verifsens(addx,addy):
-
-            grid[y1,x1]=letter 
-            word=letter
-            xh,yh=x1,y1
-            while 0<=xh<width and 0<=yh<height:
-                if grid[yh,xh]=="":
-                    return True
-                if word in words:
-                    return False
-                #lettrespossible.append(letter)
-                word+=grid[yh,xh]
-                xh+=addx
-                yh+=addy 
-            return True
-
-        for y1 in range(height):
-            for x1 in range(width):
-                for _ in range(1):
-                    xs,ys=x1,y1
-                    lettrespossible=[]
-                    if grid[y1,x1]:
-                        #print(repr(letters[y,x]))
-                        break
-                    for letter in ALPHABET:
-                        for addx,addy in [(0,1),(1,1),(1,0),(1,-1),(0,-1),(-1,-1),(-1,0),(-1,1)]:
-                            if not verifsens(addx,addy):
+                #choix de rangey, rangex, addy, addx
+                addx,addy = random.choice(tuple(possible_directions))
+                if addy==1:
+                    rangey=range((height-len(word))+1)
+                    
+                elif addy==-1:
+                    rangey=range(len(word)-1,height)
+
+                else:
+                    rangey=range(height)
+
+                if addx==1:
+                    rangex=range((width-len(word))+1)
+
+                elif addx==-1:
+                    rangex=range(len(word)-1,width)
+
+                else:
+                    rangex=range(width)
+                    addx=0
+
+                choixcoordonnees=[]
+                for y1 in rangey:
+
+                    for x1 in rangex:
+
+                        x2,y2=x1,y1 #create copy of x,y
+                        Break=False
+                        for letter in word:
+
+                            #Verify if it's a good emplacement mean: verify if it's blank OR filled with the right letter
+                            if grid[y2,x2]!="":
+                                if grid[y2,x2]!=letter:
+                                    break
+                            x2+=addx
+                            y2+=addy
+                        else:               
+                            choixcoordonnees.append((y1,x1))
+                if not choixcoordonnees: 
+                    
+                    raise GenerateError(f"Unable to place the word {word}")
+                y1,x1=random.choice(choixcoordonnees)
+                #xh,yh=coordonnees(index)
+                x2,y2=x1,y1
+                for letter in word:
+                    grid[y2,x2]=letter # a big debug: replace with yh, xh
+
+                    x2+=addx
+                    y2+=addy
+                answers.loc[word] = {'direction': (addx,addy), 'x1': x1, 'y1': y1,'x2': x2-addx, 'y2': y2-addy}
+
+            def verifsens(addx,addy):
+                """Verify if the letter can be placed without placing a word in the same direction"""
+                grid[y1,x1]=letter 
+                word=letter
+                xh,yh=x1,y1
+                while 0<=xh<width and 0<=yh<height:
+                    if grid[yh,xh]=="":
+                        return True
+                    if word in words:
+                        return False
+                    #lettrespossible.append(letter)
+                    word+=grid[yh,xh]
+                    xh+=addx
+                    yh+=addy 
+                return True
+
+            for y1 in range(height):
+                for x1 in range(width):
+                    for _ in range(1):
+                        xs,ys=x1,y1
+                        lettrespossible=[]
+                        if grid[y1,x1]:
+                            #print(repr(letters[y,x]))
+                            break
+                        for letter in ALPHABET:
+                            for addx,addy in [(0,1),(1,1),(1,0),(1,-1),(0,-1),(-1,-1),(-1,0),(-1,1)]:
+                                if not verifsens(addx,addy):
+                                    #lettrespossible.append(letter)
+                                    break
+                            else:
                                 lettrespossible.append(letter)
-                                break
-                        else:
-                            lettrespossible.append(letter)
-                    if not lettrespossible:
-                        raise GenerateError(f"Unable to place {x1},{y1}")
-                    grid[y1,x1]=random.choice(lettrespossible)
-                if grid[ys,xs] not in ALPHABET:
-                    pass
-            
-        return grid,answers
-    errs=[]
-    for _ in range(10):
-        try:
-            return _generate()
-        except GenerateError as err:
-            if debug_mode:
-                print(err)
-    else:
-        raise GenerateError("Unable to generate a grid")
-
-def print(grille,file=sys.stdout):
-    for y in range(len(grille)):
-        for x in range(len(grille[0])):
-            builtins.print(grille[y,x],end="",file=file)
-        builtins.print(file=file)
-
-def save(grille,file="motsmeles.txt"):
-    with open(file,"w") as f:
-        print(grille,file=f)
-def save_answers(answers,file="motsmeles-answers.csv"):
-    answers.to_csv(file,index=False)
+                        if not lettrespossible:
+                            raise GenerateError(f"Unable to place {x1},{y1}")
+                        grid[y1,x1]=random.choice(lettrespossible)
+                    if grid[ys,xs] not in ALPHABET:
+                        pass
+                
+            return cls(grid,words),answers
+        
+        errs=[]
+        for _ in range(10):
+            try:
+                return _generate()
+            except GenerateError as err:
+                if debug_mode:
+                    print(err)
+        else:
+            raise GenerateError("Unable to generate a grid")
+
+        
+    def solve(self):
+        answers = pd.DataFrame(index=self.words, columns=['direction', 'x1', 'y1', 'x2', 'y2']).reindex(self.words)
+        for y1 in range(self.grid.shape[0]):
+            for x1 in range(self.grid.shape[1]):
+                for direction in DIRECTIONS:
+                    x2,y2=x1,y1
+                    word=""
+                    while 0<=x2<self.grid.shape[1] and 0<=y2<self.grid.shape[0]:
+                        word+=self.grid[y2,x2]
+                        if word in self.words:
+                            answers.loc[word] = {'direction': direction, 'x1': x1, 'y1': y1,'x2': x2, 'y2': y2}
+                            break
+                        x2+=direction[0]
+                        y2+=direction[1]
+        return answers
+
+    def __repr__(self):
+        s=""
+        for y in range(len(self.grid)):
+            for x in range(len(self.grid[0])):
+                s+=self.grid[y,x]
+            s+="\n"
+        s+=" ".join(self.words)
+        return s
+
+    @classmethod
+    def load(cls,file="motsmeles.txt"):
+        with open(file) as f:
+            return cls(f.read())
+    def save(self,file="motsmeles.txt"):
+        with open(file,"w") as f:
+            f.write(repr(self))
+        
+generate=Game.generate
+load=Game.load
         
 def main():
     import argparse
     
     parser = argparse.ArgumentParser(description="générateur de mots mêlés")
     parser.add_argument("words", nargs="+", help="les mots à placer")
     parser.add_argument("-W", "--width", type=int, default=DEFAULT_WIDTH, help="the width of the grid")
```

### Comparing `motsmeles-3.1.0/PKG-INFO` & `motsmeles-3.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: motsmeles
-Version: 3.1.0
+Version: 3.3.0
 Summary: générateur de mots mêlés
 License: MIT
 Author: RadoTheProgrammer
 Author-email: rado@arazakar.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
- This is a word crossing game generator `pip install motsmeles`
+ This is a word crossing game generator, install it with `pip3 install motsmeles`
 
 # Usage
 
 To use it, just import the library
 
 ```python
 import motsmeles
 
-grid,answers=motsmeles.generate(
+game,answers=motsmeles.generate(
     [
         "PYTHON",
         "JAVA",
         "CPP",
         "HTML",
         "CSS",
         "PHP",
@@ -38,22 +38,32 @@
     width = 10, 
     height = 10)
 
 
 
 ```
 
-The `grid` variable contain the grid of the game, it's a numpy array, display it using `motsmeles.print()` or save in a file with `motsmeles.save()`
+The `game` variable contain the grid and the words of the game, you can display it or save it in a file
 
 ```python
 
-motsmeles.print(grid)
-motsmeles.save(grid,file="motsmeles.txt")
+print(game)
+game.save("motsmeles.txt")
+```
+# Solver
+You can also load a game from a file
+```python
+game = motsmeles.load("motsmeles.txt")
 ```
 
+And then solve it
+```python
+answers=game.solve()
+print(answers)
+```
 # CLI Usage
 
 You can also execute the cli version
 
 ```
 
 motsmeles PYTHON JAVA CPP HTML CSS PHP RUBY SWIFT PERL RUST -W 10 -H 10
```

