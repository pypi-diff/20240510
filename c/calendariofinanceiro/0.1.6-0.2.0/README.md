# Comparing `tmp/calendariofinanceiro-0.1.6.tar.gz` & `tmp/calendariofinanceiro-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendariofinanceiro-0.1.6.tar", max compression
+gzip compressed data, was "calendariofinanceiro-0.2.0.tar", max compression
```

## Comparing `calendariofinanceiro-0.1.6.tar` & `calendariofinanceiro-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0       76 2023-08-28 20:15:59.350856 calendariofinanceiro-0.1.6/calendariofinanceiro/__init__.py
--rw-r--r--   0        0        0     4431 2024-04-25 19:28:25.810759 calendariofinanceiro-0.1.6/calendariofinanceiro/calendariofinanceiro.py
--rw-r--r--   0        0        0    22770 2023-08-28 20:15:25.257097 calendariofinanceiro-0.1.6/calendariofinanceiro/feriados.py
--rw-r--r--   0        0        0      113 2023-08-28 17:52:08.907154 calendariofinanceiro-0.1.6/calendariofinanceiro/feriados.pyi
--rw-r--r--   0        0        0     1093 2023-08-28 17:17:50.061981 calendariofinanceiro-0.1.6/LICENSE
--rw-r--r--   0        0        0      809 2024-04-25 19:29:47.346297 calendariofinanceiro-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2248 2023-08-29 18:51:55.681718 calendariofinanceiro-0.1.6/README.md
--rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 calendariofinanceiro-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       76 2023-08-28 20:15:59.350856 calendariofinanceiro-0.2.0/calendariofinanceiro/__init__.py
+-rw-r--r--   0        0        0     4406 2024-05-10 14:05:30.450600 calendariofinanceiro-0.2.0/calendariofinanceiro/calendariofinanceiro.py
+-rw-r--r--   0        0        0     5358 2024-05-10 14:08:32.751449 calendariofinanceiro-0.2.0/calendariofinanceiro/feriados_off.py
+-rw-r--r--   0        0        0      117 2024-05-10 14:02:15.656045 calendariofinanceiro-0.2.0/calendariofinanceiro/feriados_off.pyi
+-rw-r--r--   0        0        0    22773 2024-05-10 14:02:15.671935 calendariofinanceiro-0.2.0/calendariofinanceiro/feriados_on.py
+-rw-r--r--   0        0        0      116 2024-05-10 14:01:44.354773 calendariofinanceiro-0.2.0/calendariofinanceiro/feriados_on.pyi
+-rw-r--r--   0        0        0     1093 2023-08-28 17:17:50.061981 calendariofinanceiro-0.2.0/LICENSE
+-rw-r--r--   0        0        0      809 2024-05-10 14:08:32.730492 calendariofinanceiro-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2248 2023-08-29 18:51:55.681718 calendariofinanceiro-0.2.0/README.md
+-rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 calendariofinanceiro-0.2.0/PKG-INFO
```

### Comparing `calendariofinanceiro-0.1.6/calendariofinanceiro/calendariofinanceiro.py` & `calendariofinanceiro-0.2.0/calendariofinanceiro/calendariofinanceiro.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from datetime import date
 from typing import Literal, List
 import workdays
 
-from calendariofinanceiro.feriados import feriados
+from calendariofinanceiro.feriados_on import feriados_on
+from calendariofinanceiro.feriados_off import feriados_off
 
 
 class CalendarioFinanceiro:
     def __init__(self, calendario: Literal["onshore", "offshore"]):
         if calendario == "onshore":
-            self.feriados = feriados
+            self.feriados = feriados_on
         elif calendario == "offshore":
-            self.feriados = []
+            self.feriados = feriados_off
 
     def soma_dias_uteis(self, data_dt: date, dias: int) -> date:
         """
         Soma um número específico de dias úteis a uma data de referência.
 
         :param data_dt: A data de referência.
         :param dias: O número de dias úteis a serem adicionados
@@ -33,17 +34,15 @@
 
         :param data_dt: A data de referência para o arredondamento.
         :param arredonda_pra_cima: Se True, arredonda para o próximo dia útil.
         Caso contrário, arredonda para o último dia útil.
         :return: A nova data após arredondamento
         """
         offset = 1 if arredonda_pra_cima else -1
