# Comparing `tmp/pih-mio-0.29.5.tar.gz` & `tmp/pih-mio-0.29.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-0.29.5.tar", last modified: Thu Apr 25 05:26:58 2024, max compression
+gzip compressed data, was "pih-mio-0.29.8.tar", last modified: Thu May  9 23:26:41 2024, max compression
```

## Comparing `pih-mio-0.29.5.tar` & `pih-mio-0.29.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 05:26:58.157224 pih-mio-0.29.5/
-drwxrwxrwx   0        0        0        0 2024-04-25 05:26:57.741736 pih-mio-0.29.5/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.29.5/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.29.5/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   371077 2024-04-25 04:56:03.000000 pih-mio-0.29.5/MobileHelperService/api.py
--rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.29.5/MobileHelperService/client.py
--rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.29.5/MobileHelperService/collection.py
--rw-rw-rw-   0        0        0     4462 2024-04-25 05:26:24.000000 pih-mio-0.29.5/MobileHelperService/const.py
--rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.29.5/MobileHelperService/service.py
--rw-rw-rw-   0        0        0    17336 2024-04-25 04:48:36.000000 pih-mio-0.29.5/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      331 2024-04-25 05:26:58.110334 pih-mio-0.29.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 05:26:58.063430 pih-mio-0.29.5/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      331 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-25 05:26:57.000000 pih-mio-0.29.5/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 05:26:58.157224 pih-mio-0.29.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 23:26:41.639765 pih-mio-0.29.8/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:26:40.894905 pih-mio-0.29.8/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.29.8/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.29.8/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   372866 2024-05-08 14:50:01.000000 pih-mio-0.29.8/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.29.8/MobileHelperService/client.py
+-rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.29.8/MobileHelperService/collection.py
+-rw-rw-rw-   0        0        0     4462 2024-05-09 23:22:09.000000 pih-mio-0.29.8/MobileHelperService/const.py
+-rw-rw-rw-   0        0        0      910 2024-05-09 23:19:54.000000 pih-mio-0.29.8/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0    17628 2024-05-09 23:18:14.000000 pih-mio-0.29.8/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      331 2024-05-09 23:26:41.624127 pih-mio-0.29.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 23:26:41.558324 pih-mio-0.29.8/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      331 2024-05-09 23:26:39.000000 pih-mio-0.29.8/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 23:26:41.655391 pih-mio-0.29.8/setup.cfg
```

### Comparing `pih-mio-0.29.5/MobileHelperService/api.py` & `pih-mio-0.29.8/MobileHelperService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,30 +107,28 @@
     def b(self, value: str) -> str:
         return b(value)
 
     def i(self, value: str) -> str:
         return i(value)
 
 
-SIMPLE_OUTPUT: MobileOutputBase = MobileOutputBase()
-
 def format_given_name(
     session: Session, output: Output, name: str | None = None
 ) -> str | None:
     if e(session.login):
         return None
     return output.bold(name or session.user_given_name)
 
 
 def get_wappi_status(space: str, value: A.CT_ME_WH_W.Profiles) -> str:
-    lines: list[str] = A.D_F.wappi_status(value, SIMPLE_OUTPUT).splitlines()
+    lines: list[str] = A.D_F.wappi_status(value).splitlines()
     return jnl(
         (
             j((" ", A.CT_V.BLUE_ROMB, " ", lines[0])),
-            jnl((A.D.map(lambda item: j((space, " ", item)), lines[1:]))),
+            jnl((A.D.map(lambda item: js((space, item)), lines[1:]))),  # type: ignore
         )
     )
 
 
 class MobileHelperUserSettiongsHolder:
     @staticmethod
     def get(login: str) -> MobileHelperUserSettings:
@@ -173,27 +171,27 @@
 def get_command_base_name(value: str) -> str:
     return value.split(COMMAND_NAME_VARIANT_SPLITTER)[0]
 
 
 def get_command_variant_name(value: str | None) -> str:
     if n(value):
         return ""
-    return value.replace(COMMAND_NAME_VARIANT_SPLITTER, "")
+    return nns(value).replace(COMMAND_NAME_VARIANT_SPLITTER, "")
 
 
 def command_node_name_equal(value1: str, value2: str) -> bool:
     return A.D.equal(value1, get_command_base_name(value2)) or A.D.equal(
         value1, get_command_variant_name(value2)
     )
 
 
 def mio_command(value: list[str] | str) -> str:
     if isinstance(value, str):
         return get_command_base_name(value)
-    return mio_command(one(value))
+    return mio_command(nnt(one(value)))
 
 
 def flag_name_list(value: Flags, all: bool = False) -> list[str]:
     result: list[str] = [
         item[0]
         for item in A.D.filter(lambda item: item[1] == value, list(FLAG_MAP.items()))
     ]
@@ -287,17 +285,15 @@
 class MobileMarkOutput(MarkOutput):
     def result(
         self,
         result: Result[list[Mark]],
         caption: str | None = None,
         use_index: bool = False,
     ) -> None:
-        if ne(caption):
-            self.parent.write_line(self.parent.bold(caption))
-        self.parent.write_result(result, use_index=use_index)
+        self.parent.write_result(result, use_index=use_index, title=caption)
 
 
 @dataclass
 class MessageHolder:
     body: str | None = None
     text_before: str = ""
 
