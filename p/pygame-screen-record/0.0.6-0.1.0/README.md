# Comparing `tmp/pygame-screen-record-0.0.6.tar.gz` & `tmp/pygame_screen_record-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame-screen-record-0.0.6.tar", last modified: Thu Sep 14 17:07:00 2023, max compression
+gzip compressed data, was "pygame_screen_record-0.1.0.tar", last modified: Fri May 10 05:11:22 2024, max compression
```

## Comparing `pygame-screen-record-0.0.6.tar` & `pygame_screen_record-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-09-14 17:07:00.909133 pygame-screen-record-0.0.6/
--rw-rw-rw-   0        0        0     1071 2023-09-14 16:12:32.000000 pygame-screen-record-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    19100 2023-09-14 17:07:00.897554 pygame-screen-record-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    18448 2023-09-14 17:05:57.000000 pygame-screen-record-0.0.6/README.md
--rw-rw-rw-   0        0        0      742 2023-09-14 17:06:20.000000 pygame-screen-record-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-14 17:07:00.910130 pygame-screen-record-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-14 17:07:00.513559 pygame-screen-record-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-09-14 17:07:00.628560 pygame-screen-record-0.0.6/src/pygame_screen_record/
--rw-rw-rw-   0        0        0    11563 2023-09-14 16:12:32.000000 pygame-screen-record-0.0.6/src/pygame_screen_record/EventRegister.py
--rw-rw-rw-   0        0        0    27943 2023-09-14 16:12:32.000000 pygame-screen-record-0.0.6/src/pygame_screen_record/ScreenRecorder.py
--rw-rw-rw-   0        0        0      233 2023-09-14 16:12:32.000000 pygame-screen-record-0.0.6/src/pygame_screen_record/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-14 17:07:00.870554 pygame-screen-record-0.0.6/src/pygame_screen_record.egg-info/
--rw-rw-rw-   0        0        0    19100 2023-09-14 17:07:00.000000 pygame-screen-record-0.0.6/src/pygame_screen_record.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-09-14 17:07:00.000000 pygame-screen-record-0.0.6/src/pygame_screen_record.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-14 17:07:00.000000 pygame-screen-record-0.0.6/src/pygame_screen_record.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-09-14 17:07:00.000000 pygame-screen-record-0.0.6/src/pygame_screen_record.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-09-14 17:07:00.000000 pygame-screen-record-0.0.6/src/pygame_screen_record.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-09-14 17:07:00.884563 pygame-screen-record-0.0.6/tests/
--rw-rw-rw-   0        0        0     1064 2023-09-14 16:12:32.000000 pygame-screen-record-0.0.6/tests/test_compress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:11:22.505766 pygame_screen_record-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 05:11:18.000000 pygame_screen_record-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-05-10 05:11:22.505766 pygame_screen_record-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-05-10 05:11:18.000000 pygame_screen_record-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-10 05:11:18.000000 pygame_screen_record-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:11:22.505766 pygame_screen_record-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:11:22.501766 pygame_screen_record-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:11:22.501766 pygame_screen_record-0.1.0/src/pygame_screen_record/
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-10 05:11:18.000000 pygame_screen_record-0.1.0/src/pygame_screen_record/EventRegister.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27314 2024-05-10 05:11:18.000000 pygame_screen_record-0.1.0/src/pygame_screen_record/ScreenRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-10 05:11:18.000000 pygame_screen_record-0.1.0/src/pygame_screen_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 05:11:18.000000 pygame_screen_record-0.1.0/src/pygame_screen_record/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:11:22.505766 pygame_screen_record-0.1.0/src/pygame_screen_record.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-05-10 05:11:22.000000 pygame_screen_record-0.1.0/src/pygame_screen_record.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-10 05:11:22.000000 pygame_screen_record-0.1.0/src/pygame_screen_record.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 05:11:22.000000 pygame_screen_record-0.1.0/src/pygame_screen_record.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:11:22.000000 pygame_screen_record-0.1.0/src/pygame_screen_record.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 05:11:22.000000 pygame_screen_record-0.1.0/src/pygame_screen_record.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:11:22.505766 pygame_screen_record-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-10 05:11:18.000000 pygame_screen_record-0.1.0/tests/test_compress.py
```

### Comparing `pygame-screen-record-0.0.6/LICENSE` & `pygame_screen_record-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2023 Rashid Harvey
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright (c) 2023 Rashid Harvey
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pygame-screen-record-0.0.6/PKG-INFO` & `pygame_screen_record-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,524 +1,506 @@
-Metadata-Version: 2.1
-Name: pygame-screen-record
-Version: 0.0.6
-Summary: A package that allows you to record your pygame game
-Author-email: Rashid Harvey <r.harvey@outlook.de>
-Project-URL: Homepage, https://github.com/theRealProHacker/PyGameRecorder
-Project-URL: Bug Tracker, https://github.com/theRealProHacker/PyGameRecorder/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: opencv_python>=4.7.0.68
-Requires-Dist: pygame>=2.1.3
-
-# A Simple PyGame ScreenRecorder
-
-## Why you should use this module?
-
-1. Relatively high accuracy
-2. No (noticable) performance issues
-3. Recording FPS is not bound to game FPS
-3. Straightforward usage
-4. Codebase is well commented and typed
-
-## Why you shouldn't use this module?
-
-1. The library is written in pure Python and therefore cannot compare with any lower level library.
-1. Everything is still in develompment.
-
-## Dependencies
-
-Apart from pygame and python >=3.8
-
-1. opencv-python (includes numpy)
-2. FFmpeg if you want to save videos
-
-## Install
-
-`pip install pygame-screen-record`
-
-## FAQ
-
-See the FAQ [in the wiki](https://github.com/theRealProHacker/PyGameRecorder/wiki/FAQ)
-
-## To-Dos
-
-2. Event recording (mouse, key, quit, etc.) ✔️
-3. Sound recording (Either event based with function hooking or as numpy arrays)
-4. A proper video player
-5. Add a wiki
-
-## Contributing
-
-File any bugs or feature requests as GitHub issues. After your idea was approved, we can start working on a solution and make a pull request. The codebase is pretty simple and easy to get ahold of.
-
-# How To Use
-
-Most users just want to make a recording of their game and save it in a video file. Here comes how.
-
-> Note: I am using `pg` as an alias for `pygame` in the following code snippets and I `import ScreenRecorder` instead of `pygame_screen_record.ScreenRecorder`. 
-
-A typical game script might look like this:
-
-```python
-import pygame as pg
-pg.init()
-
-init_code()
-
-try:
-    while True:
-        event_handling()
-        updating()
-        drawing()
-finally:
-    clean_up()
-    pg.quit()
-```
-
-The `try - finally - statement` is very important to catch any exceptions and clean up whether the game ended naturely or not.
-
-Adding a recorder is very simple:
-
-```python
-import pygame as pg
-from ScreenRecorder import ScreenRecorder, save_recordings
-
-pg.init()
-
-init_code()
-
-recorder = ScreenRecorder(60) # Pass your desired fps
-recorder.start_rec() # Start recording
-
-try:
-    while True:
-        event_handling()
-        updating()
-        drawing()
-finally:
-    recorder.stop_rec()	# stop recording
-    recording = recorder.get_single_recording() # returns a Recording
-    save_recordings(recording,("my_recording","mp4")) # save the recording as mp4
-    clean_up()
-    pg.quit()
-```
-
-This code will record your screen the whole game and then save it in the current working directory as `my_recording.mp4`.
-Typical values for the frames per second (fps) are 24 (for slow games), 30, 60 and 120 (Most displays only refresh at 60 Hertz, so most users won't see a difference upwards of 60 fps). Don't forget that the fps value is (at least in theory) proportional to the memory consumption of your recording.
-
-One cool thing of many is that you can chain functions:
-
-```python
-recorder = ScreenRecorder(60)
-recorder.start_rec()
-```
-is equivalent to
-
-```python
-recorder = ScreenRecorder(60).start_rec()
-```
-
-And
-
-```python
-recorder.stop_rec()
-recording = recorder.get_single_recording()
-save_recording(recording,("my_recording","mp4"))
-```
-
-is equivalent to
-
-```python
-recorder.stop_rec().get_single_recording().save("my_recording","mp4")
-```
-
-## Short word on types
-
-1. The whole codebase is typed -> If you want to contribute use types too
-1. AnyPath means any type that can be a file or directory  `str | int | bytes` normally.
-2. For me, `pg.Surface` is equivalent to `pg.surface.Surface`. (mypy thinks differently)
-
-# Advanced Recording Options
-
-Some of the options available:
-
-1. Record any surface
-2. Compress `ScreenRecorders`
-3. Stream recordings (maybe add frame streaming too?)
-4. Apply effects on recordings
-
-## Record any Surface
-
-In most cases you want to record the whole screen. But, you can also pass an optional argument `surf` to a `ScreenRecorder`.
-
-```python
-my_surface = pg.surface.Surface((900,600))
-recorder = ScreenRecorder(60,my_surface)
-```
-
-## Compress recordings
-
-You can choose to compress your recordings like this
-
-```python
-recorder = ScreenRecorder(compress=2) # fps defaults to 60 
-```
-
-What does that mean? It means that every frame will be scaled down `2`-times by two. This reduces the total memory consumption by `2^(2^2) = 16`! But normally you will only compress by one or not compress at all. The recordings will automatically be decompressed when played or saved. So don't worry about that. Just try out whether the loss in resolution is okay for your needs.
-
-## Stream recordings
-
-A stream in this sense is any object that implements a `send` function that can take a recording. To set a stream pass it to the `ScreenRecorder` constructor.
-
-```python
-class Stream:
-    def send(self,rec):
-        print(f"Recording received with {rec.frame_number} frames, a size of {rec.size} and a total length of {rec.length} s")
-
-my_stream = Stream()
-recorder = ScreenRecorder(stream=my_stream)
-```
-
-Now `recorder.stop_rec()` will send to that stream and also save the recording internally. With `recorder.stop_rec_to_stream(stream = None)` you send to the stream without saving and can optionally specify a stream that will override the recorders default stream.
-
-## Set individual recordings fps
-
-```python
-ScreenRecorder(60).start_rec(30)
-```
-
-will record at 30 fps for this one recording.
-
-## Abort a running recording
-
-`recorder.abort_rec()`
-
-## Get all recordings of a recorder
-
-```python
-all_recordings = recorder.get_recordings()
-```
-
-## Attributes of a recorder
-
-These are the attributes of a `ScreenRecorder` instance. Don't change any of these if you don't have a reason! Create a new recorder instead.
-
-`fps: float`  
-selfexp.
-
-`surf: pg.Surface`  
-selfexp.
-
-`compress: int`  
-selfexp.
-
-`size`: Tuple[int,int]  
-The size (width, height) of the recorded surface. Change this attribute only if you are also manually changing the surface at the same time.
-
-`dt: float`  
-The time between (delta time) two frames in ms.  
-`dt = 1000/fps`
-
-`recordings: List[Recording]`  
-selfexp. Same as `get_recordings()`
-
-## Post-Processing a Recording
-
-1. Add frames
-2. Resize
-3. Apply effects
-
-## Adding frames
-
-You can always append frames to a recording:
-
-`recording.add_frame(frame: pg.Surface)`
-
-## Resize a Recording
-
-You might need to rescale a whole recording to a specific size:
-
-`recording.resize(size: Tuple[int,int])`
-
-## Apply effects
-
-If there is more to do than just resizing:
-
-`recording.apply(effect: Callable[[pg.Surface], pg.Surface])`
-
-Will apply the effect on every frame of the recording.
-
-## Attributes of a recording
-
-These are pretty much the same as the attributes of a ScreenRecorder
-
-`fps: float`  
-selfexp.
-
-`surf: pg.Surface`  
-selfexp.
-
-`compress: int`  
-selfexp.
-
-`size`: Tuple[int,int]  
-selfexp. Change this attribute only if you are also manually changing the frames at the same time (e.g. Applying a resizing filter).
-
-`dt: float`  
-selfexp.
-
-`frames: List[pg.Surface]`  
-selfexp.
-
-# Advanced Saving Options
-
-Introducing the RecordingSaver
-
-`RecordingSaver(recordings: List[Recording], key: str | SupportsIndex | Callable[[int], Optional[Tuple[str,str]]], save_dir: AnyPath = None, blocking: bool = True)`
-
-```python
-recordings = recorder.get_recordings()
-saver = RecordingSaver(recordings, "mp4", "saved_files")
-saver.save()
-```
-
-Saves the given recordings as `mp4` files in `./saved_files`  
-We learned that there is a convenient way to do anything. Just call 
-
-```python
-saved_recordings = recorder.save_recordings("mp4", "saved_files")
-```
-
-## Explanation
-
-- key   
-    You can either give a str, a list or a function  
-    If key is a str that determines the format of the recordings and they will be saved as `recording_0.{key}`,`recording_1.{key}`, etc. 
-    
-    Valid formats are listed if you import `available_formats` from `ScreenRecorder.py`. You can add/update FFmpeg-supported formats by calling `add_codec(format:str, codec: int | str)`.  
-
-    An interesting option to mention is the `npz` file format. It is not a classical video format but actually a way to save numpy arrays (npz = NumPy Zipped). If you don't need to share the recording in the internet or so, this is an efficient alternative. This library has built-in support for replaying these files.    
-
-    If key is a list then the ith recording will be saved as the ith element of the recording. This should be a `(filename,format)` tuple. If an element is `None` the recording will be skipped.   
-
-    It is a very similar case if you give a function. The function gets an int passed and should return `None` or a `(filename,format)` tuple.  
-    An example for such a key is
-
-    ```python
-    key = lambda x: if x%2 == 0 then None else ("recording_{x}","mp4")
-    ```
-
-    This will return `None` (and skip the save) for every recording with an even index. 
-- save_dir  
-The directory where the recordings will be saved. Defaults to the current working directory
-- blocking  
-Whether the save should block. Defaults to True
-
-The save returns a list of paths to the recordings in the given directory. This list will not **always** be the same length as the recordings in the `Recorder` but will only return a list of recordings that were actually saved. 
-
-However, if you set `block = False` the function will return another function that returns the list of paths and must be called before the script ends! Now you might ask yourself why that makes any sense. Here is an example
-
-```python
-# At this point we have a recorder that recorded some recordings
-# Now we want to save the recordings as `mp4` and also as `npz`
-import time #to measure how long the saves took
-
-# A naive approach is this
-start = time.time()
-recorder.save_recordings("mp4","saved_files1")
-recorder.save_recordings("npz","saved_files1")
-print("First save took:",time.time() - start)
-
-# Now we use non-blocking (asynchronous) code
-start = time.time()
-join1 = recorder.save_recordings("mp4","saved_files2",False)
-join2 = recorder.save_recordings("npz","saved_files2",False)
-print("This message doen't have to wait for the save. Instead it comes almost instantly")
-
-time.sleep(2) #We add some more virtual io with time.sleep
-
-# Finally we join the save
-join1()
-join2()
-print("Second save took:",time.time() - start)
-```
-
-The second option is favorable because it takes less time than the first. Unfortunately, I haven't yet implemented a contextmanager for this so you will have to manually join or write your own and contribute to the project. 
-
-## Memory Management
-
-We talked about how to efficiently save your recordings (from a time aspect). But now we talk about how you can reduce memory consumption. Generally all video recordings will be automatically compressed by FFmpeg/numpy. However, there are three ways you can reduce memory consumption:  
-1. Reduce fps. One cool thing about this ScreenRecorder is that you can record at a different framerate than you play the game. For example you can have a game frame rate of 60 fps but only record at 30 fps. This would halve the memory usage in comparison to if you recorded at 60 fps. 
-1. Resize the recording. We already established that you can halve the recording size as often as you like. But this will only reduce memory usage while the program runs. The result will still be saved in the original size. However, you can save the recording in a smaller size by using  
-    `recording.resize(pg.Vector2(recording.size)/your_scale_factor)`  
-    This will actually save and play the recording in that size, which might look very weird. 
-    So you might not actually want to do that. 
-1. Shorten the recording length. You can cut out parts of a recording like this. Lets say you only want the first 300 frames.
-
-    ```python
-    recording[0:300]
-    #This will actually mutate the recording. If you have issues with this then just share your concerns
-    ``` 
-1. Lastly, you can reduce the depth of the recording by reducing the depth of the recorded screen `pg.display.set_mode((900,600),depth=your_depth)`. This will definitely reduce the memory usage while the program is running and it might also reduce the memory usage on the disk. However, decreasing the depth of the screen will also decrease the variety in color. But in most amateur applications this might just not matter anyway because you are not using very nuanced colors.   
-
-# Replay recordings
-
-## First note
-I had already implemented a VideoPlayer that could play a Full HD video (1920x816) pretty well (Thats over 6 MB per frame at 24 fps). However, there were several issues (without much detail):
-1. Missing sound
-1. Memory
-1. Lags/Preloading (combined with Memory)
-
-Finally, I came to the conclusion that it makes no sense to write a VideoPlayer in pure Python. 
-
-## Easiest way to replay a recording
-
-```py
-#easiest
-player = RecordingPlayer(recording).play()
-# with an on_stop callback
-def on_stop(): 
-    print("Playing finished")
-player = RecordingPlayer(recording, on_stop).play()
-# with a different surface
-my_surface = pg.Surface((900,600))
-player = RecordingPlayer(recording, None, my_surface).play()
-```
-Make sure that you are not blitting anything else to the surface. You still have to do the flipping/updating yourself (I figured it would be weird if the player did that for you). 
-
-Very important is that you always `stop` a player in your `finally-clause` even if you normally wait for the player to end. Here a contextmanager might make sense too but I'm tending to rather no. 
-
-## Advanced `RecordingPlayer` Options
-
-## Pausing
-You already know how to start a player. You can also pause the player with `pause`. Playing is also unpausing.
-
-```python
-player.pause() 
-```
-
-## Stopping
-This stops the player. As said above, always stop the player if in doubt. However, don't even try to reuse a manually stopped player. As with other objects just make a new player. It's really simple.
-
-```python
-player.stop()
-```
-
-## Seeking
-Seeking is known from files and means going to a certain position. 
-
-```python
-player.seek(300) # goes to frame 300 / the 301th frame
-player.seekms(3000.0) # goes to second 3 of the recording
-```
-
-## Telling
-Similarly telling is also known from files and means getting the current position. 
-
-```python
-player.tell() # Gets the current position
-player.tellms() # Gets the current position in milliseconds
-```
-
-## Restarting
-This method is a mixture between reviving the player after it stopped and just seeking the very first frame and playing.
-
-```python
-player.restart()
-```
-
-In the future, restart might take a new recording to play. But that is only a thought. 
-## Getting state information
-The player has a `is_` function. There are two reasons for the name
-1. It resolves the conflict with the python keyword `is`
-1. It might make the code more readable, reading `player.is_("playing")` is easy to understand and nicer to implement than making individual function for every possible state
-
-```python
-player.is_("started") 
-player.is_("stopped")  
-player.is_("playing")
-player.is_("paused")
-```
-
-They are all pretty self explanatory. But remember two things:
-1. `player.is_("stopped")` might be the most important state because you shouldn't call any other function when the player is stopped (Except restart and stop).
-1. `is_("paused")` is **not** equal to `not is_("playing")`
-
-## Making use of the `on_stop`
-The `on_stop` is a very powerful tool because callbacks are always cool. Optionally, `on_stop` will be passed the player object itself. So, you can really do anything you want. I wrote three example callbacks which are very likely to be useful to the API user. Don't forget to import them before you use them (They are not included in `*`). 
-1. `play_indefinite` will restart the player indefinitely as long as the player is not stopped manually (Stopping the player manually will overwrite the on_stop).
-
-    ```python
-    player = RecordingPlayer(recording,play_indefinite).play()
-    ``` 
-1. `play_n_times` plays the player `n` times.
-
-    ```python
-    player = RecordingPlayer(recording,play_n_times(5)).play() # plays 5 times
-    ```
-1. `play_n_wrapper` plays the player `n` times but it wraps another function to call each time.  
-To come back to our very first `on_stop`. 
-
-    ```python
-    @play_n_wrapper(5)
-    def on_stop(): 
-        print("Playing finished")
-    player = RecordingPlayer(recording,on_stop).play()
-    ```
-
-## Playing saved npz files
-
-I showed you how to save your recordings as `npz` files. However, you also need to know how to play them back. 
-For this there is a `NPZPlayer` class. It takes a path to a file and extra parameters just like the `RecordingPlayer`
-
-```python
-player = NPZPlayer("my_npz_file.npz", on_stop=my_on_stop).play()
-```
-It implements all the methods a `RecordingPlayer` implements too
-
-# Event Register
-One of my to-dos was an event register. This task is accomplished. Here comes the tutorial for this. 
-
-Let's suppose you are using events and have a deterministic game (No randomness/randomness with a seed). You just need to do four things to record your game. 
-1. `import EventRegister from EventRegister`
-1. Create a new `EventRegister` object
-1. Get your events from the object
-1. Finally, save the registered events.
-
-## Example
-
-```python
-import EventRegister from EventRegister
-
-pg.init()
-
-reg = EventRegister("in","events.json") # save as json
-
-try:
-    running = True
-    while running:
-        time.sleep(0.0099) # 100 fps
-        for event in reg.get_events(): # instead of pg.event.get()
-            if event.type == pg.QUIT:
-                running = False
-            elif event.type == pg.MOUSEBUTTONDOWN:
-                print(event.button,event.pos)
-finally:
-    pg.quit()
-    reg.save()
-```
-
-Now to replay that exact recorded game. Just swap `in` with `out` when instanciating the `reg` object and everything should work exactly as expected.
-
-## Random Seeds
-
-If your game uses randomness - which most games should - it's very simple. 
-This will automatically load or save the seed depending on the mode.  
-
-```python
-reg = EventRegister("in","events.json").seed()
-```
+Metadata-Version: 2.1
+Name: pygame-screen-record
+Version: 0.1.0
+Summary: A package that allows you to record your pygame game
+Author-email: Rashid Harvey <r.harvey@outlook.de>
+Project-URL: Homepage, https://github.com/theRealProHacker/PyGameRecorder
+Project-URL: Bug Tracker, https://github.com/theRealProHacker/PyGameRecorder/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: opencv_python>=4.7.0.68
+Requires-Dist: pygame>=2.1.3
+
+# A Simple pygame ScreenRecorder
+
+## Why you should use pygame ScreenRecorder?
+
+1. Relatively high accuracy
+2. No (noticable) performance issues
+3. Recording FPS is not bound to game FPS
+4. Straightforward usage
+5. The codebase is well commented and typed
+
+## Dependencies
+
+Apart from pygame and python >=3.8
+
+1. opencv-python (includes numpy)
+2. FFmpeg if you want to save videos
+
+## Install
+
+`pip install pygame-screen-record`
+
+## FAQ
+
+See the FAQ [in the wiki](https://github.com/theRealProHacker/PyGameRecorder/wiki/FAQ)
+
+## To-Dos
+
+2. Event recording (mouse, key, quit, etc.) ✔️
+3. Sound recording (Either event based with function hooking or as numpy arrays)
+4. A proper video player
+5. Add a wiki ✔️
+
+## Contributing
+
+File any bugs or feature requests as GitHub issues. Any comments are always welcome. 
+
+# How To Use
+
+Probably you just want to make a recording of their game and save it in a video file. Here comes how.
+
+> Note: I am using `pg` as an alias for `pygame` in the following code snippets
+
+A typical game script might look like this:
+
+```py
+import pygame as pg
+pg.init()
+
+init_code()
+
+try:
+    while True:
+        event_handling()
+        updating()
+        drawing()
+finally:
+    clean_up()
+    pg.quit()
+```
+
+The `try - finally - statement` is very important to catch any exceptions and clean up whether the game ended naturely or not.
+
+Adding a recorder is very simple:
+
+```py
+import pygame as pg
+from pygame_screen_record import ScreenRecorder
+
+pg.init()
+
+init_code()
+
+recorder = ScreenRecorder(60) # Pass your desired fps
+recorder.start_rec() # Start recording
+
+try:
+    while True:
+        event_handling()
+        updating()
+        drawing()
+finally:
+    recorder.stop_rec()	# stop recording
+    recording = recorder.save_recording("my_recording.mp4") # returns a Recording
+    clean_up()
+    pg.quit()
+```
+
+This code will record your screen the whole game and then save it in the current working directory as `my_recording.mp4`.
+Typical values for the frames per second (fps) are 24 (for slow games), 30, 60 and 120 (Most displays only refresh at 60 Hertz, so most users won't see a difference upwards of 60 fps). Don't forget that the fps value is (at least in theory) proportional to the memory consumption of your recording.
+
+One cool thing of many is that you can chain functions. So for example
+
+```py
+recorder = ScreenRecorder(60)
+recorder.start_rec()
+```
+is equivalent to
+
+```py
+recorder = ScreenRecorder(60).start_rec()
+```
+
+and you can also just write: `recorder.stop_rec().save_recording("my_recording.mp4")`
+
+# Advanced Recording Options
+
+Some of the options available:
+
+1. Record multiple recordings
+2. Record any surface
+3. Compress `ScreenRecorders`
+4. Stream recordings (maybe add frame streaming too?)
+5. Apply effects on recordings
+
+## Record multiple recordings
+
+In the example, we only recorded a single recording. However, you can record as many recordings as you like with a single `ScreenRecorder`. To stop and start recordings use `stop_rec` and `start_rec`. You can also abort recordings using `abort_rec`. 
+
+Finally, when you want to save your recordings call `save_recordings("mp4")`. More detailed saving options are given in the next chapter [Advanced Saving Options](#advanced-saving-options). 
+
+## Record any `Surface`
+
+In most cases you want to record the whole screen. But, you can also pass an optional argument `surf` to a `ScreenRecorder`.
+
+```python
+my_surface = pg.surface.Surface((900, 600))
+recorder = ScreenRecorder(60, my_surface)
+```
+
+## Compress recordings
+
+You can choose to compress your recordings like this
+
+```py
+recorder = ScreenRecorder(compress=2) # fps defaults to 60 
+```
+
+What does that mean? It means that every frame will be scaled down `2`-times by two. This reduces the total memory consumption by `2^(2^2) = 16`! But normally you will only compress by one or not compress at all. The recordings will automatically be decompressed when played or saved. So don't worry about that. Just try out whether the loss in resolution is okay for your needs.
+
+## Stream recordings
+
+A stream in this sense is any object that implements a `send` function that can take a recording. To set a stream pass it to the `ScreenRecorder` constructor.
+
+```python
+class Stream:
+    def send(self, rec):
+        print(f"Recording received with {rec.frame_number} frames, a size of {rec.size} and a total length of {rec.length} s")
+
+my_stream = Stream()
+recorder = ScreenRecorder(stream=my_stream)
+```
+
+Now `recorder.stop_rec()` will send to that stream and also save the recording internally. With `recorder.stop_rec_to_stream(stream = None)` you send to the stream without saving and can optionally specify a stream that will override the recorders default stream.
+
+## Set individual recordings fps
+
+```py
+ScreenRecorder(60).start_rec(30)
+```
+
+will record at 30 fps for this one recording.
+
+## Get all recordings of a recorder
+
+```py
+all_recordings = recorder.get_recordings()
+```
+
+## Attributes of a recorder
+
+These are the attributes of a `ScreenRecorder` instance. Don't change any of these if you don't have a reason! Create a new recorder instead.
+
+`fps: float`  
+selfexp.
+
+`surf: pg.Surface`  
+selfexp.
+
+`compress: int`  
+selfexp.
+
+`size: Tuple[int,int]`  
+The size (width, height) of the recorded surface. Change this attribute only if you are also manually changing the surface at the same time.
+
+`dt: float`  
+The time between (delta time) two frames in ms.  
+`dt = 1000/fps`
+
+`recordings: List[Recording]`  
+selfexp. Same as `get_recordings()`
+
+## Post-Processing a recording
+
+1. Add frames
+2. Resize
+3. Apply effects
+
+## Adding frames
+
+You can always append frames to a recording:
+
+`recording.add_frame(frame: pg.Surface)`
+
+## Resize a recording
+
+You might need to rescale a whole recording to a specific size:
+
+`recording.resize(size: Tuple[int,int])`
+
+## Apply effects
+
+If there is more to do than just resizing:
+
+`recording.apply(effect: Callable[[pg.Surface], pg.Surface])`
+
+Will apply the effect on every frame of the recording.
+
+## Attributes of a recording
+
+These are pretty much the same as the attributes of a ScreenRecorder
+
+`fps: float`  
+selfexp.
+
+`surf: pg.Surface`  
+selfexp.
+
+`compress: int`  
+selfexp.
+
+`size: Tuple[int, int]`
+selfexp. Change this attribute only if you are also manually changing the frames at the same time (e.g. Applying a resizing filter).
+
+`dt: float`  
+selfexp.
+
+`frames: List[pg.Surface]`  
+selfexp.
+
+# Advanced Saving Options
+
+Introducing the `RecordingSaver`
+
+`RecordingSaver(recordings: List[Recording], key: str | Sequence[str] | Callable[[int], Optional[str]], save_dir: AnyPath = None, blocking: bool = True)`
+
+```py
+recordings = recorder.get_recordings()
+saver = RecordingSaver(recordings, "mp4", "saved_files")
+saver.save()
+```
+
+Saves the given recordings as `mp4` files in `./saved_files`. But you can also just call
+
+```py
+saved_recordings = recorder.save_recordings("mp4", "saved_files")
+```
+
+## Explanation
+
+- `key`
+    You can either give a str, a list or a function  
+    If key is a str that determines the format of the recordings and they will be saved as `recording_0.{key}`,`recording_1.{key}`, etc. 
+    
+    Valid formats are listed if you call `available_formats()`. You can add/update FFmpeg-supported formats by calling `add_codec(format:str, codec: int | str)`.  
+
+    Maybe its worth to mention the `npz` file format. It is not a classical video format but actually a way to save numpy arrays (npz = **n**um**p**y **z**ipped). If you don't need to share the recording in the internet or so, this is an efficient alternative. Also this library has built-in support for replaying these files.    
+
+    If key is a sequence then the ith recording will be saved as the ith element of the recording. If an element is `None` the according recording will be skipped.   
+
+    It is a very similar case if you give a function. The function gets an int passed and should return `None` or a filename.
+
+    An example for such a key is
+
+    ```python
+    key = lambda x: if x%2 == 0 then None else ("recording_{x}","mp4")
+    ```
+
+    This will return `None` (and skip the save) for every recording with an even index. 
+- `save_dir`  
+The directory where the recordings will be saved. Defaults to the current working directory
+- `blocking`  
+Whether the save should block. Defaults to `True`
+
+The save returns a list of paths to the recordings in the given directory. This list will not **always** be the same length as the recordings in the `Recorder` but will only return a list of recordings that were actually saved. 
+
+However, if you set `block = False` the function will return another function that returns the list of paths and must be called before the script ends! Now you might ask yourself why that makes any sense. Here is an example
+
+```python
+# At this point we have a recorder that recorded some recordings
+# Now we want to save the recordings as `mp4` and also as `npz`
+import time #to measure how long the saves took
+
+# A naive approach is this
+start = time.time()
+recorder.save_recordings("mp4", "saved_files1")
+recorder.save_recordings("npz", "saved_files1")
+print("First save took:", time.time() - start)
+
+# Now we use non-blocking (asynchronous) code
+start = time.time()
+join1 = recorder.save_recordings("mp4", "saved_files2", False)
+join2 = recorder.save_recordings("npz", "saved_files2", False)
+print("This message doen't have to wait for the save. Instead it comes almost instantly")
+
+time.sleep(2) # We add some more virtual io with time.sleep
+
+# Finally we join the save
+join1()
+join2()
+print("Second save took:", time.time() - start)
+```
+
+The second option is favorable because it takes less time than the first. 
+
+## Memory Cosniderations
+
+We talked about how to efficiently save your recordings (from a time aspect). But now we talk about how you can reduce memory consumption. Generally, all video recordings will be automatically compressed by FFmpeg/numpy. However, there are three ways you can reduce memory consumption:  
+1. Reduce fps. One cool thing about this ScreenRecorder is that you can record at a different framerate than you play the game. For example you can have a game frame rate of 60 fps but only record at 30 fps. This would halve the memory usage in comparison to if you recorded at 60 fps. 
+1. Resize the recording. We already established that you can halve the recording size as often as you like. But this will only reduce memory usage while the program runs. The result will still be saved in the original size. However, you can save the recording in a smaller size by using  
+    `recording.resize(pg.Vector2(recording.size)/your_scale_factor)`  
+    This will actually save and play the recording in that size, which might look very weird. 
+    So you might not actually want to do that. 
+1. Shorten the recording length. You can cut out parts of a recording like this. Lets say you only want the first 300 frames.
+
+    ```python
+    # This will actually mutate the recording. 
+    recording[0:300]
+    ``` 
+1. Lastly, you can reduce the depth of the recording by reducing the depth of the recorded screen `pg.display.set_mode((900,600), depth=your_depth)`. This will definitely reduce the memory usage while the program is running and it might also reduce the memory usage on the disk. However, decreasing the depth of the screen will also decrease the variety in color. But in most amateur applications this might just not matter anyway because you are not using very nuanced colors.   
+
+# Replay recordings
+
+## First note
+I had already implemented a VideoPlayer that could play a Full HD video (1920x816) pretty well (Thats over 6 MB per frame at 24 fps). However, there were several issues (without much detail):
+1. Missing sound
+1. Memory
+1. Lags/Preloading (combined with Memory)
+
+Finally, I came to the conclusion that it makes no sense to write a VideoPlayer in pure Python. 
+
+## Easiest way to replay a recording
+
+```py
+# easiest
+player = RecordingPlayer(recording).play()
+
+# with an on_stop callback
+def on_stop(): 
+    print("Playing finished")
+player = RecordingPlayer(recording, on_stop).play()
+
+# with a different surface
+my_surface = pg.Surface((900,600))
+player = RecordingPlayer(recording, None, my_surface).play()
+```
+
+Make sure that you are not blitting anything else to the surface. However, you still have to do the flipping/updating yourself (I figured it would be weird if the player did that for you). 
+
+Very important is that you always `stop` a player in your `finally-clause` even if you normally wait for the player to end. Here a contextmanager might make sense too but I'm tending to rather no. 
+
+# Advanced `RecordingPlayer` Options
+
+## Pausing
+You already know how to start a player. You can also pause the player with `pause`. Playing is also unpausing.
+
+```python
+player.pause() 
+```
+
+## Stopping
+This stops the player. As said above, always stop the player if in doubt. However, don't even try to reuse a manually stopped player. Just make a new player instead, it's really simple.
+
+```python
+player.stop()
+```
+
+## Seeking
+Seeking is known from files and means going to a certain position. 
+
+```python
+player.seek(300) # goes to frame 300 / the 301th frame
+player.seekms(3000.0) # goes to second 3 of the recording
+```
+
+## Telling
+Similarly telling is also known from files and means getting the current position. 
+
+```python
+player.tell() # Gets the current position
+player.tellms() # Gets the current position in milliseconds
+```
+
+## Restarting
+This method is a mixture between reviving the player after it stopped and just seeking the very first frame and playing.
+
+```python
+player.restart()
+```
+
+## Getting state information
+The player has a `is_` function. There are two reasons for the name
+1. It resolves the conflict with the python keyword `is`
+1. It might make the code more readable, reading `player.is_("playing")` is easy to understand and nicer to implement than making individual function for every possible state
+
+```python
+player.is_("started") 
+player.is_("stopped")  
+player.is_("playing")
+player.is_("paused")
+```
+
+They are all pretty self explanatory. But remember two things:
+1. `player.is_("stopped")` might be the most important state because you shouldn't call any other function when the player is stopped (Except restart and stop).
+1. `is_("paused")` is **not** equal to `not is_("playing")` (In the beginning the player is neither playing nor paused)
+
+## Making use of the `on_stop`
+
+The `on_stop` is a very powerful tool because callbacks are always cool. Optionally, `on_stop` will be passed the player object itself. So, you can really do anything you want. I wrote three example callbacks which are very likely to be useful to the API user. Don't forget to import them before you use them (They are not included in `*`). 
+
+1. `play_indefinite` will restart the player indefinitely as long as the player is not stopped manually (Stopping the player manually will overwrite the on_stop).
+
+    ```python
+    player = RecordingPlayer(recording,play_indefinite).play()
+    ``` 
+1. `play_n_times` plays the player `n` times.
+
+    ```python
+    player = RecordingPlayer(recording,play_n_times(5)).play() # plays 5 times
+    ```
+1. `play_n_wrapper` plays the player `n` times but it wraps another function to call each time. To come back to our very first `on_stop`: 
+
+    ```python
+    @play_n_wrapper(5)
+    def on_stop(): 
+        print("Playing finished")
+    player = RecordingPlayer(recording,on_stop).play()
+    ```
+
+## Playing saved npz files
+
+I showed you how to save your recordings as `npz` files. However, you also need to know how to play them back. For this there is a `NPZPlayer` class. It takes a path to a file and extra parameters just like the `RecordingPlayer`
+
+```python
+player = NPZPlayer("my_npz_file.npz", on_stop=my_on_stop).play()
+```
+
+In all other regards it is the same as the `RecprdingPlayer`
+
+# Event Register
+One of my to-dos was an event register. This task is accomplished. Here comes the tutorial for this. 
+
+Let's suppose you are using events and have a deterministic game (No randomness/randomness with a seed). You just need to do four things to record your game. 
+1. `import EventRegister from EventRegister`
+1. Create a new `EventRegister` object
+1. Get your events from the object
+1. Finally, save the registered events.
+
+## Example
+
+```python
+import EventRegister from EventRegister
+
+pg.init()
+
+reg = EventRegister("in","events.json") # save as json
+
+try:
+    running = True
+    while running:
+        time.sleep(0.0099) # 100 fps
+        for event in reg.get_events(): # instead of pg.event.get()
+            if event.type == pg.QUIT:
+                running = False
+            elif event.type == pg.MOUSEBUTTONDOWN:
+                print(event.button,event.pos)
+finally:
+    pg.quit()
+    reg.save()
+```
+
+Now to replay that exact recorded game. Just swap `in` with `out` when instanciating the `reg` object and everything should work exactly as expected.
+
+## Random Seeds
+
+If your game uses randomness - which most games should - it's very simple. 
+This will automatically load or save the seed depending on the mode.  
+
+```python
+reg = EventRegister("in","events.json").seed()
+```
```

### Comparing `pygame-screen-record-0.0.6/README.md` & `pygame_screen_record-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,508 +1,490 @@
-# A Simple PyGame ScreenRecorder
-
-## Why you should use this module?
-
-1. Relatively high accuracy
-2. No (noticable) performance issues
-3. Recording FPS is not bound to game FPS
-3. Straightforward usage
-4. Codebase is well commented and typed
-
-## Why you shouldn't use this module?
-
-1. The library is written in pure Python and therefore cannot compare with any lower level library.
-1. Everything is still in develompment.
-
-## Dependencies
-
-Apart from pygame and python >=3.8
-
-1. opencv-python (includes numpy)
-2. FFmpeg if you want to save videos
-
-## Install
-
-`pip install pygame-screen-record`
-
-## FAQ
-
-See the FAQ [in the wiki](https://github.com/theRealProHacker/PyGameRecorder/wiki/FAQ)
-
-## To-Dos
-
-2. Event recording (mouse, key, quit, etc.) ✔️
-3. Sound recording (Either event based with function hooking or as numpy arrays)
-4. A proper video player
-5. Add a wiki
-
-## Contributing
-
-File any bugs or feature requests as GitHub issues. After your idea was approved, we can start working on a solution and make a pull request. The codebase is pretty simple and easy to get ahold of.
-
-# How To Use
-
-Most users just want to make a recording of their game and save it in a video file. Here comes how.
-
-> Note: I am using `pg` as an alias for `pygame` in the following code snippets and I `import ScreenRecorder` instead of `pygame_screen_record.ScreenRecorder`. 
-
-A typical game script might look like this:
-
-```python
-import pygame as pg
-pg.init()
-
-init_code()
-
-try:
-    while True:
-        event_handling()
-        updating()
-        drawing()
-finally:
-    clean_up()
-    pg.quit()
-```
-
-The `try - finally - statement` is very important to catch any exceptions and clean up whether the game ended naturely or not.
-
-Adding a recorder is very simple:
-
-```python
-import pygame as pg
-from ScreenRecorder import ScreenRecorder, save_recordings
-
-pg.init()
-
-init_code()
-
-recorder = ScreenRecorder(60) # Pass your desired fps
-recorder.start_rec() # Start recording
-
-try:
-    while True:
-        event_handling()
-        updating()
-        drawing()
-finally:
-    recorder.stop_rec()	# stop recording
-    recording = recorder.get_single_recording() # returns a Recording
-    save_recordings(recording,("my_recording","mp4")) # save the recording as mp4
-    clean_up()
-    pg.quit()
-```
-
-This code will record your screen the whole game and then save it in the current working directory as `my_recording.mp4`.
-Typical values for the frames per second (fps) are 24 (for slow games), 30, 60 and 120 (Most displays only refresh at 60 Hertz, so most users won't see a difference upwards of 60 fps). Don't forget that the fps value is (at least in theory) proportional to the memory consumption of your recording.
-
-One cool thing of many is that you can chain functions:
-
-```python
-recorder = ScreenRecorder(60)
-recorder.start_rec()
-```
-is equivalent to
-
-```python
-recorder = ScreenRecorder(60).start_rec()
-```
-
-And
-
-```python
-recorder.stop_rec()
-recording = recorder.get_single_recording()
-save_recording(recording,("my_recording","mp4"))
-```
-
-is equivalent to
-
-```python
-recorder.stop_rec().get_single_recording().save("my_recording","mp4")
-```
-
-## Short word on types
-
-1. The whole codebase is typed -> If you want to contribute use types too
-1. AnyPath means any type that can be a file or directory  `str | int | bytes` normally.
-2. For me, `pg.Surface` is equivalent to `pg.surface.Surface`. (mypy thinks differently)
-
-# Advanced Recording Options
-
-Some of the options available:
-
-1. Record any surface
-2. Compress `ScreenRecorders`
-3. Stream recordings (maybe add frame streaming too?)
-4. Apply effects on recordings
-
-## Record any Surface
-
-In most cases you want to record the whole screen. But, you can also pass an optional argument `surf` to a `ScreenRecorder`.
-
-```python
-my_surface = pg.surface.Surface((900,600))
-recorder = ScreenRecorder(60,my_surface)
-```
-
-## Compress recordings
-
-You can choose to compress your recordings like this
-
-```python
-recorder = ScreenRecorder(compress=2) # fps defaults to 60 
-```
-
-What does that mean? It means that every frame will be scaled down `2`-times by two. This reduces the total memory consumption by `2^(2^2) = 16`! But normally you will only compress by one or not compress at all. The recordings will automatically be decompressed when played or saved. So don't worry about that. Just try out whether the loss in resolution is okay for your needs.
-
-## Stream recordings
-
-A stream in this sense is any object that implements a `send` function that can take a recording. To set a stream pass it to the `ScreenRecorder` constructor.
-
-```python
-class Stream:
-    def send(self,rec):
-        print(f"Recording received with {rec.frame_number} frames, a size of {rec.size} and a total length of {rec.length} s")
-
-my_stream = Stream()
-recorder = ScreenRecorder(stream=my_stream)
-```
-
-Now `recorder.stop_rec()` will send to that stream and also save the recording internally. With `recorder.stop_rec_to_stream(stream = None)` you send to the stream without saving and can optionally specify a stream that will override the recorders default stream.
-
-## Set individual recordings fps
-
-```python
-ScreenRecorder(60).start_rec(30)
-```
-
-will record at 30 fps for this one recording.
-
-## Abort a running recording
-
-`recorder.abort_rec()`
-
-## Get all recordings of a recorder
-
-```python
-all_recordings = recorder.get_recordings()
-```
-
-## Attributes of a recorder
-
-These are the attributes of a `ScreenRecorder` instance. Don't change any of these if you don't have a reason! Create a new recorder instead.
-
-`fps: float`  
-selfexp.
-
-`surf: pg.Surface`  
-selfexp.
-
-`compress: int`  
-selfexp.
-
-`size`: Tuple[int,int]  
-The size (width, height) of the recorded surface. Change this attribute only if you are also manually changing the surface at the same time.
-
-`dt: float`  
-The time between (delta time) two frames in ms.  
-`dt = 1000/fps`
-
-`recordings: List[Recording]`  
-selfexp. Same as `get_recordings()`
-
-## Post-Processing a Recording
-
-1. Add frames
-2. Resize
-3. Apply effects
-
-## Adding frames
-
-You can always append frames to a recording:
-
-`recording.add_frame(frame: pg.Surface)`
-
-## Resize a Recording
-
-You might need to rescale a whole recording to a specific size:
-
-`recording.resize(size: Tuple[int,int])`
-
-## Apply effects
-
-If there is more to do than just resizing:
-
-`recording.apply(effect: Callable[[pg.Surface], pg.Surface])`
-
-Will apply the effect on every frame of the recording.
-
-## Attributes of a recording
-
-These are pretty much the same as the attributes of a ScreenRecorder
-
-`fps: float`  
-selfexp.
-
-`surf: pg.Surface`  
-selfexp.
-
-`compress: int`  
-selfexp.
-
-`size`: Tuple[int,int]  
-selfexp. Change this attribute only if you are also manually changing the frames at the same time (e.g. Applying a resizing filter).
-
-`dt: float`  
-selfexp.
-
-`frames: List[pg.Surface]`  
-selfexp.
-
-# Advanced Saving Options
-
-Introducing the RecordingSaver
-
-`RecordingSaver(recordings: List[Recording], key: str | SupportsIndex | Callable[[int], Optional[Tuple[str,str]]], save_dir: AnyPath = None, blocking: bool = True)`
-
-```python
-recordings = recorder.get_recordings()
-saver = RecordingSaver(recordings, "mp4", "saved_files")
-saver.save()
-```
-
-Saves the given recordings as `mp4` files in `./saved_files`  
-We learned that there is a convenient way to do anything. Just call 
-
-```python
-saved_recordings = recorder.save_recordings("mp4", "saved_files")
-```
-
-## Explanation
-
-- key   
-    You can either give a str, a list or a function  
-    If key is a str that determines the format of the recordings and they will be saved as `recording_0.{key}`,`recording_1.{key}`, etc. 
-    
-    Valid formats are listed if you import `available_formats` from `ScreenRecorder.py`. You can add/update FFmpeg-supported formats by calling `add_codec(format:str, codec: int | str)`.  
-
-    An interesting option to mention is the `npz` file format. It is not a classical video format but actually a way to save numpy arrays (npz = NumPy Zipped). If you don't need to share the recording in the internet or so, this is an efficient alternative. This library has built-in support for replaying these files.    
-
-    If key is a list then the ith recording will be saved as the ith element of the recording. This should be a `(filename,format)` tuple. If an element is `None` the recording will be skipped.   
-
-    It is a very similar case if you give a function. The function gets an int passed and should return `None` or a `(filename,format)` tuple.  
-    An example for such a key is
-
-    ```python
-    key = lambda x: if x%2 == 0 then None else ("recording_{x}","mp4")
-    ```
-
-    This will return `None` (and skip the save) for every recording with an even index. 
-- save_dir  
-The directory where the recordings will be saved. Defaults to the current working directory
-- blocking  
-Whether the save should block. Defaults to True
-
-The save returns a list of paths to the recordings in the given directory. This list will not **always** be the same length as the recordings in the `Recorder` but will only return a list of recordings that were actually saved. 
-
-However, if you set `block = False` the function will return another function that returns the list of paths and must be called before the script ends! Now you might ask yourself why that makes any sense. Here is an example
-
-```python
-# At this point we have a recorder that recorded some recordings
-# Now we want to save the recordings as `mp4` and also as `npz`
-import time #to measure how long the saves took
-
-# A naive approach is this
-start = time.time()
-recorder.save_recordings("mp4","saved_files1")
-recorder.save_recordings("npz","saved_files1")
-print("First save took:",time.time() - start)
-
-# Now we use non-blocking (asynchronous) code
-start = time.time()
-join1 = recorder.save_recordings("mp4","saved_files2",False)
-join2 = recorder.save_recordings("npz","saved_files2",False)
-print("This message doen't have to wait for the save. Instead it comes almost instantly")
-
-time.sleep(2) #We add some more virtual io with time.sleep
-
-# Finally we join the save
-join1()
-join2()
-print("Second save took:",time.time() - start)
-```
-
-The second option is favorable because it takes less time than the first. Unfortunately, I haven't yet implemented a contextmanager for this so you will have to manually join or write your own and contribute to the project. 
-
-## Memory Management
-
-We talked about how to efficiently save your recordings (from a time aspect). But now we talk about how you can reduce memory consumption. Generally all video recordings will be automatically compressed by FFmpeg/numpy. However, there are three ways you can reduce memory consumption:  
-1. Reduce fps. One cool thing about this ScreenRecorder is that you can record at a different framerate than you play the game. For example you can have a game frame rate of 60 fps but only record at 30 fps. This would halve the memory usage in comparison to if you recorded at 60 fps. 
-1. Resize the recording. We already established that you can halve the recording size as often as you like. But this will only reduce memory usage while the program runs. The result will still be saved in the original size. However, you can save the recording in a smaller size by using  
-    `recording.resize(pg.Vector2(recording.size)/your_scale_factor)`  
-    This will actually save and play the recording in that size, which might look very weird. 
-    So you might not actually want to do that. 
-1. Shorten the recording length. You can cut out parts of a recording like this. Lets say you only want the first 300 frames.
-
-    ```python
-    recording[0:300]
-    #This will actually mutate the recording. If you have issues with this then just share your concerns
-    ``` 
-1. Lastly, you can reduce the depth of the recording by reducing the depth of the recorded screen `pg.display.set_mode((900,600),depth=your_depth)`. This will definitely reduce the memory usage while the program is running and it might also reduce the memory usage on the disk. However, decreasing the depth of the screen will also decrease the variety in color. But in most amateur applications this might just not matter anyway because you are not using very nuanced colors.   
-
-# Replay recordings
-
-## First note
-I had already implemented a VideoPlayer that could play a Full HD video (1920x816) pretty well (Thats over 6 MB per frame at 24 fps). However, there were several issues (without much detail):
-1. Missing sound
-1. Memory
-1. Lags/Preloading (combined with Memory)
-
-Finally, I came to the conclusion that it makes no sense to write a VideoPlayer in pure Python. 
-
-## Easiest way to replay a recording
-
-```py
-#easiest
-player = RecordingPlayer(recording).play()
-# with an on_stop callback
-def on_stop(): 
-    print("Playing finished")
-player = RecordingPlayer(recording, on_stop).play()
-# with a different surface
-my_surface = pg.Surface((900,600))
-player = RecordingPlayer(recording, None, my_surface).play()
-```
-Make sure that you are not blitting anything else to the surface. You still have to do the flipping/updating yourself (I figured it would be weird if the player did that for you). 
-
-Very important is that you always `stop` a player in your `finally-clause` even if you normally wait for the player to end. Here a contextmanager might make sense too but I'm tending to rather no. 
-
-## Advanced `RecordingPlayer` Options
-
-## Pausing
-You already know how to start a player. You can also pause the player with `pause`. Playing is also unpausing.
-
-```python
-player.pause() 
-```
-
-## Stopping
-This stops the player. As said above, always stop the player if in doubt. However, don't even try to reuse a manually stopped player. As with other objects just make a new player. It's really simple.
-
-```python
-player.stop()
-```
-
-## Seeking
-Seeking is known from files and means going to a certain position. 
-
-```python
-player.seek(300) # goes to frame 300 / the 301th frame
-player.seekms(3000.0) # goes to second 3 of the recording
-```
-
-## Telling
-Similarly telling is also known from files and means getting the current position. 
-
-```python
-player.tell() # Gets the current position
-player.tellms() # Gets the current position in milliseconds
-```
-
-## Restarting
-This method is a mixture between reviving the player after it stopped and just seeking the very first frame and playing.
-
-```python
-player.restart()
-```
-
-In the future, restart might take a new recording to play. But that is only a thought. 
-## Getting state information
-The player has a `is_` function. There are two reasons for the name
-1. It resolves the conflict with the python keyword `is`
-1. It might make the code more readable, reading `player.is_("playing")` is easy to understand and nicer to implement than making individual function for every possible state
-
-```python
-player.is_("started") 
-player.is_("stopped")  
-player.is_("playing")
-player.is_("paused")
-```
-
-They are all pretty self explanatory. But remember two things:
-1. `player.is_("stopped")` might be the most important state because you shouldn't call any other function when the player is stopped (Except restart and stop).
-1. `is_("paused")` is **not** equal to `not is_("playing")`
-
-## Making use of the `on_stop`
-The `on_stop` is a very powerful tool because callbacks are always cool. Optionally, `on_stop` will be passed the player object itself. So, you can really do anything you want. I wrote three example callbacks which are very likely to be useful to the API user. Don't forget to import them before you use them (They are not included in `*`). 
-1. `play_indefinite` will restart the player indefinitely as long as the player is not stopped manually (Stopping the player manually will overwrite the on_stop).
-
-    ```python
-    player = RecordingPlayer(recording,play_indefinite).play()
-    ``` 
-1. `play_n_times` plays the player `n` times.
-
-    ```python
-    player = RecordingPlayer(recording,play_n_times(5)).play() # plays 5 times
-    ```
-1. `play_n_wrapper` plays the player `n` times but it wraps another function to call each time.  
-To come back to our very first `on_stop`. 
-
-    ```python
-    @play_n_wrapper(5)
-    def on_stop(): 
-        print("Playing finished")
-    player = RecordingPlayer(recording,on_stop).play()
-    ```
-
-## Playing saved npz files
-
-I showed you how to save your recordings as `npz` files. However, you also need to know how to play them back. 
-For this there is a `NPZPlayer` class. It takes a path to a file and extra parameters just like the `RecordingPlayer`
-
-```python
-player = NPZPlayer("my_npz_file.npz", on_stop=my_on_stop).play()
-```
-It implements all the methods a `RecordingPlayer` implements too
-
-# Event Register
-One of my to-dos was an event register. This task is accomplished. Here comes the tutorial for this. 
-
-Let's suppose you are using events and have a deterministic game (No randomness/randomness with a seed). You just need to do four things to record your game. 
-1. `import EventRegister from EventRegister`
-1. Create a new `EventRegister` object
-1. Get your events from the object
-1. Finally, save the registered events.
-
-## Example
-
-```python
-import EventRegister from EventRegister
-
-pg.init()
-
-reg = EventRegister("in","events.json") # save as json
-
-try:
-    running = True
-    while running:
-        time.sleep(0.0099) # 100 fps
-        for event in reg.get_events(): # instead of pg.event.get()
-            if event.type == pg.QUIT:
-                running = False
-            elif event.type == pg.MOUSEBUTTONDOWN:
-                print(event.button,event.pos)
-finally:
-    pg.quit()
-    reg.save()
-```
-
-Now to replay that exact recorded game. Just swap `in` with `out` when instanciating the `reg` object and everything should work exactly as expected.
-
-## Random Seeds
-
-If your game uses randomness - which most games should - it's very simple. 
-This will automatically load or save the seed depending on the mode.  
-
-```python
-reg = EventRegister("in","events.json").seed()
+# A Simple pygame ScreenRecorder
+
+## Why you should use pygame ScreenRecorder?
+
+1. Relatively high accuracy
+2. No (noticable) performance issues
+3. Recording FPS is not bound to game FPS
+4. Straightforward usage
+5. The codebase is well commented and typed
+
+## Dependencies
+
+Apart from pygame and python >=3.8
+
+1. opencv-python (includes numpy)
+2. FFmpeg if you want to save videos
+
+## Install
+
+`pip install pygame-screen-record`
+
+## FAQ
+
+See the FAQ [in the wiki](https://github.com/theRealProHacker/PyGameRecorder/wiki/FAQ)
+
+## To-Dos
+
+2. Event recording (mouse, key, quit, etc.) ✔️
+3. Sound recording (Either event based with function hooking or as numpy arrays)
+4. A proper video player
+5. Add a wiki ✔️
+
+## Contributing
+
+File any bugs or feature requests as GitHub issues. Any comments are always welcome. 
+
+# How To Use
+
+Probably you just want to make a recording of their game and save it in a video file. Here comes how.
+
+> Note: I am using `pg` as an alias for `pygame` in the following code snippets
+
+A typical game script might look like this:
+
+```py
+import pygame as pg
+pg.init()
+
+init_code()
+
+try:
+    while True:
+        event_handling()
+        updating()
+        drawing()
+finally:
+    clean_up()
+    pg.quit()
+```
+
+The `try - finally - statement` is very important to catch any exceptions and clean up whether the game ended naturely or not.
+
+Adding a recorder is very simple:
+
+```py
+import pygame as pg
+from pygame_screen_record import ScreenRecorder
+
+pg.init()
+
+init_code()
+
+recorder = ScreenRecorder(60) # Pass your desired fps
+recorder.start_rec() # Start recording
+
+try:
+    while True:
+        event_handling()
+        updating()
+        drawing()
+finally:
+    recorder.stop_rec()	# stop recording
+    recording = recorder.save_recording("my_recording.mp4") # returns a Recording
+    clean_up()
+    pg.quit()
+```
+
+This code will record your screen the whole game and then save it in the current working directory as `my_recording.mp4`.
+Typical values for the frames per second (fps) are 24 (for slow games), 30, 60 and 120 (Most displays only refresh at 60 Hertz, so most users won't see a difference upwards of 60 fps). Don't forget that the fps value is (at least in theory) proportional to the memory consumption of your recording.
+
+One cool thing of many is that you can chain functions. So for example
+
+```py
+recorder = ScreenRecorder(60)
+recorder.start_rec()
+```
+is equivalent to
+
+```py
+recorder = ScreenRecorder(60).start_rec()
+```
+
+and you can also just write: `recorder.stop_rec().save_recording("my_recording.mp4")`
+
+# Advanced Recording Options
+
+Some of the options available:
+
+1. Record multiple recordings
+2. Record any surface
+3. Compress `ScreenRecorders`
+4. Stream recordings (maybe add frame streaming too?)
+5. Apply effects on recordings
+
+## Record multiple recordings
+
+In the example, we only recorded a single recording. However, you can record as many recordings as you like with a single `ScreenRecorder`. To stop and start recordings use `stop_rec` and `start_rec`. You can also abort recordings using `abort_rec`. 
+
+Finally, when you want to save your recordings call `save_recordings("mp4")`. More detailed saving options are given in the next chapter [Advanced Saving Options](#advanced-saving-options). 
+
+## Record any `Surface`
+
+In most cases you want to record the whole screen. But, you can also pass an optional argument `surf` to a `ScreenRecorder`.
+
+```python
+my_surface = pg.surface.Surface((900, 600))
+recorder = ScreenRecorder(60, my_surface)
+```
+
+## Compress recordings
+
+You can choose to compress your recordings like this
+
+```py
+recorder = ScreenRecorder(compress=2) # fps defaults to 60 
+```
+
+What does that mean? It means that every frame will be scaled down `2`-times by two. This reduces the total memory consumption by `2^(2^2) = 16`! But normally you will only compress by one or not compress at all. The recordings will automatically be decompressed when played or saved. So don't worry about that. Just try out whether the loss in resolution is okay for your needs.
+
+## Stream recordings
+
+A stream in this sense is any object that implements a `send` function that can take a recording. To set a stream pass it to the `ScreenRecorder` constructor.
+
+```python
+class Stream:
+    def send(self, rec):
+        print(f"Recording received with {rec.frame_number} frames, a size of {rec.size} and a total length of {rec.length} s")
+
+my_stream = Stream()
+recorder = ScreenRecorder(stream=my_stream)
+```
+
+Now `recorder.stop_rec()` will send to that stream and also save the recording internally. With `recorder.stop_rec_to_stream(stream = None)` you send to the stream without saving and can optionally specify a stream that will override the recorders default stream.
+
+## Set individual recordings fps
+
+```py
+ScreenRecorder(60).start_rec(30)
+```
+
+will record at 30 fps for this one recording.
+
+## Get all recordings of a recorder
+
+```py
+all_recordings = recorder.get_recordings()
+```
+
+## Attributes of a recorder
+
+These are the attributes of a `ScreenRecorder` instance. Don't change any of these if you don't have a reason! Create a new recorder instead.
+
+`fps: float`  
+selfexp.
+
+`surf: pg.Surface`  
+selfexp.
+
+`compress: int`  
+selfexp.
+
+`size: Tuple[int,int]`  
+The size (width, height) of the recorded surface. Change this attribute only if you are also manually changing the surface at the same time.
+
+`dt: float`  
+The time between (delta time) two frames in ms.  
+`dt = 1000/fps`
+
+`recordings: List[Recording]`  
+selfexp. Same as `get_recordings()`
+
+## Post-Processing a recording
+
+1. Add frames
+2. Resize
+3. Apply effects
+
+## Adding frames
+
+You can always append frames to a recording:
+
+`recording.add_frame(frame: pg.Surface)`
+
+## Resize a recording
+
+You might need to rescale a whole recording to a specific size:
+
+`recording.resize(size: Tuple[int,int])`
+
+## Apply effects
+
+If there is more to do than just resizing:
+
+`recording.apply(effect: Callable[[pg.Surface], pg.Surface])`
+
+Will apply the effect on every frame of the recording.
+
+## Attributes of a recording
+
+These are pretty much the same as the attributes of a ScreenRecorder
+
+`fps: float`  
+selfexp.
+
+`surf: pg.Surface`  
+selfexp.
+
+`compress: int`  
+selfexp.
+
+`size: Tuple[int, int]`
+selfexp. Change this attribute only if you are also manually changing the frames at the same time (e.g. Applying a resizing filter).
+
+`dt: float`  
+selfexp.
+
+`frames: List[pg.Surface]`  
+selfexp.
+
+# Advanced Saving Options
+
+Introducing the `RecordingSaver`
+
+`RecordingSaver(recordings: List[Recording], key: str | Sequence[str] | Callable[[int], Optional[str]], save_dir: AnyPath = None, blocking: bool = True)`
+
+```py
+recordings = recorder.get_recordings()
+saver = RecordingSaver(recordings, "mp4", "saved_files")
+saver.save()
+```
+
+Saves the given recordings as `mp4` files in `./saved_files`. But you can also just call
+
+```py
+saved_recordings = recorder.save_recordings("mp4", "saved_files")
+```
+
+## Explanation
+
+- `key`
+    You can either give a str, a list or a function  
+    If key is a str that determines the format of the recordings and they will be saved as `recording_0.{key}`,`recording_1.{key}`, etc. 
+    
+    Valid formats are listed if you call `available_formats()`. You can add/update FFmpeg-supported formats by calling `add_codec(format:str, codec: int | str)`.  
+
+    Maybe its worth to mention the `npz` file format. It is not a classical video format but actually a way to save numpy arrays (npz = **n**um**p**y **z**ipped). If you don't need to share the recording in the internet or so, this is an efficient alternative. Also this library has built-in support for replaying these files.    
+
+    If key is a sequence then the ith recording will be saved as the ith element of the recording. If an element is `None` the according recording will be skipped.   
+
+    It is a very similar case if you give a function. The function gets an int passed and should return `None` or a filename.
+
+    An example for such a key is
+
+    ```python
+    key = lambda x: if x%2 == 0 then None else ("recording_{x}","mp4")
+    ```
+
+    This will return `None` (and skip the save) for every recording with an even index. 
+- `save_dir`  
+The directory where the recordings will be saved. Defaults to the current working directory
+- `blocking`  
+Whether the save should block. Defaults to `True`
+
+The save returns a list of paths to the recordings in the given directory. This list will not **always** be the same length as the recordings in the `Recorder` but will only return a list of recordings that were actually saved. 
+
+However, if you set `block = False` the function will return another function that returns the list of paths and must be called before the script ends! Now you might ask yourself why that makes any sense. Here is an example
+
+```python
+# At this point we have a recorder that recorded some recordings
+# Now we want to save the recordings as `mp4` and also as `npz`
+import time #to measure how long the saves took
+
+# A naive approach is this
+start = time.time()
+recorder.save_recordings("mp4", "saved_files1")
+recorder.save_recordings("npz", "saved_files1")
+print("First save took:", time.time() - start)
+
+# Now we use non-blocking (asynchronous) code
+start = time.time()
+join1 = recorder.save_recordings("mp4", "saved_files2", False)
+join2 = recorder.save_recordings("npz", "saved_files2", False)
+print("This message doen't have to wait for the save. Instead it comes almost instantly")
+
+time.sleep(2) # We add some more virtual io with time.sleep
+
+# Finally we join the save
+join1()
+join2()
+print("Second save took:", time.time() - start)
+```
+
+The second option is favorable because it takes less time than the first. 
+
+## Memory Cosniderations
+
+We talked about how to efficiently save your recordings (from a time aspect). But now we talk about how you can reduce memory consumption. Generally, all video recordings will be automatically compressed by FFmpeg/numpy. However, there are three ways you can reduce memory consumption:  
+1. Reduce fps. One cool thing about this ScreenRecorder is that you can record at a different framerate than you play the game. For example you can have a game frame rate of 60 fps but only record at 30 fps. This would halve the memory usage in comparison to if you recorded at 60 fps. 
+1. Resize the recording. We already established that you can halve the recording size as often as you like. But this will only reduce memory usage while the program runs. The result will still be saved in the original size. However, you can save the recording in a smaller size by using  
+    `recording.resize(pg.Vector2(recording.size)/your_scale_factor)`  
+    This will actually save and play the recording in that size, which might look very weird. 
+    So you might not actually want to do that. 
+1. Shorten the recording length. You can cut out parts of a recording like this. Lets say you only want the first 300 frames.
+
+    ```python
+    # This will actually mutate the recording. 
+    recording[0:300]
+    ``` 
+1. Lastly, you can reduce the depth of the recording by reducing the depth of the recorded screen `pg.display.set_mode((900,600), depth=your_depth)`. This will definitely reduce the memory usage while the program is running and it might also reduce the memory usage on the disk. However, decreasing the depth of the screen will also decrease the variety in color. But in most amateur applications this might just not matter anyway because you are not using very nuanced colors.   
+
+# Replay recordings
+
+## First note
+I had already implemented a VideoPlayer that could play a Full HD video (1920x816) pretty well (Thats over 6 MB per frame at 24 fps). However, there were several issues (without much detail):
+1. Missing sound
+1. Memory
+1. Lags/Preloading (combined with Memory)
+
+Finally, I came to the conclusion that it makes no sense to write a VideoPlayer in pure Python. 
+
+## Easiest way to replay a recording
+
+```py
+# easiest
+player = RecordingPlayer(recording).play()
+
+# with an on_stop callback
+def on_stop(): 
+    print("Playing finished")
+player = RecordingPlayer(recording, on_stop).play()
+
+# with a different surface
+my_surface = pg.Surface((900,600))
+player = RecordingPlayer(recording, None, my_surface).play()
+```
+
+Make sure that you are not blitting anything else to the surface. However, you still have to do the flipping/updating yourself (I figured it would be weird if the player did that for you). 
+
+Very important is that you always `stop` a player in your `finally-clause` even if you normally wait for the player to end. Here a contextmanager might make sense too but I'm tending to rather no. 
+
+# Advanced `RecordingPlayer` Options
+
+## Pausing
+You already know how to start a player. You can also pause the player with `pause`. Playing is also unpausing.
+
+```python
+player.pause() 
+```
+
+## Stopping
+This stops the player. As said above, always stop the player if in doubt. However, don't even try to reuse a manually stopped player. Just make a new player instead, it's really simple.
+
+```python
+player.stop()
+```
+
+## Seeking
+Seeking is known from files and means going to a certain position. 
+
+```python
+player.seek(300) # goes to frame 300 / the 301th frame
+player.seekms(3000.0) # goes to second 3 of the recording
+```
+
+## Telling
+Similarly telling is also known from files and means getting the current position. 
+
+```python
+player.tell() # Gets the current position
+player.tellms() # Gets the current position in milliseconds
+```
+
+## Restarting
+This method is a mixture between reviving the player after it stopped and just seeking the very first frame and playing.
+
+```python
+player.restart()
+```
+
+## Getting state information
+The player has a `is_` function. There are two reasons for the name
+1. It resolves the conflict with the python keyword `is`
+1. It might make the code more readable, reading `player.is_("playing")` is easy to understand and nicer to implement than making individual function for every possible state
+
+```python
+player.is_("started") 
+player.is_("stopped")  
+player.is_("playing")
+player.is_("paused")
+```
+
+They are all pretty self explanatory. But remember two things:
+1. `player.is_("stopped")` might be the most important state because you shouldn't call any other function when the player is stopped (Except restart and stop).
+1. `is_("paused")` is **not** equal to `not is_("playing")` (In the beginning the player is neither playing nor paused)
+
+## Making use of the `on_stop`
+
+The `on_stop` is a very powerful tool because callbacks are always cool. Optionally, `on_stop` will be passed the player object itself. So, you can really do anything you want. I wrote three example callbacks which are very likely to be useful to the API user. Don't forget to import them before you use them (They are not included in `*`). 
+
+1. `play_indefinite` will restart the player indefinitely as long as the player is not stopped manually (Stopping the player manually will overwrite the on_stop).
+
+    ```python
+    player = RecordingPlayer(recording,play_indefinite).play()
+    ``` 
+1. `play_n_times` plays the player `n` times.
+
+    ```python
+    player = RecordingPlayer(recording,play_n_times(5)).play() # plays 5 times
+    ```
+1. `play_n_wrapper` plays the player `n` times but it wraps another function to call each time. To come back to our very first `on_stop`: 
+
+    ```python
+    @play_n_wrapper(5)
+    def on_stop(): 
+        print("Playing finished")
+    player = RecordingPlayer(recording,on_stop).play()
+    ```
+
+## Playing saved npz files
+
+I showed you how to save your recordings as `npz` files. However, you also need to know how to play them back. For this there is a `NPZPlayer` class. It takes a path to a file and extra parameters just like the `RecordingPlayer`
+
+```python
+player = NPZPlayer("my_npz_file.npz", on_stop=my_on_stop).play()
+```
+
+In all other regards it is the same as the `RecprdingPlayer`
+
+# Event Register
+One of my to-dos was an event register. This task is accomplished. Here comes the tutorial for this. 
+
+Let's suppose you are using events and have a deterministic game (No randomness/randomness with a seed). You just need to do four things to record your game. 
+1. `import EventRegister from EventRegister`
+1. Create a new `EventRegister` object
+1. Get your events from the object
+1. Finally, save the registered events.
+
+## Example
+
+```python
+import EventRegister from EventRegister
+
+pg.init()
+
+reg = EventRegister("in","events.json") # save as json
+
+try:
+    running = True
+    while running:
+        time.sleep(0.0099) # 100 fps
+        for event in reg.get_events(): # instead of pg.event.get()
+            if event.type == pg.QUIT:
+                running = False
+            elif event.type == pg.MOUSEBUTTONDOWN:
+                print(event.button,event.pos)
+finally:
+    pg.quit()
+    reg.save()
+```
+
+Now to replay that exact recorded game. Just swap `in` with `out` when instanciating the `reg` object and everything should work exactly as expected.
+
+## Random Seeds
+
+If your game uses randomness - which most games should - it's very simple. 
+This will automatically load or save the seed depending on the mode.  
+
+```python
+reg = EventRegister("in","events.json").seed()
 ```
```

### Comparing `pygame-screen-record-0.0.6/src/pygame_screen_record/EventRegister.py` & `pygame_screen_record-0.1.0/src/pygame_screen_record/EventRegister.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,340 +1,340 @@
-from collections import defaultdict
-import json
-import logging
-import random
-import time
-from typing import Any, Callable, Iterable, Optional, Union, List, Dict
-from dataclasses import dataclass, astuple
-import pygame as pg
-
-################################################################################################
-# helpers
-
-
-def skip_none(x, y):
-    return y if x is None else x
-
-
-def dfilter(
-    d: dict,
-    *,
-    key: Optional[Union[Callable[[Any], bool], list]] = None,
-    value: Optional[Union[Callable[[Any], bool], list]] = None,
-):
-    """Filter a dictionary by key or value. You must specify either key or value"""
-    if (key is None) ^ (value is None):  # xor
-        if value is None:
-            if isinstance(key, list):
-                key = key.__contains__
-            return {k: v for k, v in d.items() if key(k)}  # type: ignore
-        elif key is None:
-            if isinstance(value, list):
-                value = value.__contains__
-            return {k: v for k, v in d.items() if value(v)}
-    else:
-        raise TypeError("Exactly one of key and value have to be None")
-
-
-start_lambda = lambda starts: lambda k: any((k.startswith(s) for s in starts))
-
-
-def starts_with(s: Union[Iterable[str], str]):
-    """Returns all the pg.locals that start with any of the given strings"""
-    try:
-        return dfilter(pg.__dict__, key=start_lambda(s)).values()
-    except TypeError:
-        return dfilter(pg.__dict__, key=start_lambda([s])).values()
-
-
-time_since = lambda t: time.time() - t
-
-
-def false_lambda():
-    return False
-
-
-def dict_lambda():
-    return {}
-
-
-def read(path: str):
-    with open(path, "r") as f:
-        return json.load(f)
-
-
-def write(object: Any, path: str):
-    with open(path, "w") as f:
-        json.dump(object, f, ensure_ascii=False)
-
-
-def find(pred: Callable[[Any], bool], l: Iterable) -> Any:
-    for x in l:
-        if pred(x):
-            return x
-
-
-def print_names(l: Union[Iterable[pg.event.Event], Iterable[int]]):
-    try:
-        for e in l:
-            print(pg.event.event_name(e.type))  # type: ignore
-    except (AttributeError, TypeError):
-        for e in l:
-            print(pg.event.event_name(e))  # type: ignore
-
-
-def safe_item_set(d: dict):
-    conv_l_t = lambda l: tuple(l) if type(l) is list else l
-    return {(k, conv_l_t(v)) for k, v in d.items()}
-
-
-################################################################################################
-
-
-################################################################################################
-# Typing
-@dataclass
-class SavedEvent:
-    type: int
-    attrs: dict
-    time: float
-
-
-################################################################################################
-
-
-################################################################################################
-# compressions
-defaults: Dict["str", Dict["str", Any]] = {
-    "window": {
-        "value": None,
-        "events": [
-            32774,
-            32785,
-            770,
-            32776,
-            32783,
-            1024,
-            1025,
-            1026,
-            768,
-            771,
-            769,
-            32784,
-            32786,
-            32777,
-            32787,
-        ],
-    },
-    "touch": {"value": False, "events": [1024]},
-    "buttons": {"value": [0] * 3, "events": [1024]},  #  mouse move
-    "mod": {"value": 0, "events": [771, 769]},  # Key up/key down
-}
-
-
-def_lookup: Dict[int, Dict[str, Any]] = defaultdict(dict)
-
-for attr, d in defaults.items():
-    for event in d["events"]:
-        def_lookup[event][attr] = d["value"]
-
-
-def single_compress(se: SavedEvent) -> SavedEvent:
-    """
-    Mutates the given SavedEvent and returns it
-    """
-    if (default := def_lookup.get(se.type)) is not None:
-        eit = safe_item_set(se.attrs)
-        se.attrs = {k: v for k, v in (eit - (eit & safe_item_set(default)))}
-    return se
-
-
-def single_decompress(se: SavedEvent):
-    """
-    Mutates the given SavedEvent and returns it
-    """
-    if (d := def_lookup.get(se.type)) is not None:
-        se.attrs |= d
-    return se
-
-
-################################################################################################
-
-
-################################################################################################
-
-old_events = {
-    "mouse_foc": pg.mouse.get_focused,
-    "mouse_pos": pg.mouse.get_pos,
-    "mouse_rel": pg.mouse.get_rel,
-    "mouse_pressed": pg.mouse.get_pressed,
-    "key_foc": pg.key.get_focused,
-    "key_pressed": pg.key.get_pressed,
-    "key_mods": pg.key.get_mods,
-}
-
-
-class EventRegister:
-    """
-    As the name suggests this class registers the pygame events so that you can then save them.
-    """
-
-    starts = {"MOUSE", "KEY", "WINDOW"}
-
-    def __init__(
-        self,
-        in_out: str = "in",
-        path: Optional[str] = None,
-        events: Optional[Iterable[int]] = None,
-        no_catch_events: Optional[Iterable[int]] = None,
-    ):
-        default_events = set(starts_with(self.starts))
-        self.events: set[int] = set(skip_none(events, default_events)) | {pg.QUIT}
-        self.no_catch_events: set[int] = set(skip_none(no_catch_events, set())) | {
-            pg.QUIT
-        }
-        assert in_out in ("in", "out"), 'in_out has to be either "in" or "out"'
-        self._type = in_out
-        self.path: Optional[str] = path
-        self.random_seed = None
-        self.start = time.time()
-        self.rec_events: list[SavedEvent] = []
-        self._reci = 0
-        if self._type == "out":
-            assert isinstance(self.path, str), "path must be a string"
-            r = read(self.path)
-            self.random_seed = r["random_seed"]
-            self.rec_events = [single_decompress(SavedEvent(*x)) for x in r["events"]]
-            self._focus = pg.mouse.get_focused()
-            self._mouse_pos = pg.mouse.get_pos()
-            self._mouse_rel = pg.mouse.get_rel()
-            self._mouse_pressed = list(pg.mouse.get_pressed())
-            self._key_pressed: dict = defaultdict(false_lambda)
-            for i, pressed in enumerate(pg.key.get_pressed()):
-                self._key_pressed[i] = pressed
-            self._key_mod = pg.key.get_mods()
-            pg.mouse.get_focused = self.focused
-            pg.mouse.get_pos = self.mouse_pos
-            pg.mouse.get_rel = self.mouse_rel
-            pg.mouse.get_pressed = self.mouse_pressed  # type: ignore
-            pg.key.get_focused = self.focused
-            pg.key.get_pressed = self.key_pressed
-            pg.key.get_mods = self.key_mods
-
-    def _add_events(self, events: Iterable[pg.event.Event]):
-        assert self._type == "in", "Can only add events when inputting"
-        for e in events:
-            if (t := e.type) in self.events:  # python 3.10
-                self.rec_events.append(
-                    SavedEvent(t, e.__dict__, time_since(self.start))
-                )
-
-    def _get_events(self) -> List[pg.event.Event]:
-        assert self._type == "out", "Can only get events when outputting"
-        this_events: list[pg.event.Event] = []
-        for e in self.rec_events[self._reci :]:
-            if time_since(self.start) >= e.time:
-                self._reci += 1
-                this_events.append(pg.event.Event(e.type, e.attrs))
-                if e.type == pg.MOUSEMOTION:
-                    self._mouse_pos = e.attrs["pos"]
-                    self._mouse_rel = e.attrs["rel"]
-                elif e.type == pg.MOUSEBUTTONDOWN:
-                    try:
-                        self._mouse_pressed[e.attrs["button"] - 1] = True
-                    except IndexError:
-                        pass
-                elif e.type == pg.MOUSEBUTTONUP:
-                    try:
-                        self._mouse_pressed[e.attrs["button"] - 1] = False
-                    except IndexError:
-                        pass
-                elif e.type in (pg.KEYDOWN, pg.KEYUP):
-                    self._key_mod = e.attrs["mod"]
-                    if e.type == pg.KEYDOWN:
-                        self._key_pressed[e.attrs["key"] - self._key_mod] = True
-                    elif e.type == pg.KEYUP:
-                        self._key_pressed[e.attrs["key"] - self._key_mod] = False
-                elif e.type == pg.WINDOWFOCUSGAINED:
-                    self._focus = True
-                elif e.type == pg.WINDOWFOCUSLOST:
-                    self._focus = False
-            else:
-                return this_events
-        return this_events
-
-    def seed(
-        self, random_seed: Union[int, float, str, bytes, bytearray] = 0
-    ) -> "EventRegister":
-        """
-        Seed the `EventRegister` a random seed.
-        Just call this on the instance to have a work around for random games (ie. most games).
-        If you pass a non-faulty `random_seed` to this then it will overwrite the instances current `random_seed`.
-        But in most cases just don't pass anything.
-        """
-        if self._type == "in":
-            self.random_seed = random_seed or random.random()
-        else:
-            self.random_seed = random_seed or self.random_seed
-        random.seed(self.random_seed)
-        return self
-
-    def get_events(self) -> List[pg.event.Event]:
-        """Get the next events. To use an `EventRegister`, call this instead of `pg.event.get()`"""
-        events = pg.event.get()
-        if self._type == "out":
-            return [
-                *filter(lambda e: e.type in self.no_catch_events, events)
-            ] + self._get_events()
-        elif self._type == "in":
-            self._add_events(events)
-            return events
-        else:
-            raise RuntimeError('self._type must be "out" or "in"')
-
-    def save(self):
-        """Wraps up the `EventRegister`. You must call this at the end of your script."""
-        if self._type == "in":
-            if not self.rec_events[-1].type == pg.QUIT:
-                logging.debug("Saving but PyGame hasn't finished yet")
-                self.rec_events.append((pg.QUIT, {}, self.rec_events[-1][2] + 0.1))
-            events = [astuple(single_compress(x)) for x in self.rec_events]
-            write({"events": events, "random_seed": self.random_seed}, self.path)
-        else:
-            pg.mouse.get_focused = old_events["mouse_foc"]
-            pg.mouse.get_pos = old_events["mouse_pos"]
-            pg.mouse.get_rel = old_events["mouse_rel"]
-            pg.mouse.get_pressed = old_events["mouse_pressed"]
-            pg.key.get_focused = old_events["key_foc"]
-            pg.key.get_pressed = old_events["key_pressed"]
-            pg.key.get_mods = old_events["key_mods"]
-
-    # class getters
-
-    def focused(self):
-        return self._focus
-
-    def mouse_pos(self):
-        return self._mouse_pos
-
-    def mouse_rel(self):
-        return self._mouse_rel
-
-    def mouse_pressed(self):
-        return tuple(self._mouse_pressed)
-
-    def key_pressed(self):
-        return self._key_pressed
-
-    def key_mods(self):
-        return self._key_mod
-
-
-################################################################################################
-
-
-__all__ = ["EventRegister"]
-
-################################################################################################
-
-if __name__ == "__main__":
-    print("EventRegister")
+from collections import defaultdict
+import json
+import logging
+import random
+import time
+from typing import Any, Callable, Iterable, Optional, Union, List, Dict
+from dataclasses import dataclass, astuple
+import pygame as pg
+
+################################################################################################
+# helpers
+
+
+def skip_none(x, y):
+    return y if x is None else x
+
+
+def dfilter(
+    d: dict,
+    *,
+    key: Optional[Union[Callable[[Any], bool], list]] = None,
+    value: Optional[Union[Callable[[Any], bool], list]] = None,
+):
+    """Filter a dictionary by key or value. You must specify either key or value"""
+    if (key is None) ^ (value is None):  # xor
+        if value is None:
+            if isinstance(key, list):
+                key = key.__contains__
+            return {k: v for k, v in d.items() if key(k)}  # type: ignore
+        elif key is None:
+            if isinstance(value, list):
+                value = value.__contains__
+            return {k: v for k, v in d.items() if value(v)}
+    else:
+        raise TypeError("Exactly one of key and value have to be None")
+
+
+start_lambda = lambda starts: lambda k: any((k.startswith(s) for s in starts))
+
+
+def starts_with(s: Union[Iterable[str], str]):
+    """Returns all the pg.locals that start with any of the given strings"""
+    try:
+        return dfilter(pg.__dict__, key=start_lambda(s)).values()
+    except TypeError:
+        return dfilter(pg.__dict__, key=start_lambda([s])).values()
+
+
+time_since = lambda t: time.time() - t
+
+
+def false_lambda():
+    return False
+
+
+def dict_lambda():
+    return {}
+
+
+def read(path: str):
+    with open(path, "r") as f:
+        return json.load(f)
+
+
+def write(object: Any, path: str):
+    with open(path, "w") as f:
+        json.dump(object, f, ensure_ascii=False)
+
+
+def find(pred: Callable[[Any], bool], l: Iterable) -> Any:
+    for x in l:
+        if pred(x):
+            return x
+
+
+def print_names(l: Union[Iterable[pg.event.Event], Iterable[int]]):
+    try:
+        for e in l:
+            print(pg.event.event_name(e.type))  # type: ignore
+    except (AttributeError, TypeError):
+        for e in l:
+            print(pg.event.event_name(e))  # type: ignore
+
+
+def safe_item_set(d: dict):
+    conv_l_t = lambda l: tuple(l) if type(l) is list else l
+    return {(k, conv_l_t(v)) for k, v in d.items()}
+
+
+################################################################################################
+
+
+################################################################################################
+# Typing
+@dataclass
+class SavedEvent:
+    type: int
+    attrs: dict
+    time: float
+
+
+################################################################################################
+
+
+################################################################################################
+# compressions
+defaults: Dict["str", Dict["str", Any]] = {
+    "window": {
+        "value": None,
+        "events": [
+            32774,
+            32785,
+            770,
+            32776,
+            32783,
+            1024,
+            1025,
+            1026,
+            768,
+            771,
+            769,
+            32784,
+            32786,
+            32777,
+            32787,
+        ],
+    },
+    "touch": {"value": False, "events": [1024]},
+    "buttons": {"value": [0] * 3, "events": [1024]},  #  mouse move
+    "mod": {"value": 0, "events": [771, 769]},  # Key up/key down
+}
+
+
+def_lookup: Dict[int, Dict[str, Any]] = defaultdict(dict)
+
+for attr, d in defaults.items():
+    for event in d["events"]:
+        def_lookup[event][attr] = d["value"]
+
+
+def single_compress(se: SavedEvent) -> SavedEvent:
+    """
+    Mutates the given SavedEvent and returns it
+    """
+    if (default := def_lookup.get(se.type)) is not None:
+        eit = safe_item_set(se.attrs)
+        se.attrs = {k: v for k, v in (eit - (eit & safe_item_set(default)))}
+    return se
+
+
+def single_decompress(se: SavedEvent):
+    """
+    Mutates the given SavedEvent and returns it
+    """
+    if (d := def_lookup.get(se.type)) is not None:
+        se.attrs |= d
+    return se
+
+
+################################################################################################
+
+
+################################################################################################
+
+old_events = {
+    "mouse_foc": pg.mouse.get_focused,
+    "mouse_pos": pg.mouse.get_pos,
+    "mouse_rel": pg.mouse.get_rel,
+    "mouse_pressed": pg.mouse.get_pressed,
+    "key_foc": pg.key.get_focused,
+    "key_pressed": pg.key.get_pressed,
+    "key_mods": pg.key.get_mods,
+}
+
+
+class EventRegister:
+    """
+    As the name suggests this class registers the pygame events so that you can then save them.
+    """
+
+    starts = {"MOUSE", "KEY", "WINDOW"}
+
+    def __init__(
+        self,
+        in_out: str = "in",
+        path: Optional[str] = None,
+        events: Optional[Iterable[int]] = None,
+        no_catch_events: Optional[Iterable[int]] = None,
+    ):
+        default_events = set(starts_with(self.starts))
+        self.events: set[int] = set(skip_none(events, default_events)) | {pg.QUIT}
+        self.no_catch_events: set[int] = set(skip_none(no_catch_events, set())) | {
+            pg.QUIT
+        }
+        assert in_out in ("in", "out"), 'in_out has to be either "in" or "out"'
+        self._type = in_out
+        self.path: Optional[str] = path
+        self.random_seed = None
+        self.start = time.time()
+        self.rec_events: list[SavedEvent] = []
+        self._reci = 0
+        if self._type == "out":
+            assert isinstance(self.path, str), "path must be a string"
+            r = read(self.path)
+            self.random_seed = r["random_seed"]
+            self.rec_events = [single_decompress(SavedEvent(*x)) for x in r["events"]]
+            self._focus = pg.mouse.get_focused()
+            self._mouse_pos = pg.mouse.get_pos()
+            self._mouse_rel = pg.mouse.get_rel()
+            self._mouse_pressed = list(pg.mouse.get_pressed())
+            self._key_pressed: dict = defaultdict(false_lambda)
+            for i, pressed in enumerate(pg.key.get_pressed()):
+                self._key_pressed[i] = pressed
+            self._key_mod = pg.key.get_mods()
+            pg.mouse.get_focused = self.focused
+            pg.mouse.get_pos = self.mouse_pos
+            pg.mouse.get_rel = self.mouse_rel
+            pg.mouse.get_pressed = self.mouse_pressed  # type: ignore
+            pg.key.get_focused = self.focused
+            pg.key.get_pressed = self.key_pressed
+            pg.key.get_mods = self.key_mods
+
+    def _add_events(self, events: Iterable[pg.event.Event]):
+        assert self._type == "in", "Can only add events when inputting"
+        for e in events:
+            if (t := e.type) in self.events:  # python 3.10
+                self.rec_events.append(
+                    SavedEvent(t, e.__dict__, time_since(self.start))
+                )
+
+    def _get_events(self) -> List[pg.event.Event]:
+        assert self._type == "out", "Can only get events when outputting"
+        this_events: list[pg.event.Event] = []
+        for e in self.rec_events[self._reci :]:
+            if time_since(self.start) >= e.time:
+                self._reci += 1
+                this_events.append(pg.event.Event(e.type, e.attrs))
+                if e.type == pg.MOUSEMOTION:
+                    self._mouse_pos = e.attrs["pos"]
+                    self._mouse_rel = e.attrs["rel"]
+                elif e.type == pg.MOUSEBUTTONDOWN:
+                    try:
+                        self._mouse_pressed[e.attrs["button"] - 1] = True
+                    except IndexError:
+                        pass
+                elif e.type == pg.MOUSEBUTTONUP:
+                    try:
+                        self._mouse_pressed[e.attrs["button"] - 1] = False
+                    except IndexError:
+                        pass
+                elif e.type in (pg.KEYDOWN, pg.KEYUP):
+                    self._key_mod = e.attrs["mod"]
+                    if e.type == pg.KEYDOWN:
+                        self._key_pressed[e.attrs["key"] - self._key_mod] = True
+                    elif e.type == pg.KEYUP:
+                        self._key_pressed[e.attrs["key"] - self._key_mod] = False
+                elif e.type == pg.WINDOWFOCUSGAINED:
+                    self._focus = True
+                elif e.type == pg.WINDOWFOCUSLOST:
+                    self._focus = False
+            else:
+                return this_events
+        return this_events
+
+    def seed(
+        self, random_seed: Union[int, float, str, bytes, bytearray] = 0
+    ) -> "EventRegister":
+        """
+        Seed the `EventRegister` a random seed.
+        Just call this on the instance to have a work around for random games (ie. most games).
+        If you pass a non-faulty `random_seed` to this then it will overwrite the instances current `random_seed`.
+        But in most cases just don't pass anything.
+        """
+        if self._type == "in":
+            self.random_seed = random_seed or random.random()
+        else:
+            self.random_seed = random_seed or self.random_seed
+        random.seed(self.random_seed)
+        return self
+
+    def get_events(self) -> List[pg.event.Event]:
+        """Get the next events. To use an `EventRegister`, call this instead of `pg.event.get()`"""
+        events = pg.event.get()
+        if self._type == "out":
+            return [
+                *filter(lambda e: e.type in self.no_catch_events, events)
+            ] + self._get_events()
+        elif self._type == "in":
+            self._add_events(events)
+            return events
+        else:
+            raise RuntimeError('self._type must be "out" or "in"')
+
+    def save(self):
+        """Wraps up the `EventRegister`. You must call this at the end of your script."""
+        if self._type == "in":
+            if not self.rec_events[-1].type == pg.QUIT:
+                logging.debug("Saving but PyGame hasn't finished yet")
+                self.rec_events.append((pg.QUIT, {}, self.rec_events[-1][2] + 0.1))
+            events = [astuple(single_compress(x)) for x in self.rec_events]
+            write({"events": events, "random_seed": self.random_seed}, self.path)
+        else:
+            pg.mouse.get_focused = old_events["mouse_foc"]
+            pg.mouse.get_pos = old_events["mouse_pos"]
+            pg.mouse.get_rel = old_events["mouse_rel"]
+            pg.mouse.get_pressed = old_events["mouse_pressed"]
+            pg.key.get_focused = old_events["key_foc"]
+            pg.key.get_pressed = old_events["key_pressed"]
+            pg.key.get_mods = old_events["key_mods"]
+
+    # class getters
+
+    def focused(self):
+        return self._focus
+
+    def mouse_pos(self):
+        return self._mouse_pos
+
+    def mouse_rel(self):
+        return self._mouse_rel
+
+    def mouse_pressed(self):
+        return tuple(self._mouse_pressed)
+
+    def key_pressed(self):
+        return self._key_pressed
+
+    def key_mods(self):
+        return self._key_mod
+
+
+################################################################################################
+
+
+__all__ = ["EventRegister"]
+
+################################################################################################
+
+if __name__ == "__main__":
+    print("EventRegister")
```

### Comparing `pygame-screen-record-0.0.6/src/pygame_screen_record.egg-info/PKG-INFO` & `pygame_screen_record-0.1.0/src/pygame_screen_record.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,524 +1,506 @@
-Metadata-Version: 2.1
-Name: pygame-screen-record
-Version: 0.0.6
-Summary: A package that allows you to record your pygame game
-Author-email: Rashid Harvey <r.harvey@outlook.de>
-Project-URL: Homepage, https://github.com/theRealProHacker/PyGameRecorder
-Project-URL: Bug Tracker, https://github.com/theRealProHacker/PyGameRecorder/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: opencv_python>=4.7.0.68
-Requires-Dist: pygame>=2.1.3
-
-# A Simple PyGame ScreenRecorder
-
-## Why you should use this module?
-
-1. Relatively high accuracy
-2. No (noticable) performance issues
-3. Recording FPS is not bound to game FPS
-3. Straightforward usage
-4. Codebase is well commented and typed
-
-## Why you shouldn't use this module?
-
-1. The library is written in pure Python and therefore cannot compare with any lower level library.
-1. Everything is still in develompment.
-
-## Dependencies
-
-Apart from pygame and python >=3.8
-
-1. opencv-python (includes numpy)
-2. FFmpeg if you want to save videos
-
-## Install
-
-`pip install pygame-screen-record`
-
-## FAQ
-
-See the FAQ [in the wiki](https://github.com/theRealProHacker/PyGameRecorder/wiki/FAQ)
-
-## To-Dos
-
-2. Event recording (mouse, key, quit, etc.) ✔️
-3. Sound recording (Either event based with function hooking or as numpy arrays)
-4. A proper video player
-5. Add a wiki
-
-## Contributing
-
-File any bugs or feature requests as GitHub issues. After your idea was approved, we can start working on a solution and make a pull request. The codebase is pretty simple and easy to get ahold of.
-
-# How To Use
-
-Most users just want to make a recording of their game and save it in a video file. Here comes how.
-
-> Note: I am using `pg` as an alias for `pygame` in the following code snippets and I `import ScreenRecorder` instead of `pygame_screen_record.ScreenRecorder`. 
-
-A typical game script might look like this:
-
-```python
-import pygame as pg
-pg.init()
-
-init_code()
-
-try:
-    while True:
-        event_handling()
-        updating()
-        drawing()
-finally:
-    clean_up()
-    pg.quit()
-```
-
-The `try - finally - statement` is very important to catch any exceptions and clean up whether the game ended naturely or not.
-
-Adding a recorder is very simple:
-
-```python
-import pygame as pg
-from ScreenRecorder import ScreenRecorder, save_recordings
-
-pg.init()
-
-init_code()
-
-recorder = ScreenRecorder(60) # Pass your desired fps
-recorder.start_rec() # Start recording
-
-try:
-    while True:
-        event_handling()
-        updating()
-        drawing()
-finally:
-    recorder.stop_rec()	# stop recording
-    recording = recorder.get_single_recording() # returns a Recording
-    save_recordings(recording,("my_recording","mp4")) # save the recording as mp4
-    clean_up()
-    pg.quit()
-```
-
-This code will record your screen the whole game and then save it in the current working directory as `my_recording.mp4`.
-Typical values for the frames per second (fps) are 24 (for slow games), 30, 60 and 120 (Most displays only refresh at 60 Hertz, so most users won't see a difference upwards of 60 fps). Don't forget that the fps value is (at least in theory) proportional to the memory consumption of your recording.
-
-One cool thing of many is that you can chain functions:
-
-```python
-recorder = ScreenRecorder(60)
-recorder.start_rec()
-```
-is equivalent to
-
-```python
-recorder = ScreenRecorder(60).start_rec()
-```
-
-And
-
-```python
-recorder.stop_rec()
-recording = recorder.get_single_recording()
-save_recording(recording,("my_recording","mp4"))
-```
-
-is equivalent to
-
-```python
-recorder.stop_rec().get_single_recording().save("my_recording","mp4")
-```
-
-## Short word on types
-
-1. The whole codebase is typed -> If you want to contribute use types too
-1. AnyPath means any type that can be a file or directory  `str | int | bytes` normally.
-2. For me, `pg.Surface` is equivalent to `pg.surface.Surface`. (mypy thinks differently)
-
-# Advanced Recording Options
-
-Some of the options available:
-
-1. Record any surface
-2. Compress `ScreenRecorders`
-3. Stream recordings (maybe add frame streaming too?)
-4. Apply effects on recordings
-
-## Record any Surface
-
-In most cases you want to record the whole screen. But, you can also pass an optional argument `surf` to a `ScreenRecorder`.
-
-```python
-my_surface = pg.surface.Surface((900,600))
-recorder = ScreenRecorder(60,my_surface)
-```
-
-## Compress recordings
-
-You can choose to compress your recordings like this
-
-```python
-recorder = ScreenRecorder(compress=2) # fps defaults to 60 
-```
-
-What does that mean? It means that every frame will be scaled down `2`-times by two. This reduces the total memory consumption by `2^(2^2) = 16`! But normally you will only compress by one or not compress at all. The recordings will automatically be decompressed when played or saved. So don't worry about that. Just try out whether the loss in resolution is okay for your needs.
-
-## Stream recordings
-
-A stream in this sense is any object that implements a `send` function that can take a recording. To set a stream pass it to the `ScreenRecorder` constructor.
-
-```python
-class Stream:
-    def send(self,rec):
-        print(f"Recording received with {rec.frame_number} frames, a size of {rec.size} and a total length of {rec.length} s")
-
-my_stream = Stream()
-recorder = ScreenRecorder(stream=my_stream)
-```
-
-Now `recorder.stop_rec()` will send to that stream and also save the recording internally. With `recorder.stop_rec_to_stream(stream = None)` you send to the stream without saving and can optionally specify a stream that will override the recorders default stream.
-
-## Set individual recordings fps
-
-```python
-ScreenRecorder(60).start_rec(30)
-```
-
-will record at 30 fps for this one recording.
-
-## Abort a running recording
-
-`recorder.abort_rec()`
-
-## Get all recordings of a recorder
-
-```python
-all_recordings = recorder.get_recordings()
-```
-
-## Attributes of a recorder
-
-These are the attributes of a `ScreenRecorder` instance. Don't change any of these if you don't have a reason! Create a new recorder instead.
-
-`fps: float`  
-selfexp.
-
-`surf: pg.Surface`  
-selfexp.
-
-`compress: int`  
-selfexp.
-
-`size`: Tuple[int,int]  
-The size (width, height) of the recorded surface. Change this attribute only if you are also manually changing the surface at the same time.
-
-`dt: float`  
-The time between (delta time) two frames in ms.  
-`dt = 1000/fps`
-
-`recordings: List[Recording]`  
-selfexp. Same as `get_recordings()`
-
-## Post-Processing a Recording
-
-1. Add frames
-2. Resize
-3. Apply effects
-
-## Adding frames
-
-You can always append frames to a recording:
-
-`recording.add_frame(frame: pg.Surface)`
-
-## Resize a Recording
-
-You might need to rescale a whole recording to a specific size:
-
-`recording.resize(size: Tuple[int,int])`
-
-## Apply effects
-
-If there is more to do than just resizing:
-
-`recording.apply(effect: Callable[[pg.Surface], pg.Surface])`
-
-Will apply the effect on every frame of the recording.
-
-## Attributes of a recording
-
-These are pretty much the same as the attributes of a ScreenRecorder
-
-`fps: float`  
-selfexp.
-
-`surf: pg.Surface`  
-selfexp.
-
-`compress: int`  
-selfexp.
-
-`size`: Tuple[int,int]  
-selfexp. Change this attribute only if you are also manually changing the frames at the same time (e.g. Applying a resizing filter).
-
-`dt: float`  
-selfexp.
-
-`frames: List[pg.Surface]`  
-selfexp.
-
-# Advanced Saving Options
-
-Introducing the RecordingSaver
-
-`RecordingSaver(recordings: List[Recording], key: str | SupportsIndex | Callable[[int], Optional[Tuple[str,str]]], save_dir: AnyPath = None, blocking: bool = True)`
-
-```python
-recordings = recorder.get_recordings()
-saver = RecordingSaver(recordings, "mp4", "saved_files")
-saver.save()
-```
-
-Saves the given recordings as `mp4` files in `./saved_files`  
-We learned that there is a convenient way to do anything. Just call 
-
-```python
-saved_recordings = recorder.save_recordings("mp4", "saved_files")
-```
-
-## Explanation
-
-- key   
-    You can either give a str, a list or a function  
-    If key is a str that determines the format of the recordings and they will be saved as `recording_0.{key}`,`recording_1.{key}`, etc. 
-    
-    Valid formats are listed if you import `available_formats` from `ScreenRecorder.py`. You can add/update FFmpeg-supported formats by calling `add_codec(format:str, codec: int | str)`.  
-
-    An interesting option to mention is the `npz` file format. It is not a classical video format but actually a way to save numpy arrays (npz = NumPy Zipped). If you don't need to share the recording in the internet or so, this is an efficient alternative. This library has built-in support for replaying these files.    
-
-    If key is a list then the ith recording will be saved as the ith element of the recording. This should be a `(filename,format)` tuple. If an element is `None` the recording will be skipped.   
-
-    It is a very similar case if you give a function. The function gets an int passed and should return `None` or a `(filename,format)` tuple.  
-    An example for such a key is
-
-    ```python
-    key = lambda x: if x%2 == 0 then None else ("recording_{x}","mp4")
-    ```
-
-    This will return `None` (and skip the save) for every recording with an even index. 
-- save_dir  
-The directory where the recordings will be saved. Defaults to the current working directory
-- blocking  
-Whether the save should block. Defaults to True
-
-The save returns a list of paths to the recordings in the given directory. This list will not **always** be the same length as the recordings in the `Recorder` but will only return a list of recordings that were actually saved. 
-
-However, if you set `block = False` the function will return another function that returns the list of paths and must be called before the script ends! Now you might ask yourself why that makes any sense. Here is an example
-
-```python
-# At this point we have a recorder that recorded some recordings
-# Now we want to save the recordings as `mp4` and also as `npz`
-import time #to measure how long the saves took
-
-# A naive approach is this
-start = time.time()
-recorder.save_recordings("mp4","saved_files1")
-recorder.save_recordings("npz","saved_files1")
-print("First save took:",time.time() - start)
-
-# Now we use non-blocking (asynchronous) code
-start = time.time()
-join1 = recorder.save_recordings("mp4","saved_files2",False)
-join2 = recorder.save_recordings("npz","saved_files2",False)
-print("This message doen't have to wait for the save. Instead it comes almost instantly")
-
-time.sleep(2) #We add some more virtual io with time.sleep
-
-# Finally we join the save
-join1()
-join2()
-print("Second save took:",time.time() - start)
-```
-
-The second option is favorable because it takes less time than the first. Unfortunately, I haven't yet implemented a contextmanager for this so you will have to manually join or write your own and contribute to the project. 
-
-## Memory Management
-
-We talked about how to efficiently save your recordings (from a time aspect). But now we talk about how you can reduce memory consumption. Generally all video recordings will be automatically compressed by FFmpeg/numpy. However, there are three ways you can reduce memory consumption:  
-1. Reduce fps. One cool thing about this ScreenRecorder is that you can record at a different framerate than you play the game. For example you can have a game frame rate of 60 fps but only record at 30 fps. This would halve the memory usage in comparison to if you recorded at 60 fps. 
-1. Resize the recording. We already established that you can halve the recording size as often as you like. But this will only reduce memory usage while the program runs. The result will still be saved in the original size. However, you can save the recording in a smaller size by using  
-    `recording.resize(pg.Vector2(recording.size)/your_scale_factor)`  
-    This will actually save and play the recording in that size, which might look very weird. 
-    So you might not actually want to do that. 
-1. Shorten the recording length. You can cut out parts of a recording like this. Lets say you only want the first 300 frames.
-
-    ```python
-    recording[0:300]
-    #This will actually mutate the recording. If you have issues with this then just share your concerns
-    ``` 
-1. Lastly, you can reduce the depth of the recording by reducing the depth of the recorded screen `pg.display.set_mode((900,600),depth=your_depth)`. This will definitely reduce the memory usage while the program is running and it might also reduce the memory usage on the disk. However, decreasing the depth of the screen will also decrease the variety in color. But in most amateur applications this might just not matter anyway because you are not using very nuanced colors.   
-
-# Replay recordings
-
-## First note
-I had already implemented a VideoPlayer that could play a Full HD video (1920x816) pretty well (Thats over 6 MB per frame at 24 fps). However, there were several issues (without much detail):
-1. Missing sound
-1. Memory
-1. Lags/Preloading (combined with Memory)
-
-Finally, I came to the conclusion that it makes no sense to write a VideoPlayer in pure Python. 
-
-## Easiest way to replay a recording
-
-```py
-#easiest
-player = RecordingPlayer(recording).play()
-# with an on_stop callback
-def on_stop(): 
-    print("Playing finished")
-player = RecordingPlayer(recording, on_stop).play()
-# with a different surface
-my_surface = pg.Surface((900,600))
-player = RecordingPlayer(recording, None, my_surface).play()
-```
-Make sure that you are not blitting anything else to the surface. You still have to do the flipping/updating yourself (I figured it would be weird if the player did that for you). 
-
-Very important is that you always `stop` a player in your `finally-clause` even if you normally wait for the player to end. Here a contextmanager might make sense too but I'm tending to rather no. 
-
-## Advanced `RecordingPlayer` Options
-
-## Pausing
-You already know how to start a player. You can also pause the player with `pause`. Playing is also unpausing.
-
-```python
-player.pause() 
-```
-
-## Stopping
-This stops the player. As said above, always stop the player if in doubt. However, don't even try to reuse a manually stopped player. As with other objects just make a new player. It's really simple.
-
-```python
-player.stop()
-```
-
-## Seeking
-Seeking is known from files and means going to a certain position. 
-
-```python
-player.seek(300) # goes to frame 300 / the 301th frame
-player.seekms(3000.0) # goes to second 3 of the recording
-```
-
-## Telling
-Similarly telling is also known from files and means getting the current position. 
-
-```python
-player.tell() # Gets the current position
-player.tellms() # Gets the current position in milliseconds
-```
-
-## Restarting
-This method is a mixture between reviving the player after it stopped and just seeking the very first frame and playing.
-
-```python
-player.restart()
-```
-
-In the future, restart might take a new recording to play. But that is only a thought. 
-## Getting state information
-The player has a `is_` function. There are two reasons for the name
-1. It resolves the conflict with the python keyword `is`
-1. It might make the code more readable, reading `player.is_("playing")` is easy to understand and nicer to implement than making individual function for every possible state
-
-```python
-player.is_("started") 
-player.is_("stopped")  
-player.is_("playing")
-player.is_("paused")
-```
-
-They are all pretty self explanatory. But remember two things:
-1. `player.is_("stopped")` might be the most important state because you shouldn't call any other function when the player is stopped (Except restart and stop).
-1. `is_("paused")` is **not** equal to `not is_("playing")`
-
-## Making use of the `on_stop`
-The `on_stop` is a very powerful tool because callbacks are always cool. Optionally, `on_stop` will be passed the player object itself. So, you can really do anything you want. I wrote three example callbacks which are very likely to be useful to the API user. Don't forget to import them before you use them (They are not included in `*`). 
-1. `play_indefinite` will restart the player indefinitely as long as the player is not stopped manually (Stopping the player manually will overwrite the on_stop).
-
-    ```python
-    player = RecordingPlayer(recording,play_indefinite).play()
-    ``` 
-1. `play_n_times` plays the player `n` times.
-
-    ```python
-    player = RecordingPlayer(recording,play_n_times(5)).play() # plays 5 times
-    ```
-1. `play_n_wrapper` plays the player `n` times but it wraps another function to call each time.  
-To come back to our very first `on_stop`. 
-
-    ```python
-    @play_n_wrapper(5)
-    def on_stop(): 
-        print("Playing finished")
-    player = RecordingPlayer(recording,on_stop).play()
-    ```
-
-## Playing saved npz files
-
-I showed you how to save your recordings as `npz` files. However, you also need to know how to play them back. 
-For this there is a `NPZPlayer` class. It takes a path to a file and extra parameters just like the `RecordingPlayer`
-
-```python
-player = NPZPlayer("my_npz_file.npz", on_stop=my_on_stop).play()
-```
-It implements all the methods a `RecordingPlayer` implements too
-
-# Event Register
-One of my to-dos was an event register. This task is accomplished. Here comes the tutorial for this. 
-
-Let's suppose you are using events and have a deterministic game (No randomness/randomness with a seed). You just need to do four things to record your game. 
-1. `import EventRegister from EventRegister`
-1. Create a new `EventRegister` object
-1. Get your events from the object
-1. Finally, save the registered events.
-
-## Example
-
-```python
-import EventRegister from EventRegister
-
-pg.init()
-
-reg = EventRegister("in","events.json") # save as json
-
-try:
-    running = True
-    while running:
-        time.sleep(0.0099) # 100 fps
-        for event in reg.get_events(): # instead of pg.event.get()
-            if event.type == pg.QUIT:
-                running = False
-            elif event.type == pg.MOUSEBUTTONDOWN:
-                print(event.button,event.pos)
-finally:
-    pg.quit()
-    reg.save()
-```
-
-Now to replay that exact recorded game. Just swap `in` with `out` when instanciating the `reg` object and everything should work exactly as expected.
-
-## Random Seeds
-
-If your game uses randomness - which most games should - it's very simple. 
-This will automatically load or save the seed depending on the mode.  
-
-```python
-reg = EventRegister("in","events.json").seed()
-```
+Metadata-Version: 2.1
+Name: pygame-screen-record
+Version: 0.1.0
+Summary: A package that allows you to record your pygame game
+Author-email: Rashid Harvey <r.harvey@outlook.de>
+Project-URL: Homepage, https://github.com/theRealProHacker/PyGameRecorder
+Project-URL: Bug Tracker, https://github.com/theRealProHacker/PyGameRecorder/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: opencv_python>=4.7.0.68
+Requires-Dist: pygame>=2.1.3
+
+# A Simple pygame ScreenRecorder
+
+## Why you should use pygame ScreenRecorder?
+
+1. Relatively high accuracy
+2. No (noticable) performance issues
+3. Recording FPS is not bound to game FPS
+4. Straightforward usage
+5. The codebase is well commented and typed
+
+## Dependencies
+
+Apart from pygame and python >=3.8
+
+1. opencv-python (includes numpy)
+2. FFmpeg if you want to save videos
+
+## Install
+
+`pip install pygame-screen-record`
+
+## FAQ
+
+See the FAQ [in the wiki](https://github.com/theRealProHacker/PyGameRecorder/wiki/FAQ)
+
+## To-Dos
+
+2. Event recording (mouse, key, quit, etc.) ✔️
+3. Sound recording (Either event based with function hooking or as numpy arrays)
+4. A proper video player
+5. Add a wiki ✔️
+
+## Contributing
+
+File any bugs or feature requests as GitHub issues. Any comments are always welcome. 
+
+# How To Use
+
+Probably you just want to make a recording of their game and save it in a video file. Here comes how.
+
+> Note: I am using `pg` as an alias for `pygame` in the following code snippets
+
+A typical game script might look like this:
+
+```py
+import pygame as pg
+pg.init()
+
+init_code()
+
+try:
+    while True:
+        event_handling()
+        updating()
+        drawing()
+finally:
+    clean_up()
+    pg.quit()
+```
+
+The `try - finally - statement` is very important to catch any exceptions and clean up whether the game ended naturely or not.
+
+Adding a recorder is very simple:
+
+```py
+import pygame as pg
+from pygame_screen_record import ScreenRecorder
+
+pg.init()
+
+init_code()
+
+recorder = ScreenRecorder(60) # Pass your desired fps
+recorder.start_rec() # Start recording
+
+try:
+    while True:
+        event_handling()
+        updating()
+        drawing()
+finally:
+    recorder.stop_rec()	# stop recording
+    recording = recorder.save_recording("my_recording.mp4") # returns a Recording
+    clean_up()
+    pg.quit()
+```
+
+This code will record your screen the whole game and then save it in the current working directory as `my_recording.mp4`.
+Typical values for the frames per second (fps) are 24 (for slow games), 30, 60 and 120 (Most displays only refresh at 60 Hertz, so most users won't see a difference upwards of 60 fps). Don't forget that the fps value is (at least in theory) proportional to the memory consumption of your recording.
+
+One cool thing of many is that you can chain functions. So for example
+
+```py
+recorder = ScreenRecorder(60)
+recorder.start_rec()
+```
+is equivalent to
+
+```py
+recorder = ScreenRecorder(60).start_rec()
+```
+
+and you can also just write: `recorder.stop_rec().save_recording("my_recording.mp4")`
+
+# Advanced Recording Options
+
+Some of the options available:
+
+1. Record multiple recordings
+2. Record any surface
+3. Compress `ScreenRecorders`
+4. Stream recordings (maybe add frame streaming too?)
+5. Apply effects on recordings
+
+## Record multiple recordings
+
+In the example, we only recorded a single recording. However, you can record as many recordings as you like with a single `ScreenRecorder`. To stop and start recordings use `stop_rec` and `start_rec`. You can also abort recordings using `abort_rec`. 
+
+Finally, when you want to save your recordings call `save_recordings("mp4")`. More detailed saving options are given in the next chapter [Advanced Saving Options](#advanced-saving-options). 
+
+## Record any `Surface`
+
+In most cases you want to record the whole screen. But, you can also pass an optional argument `surf` to a `ScreenRecorder`.
+
+```python
+my_surface = pg.surface.Surface((900, 600))
+recorder = ScreenRecorder(60, my_surface)
+```
+
+## Compress recordings
+
+You can choose to compress your recordings like this
+
+```py
+recorder = ScreenRecorder(compress=2) # fps defaults to 60 
+```
+
+What does that mean? It means that every frame will be scaled down `2`-times by two. This reduces the total memory consumption by `2^(2^2) = 16`! But normally you will only compress by one or not compress at all. The recordings will automatically be decompressed when played or saved. So don't worry about that. Just try out whether the loss in resolution is okay for your needs.
+
+## Stream recordings
+
+A stream in this sense is any object that implements a `send` function that can take a recording. To set a stream pass it to the `ScreenRecorder` constructor.
+
+```python
+class Stream:
+    def send(self, rec):
+        print(f"Recording received with {rec.frame_number} frames, a size of {rec.size} and a total length of {rec.length} s")
+
+my_stream = Stream()
+recorder = ScreenRecorder(stream=my_stream)
+```
+
+Now `recorder.stop_rec()` will send to that stream and also save the recording internally. With `recorder.stop_rec_to_stream(stream = None)` you send to the stream without saving and can optionally specify a stream that will override the recorders default stream.
+
+## Set individual recordings fps
+
+```py
+ScreenRecorder(60).start_rec(30)
+```
+
+will record at 30 fps for this one recording.
+
+## Get all recordings of a recorder
+
+```py
+all_recordings = recorder.get_recordings()
+```
+
+## Attributes of a recorder
+
+These are the attributes of a `ScreenRecorder` instance. Don't change any of these if you don't have a reason! Create a new recorder instead.
+
+`fps: float`  
+selfexp.
+
+`surf: pg.Surface`  
+selfexp.
+
+`compress: int`  
+selfexp.
+
+`size: Tuple[int,int]`  
+The size (width, height) of the recorded surface. Change this attribute only if you are also manually changing the surface at the same time.
+
+`dt: float`  
+The time between (delta time) two frames in ms.  
+`dt = 1000/fps`
+
+`recordings: List[Recording]`  
+selfexp. Same as `get_recordings()`
+
+## Post-Processing a recording
+
+1. Add frames
+2. Resize
+3. Apply effects
+
+## Adding frames
+
+You can always append frames to a recording:
+
+`recording.add_frame(frame: pg.Surface)`
+
+## Resize a recording
+
+You might need to rescale a whole recording to a specific size:
+
+`recording.resize(size: Tuple[int,int])`
+
+## Apply effects
+
+If there is more to do than just resizing:
+
+`recording.apply(effect: Callable[[pg.Surface], pg.Surface])`
+
+Will apply the effect on every frame of the recording.
+
+## Attributes of a recording
+
+These are pretty much the same as the attributes of a ScreenRecorder
+
+`fps: float`  
+selfexp.
+
+`surf: pg.Surface`  
+selfexp.
+
+`compress: int`  
+selfexp.
+
+`size: Tuple[int, int]`
+selfexp. Change this attribute only if you are also manually changing the frames at the same time (e.g. Applying a resizing filter).
+
+`dt: float`  
+selfexp.
+
+`frames: List[pg.Surface]`  
+selfexp.
+
+# Advanced Saving Options
+
+Introducing the `RecordingSaver`
+
+`RecordingSaver(recordings: List[Recording], key: str | Sequence[str] | Callable[[int], Optional[str]], save_dir: AnyPath = None, blocking: bool = True)`
+
+```py
+recordings = recorder.get_recordings()
+saver = RecordingSaver(recordings, "mp4", "saved_files")
+saver.save()
+```
+
+Saves the given recordings as `mp4` files in `./saved_files`. But you can also just call
+
+```py
+saved_recordings = recorder.save_recordings("mp4", "saved_files")
+```
+
+## Explanation
+
+- `key`
+    You can either give a str, a list or a function  
+    If key is a str that determines the format of the recordings and they will be saved as `recording_0.{key}`,`recording_1.{key}`, etc. 
+    
+    Valid formats are listed if you call `available_formats()`. You can add/update FFmpeg-supported formats by calling `add_codec(format:str, codec: int | str)`.  
+
+    Maybe its worth to mention the `npz` file format. It is not a classical video format but actually a way to save numpy arrays (npz = **n**um**p**y **z**ipped). If you don't need to share the recording in the internet or so, this is an efficient alternative. Also this library has built-in support for replaying these files.    
+
+    If key is a sequence then the ith recording will be saved as the ith element of the recording. If an element is `None` the according recording will be skipped.   
+
+    It is a very similar case if you give a function. The function gets an int passed and should return `None` or a filename.
+
+    An example for such a key is
+
+    ```python
+    key = lambda x: if x%2 == 0 then None else ("recording_{x}","mp4")
+    ```
+
+    This will return `None` (and skip the save) for every recording with an even index. 
+- `save_dir`  
+The directory where the recordings will be saved. Defaults to the current working directory
+- `blocking`  
+Whether the save should block. Defaults to `True`
+
+The save returns a list of paths to the recordings in the given directory. This list will not **always** be the same length as the recordings in the `Recorder` but will only return a list of recordings that were actually saved. 
+
+However, if you set `block = False` the function will return another function that returns the list of paths and must be called before the script ends! Now you might ask yourself why that makes any sense. Here is an example
+
+```python
+# At this point we have a recorder that recorded some recordings
+# Now we want to save the recordings as `mp4` and also as `npz`
+import time #to measure how long the saves took
+
+# A naive approach is this
+start = time.time()
+recorder.save_recordings("mp4", "saved_files1")
+recorder.save_recordings("npz", "saved_files1")
+print("First save took:", time.time() - start)
+
+# Now we use non-blocking (asynchronous) code
+start = time.time()
+join1 = recorder.save_recordings("mp4", "saved_files2", False)
+join2 = recorder.save_recordings("npz", "saved_files2", False)
+print("This message doen't have to wait for the save. Instead it comes almost instantly")
+
+time.sleep(2) # We add some more virtual io with time.sleep
+
+# Finally we join the save
+join1()
+join2()
+print("Second save took:", time.time() - start)
+```
+
+The second option is favorable because it takes less time than the first. 
+
+## Memory Cosniderations
+
+We talked about how to efficiently save your recordings (from a time aspect). But now we talk about how you can reduce memory consumption. Generally, all video recordings will be automatically compressed by FFmpeg/numpy. However, there are three ways you can reduce memory consumption:  
+1. Reduce fps. One cool thing about this ScreenRecorder is that you can record at a different framerate than you play the game. For example you can have a game frame rate of 60 fps but only record at 30 fps. This would halve the memory usage in comparison to if you recorded at 60 fps. 
+1. Resize the recording. We already established that you can halve the recording size as often as you like. But this will only reduce memory usage while the program runs. The result will still be saved in the original size. However, you can save the recording in a smaller size by using  
+    `recording.resize(pg.Vector2(recording.size)/your_scale_factor)`  
+    This will actually save and play the recording in that size, which might look very weird. 
+    So you might not actually want to do that. 
+1. Shorten the recording length. You can cut out parts of a recording like this. Lets say you only want the first 300 frames.
+
+    ```python
+    # This will actually mutate the recording. 
+    recording[0:300]
+    ``` 
+1. Lastly, you can reduce the depth of the recording by reducing the depth of the recorded screen `pg.display.set_mode((900,600), depth=your_depth)`. This will definitely reduce the memory usage while the program is running and it might also reduce the memory usage on the disk. However, decreasing the depth of the screen will also decrease the variety in color. But in most amateur applications this might just not matter anyway because you are not using very nuanced colors.   
+
+# Replay recordings
+
+## First note
+I had already implemented a VideoPlayer that could play a Full HD video (1920x816) pretty well (Thats over 6 MB per frame at 24 fps). However, there were several issues (without much detail):
+1. Missing sound
+1. Memory
+1. Lags/Preloading (combined with Memory)
+
+Finally, I came to the conclusion that it makes no sense to write a VideoPlayer in pure Python. 
+
+## Easiest way to replay a recording
+
+```py
+# easiest
+player = RecordingPlayer(recording).play()
+
+# with an on_stop callback
+def on_stop(): 
+    print("Playing finished")
+player = RecordingPlayer(recording, on_stop).play()
+
+# with a different surface
+my_surface = pg.Surface((900,600))
+player = RecordingPlayer(recording, None, my_surface).play()
+```
+
+Make sure that you are not blitting anything else to the surface. However, you still have to do the flipping/updating yourself (I figured it would be weird if the player did that for you). 
+
+Very important is that you always `stop` a player in your `finally-clause` even if you normally wait for the player to end. Here a contextmanager might make sense too but I'm tending to rather no. 
+
+# Advanced `RecordingPlayer` Options
+
+## Pausing
+You already know how to start a player. You can also pause the player with `pause`. Playing is also unpausing.
+
+```python
+player.pause() 
+```
+
+## Stopping
+This stops the player. As said above, always stop the player if in doubt. However, don't even try to reuse a manually stopped player. Just make a new player instead, it's really simple.
+
+```python
+player.stop()
+```
+
+## Seeking
+Seeking is known from files and means going to a certain position. 
+
+```python
+player.seek(300) # goes to frame 300 / the 301th frame
+player.seekms(3000.0) # goes to second 3 of the recording
+```
+
+## Telling
+Similarly telling is also known from files and means getting the current position. 
+
+```python
+player.tell() # Gets the current position
+player.tellms() # Gets the current position in milliseconds
+```
+
+## Restarting
+This method is a mixture between reviving the player after it stopped and just seeking the very first frame and playing.
+
+```python
+player.restart()
+```
+
+## Getting state information
+The player has a `is_` function. There are two reasons for the name
+1. It resolves the conflict with the python keyword `is`
+1. It might make the code more readable, reading `player.is_("playing")` is easy to understand and nicer to implement than making individual function for every possible state
+
+```python
+player.is_("started") 
+player.is_("stopped")  
+player.is_("playing")
+player.is_("paused")
+```
+
+They are all pretty self explanatory. But remember two things:
+1. `player.is_("stopped")` might be the most important state because you shouldn't call any other function when the player is stopped (Except restart and stop).
+1. `is_("paused")` is **not** equal to `not is_("playing")` (In the beginning the player is neither playing nor paused)
+
+## Making use of the `on_stop`
+
+The `on_stop` is a very powerful tool because callbacks are always cool. Optionally, `on_stop` will be passed the player object itself. So, you can really do anything you want. I wrote three example callbacks which are very likely to be useful to the API user. Don't forget to import them before you use them (They are not included in `*`). 
+
+1. `play_indefinite` will restart the player indefinitely as long as the player is not stopped manually (Stopping the player manually will overwrite the on_stop).
+
+    ```python
+    player = RecordingPlayer(recording,play_indefinite).play()
+    ``` 
+1. `play_n_times` plays the player `n` times.
+
+    ```python
+    player = RecordingPlayer(recording,play_n_times(5)).play() # plays 5 times
+    ```
+1. `play_n_wrapper` plays the player `n` times but it wraps another function to call each time. To come back to our very first `on_stop`: 
+
+    ```python
+    @play_n_wrapper(5)
+    def on_stop(): 
+        print("Playing finished")
+    player = RecordingPlayer(recording,on_stop).play()
+    ```
+
+## Playing saved npz files
+
+I showed you how to save your recordings as `npz` files. However, you also need to know how to play them back. For this there is a `NPZPlayer` class. It takes a path to a file and extra parameters just like the `RecordingPlayer`
+
+```python
+player = NPZPlayer("my_npz_file.npz", on_stop=my_on_stop).play()
+```
+
+In all other regards it is the same as the `RecprdingPlayer`
+
+# Event Register
+One of my to-dos was an event register. This task is accomplished. Here comes the tutorial for this. 
+
+Let's suppose you are using events and have a deterministic game (No randomness/randomness with a seed). You just need to do four things to record your game. 
+1. `import EventRegister from EventRegister`
+1. Create a new `EventRegister` object
+1. Get your events from the object
+1. Finally, save the registered events.
+
+## Example
+
+```python
+import EventRegister from EventRegister
+
+pg.init()
+
+reg = EventRegister("in","events.json") # save as json
+
+try:
+    running = True
+    while running:
+        time.sleep(0.0099) # 100 fps
+        for event in reg.get_events(): # instead of pg.event.get()
+            if event.type == pg.QUIT:
+                running = False
+            elif event.type == pg.MOUSEBUTTONDOWN:
+                print(event.button,event.pos)
+finally:
+    pg.quit()
+    reg.save()
+```
+
+Now to replay that exact recorded game. Just swap `in` with `out` when instanciating the `reg` object and everything should work exactly as expected.
+
+## Random Seeds
+
+If your game uses randomness - which most games should - it's very simple. 
+This will automatically load or save the seed depending on the mode.  
+
+```python
+reg = EventRegister("in","events.json").seed()
+```
```

### Comparing `pygame-screen-record-0.0.6/tests/test_compress.py` & `pygame_screen_record-0.1.0/tests/test_compress.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import json
-from copy import copy
-from dataclasses import astuple
-
-from pygame_screen_record.EventRegister import (
-    SavedEvent,
-    read,
-    single_compress,
-    single_decompress,
-)
-
-
-def test_compress():
-    file = "events_ex1.json"
-    try:
-        uncomp = read(file)["events"]
-        _comp = [single_compress(SavedEvent(*ev)) for ev in uncomp]
-        comp = [astuple(x) for x in _comp]
-        decomp = [astuple(single_decompress(copy(ev))) for ev in _comp]
-        print("File:", len(json.dumps(uncomp)))
-        print("Compressed:", comp_size := len(json.dumps(comp)))
-        print("Decompressed:", decomp_size := len(json.dumps(decomp)))
-        print(
-            "Compression_rate:",
-            str(comp_rate := (comp_size / decomp_size) * 100) + "%",
-            "(Pretty Good)" if comp_rate <= 60 else "",
-        )
-    except FileNotFoundError:
-        print(
-            f"Test compress failed: Likely {file} missing in current working directory"
-        )
-
-
-if __name__ == "__main__":
-    test_compress()
+import json
+from copy import copy
+from dataclasses import astuple
+
+from pygame_screen_record.EventRegister import (
+    SavedEvent,
+    read,
+    single_compress,
+    single_decompress,
+)
+
+
+def test_compress():
+    file = "events_ex1.json"
+    try:
+        uncomp = read(file)["events"]
+        _comp = [single_compress(SavedEvent(*ev)) for ev in uncomp]
+        comp = [astuple(x) for x in _comp]
+        decomp = [astuple(single_decompress(copy(ev))) for ev in _comp]
+        print("File:", len(json.dumps(uncomp)))
+        print("Compressed:", comp_size := len(json.dumps(comp)))
+        print("Decompressed:", decomp_size := len(json.dumps(decomp)))
+        print(
+            "Compression_rate:",
+            str(comp_rate := (comp_size / decomp_size) * 100) + "%",
+            "(Pretty Good)" if comp_rate <= 60 else "",
+        )
+    except FileNotFoundError:
+        print(
+            f"Test compress failed: Likely {file} missing in current working directory"
+        )
+
+
+if __name__ == "__main__":
+    test_compress()
```