-        return self.soma_dias_uteis(
-            self.soma_dias_uteis(data_dt, -offset), offset
-        )
+        return self.soma_dias_uteis(self.soma_dias_uteis(data_dt, -offset), offset)
 
     def monta_lista_dias_uteis(
         self,
         data_inicial: date,
         data_final: date,
         incluir_primeira: bool = True,
     ) -> List[date]:
@@ -78,39 +77,33 @@
          as datas de fechamento serão geradas.
         :return: Uma lista de datas de fechamento retroativas.
         """
         lista_fechamentos = []
         data_i = data_final
         for i in range(numero_meses):
             lista_fechamentos.append(data_i)
-            data_i = self.soma_dias_uteis(
-                date(data_i.year, data_i.month, 1), -1
-            )
+            data_i = self.soma_dias_uteis(date(data_i.year, data_i.month, 1), -1)
         return lista_fechamentos
 
     def fechamento_mes_anterior(self, data: date) -> date:
         """
         Retorna a data de fechamento do mês anterior à data fornecida.
 
         :param data: A data de referência para a qual se deseja obter
         o fechamento do mês anterior.
         :return: A data de fechamento do mês anterior.
         """
-        fechamento_m1 = self.soma_dias_uteis(
-            date(data.year, data.month, 1), -1
-        )
+        fechamento_m1 = self.soma_dias_uteis(date(data.year, data.month, 1), -1)
         return fechamento_m1
 
     def busca_fechamento_mes_ano(self, mes: int, ano: int) -> date:
         """
         A partir de um mês e ano, constrói a data de fechamento referente.
 
         :param mes: Mês de referência do fechamento (Janeiro=1)
         :param ano: Ano de referência do fechamento
         :return: A data de fechamento correspondente ao mês e ano passados.
         """
         proximo_mes = mes + 1 if mes < 12 else 1
         proximo_ano = ano if mes < 12 else ano + 1
-        fechamento = self.soma_dias_uteis(
-            date(proximo_ano, proximo_mes, 1), -1
-        )
+        fechamento = self.soma_dias_uteis(date(proximo_ano, proximo_mes, 1), -1)
         return fechamento
```

### Comparing `calendariofinanceiro-0.1.6/calendariofinanceiro/feriados.py` & `calendariofinanceiro-0.2.0/calendariofinanceiro/feriados_on.py`

 * *Files 0% similar despite different names*

```diff
@@ -1187,8 +1187,8 @@
     "2099-06-11",
     "2099-09-07",
     "2099-10-12",
     "2099-11-02",
     "2099-11-15",
     "2099-12-25",
 }
-feriados = [date.fromisoformat(feriado) for feriado in feriados_str]
+feriados_on = [date.fromisoformat(feriado) for feriado in feriados_str]
```

### Comparing `calendariofinanceiro-0.1.6/LICENSE` & `calendariofinanceiro-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calendariofinanceiro-0.1.6/pyproject.toml` & `calendariofinanceiro-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calendariofinanceiro"
-version = "0.1.6"
+version = "0.2.0"
 description = "O pacote CalendarioFinanceiro é uma ferramenta Python projetada para facilitar a manipulação de datas financeiras em diferentes calendários, como 'onshore' (Brasil) e 'offshore'. Com este pacote, você pode realizar operações como adicionar dias úteis a uma data, criar listas de dias úteis entre intervalos de datas e muito mais. Ele é uma solução eficiente para lidar com cálculos de datas em cenários financeiros, onde a consideração de dias úteis e feriados é essencial."
 authors = ["eduardo.barreto <edugobarreto@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 workdays = "^1.4"
```

### Comparing `calendariofinanceiro-0.1.6/README.md` & `calendariofinanceiro-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `calendariofinanceiro-0.1.6/PKG-INFO` & `calendariofinanceiro-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendariofinanceiro
-Version: 0.1.6
+Version: 0.2.0
 Summary: O pacote CalendarioFinanceiro é uma ferramenta Python projetada para facilitar a manipulação de datas financeiras em diferentes calendários, como 'onshore' (Brasil) e 'offshore'. Com este pacote, você pode realizar operações como adicionar dias úteis a uma data, criar listas de dias úteis entre intervalos de datas e muito mais. Ele é uma solução eficiente para lidar com cálculos de datas em cenários financeiros, onde a consideração de dias úteis e feriados é essencial.
 Author: eduardo.barreto
 Author-email: edugobarreto@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