@@ -367,16 +363,21 @@
         text: str,
         text_before: str | None = None,
         text_after: str | None = None,
     ) -> str:
         return text
 
     def whatsapp_send(self, text: str) -> bool:
-        #A.L.debug_bot(text)
-        return A.ME_WH_W.send(self.get_recipient(), text, self.profile)
+        # A.L.debug_bot(text)
+        return A.ME_WH_W.send(
+            self.get_recipient(), A.D_F.whatsapp_message(text), self.profile
+        )
+
+    def index_str(self, index: int, text: str, max_index: int | None = None) -> str:
+        return j(("<li>", super().index_str(index, text, max_index), "</li>"))
 
     @contextmanager
     def make_send_to_group(self, group: A.CT.MESSAGE.WHATSAPP.GROUP):
         try:
             while_not_do(lambda: e(self.message_buffer))
             self.recipient = A.D.get(group)
             yield True
@@ -539,15 +540,15 @@
         return A.ME_WH_W.send_video(
             self.session.recipient, caption, video_content, self.profile
         )
 
     def write_image(self, caption: str, image_content: str) -> bool:
         return A.ME_WH_W.send_image(
             self.session.recipient,
-            j((self.text_before, caption)),
+            A.D_F.whatsapp_message(j((self.text_before, caption))),
             image_content,
             self.profile,
         )
 
     def write_document(
         self, caption: str, file_name: str, document_content: str
     ) -> None:
@@ -620,24 +621,27 @@
 
     def separated_line(self) -> None:
         self.type = BM.add(self.type, MessageType.SEPARATE_ONCE)
 
     def header(self, value: str) -> None:
         self.write_line(js(("", A.CT_V.BULLET, nl(self.bold(value)))))
 
-    def bold(self, value: str) -> str:
-        return b(value)
+    def bold(self, value: Any) -> str:
+        return j(("<b>", value, "</b>"))
 
-    def italic(self, value: str) -> str:
-        return i(value)
+    # b(value)
+
+    def italic(self, value: Any) -> str:
+        return j(("<i>", value, "</i>"))
+        # i(value)
 
     def free_marks_by_group_for_result(
         self, group: MarkGroup, result: Result, use_index: bool
     ) -> None:
-        group_name: str = group.GroupName
+        group_name: str = nns(group.GroupName)
         self.write_line(
             js(
                 (
                     "Свободные карты доступа для группы доступа",
                     j((esc(group_name), ":")),
                 )
             )
@@ -653,29 +657,29 @@
         self,
         result: Result,
         caption: str | None = None,
         use_index: bool = False,
         modify_table_function: Callable | None = None,
         label_function: Callable | None = None,
     ) -> None:
-        if caption is not None:
-            self.write_line(nl(caption))
+        if nn(caption):
+            self.write_line(nl(nnt(caption)))
         is_result_type: bool = isinstance(result, Result)
         field_list = result.fields if is_result_type else result.fields
         data: Any = result.data if is_result_type else result.data
         if e(data):
             self.error("Не найдено!")
         else:
             if not isinstance(data, list):
                 data = [data]
             length: int = len(data)
             if length == 1:
                 use_index = False
             if use_index:
-                field_list.list.insert(0, A.CT_FC.INDEX)
+                nnt(field_list.list).insert(0, A.CT_FC.INDEX)
             item_data: Any = None
             result_text_list: list[list[str]] = []
             for index, item in enumerate(data):
                 row_data: list = []
                 for field_item_obj in field_list.get_list():
                     field_item: FieldItem = field_item_obj
                     if field_item.visible:
@@ -687,39 +691,39 @@
                                     len(str(length))
                                     - len(str(index + 1))
                                     + 1
                                     + (1 if index < 9 and len(str(length)) > 1 else 0)
                                 )
                             )
                         elif not isinstance(item, dict):
-                            if label_function is not None:
+                            if nn(label_function):
                                 modified_item_data = label_function(field_item, item)
-                                if modified_item_data is None:
+                                if n(modified_item_data):
                                     modified_item_data = getattr(item, field_item.name)
                                 row_data.append(
                                     A.D.check(
                                         modified_item_data,
                                         lambda: modified_item_data,
                                         "",
                                     )
-                                    if modified_item_data is None
+                                    if n(modified_item_data)
                                     else modified_item_data
                                 )
                             else:
                                 item_data = getattr(item, field_item.name)
                                 row_data.append(
                                     A.D.check(item_data, lambda: item_data, "")
                                 )
                         elif field_item.name in item:
                             item_data = item[field_item.name]
-                            if label_function is not None:
+                            if nn(label_function):
                                 modified_item_data = label_function(field_item, item)
                                 row_data.append(
                                     item_data
-                                    if modified_item_data is None
+                                    if n(modified_item_data)
                                     else modified_item_data
                                 )
                             else:
                                 row_data.append(item_data)
                 row_data = A.D.map(lambda item: str(item), row_data)
                 result_text_list.append(row_data)
             self.write_line(
@@ -920,33 +924,37 @@
         self.answer = self.input(text).lower().strip()
         return (
             (
                 self.answer in YES_VARIANTS
                 if default_yes_label
                 else self.answer not in ["0", "no", "нет"]
             )
-            if yes_checker is None
+            if n(yes_checker)
             else yes_checker(self.answer)
         )
 
     def item_by_index(
         self,
         caption: str,
         data: list[Any],
         label_function: Callable[[Any, int], str] | None = None,
         use_zero_index: bool = False,
         allow_choose_all: bool = False,
+        sticky_items: tuple[int, ...] | None = None,
+        # simple_integer_parse: bool = True,
     ) -> Any:
         with self.make_type(INPUT_TYPE.INDEX):
             return super().item_by_index(
                 j((caption, ", отправив число")),
                 data,
                 label_function,
                 use_zero_index,
                 allow_choose_all,
+                sticky_items,
+                # simple_integer_parse,
             )
 
     def interrupt_for_new_command(self) -> None:
         self.stdin.interrupt_type = InterruptionTypes.NEW_COMMAND
 
     def interrupt(self) -> None:
         self.stdin.interrupt_type = InterruptionTypes.EXIT
@@ -988,15 +996,15 @@
         )
 
 
 @dataclass
 class CommandNode:
     name_list: list[str] | None = None
     title_and_label: list[str] | Callable[[], list[str]] | None = None
-    handler: Callable[[], None] | None = None
+    handler: Callable[[], Any] | None = None
     allowed_groups: list[Groups] | None = None
     wait_for_input: bool = True
     show_in_main_menu: bool = False
     parent: Any = None
     text: str | Callable[[], str] | None = None
     visible: bool = True
     show_always: bool = False
@@ -1122,14 +1130,15 @@
     if e(value):
         return None
     for file_pattern_index, pattern in enumerate(FILE_PATTERN_LIST):
         if nnt(value).find(pattern) == 0:
             return file_pattern_index
     return None
 
+
 class MobileHelper(OutputStub):
 
     command_base_name_collection: tuple[str, ...] | None = None
     command_node_name_collection: tuple[str, ...] | None = None
     allowed_group_collection: set[Groups] | None = None
 
     def flag_string_represent(self, value: Flags, all: bool = True) -> str:
@@ -1923,15 +1932,21 @@
         ]
         self.menu.journals = [add_journal_record_node, show_journal_node]
         #######################
         call_centre_unit_node: CommandNode = CommandNode(
             ["callcentre", "колл-центр"],
             ["Колл-центр"],
             lambda: self.menu_handler(self.menu.call_centre),
-            text=f"Алло, алло... С этих слов начинается общение наших клиентов c колцентром. Работники коллцентра принимают звонки и работают с запросами от клиентов и в этом им помогает:\n\n{A.CT.VISUAL.BULLET} программа *Инфинити*, отвечающая за звонки\n{A.CT.VISUAL.BULLET} программа *Полибейс*, в которой заноситься информация о клиенте\n{A.CT.VISUAL.BULLET} браузер *Google Chrome*, с набором ресурсов\n\nНиже представлены курсы по всем трем программам.",
+            text=jnl(
+                (
+                    A.D_F.wappi_status(A.CT_ME_WH_W.Profiles.CALL_CENTRE),
+                    "",
+                    f"Алло, алло... С этих слов начинается общение наших клиентов c колцентром. Работники коллцентра принимают звонки и работают с запросами от клиентов и в этом им помогает:\n\n{A.CT.VISUAL.BULLET} программа *Инфинити*, отвечающая за звонки\n{A.CT.VISUAL.BULLET} программа *Полибейс*, в которой заноситься информация о клиенте\n{A.CT.VISUAL.BULLET} браузер *Google Chrome*, с набором ресурсов\n\nНиже представлены курсы по всем трем программам.",
+                )
+            ),
         )
         it_unit_node: CommandNode = CommandNode(
             ["it", "ит"],
             ["ИТ отдел"],
             lambda: self.menu_handler(self.menu.it),
             text=self.get_it_telephone_number_text,
         )
@@ -1997,15 +2012,15 @@
                 (
                     "Руководитель: ",
                     self.output.bold(
                         one(A.R_U.by_job_position(A.CT_AD.JobPositions.MARKETER)).name
                     ),
                     ".",
                     nl() * 2,
-                    A.D_F.wappi_status(A.CT_ME_WH_W.Profiles.MARKETER, self.output),
+                    A.D_F.wappi_status(A.CT_ME_WH_W.Profiles.MARKETER),
                 )
             ),
         )
         self.menu.unit = [
             it_unit_node,
             call_centre_unit_node,
             hr_unit_node,
@@ -2030,15 +2045,15 @@
         #######################
         polibase_person_information_node: CommandNode = CommandNode(
             ["info|rmation", "инфо|рмация"],
             lambda: [
                 "Информация о пациенте",
                 "Информация" + (" о пациенте" if self.in_choose_command else ""),
             ],
-            self.polibase_person_show_information_handler,
+            self.polibase_person_information_show_handler,
         )
         polibase_doctor_visits_node: CommandNode = CommandNode(
             ["visit|s", "приём|ы", "визит|ы", "прием|ы"],
             lambda: ["Список моих приёмов", "Показать список моих приёмов"],
             self.polibase_visit_handler,
             filter_function=lambda: self.am_i_doctor,
         )
@@ -2409,15 +2424,15 @@
         #######################
         polibase_restart_node: CommandNode = CommandNode(
             ["restart", "перезагруз|ить"],
             A.D.map(
                 lambda item: js((item, "Polibase")),
                 ["Перезагрузка сервера", "Перезагрузить сервер"],
             ),
-            self.console_apps_api.polibase_restart,
+            lambda: self.console_apps_api.polibase_restart(self.is_test),
             ADMIN_GROUPS,
         )
         polibase_show_password_node: CommandNode = CommandNode(
             self.keywords.command.PASSWORD,
             lambda: (
                 [
                     "Пароль пользователя Полибейс",
@@ -2800,22 +2815,25 @@
                                 nl("или"),
                                 "   ",
                                 A.CT_V.BULLET,
                                 " ",
                                 self.output.bold("П"),
                                 " асифик ",
                                 self.output.bold("И"),
-                                " нтернейшнл ",
+                                " нтернешнл ",
                                 self.output.bold("Х"),
                                 nl(" оспитал.", count=2),
-                                self.output.bold("Автор: "),
+                                self.output.bold("Автор"),
+                                ": ",
                                 nl("Караченцев Никита Александрович"),
-                                self.output.bold("Версия: "),
+                                self.output.bold("Версия"),
+                                ": ",
                                 nl(VERSION),
-                                self.output.bold("Сервер: "),
+                                self.output.bold("Сервер"),
+                                ": ",
                                 A.SYS.host(),
                                 nl(),
                                 LINE,
                                 nl(),
                                 get_wappi_status("  ", A.CT_ME_WH_W.Profiles.IT),
                                 nl() * 2,
                                 get_wappi_status(
@@ -3521,15 +3539,15 @@
     def output(self) -> MobileOutput:
         return self.pih.output
 
     @property
     def input(self) -> MobileInput:
         return self.pih.input
 
-    def bold(self, value: str) -> str:
+    def bold(self, value: Any) -> str:
         return self.output.bold(value)
 
     @property
     def arg_list_exclude_file(self) -> list[str]:
         return A.D.filter(
             lambda item: not item.startswith(FILE_PATTERN_LIST), self.arg_list
         )
@@ -3546,15 +3564,15 @@
         filter_function: Callable[[str], bool] | None = None,
     ) -> Any:
         result: str | None = (
             A.D.by_index(
                 (
                     self.arg_list
                     if n(filter_function)
-                    else A.D.filter(filter_function, self.arg_list)
+                    else A.D.filter(filter_function, self.arg_list)  # type: ignore
                 ),
                 index,
                 default_value,
             )
             if e(self.session.arg_list or [])
             else self.session.arg(index, default_value)
         )
@@ -3576,15 +3594,15 @@
 
     @property
     def in_all_commands(self) -> bool:
         return self.in_main_menu and self.is_all
 
     @property
     def argless(self) -> bool:
-        return self.arg_len == 0
+        return self.arg_len == 0  # or (self.arg_len == 1 and n(self.arg_list[0]))
 
     def drop_args(self) -> None:
         self.session.arg_list = []
         self.arg_list = []
 
     def zabbix_help(self) -> str:
         return jnl(
@@ -3613,15 +3631,15 @@
 
     def zabbix_command_handler(self) -> None:
         self.console_apps_api.show_zabbix()
 
     def get_joke_handler(self, set_settings: bool = False) -> None:
         if set_settings:
             if A.C_U.has_property(
-                self.session.user,
+                nnt(self.session.user),
                 A.CT_AD_UP.Jokeless,
             ):
                 self.output.error(
                     j(
                         (
                             "Отправка анегдота при входе или выходе отключена Администратором.",
                             nl(),
@@ -3862,28 +3880,28 @@
                         j(("lower(use_name)=", escs(value))),
                         js(("lower(use_cliname) like", escs(j(("%", value, "%"))))),
                     ),
                     " or ",
                 )
             )
         else:
-            result = get_by_login(self.session.login)  # type: ignore
+            result = get_by_login(nns(self.session.login))
         if e(result):
             self.output.error("Пользователь Полибейс не найден")
         else:
             self.write_line(
                 j(
                     (
                         self.output.bold("Логин"),
                         ": ",
-                        result[LOGIN],
+                        nnt(result)[LOGIN],
                         nl(),
                         self.output.bold("Пароль"),
                         ": ",
-                        result[PASSWORD],
+                        nnt(result)[PASSWORD],
                     )
                 )
             )
 
     def robocopy_job_run_handler(self) -> None:
         forced: bool = self.is_forced
         source_job_name: str | None = None
@@ -3968,15 +3986,15 @@
                 A.D_F_B.job_full_name(name, source, destination)
             ]
             status: int | None = None
             date: str | None = None
             if job_status.active:
                 date = self.output.bold("выполняется")
             else:
-                if job_status.last_created is not None:
+                if nn(job_status.last_created):
                     date = A.D_F.datetime(job_status.last_created)
                 status = job_status.last_status
             return j(
                 (
                     j(
                         (
                             "   ",
@@ -4166,24 +4184,24 @@
         )
 
     def under_construction_handler(self) -> None:
         self.output.error(f"Извините, {self.user_given_name}, раздел в разработке 😞")
 
     def user_property_set_handler(self, index: int | None = None) -> None:
         action_list: FieldItemList = A.CT_FC.AD.USER_ACTION
-        if index is not None:
+        if nn(index):
             if index < 0 or index >= action_list.length():
                 index = None
         if index == 0 and self.is_all:
             self.console_apps_api.start_user_telephone_number_editor()
         else:
             self.console_apps_api.start_user_property_setter(
                 (
                     self.input.indexed_field_list("Выберите действие", action_list)
-                    if index is None
+                    if n(index)
                     else action_list.get_name_list()[index]
                 ),
                 self.arg(),
                 True,
             )
 
     @property
@@ -4533,30 +4551,35 @@
             self.output.error("Ничего не найдено")
 
     def who_handler(self) -> None:
         was_found: bool = False
         with self.output.make_allow_show_error(False):
             value: str = self.arg() or self.input.input("Введите поисковый запрос")
             if lw(value) == "я":
-                value = self.session.login
+                value = self.session.user.name
             try:
                 self.user_find_handler(value)
                 was_found = True
             except NotFound as _:
                 pass
+            try:
+                self.mark_find_handler(value)
+                was_found = True
+            except NotFound as _:
+                pass
             if A.C_P.person_pin(value):
                 try:
-                    self.polibase_person_show_information_handler(
-                        value, show_title=True
+                    self.polibase_person_information_show_handler(
+                        value, show_title=True, raise_exception=True
                     )
                     was_found = True
                 except NotFound as _:
                     pass
         if not was_found:
-            self.output.error("Ничего не найдена")
+            self.output.error("Никто не найден")
 
     def run_command_handler(self, command_type: A.CT_CMDT | None = None) -> None:
         def filter_function(item: Note) -> bool:
             title_list: list[str] = item.title.split(A.CT.SPLITTER)  # type: ignore
             if len(title_list) > 1:
                 return title_list[0].lower() in A.D.get(command_type)[1:]
             return True
@@ -4886,15 +4909,17 @@
                         line_count += 1
                     command_part_item: str = extract_parameters(
                         text or jnl(command_line_list)
                     )
                     command_result: str | None = None
                     try:
                         command_result = A.EXC.execute_python_localy(
-                            command_part_item, {"self": self}, catch_exceptions=True
+                            command_part_item,
+                            {"self": self, "parameters": self.arg_list},
+                            catch_exceptions=True,
                         )
                     except Exception as exception:
                         if isinstance(exception, InternalInterrupt):
                             raise exception
                         self.output.error(jnl(traceback.format_exception(exception)))
                         with self.output.make_separated_lines():
                             self.write_line(text)
@@ -5500,15 +5525,14 @@
         self.console_apps_api.who_lost_the_mark(self.arg())
 
     def marketer_review_statistics_handler(self) -> None:
         self.execute_python_file(
             "marketer_statistics_create",
             redirect_to_mobile_output=True,
         )
-        # A.R_F.execute("doctor_list_review_partipant")
 
     def marketer_review_settings_handler(self) -> None:
         def show_settings() -> None:
             self.write_line(
                 js(
                     (
                         "Состояние:",
@@ -5773,20 +5797,20 @@
                             (
                                 self.user_given_name,
                                 ", спасибо, что прошли обучайющий курс!",
                             )
                         )
                     )
             elif action_index == 2:
-                if node_list is not None:
+                if nn(node_list):
                     main_title: str | None = self.get_command_title(
                         self.current_command
                     )
                     if ne(main_title):
-                        self.output.head(main_title) is not None
+                        self.output.head(main_title)
                     self.study_course_handler(
                         self.input.index(
                             "Пожалуйста, выберите раздел обучения",
                             A.D.to_list(node_list, True),
                             lambda item, _: self.output.bold(
                                 self.get_command_node_title(item)
                             ),
@@ -5818,19 +5842,21 @@
                     self.output.head(j(("Раздел ", index + 1, ": ", main_title)))
                 content: list[Callable[[], str]] = help_content_holder.content
                 len_content: int = len(content)
                 for index, content_item in enumerate(content):
                     content_item: HelpContent = content_item
                     text: str | None = content_item.text
                     title: str | None = content_item.title or main_title
-                    if text is not None:
+                    if nn(text):
                         self.write_line(nl(text))
                     self.output.separated_line()
-                    content_link: Callable[[], str] | IndexedLink = content_item.content
-                    if content_link is not None:
+                    content_link: Callable[[], str] | IndexedLink | None = (
+                        content_item.content
+                    )
+                    if nn(content_link):
                         content_body: str | None = None
                         if callable(content_link):
                             content_body = content_link()
                         else:
                             content_body = getattr(
                                 content_link.object,
                                 f"{content_link.attribute}{index + 1}",
@@ -6657,24 +6683,24 @@
                         )
             return result
 
         self.output.write_result(
             it_user_list,
             False,
             label_function=label_function,
-            title=nl("ИТ отдел это:"),
+            title="ИТ отдел это:",
             separated_result_item=True,
         )
         self.write_line(self.get_it_telephone_number_text())
 
     def user_find_handler(self, value: str | None = None) -> None:
-        self.console_apps_api.find_user(value or self.arg())
+        self.console_apps_api.user_find(value or self.arg())
 
-    def find_mark_handler(self) -> None:
-        self.console_apps_api.mark_find(self.arg())
+    def mark_find_handler(self, value: str | None = None) -> None:
+        self.console_apps_api.mark_find(value or self.arg())
 
     def find_free_mark_handler(self) -> None:
         value: str | None = self.arg()
         try:
             result_mark: Mark = one(A.R_M.by_any(value or self.input.mark.any()))
 
             def label_function(data_item: Mark, _: int) -> str:
@@ -7565,16 +7591,19 @@
                     file_search_request,
                     parameters,
                     stdout_redirect,
                     catch_exceptions,
                     redirect_to_mobile_output,
                 )
 
-    def polibase_person_show_information_handler(
-        self, value: str | None = None, show_title: bool = False
+    def polibase_person_information_show_handler(
+        self,
+        value: str | None = None,
+        show_title: bool = False,
+        raise_exception: bool = False,
     ) -> None:
         value = value or self.arg()
         while True:
             try:
 
                 def data_label_function(
                     _, field: FieldItem, person: PolibasePerson, data: Any
@@ -7611,18 +7640,22 @@
                     A.R_P.persons_by_any(value or self.input.polibase_person_any()),
                     data_label_function=data_label_function,
                     title="Найденные пациенты:" if show_title else None,
                 )
                 break
             except NotFound as error:
                 self.output.error(error)
+                if raise_exception:
+                    raise error
                 value = None
                 self.drop_args()
             except BarcodeNotFound as error:
                 self.output.error(error)
+                if raise_exception:
+                    raise error
 
     def create_command_list(self) -> list[list[CommandNode]]:
         def init_command_node_tree(
             tail: CommandNode | dict | set, parent: CommandNode | None = None
         ):
             if isinstance(tail, dict):
                 for node in tail:
@@ -7692,17 +7725,15 @@
         for group in MobileHelper.allowed_group_collection:
             A.C_A.by_group(group, False, session, False, False)
 
     def command_sort_function(self, value: list[CommandNode]) -> str:
         name_list: list[str] = []
         for item in value:
             name_list.append(
-                self.get_command_node_label(item)
-                if item.order is None
-                else chr(item.order)
+                self.get_command_node_label(item) if n(item.order) else chr(item.order)
             )
         return j(name_list).lower()
 
     def command_list_filter_function(
         self,
         value: list[CommandNode] | CommandNode,
         session_holder: SessionBase | None = None,
@@ -7710,15 +7741,15 @@
         in_search: bool = False,
     ) -> bool:
         session_holder = session_holder or self.session
         allow_to_add: bool = True
         if not isinstance(value, list):
             value = [value]
         for command_node in value:
-            if command_node.allowed_groups is not None:
+            if nn(command_node.allowed_groups):
                 if e(command_node.allowed_groups):
                     allow_to_add = True
                 else:
                     allow_to_add = False
                     for group in command_node.allowed_groups:
                         allow_to_add = (
                             allow_to_add or group in session_holder.allowed_groups
@@ -8042,15 +8073,15 @@
 
     def get_command_node_title_or_label(self, value: str | CommandNode) -> list[str]:
         result: list[str] | None = None
         if isinstance(value, CommandNode):
             if ne(value.title_and_label):
                 if callable(value.title_and_label):
                     temp_string_list: list[str] = value.title_and_label()
-                    if temp_string_list is not None:
+                    if nn(temp_string_list):
                         result = temp_string_list
                 else:
                     result = value.title_and_label
             else:
                 value_string_list: list[str] = value.name_list
                 result = (
                     value_string_list[0]
@@ -8153,15 +8184,15 @@
         auto_select: bool = True,
     ) -> CommandNode | list[CommandNode]:
         if auto_select and len(data) == 1:
             return data[0]
         data.insert(0, [self.exit_node])
         with self.output.make_exit_message_visibility(False):
             return self.input.item_by_index(
-                caption, data, label_function, use_zero_index
+                caption, data, label_function, use_zero_index, sticky_items=(0,)
             )
 
     def main_menu_handler(self) -> None:
         is_all: bool = self.is_all
 
         def filter_function(command: list[CommandNode]) -> bool:
             command_node: CommandNode | None = None
@@ -8216,15 +8247,15 @@
             has_settings: bool = self.has_settings
             if self.has_settings:
                 settings_handler: Callable[[], None] | None = value[-1].settings_handler
                 has_settings = nn(settings_handler)
                 if has_settings:
                     handler = settings_handler
                 else:
-                    self.output.error("Клманда не поддерживает режим настройки")
+                    self.output.error("Команда не поддерживает режим настройки")
             is_cyclic: bool = self.has_flag(Flags.CYCLIC)
             is_addressed: bool = self.has_flag(Flags.ADDRESS)
             is_addressed_as_link: bool = self.has_flag(Flags.ADDRESS_AS_LINK)
 
             # title
             with self.output.make_indent(2):
                 if (
@@ -8364,24 +8395,40 @@
             filter_empty=True,
         )
 
     def wait_for_input(self) -> bool:
         return self.stdin.wait_for_data_input
 
     def do_input(self, line: str):
+        line = nns(A.D.space_format(line))
+        data: str | None = None
         if self.stdin.wait_for_data_input:
             self.stdin.interrupt_type = 0
-            lower_line: str = line.lower()
+            lower_line: str = nns(lw(line))
             if lower_line in self.keywords.command.EXIT:
                 interrupt_type = InterruptionTypes.EXIT
                 self.stdin.interrupt_type = interrupt_type
                 self.return_result(interrupt_type=interrupt_type)
             if lower_line in self.keywords.command.BACK:
                 self.stdin.interrupt_type = InterruptionTypes.BACK
+            values: tuple[list[str], tuple[str]] = A.D.separate_unquoted_and_quoted(
+                line.strip()
+            )
+            index_input: bool = self.input.type == INPUT_TYPE.INDEX
             for index, arg_item in enumerate(
-                A.D.not_empty_items(line.strip().split(" "))
+                A.D.not_empty_items(values[0] + values[1])
             ):
                 if arg_item in FLAG_MAP:
                     flag: Flags = FLAG_MAP[arg_item]
                     self.flags = BM.add(self.flags, flag)
                     self.flag_information.append((index, arg_item, flag))
-            self.stdin.data = line
+                if index_input:
+                    if n(data) and A.D_C.decimal(arg_item):
+                        data = arg_item
+                    else:
+                        self.arg_list.append(arg_item)
+            # if index_input:
+            #    if n(data):
+            #        if ne(self.arg_list):
+            #            self.arg_list[0] = None
+            data = data or line
+            self.stdin.data = data
```

### Comparing `pih-mio-0.29.5/MobileHelperService/client.py` & `pih-mio-0.29.8/MobileHelperService/client.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.29.5/MobileHelperService/const.py` & `pih-mio-0.29.8/MobileHelperService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 NAME: str = "MobileHelper"
 
 DEFAULT_COUNT = 100
 ADMIN_ALIAS: str = "admin"
 COUNT_ALIAS: str = "count"
-VERSION: str = "0.29.5"
+VERSION: str = "0.29.8"
 
 HOST = Hosts.WS255
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Mobile helper service",
     host=HOST.NAME,
```

### Comparing `pih-mio-0.29.5/MobileHelperService/service_api.py` & `pih-mio-0.29.8/MobileHelperService/service_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,34 +38,32 @@
 from collections import defaultdict
 from typing import Callable, Any
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
-ADMIN_LOGIN: str = "nak"
-
 
 def sender_is_cli(value: str) -> bool:
     return value in A.D.map(
         lambda item: item[1],
         A.D.filter(
-            lambda item: item[0].lower().endswith("cli"),
+            lambda item: lw(item[0]).endswith("cli"),
             A.D.to_list(A.CT_ME_WH.GROUP, None),  # type: ignore
         ),
     )
 
 
 class MobileHelperService:
 
-    is_admin: bool = False
+    is_administrator: bool = False
 
     @staticmethod
-    def as_admin() -> bool:
-        return MobileHelperService.is_admin or not A.D.contains(A.SYS.host(), SD.host)  # type: ignore
+    def as_administator() -> bool:
+        return MobileHelperService.is_administrator or not A.D.contains(A.SYS.host(), SD.host)  # type: ignore
 
     @staticmethod
     def count() -> int:
         return A.SE.named_arg(COUNT_ALIAS)  # type: ignore
 
     mobile_helper_client_map: dict[str, Api] = {}
 
@@ -86,28 +84,28 @@
         A.SE.add_arg(COUNT_ALIAS, nargs="?", const=1, type=int, default=DEFAULT_COUNT)
         service_desctiption: ServiceDescription | None = (
             A.SRV_A.create_support_service_or_master_service_description(
                 self.service_description
             )
         )
         if A.SRV.is_service_as_support(service_desctiption):
-            MobileHelperService.is_admin = lw(A.SE.named_arg(ADMIN_ALIAS)) in [
+            MobileHelperService.is_administrator = lw(A.SE.named_arg(ADMIN_ALIAS)) in [
                 "1",
                 "true",
                 "yes",
             ]
         else:
-            MobileHelperService.is_admin = False
+            MobileHelperService.is_administrator = False
 
         def service_starts_handler() -> None:
-            if MobileHelperService.as_admin():
+            if MobileHelperService.as_administator():
                 self.create_mobile_helper(
-                    A.D.get(A.CT_ME_WH_G.PIH_CLI),
+                    A.CT_ME_WH_G.PIH_CLI,
                     None,
-                    A.D_U.by_login(ADMIN_LOGIN).telephoneNumber,
+                    A.D_U.by_login(A.S.get(A.CT_S.PIH_CLI_ADMINISTRATOR_LOGIN)).telephoneNumber,
                 )
             MobileHelperService.service_starts_handler()
 
         if ne(service_desctiption):
             A.SRV_A.serve(
                 service_desctiption,
                 self.service_call_handler,  # type: ignore
@@ -116,23 +114,24 @@
                 isolate=ISOLATED,
             )
             return True
         return False
 
     def create_mobile_helper(
         self,
-        sender: str,
+        sender: str | A.CT_ME_WH_G,
         external_flags: int | None = None,
         recipient: str | None = None,
     ) -> Api:
-        is_cli: bool = sender_is_cli(sender)
+        sender_value: str = A.D.get(sender)
+        is_cli: bool = sender_is_cli(sender_value)
         if is_cli:
             external_flags = BM.add(external_flags, Flags.CLI)
         stdin: Stdin = Stdin()
-        session: MobileSession = MobileSession(sender, external_flags)
+        session: MobileSession = MobileSession(sender_value, external_flags)
         output: MobileOutput = MobileOutput(session)
         try:
             session.say_hello(recipient)
             if not is_cli:
                 output.write_line(
                     j(
                         (
@@ -163,34 +162,34 @@
                     )
                 )
         except NotFound as error:
             output.error(
                 "К сожалению, не могу идентифицировать Вас. ИТ отдел добавит Вас после окончания процедуры идентификации."
             )
             raise error
-        as_admin: bool = is_cli
-        if not as_admin:
+        as_administrator: bool = is_cli
+        if not as_administrator:
             try:
-                as_admin = A.C_U.by_group(
-                    nnt(A.R_U.by_telephone_number(sender).data), A.CT_AD.Groups.Admin
+                as_administrator = A.C_U.by_group(
+                    nnt(A.R_U.by_telephone_number(sender_value).data), A.CT_AD.Groups.Admin
                 )
             except NotFound as _:
                 pass
         input: MobileInput = MobileInput(
             stdin,
             MobileUserInput(),
             MobileMarkInput(),
             output,
             session,
-            [None, -1][as_admin],
+            [None, -1][as_administrator],
         )
         api: Api = Api(PIH(input, output, session), stdin)
         if is_cli:
             api.external_flags = external_flags
-        MobileHelperService.mobile_helper_client_map[sender] = api
+        MobileHelperService.mobile_helper_client_map[sender_value] = api
         return api
 
     @staticmethod
     def say_good_bye(mobile_helper: Api, with_error: bool = False) -> None:
         mobile_helper.say_good_bye(with_error=with_error)
         mobile_helper.show_good_bye = False
 
@@ -284,15 +283,15 @@
                         None,
                         external_flags,
                         chat_id,
                         return_result_key,
                         args,
                     )
                 else:
-                    for recipient_user in interruption.recipient_user_list():
+                    for recipient_user in interruption.recipient_user_list(): # type: ignore
                         recipient_user: User = recipient_user
                         self.pih_handler(
                             nnt(recipient_user.telephoneNumber),
                             js((self.root, nnt(interruption).command_name)),
                             nnt(interruption).sender_user,
                             nnt(interruption).flags,
                         )
@@ -323,31 +322,32 @@
                     message: WhatsAppMessage | None = A.D_Ex_E.whatsapp_message(
                         parameter_list
                     )
 
                     if nn(message):
                         if (
                             A.D.get_by_value(
-                                A.CT_ME_WH_W.Profiles, nnt(message).profile_id
+                                A.CT_ME_WH_W.Profiles, nnt(message).profile_id # type: ignore
                             )
                             == A.CT_ME_WH_W.Profiles.IT
                         ):
+                            sender_as_cli: bool = sender_is_cli(nnt(nnt(message).chatId))
                             allow_for_group: bool = ne(
                                 nnt(message).chatId
-                            ) and sender_is_cli(nnt(nnt(message).chatId))
+                            ) and sender_as_cli
                             if n(nnt(message).chatId) or allow_for_group:
                                 telephone_number: str = if_else(
                                     allow_for_group,
                                     nnt(message).chatId,
                                     nnt(message).sender,
                                 )
                                 if allow_for_group:
                                     nnt(message).chatId = nnt(message).sender
                                     nnt(message).sender = telephone_number
-                                if n(self.checker) or self.checker(telephone_number):
+                                if n(self.checker) or nnt(self.checker)(telephone_number):
                                     if self.is_client_stack_full():
                                         return True
                                     else:
                                         if (
                                             telephone_number
                                             in self.allow_send_to_next_service_in_chain
                                         ):
@@ -379,26 +379,26 @@
             return False
         return None
 
     @staticmethod
     def service_starts_handler() -> None:
         A.O.write_line(nl())
         A.O.blue("Configuration:")
-        as_admin: bool = MobileHelperService.as_admin()
+        as_administrator: bool = MobileHelperService.as_administator()
         with A.O.make_indent(1):
-            A.O.value("As admin", str(as_admin))
-            if not as_admin:
+            A.O.value("As admin", str(as_administrator))
+            if not as_administrator:
                 A.O.value("Count", str(MobileHelperService.count()))
         A.SRV_A.subscribe_on(
             A.CT_SC.send_event,
             A.CT_SubT.ON_RESULT_SEQUENTIALLY,
             SD.name,
         )
         profile = A.CT_ME_WH_W.Profiles
-        if as_admin:
+        if as_administrator:
             space: str = "     "
 
             A.ME_WH_W_Q.add_message(
                 Message(
                     j(
                         (
                             " ",
```

