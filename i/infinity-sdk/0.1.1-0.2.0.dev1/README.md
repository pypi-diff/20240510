# Comparing `tmp/infinity_sdk-0.1.1-py3-none-any.whl.zip` & `tmp/infinity_sdk-0.2.0.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,28 @@
-Zip file size: 50799 bytes, number of entries: 26
+Zip file size: 50243 bytes, number of entries: 26
 -rw-rw-r--  2.0 unx     1157 b- defN 24-Apr-11 08:29 infinity/__init__.py
 -rw-rw-r--  2.0 unx     1165 b- defN 24-May-01 07:09 infinity/common.py
 -rw-rw-r--  2.0 unx     1791 b- defN 24-Apr-11 15:10 infinity/connection_pool.py
 -rw-rw-r--  2.0 unx     1387 b- defN 24-Mar-30 15:25 infinity/db.py
 -rw-rw-r--  2.0 unx     4076 b- defN 24-Apr-23 12:28 infinity/errors.py
 -rw-rw-r--  2.0 unx     2421 b- defN 24-Mar-27 16:25 infinity/index.py
--rw-rw-r--  2.0 unx     1823 b- defN 24-May-10 02:58 infinity/infinity.py
+-rw-rw-r--  2.0 unx     1237 b- defN 24-May-06 01:57 infinity/infinity.py
 -rw-rw-r--  2.0 unx     2427 b- defN 24-Mar-27 16:25 infinity/table.py
 -rw-rw-r--  2.0 unx     1391 b- defN 24-Mar-27 16:25 infinity/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Mar-27 16:25 infinity/remote_thrift/__init__.py
--rw-rw-r--  2.0 unx    13944 b- defN 24-May-10 02:58 infinity/remote_thrift/client.py
+-rw-rw-r--  2.0 unx    13663 b- defN 24-May-06 03:21 infinity/remote_thrift/client.py
 -rw-rw-r--  2.0 unx      680 b- defN 24-Mar-17 04:21 infinity/remote_thrift/common.py
 -rw-rw-r--  2.0 unx    12738 b- defN 24-Apr-25 05:37 infinity/remote_thrift/db.py
--rw-rw-r--  2.0 unx     4498 b- defN 24-May-10 02:58 infinity/remote_thrift/infinity.py
+-rw-rw-r--  2.0 unx     4176 b- defN 24-May-06 03:21 infinity/remote_thrift/infinity.py
 -rw-rw-r--  2.0 unx     9938 b- defN 24-Mar-30 15:25 infinity/remote_thrift/query_builder.py
 -rw-rw-r--  2.0 unx    18182 b- defN 24-Apr-28 04:18 infinity/remote_thrift/table.py
 -rw-rw-r--  2.0 unx    10297 b- defN 24-Mar-27 16:25 infinity/remote_thrift/types.py
 -rw-rw-r--  2.0 unx     7204 b- defN 24-Apr-02 08:30 infinity/remote_thrift/utils.py
--rw-rw-r--  2.0 unx   183820 b- defN 24-May-10 02:58 infinity/remote_thrift/infinity_thrift_rpc/InfinityService.py
+-rw-rw-r--  2.0 unx   177661 b- defN 24-May-05 13:04 infinity/remote_thrift/infinity_thrift_rpc/InfinityService.py
 -rw-rw-r--  2.0 unx       53 b- defN 24-Mar-27 16:25 infinity/remote_thrift/infinity_thrift_rpc/__init__.py
 -rw-rw-r--  2.0 unx      366 b- defN 24-Apr-18 13:59 infinity/remote_thrift/infinity_thrift_rpc/constants.py
--rw-rw-r--  2.0 unx   275131 b- defN 24-May-10 02:58 infinity/remote_thrift/infinity_thrift_rpc/ttypes.py
--rw-rw-r--  2.0 unx     2022 b- defN 24-May-10 04:57 infinity_sdk-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-10 04:57 infinity_sdk-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-May-10 04:57 infinity_sdk-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2254 b- defN 24-May-10 04:57 infinity_sdk-0.1.1.dist-info/RECORD
-26 files, 558866 bytes uncompressed, 47141 bytes compressed:  91.6%
+-rw-rw-r--  2.0 unx   272498 b- defN 24-May-05 13:04 infinity/remote_thrift/infinity_thrift_rpc/ttypes.py
+-rw-rw-r--  2.0 unx     2027 b- defN 24-May-07 08:07 infinity_sdk-0.2.0.dev1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-07 08:07 infinity_sdk-0.2.0.dev1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-May-07 08:07 infinity_sdk-0.2.0.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2274 b- defN 24-May-07 08:07 infinity_sdk-0.2.0.dev1.dist-info/RECORD
+26 files, 548910 bytes uncompressed, 46545 bytes compressed:  91.5%
```

## zipnote {}

```diff
@@ -60,20 +60,20 @@
 
 Filename: infinity/remote_thrift/infinity_thrift_rpc/constants.py
 Comment: 
 
 Filename: infinity/remote_thrift/infinity_thrift_rpc/ttypes.py
 Comment: 
 
-Filename: infinity_sdk-0.1.1.dist-info/METADATA
+Filename: infinity_sdk-0.2.0.dev1.dist-info/METADATA
 Comment: 
 
-Filename: infinity_sdk-0.1.1.dist-info/WHEEL
+Filename: infinity_sdk-0.2.0.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: infinity_sdk-0.1.1.dist-info/top_level.txt
+Filename: infinity_sdk-0.2.0.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: infinity_sdk-0.1.1.dist-info/RECORD
+Filename: infinity_sdk-0.2.0.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## infinity/infinity.py

```diff
@@ -12,32 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from abc import ABC, abstractmethod
 from enum import Enum
 
 from infinity import URI
 
-
-class ShowVariable(Enum):
-    QUERY_COUNT = "query_count"
-    SESSION_COUNT = "session_count"
-    BUFFER_POOL_USAGE = "buffer_pool_usage"
-    VERSION = "version"
-    QUERY_MEMORY_LIMIT = "query_memory_limit"
-    QUERY_CPU_LIMIT = "query_cpu_limit"
-    LOG_LEVEL = "log_level"
-    SCHEDULE_POLICY = "schedule_policy"
-    LISTEN_ADDRESS = "listen_address"
-    SQL_PORT = "sql_port"
-    SDK_PORT = "sdk_port"
-    HTTP_API_PORT = "http_api_port"
-    DATA_URL = "data_url"
-    TIME_ZONE = "time_zone"
-
-
 # abstract class
 class InfinityConnection(ABC):
     def __init__(self, uri: URI):
         self.uri = uri
 
     @abstractmethod
     def create_database(self, db_name, options=None):
@@ -58,11 +40,7 @@
     @abstractmethod
     def get_database(self, db_name):
         pass
 
     @abstractmethod
     def disconnect(self):
         pass
-
-    @abstractmethod
-    def show_variable(self, variable: ShowVariable):
-        pass
```

## infinity/remote_thrift/client.py

```diff
@@ -14,15 +14,14 @@
 
 from thrift.protocol import TBinaryProtocol
 from thrift.protocol import TCompactProtocol
 from thrift.transport import TSocket
 from thrift.transport.TTransport import TTransportException
 
 from infinity import URI
-from infinity.infinity import ShowVariable
 from infinity.remote_thrift.infinity_thrift_rpc import *
 from infinity.remote_thrift.infinity_thrift_rpc.ttypes import *
 from infinity.errors import ErrorCode
 
 
 class ThriftInfinityClient:
     def __init__(self, uri: URI):
@@ -209,18 +208,14 @@
         try:
             res = self.client.Disconnect(CommonRequest(session_id=self.session_id))
         except Exception:
             pass
         self.transport.close()
         return res
 
-    def show_variable(self, variable: ShowVariable):
-        return self.client.ShowVariable(ShowVariableRequest(session_id=self.session_id,
-                                                            variable_name=str(variable.value)))
-
     def show_tables(self, db_name: str):
         return self.client.ShowTables(ShowTablesRequest(session_id=self.session_id, db_name=db_name))
 
     def show_segments(self, db_name: str, table_name: str):
         return self.client.ShowSegments(
             ShowSegmentsRequest(session_id=self.session_id, db_name=db_name, table_name=table_name))
```

## infinity/remote_thrift/infinity.py

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 from abc import ABC
 
 import infinity.remote_thrift.infinity_thrift_rpc.ttypes as ttypes
 from infinity import InfinityConnection
 from infinity.errors import ErrorCode
-from infinity.infinity import ShowVariable
 from infinity.remote_thrift.client import ThriftInfinityClient
 from infinity.remote_thrift.db import RemoteDatabase
 from infinity.remote_thrift.utils import name_validity_check, select_res_to_polars
 from infinity.common import ConflictType
 
 
 class RemoteThriftInfinityConnection(InfinityConnection, ABC):
@@ -99,14 +98,7 @@
             return res
         else:
             raise Exception(f"ERROR:{res.error_code}, {res.error_msg}")
 
     @property
     def client(self):
         return self._client
-
-    def show_variable(self, variable: ShowVariable):
-        res = self._client.show_variable(variable)
-        if res.error_code == ErrorCode.OK:
-            return select_res_to_polars(res)
-        else:
-            raise Exception(f"ERROR:{res.error_code}, {res.error_msg}")
```

## infinity/remote_thrift/infinity_thrift_rpc/InfinityService.py

```diff
@@ -130,22 +130,14 @@
         """
         Parameters:
          - request
 
         """
         pass
 
-    def ShowVariable(self, request):
-        """
-        Parameters:
-         - request
-
-        """
-        pass
-
     def ShowTable(self, request):
         """
         Parameters:
          - request
 
         """
         pass
@@ -732,46 +724,14 @@
         result = ListIndex_result()
         result.read(iprot)
         iprot.readMessageEnd()
         if result.success is not None:
             return result.success
         raise TApplicationException(TApplicationException.MISSING_RESULT, "ListIndex failed: unknown result")
 
-    def ShowVariable(self, request):
-        """
-        Parameters:
-         - request
-
-        """
-        self.send_ShowVariable(request)
-        return self.recv_ShowVariable()
-
-    def send_ShowVariable(self, request):
-        self._oprot.writeMessageBegin('ShowVariable', TMessageType.CALL, self._seqid)
-        args = ShowVariable_args()
-        args.request = request
-        args.write(self._oprot)
-        self._oprot.writeMessageEnd()
-        self._oprot.trans.flush()
-
-    def recv_ShowVariable(self):
-        iprot = self._iprot
-        (fname, mtype, rseqid) = iprot.readMessageBegin()
-        if mtype == TMessageType.EXCEPTION:
-            x = TApplicationException()
-            x.read(iprot)
-            iprot.readMessageEnd()
-            raise x
-        result = ShowVariable_result()
-        result.read(iprot)
-        iprot.readMessageEnd()
-        if result.success is not None:
-            return result.success
-        raise TApplicationException(TApplicationException.MISSING_RESULT, "ShowVariable failed: unknown result")
-
     def ShowTable(self, request):
         """
         Parameters:
          - request
 
         """
         self.send_ShowTable(request)
@@ -1232,15 +1192,14 @@
         self._processMap["Select"] = Processor.process_Select
         self._processMap["Explain"] = Processor.process_Explain
         self._processMap["Delete"] = Processor.process_Delete
         self._processMap["Update"] = Processor.process_Update
         self._processMap["ListDatabase"] = Processor.process_ListDatabase
         self._processMap["ListTable"] = Processor.process_ListTable
         self._processMap["ListIndex"] = Processor.process_ListIndex
-        self._processMap["ShowVariable"] = Processor.process_ShowVariable
         self._processMap["ShowTable"] = Processor.process_ShowTable
         self._processMap["ShowColumns"] = Processor.process_ShowColumns
         self._processMap["ShowDatabase"] = Processor.process_ShowDatabase
         self._processMap["ShowTables"] = Processor.process_ShowTables
         self._processMap["ShowSegments"] = Processor.process_ShowSegments
         self._processMap["ShowSegment"] = Processor.process_ShowSegment
         self._processMap["ShowBlocks"] = Processor.process_ShowBlocks
@@ -1614,37 +1573,14 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("ListIndex", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
-    def process_ShowVariable(self, seqid, iprot, oprot):
-        args = ShowVariable_args()
-        args.read(iprot)
-        iprot.readMessageEnd()
-        result = ShowVariable_result()
-        try:
-            result.success = self._handler.ShowVariable(args.request)
-            msg_type = TMessageType.REPLY
-        except TTransport.TTransportException:
-            raise
-        except TApplicationException as ex:
-            logging.exception('TApplication exception in handler')
-            msg_type = TMessageType.EXCEPTION
-            result = ex
-        except Exception:
-            logging.exception('Unexpected exception in handler')
-            msg_type = TMessageType.EXCEPTION
-            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
-        oprot.writeMessageBegin("ShowVariable", msg_type, seqid)
-        result.write(oprot)
-        oprot.writeMessageEnd()
-        oprot.trans.flush()
-
     def process_ShowTable(self, seqid, iprot, oprot):
         args = ShowTable_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = ShowTable_result()
         try:
             result.success = self._handler.ShowTable(args.request)
@@ -3817,139 +3753,14 @@
         return not (self == other)
 all_structs.append(ListIndex_result)
 ListIndex_result.thrift_spec = (
     (0, TType.STRUCT, 'success', [ListIndexResponse, None], None, ),  # 0
 )
 
 
-class ShowVariable_args(object):
-    """
-    Attributes:
-     - request
-
-    """
-
-
-    def __init__(self, request=None,):
-        self.request = request
-
-    def read(self, iprot):
-        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
-            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
-            return
-        iprot.readStructBegin()
-        while True:
-            (fname, ftype, fid) = iprot.readFieldBegin()
-            if ftype == TType.STOP:
-                break
-            if fid == 1:
-                if ftype == TType.STRUCT:
-                    self.request = ShowVariableRequest()
-                    self.request.read(iprot)
-                else:
-                    iprot.skip(ftype)
-            else:
-                iprot.skip(ftype)
-            iprot.readFieldEnd()
-        iprot.readStructEnd()
-
-    def write(self, oprot):
-        if oprot._fast_encode is not None and self.thrift_spec is not None:
-            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
-            return
-        oprot.writeStructBegin('ShowVariable_args')
-        if self.request is not None:
-            oprot.writeFieldBegin('request', TType.STRUCT, 1)
-            self.request.write(oprot)
-            oprot.writeFieldEnd()
-        oprot.writeFieldStop()
-        oprot.writeStructEnd()
-
-    def validate(self):
-        return
-
-    def __repr__(self):
-        L = ['%s=%r' % (key, value)
-             for key, value in self.__dict__.items()]
-        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
-
-    def __eq__(self, other):
-        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
-
-    def __ne__(self, other):
-        return not (self == other)
-all_structs.append(ShowVariable_args)
-ShowVariable_args.thrift_spec = (
-    None,  # 0
-    (1, TType.STRUCT, 'request', [ShowVariableRequest, None], None, ),  # 1
-)
-
-
-class ShowVariable_result(object):
-    """
-    Attributes:
-     - success
-
-    """
-
-
-    def __init__(self, success=None,):
-        self.success = success
-
-    def read(self, iprot):
-        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
-            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
-            return
-        iprot.readStructBegin()
-        while True:
-            (fname, ftype, fid) = iprot.readFieldBegin()
-            if ftype == TType.STOP:
-                break
-            if fid == 0:
-                if ftype == TType.STRUCT:
-                    self.success = SelectResponse()
-                    self.success.read(iprot)
-                else:
-                    iprot.skip(ftype)
-            else:
-                iprot.skip(ftype)
-            iprot.readFieldEnd()
-        iprot.readStructEnd()
-
-    def write(self, oprot):
-        if oprot._fast_encode is not None and self.thrift_spec is not None:
-            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
-            return
-        oprot.writeStructBegin('ShowVariable_result')
-        if self.success is not None:
-            oprot.writeFieldBegin('success', TType.STRUCT, 0)
-            self.success.write(oprot)
-            oprot.writeFieldEnd()
-        oprot.writeFieldStop()
-        oprot.writeStructEnd()
-
-    def validate(self):
-        return
-
-    def __repr__(self):
-        L = ['%s=%r' % (key, value)
-             for key, value in self.__dict__.items()]
-        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
-
-    def __eq__(self, other):
-        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
-
-    def __ne__(self, other):
-        return not (self == other)
-all_structs.append(ShowVariable_result)
-ShowVariable_result.thrift_spec = (
-    (0, TType.STRUCT, 'success', [SelectResponse, None], None, ),  # 0
-)
-
-
 class ShowTable_args(object):
     """
     Attributes:
      - request
 
     """
```

## infinity/remote_thrift/infinity_thrift_rpc/ttypes.py

```diff
@@ -5808,82 +5808,14 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
-class ShowVariableRequest(object):
-    """
-    Attributes:
-     - session_id
-     - variable_name
-
-    """
-
-
-    def __init__(self, session_id=None, variable_name=None,):
-        self.session_id = session_id
-        self.variable_name = variable_name
-
-    def read(self, iprot):
-        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
-            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
-            return
-        iprot.readStructBegin()
-        while True:
-            (fname, ftype, fid) = iprot.readFieldBegin()
-            if ftype == TType.STOP:
-                break
-            if fid == 1:
-                if ftype == TType.I64:
-                    self.session_id = iprot.readI64()
-                else:
-                    iprot.skip(ftype)
-            elif fid == 2:
-                if ftype == TType.STRING:
-                    self.variable_name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                else:
-                    iprot.skip(ftype)
-            else:
-                iprot.skip(ftype)
-            iprot.readFieldEnd()
-        iprot.readStructEnd()
-
-    def write(self, oprot):
-        if oprot._fast_encode is not None and self.thrift_spec is not None:
-            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
-            return
-        oprot.writeStructBegin('ShowVariableRequest')
-        if self.session_id is not None:
-            oprot.writeFieldBegin('session_id', TType.I64, 1)
-            oprot.writeI64(self.session_id)
-            oprot.writeFieldEnd()
-        if self.variable_name is not None:
-            oprot.writeFieldBegin('variable_name', TType.STRING, 2)
-            oprot.writeString(self.variable_name.encode('utf-8') if sys.version_info[0] == 2 else self.variable_name)
-            oprot.writeFieldEnd()
-        oprot.writeFieldStop()
-        oprot.writeStructEnd()
-
-    def validate(self):
-        return
-
-    def __repr__(self):
-        L = ['%s=%r' % (key, value)
-             for key, value in self.__dict__.items()]
-        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
-
-    def __eq__(self, other):
-        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
-
-    def __ne__(self, other):
-        return not (self == other)
-
-
 class ShowTablesRequest(object):
     """
     Attributes:
      - session_id
      - db_name
 
     """
@@ -7324,20 +7256,14 @@
     (1, TType.STRING, 'db_name', 'UTF8', None, ),  # 1
     (2, TType.STRING, 'table_name', 'UTF8', None, ),  # 2
     (3, TType.STRUCT, 'where_expr', [ParsedExpr, None], None, ),  # 3
     (4, TType.LIST, 'update_expr_array', (TType.STRUCT, [UpdateExpr, None], False), [
     ], ),  # 4
     (5, TType.I64, 'session_id', None, None, ),  # 5
 )
-all_structs.append(ShowVariableRequest)
-ShowVariableRequest.thrift_spec = (
-    None,  # 0
-    (1, TType.I64, 'session_id', None, None, ),  # 1
-    (2, TType.STRING, 'variable_name', 'UTF8', None, ),  # 2
-)
 all_structs.append(ShowTablesRequest)
 ShowTablesRequest.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'session_id', None, None, ),  # 1
     (2, TType.STRING, 'db_name', 'UTF8', None, ),  # 2
 )
 all_structs.append(ShowSegmentsRequest)
```

## Comparing `infinity_sdk-0.1.1.dist-info/METADATA` & `infinity_sdk-0.2.0.dev1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinity_sdk
-Version: 0.1.1
+Version: 0.2.0.dev1
 Summary: infinity
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: sqlglot ~=11.7.1
 Requires-Dist: pydantic ~=2.7.1
 Requires-Dist: thrift ~=0.20.0
 Requires-Dist: setuptools ~=69.5.1
```

## Comparing `infinity_sdk-0.1.1.dist-info/RECORD` & `infinity_sdk-0.2.0.dev1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 infinity/__init__.py,sha256=2C0wTgGopUqis1YUSz9-pxhqpsBk8ey73sbmbG-4Wio,1157
 infinity/common.py,sha256=6EmWFwn-uDwSd-Q8zQpUSlaOOhq-8-EQ0We6oP0hY1Y,1165
 infinity/connection_pool.py,sha256=OPTfDnqqh0YqzOt-4863d8_-lsQ56O378f2tCI-zB4I,1791
 infinity/db.py,sha256=WFZ_BcofXmsxUtV6PyKrOsAwrtkBbXse9RclA590QJw,1387
 infinity/errors.py,sha256=yGxmW-3UK2NYYaluTqb-l7kZjHvbGWfAhlvD6qE0ip0,4076
 infinity/index.py,sha256=VjucD7hL56A0uABYmTeEWRxNmI_WxtmHZQCtrR1zrCo,2421
-infinity/infinity.py,sha256=KcrTYjwAkqdW7eO7pIGn-32Gj-2rMu1ONklq62ErkgY,1823
+infinity/infinity.py,sha256=XAS6KQvYlRtpL8SFSbcRcCpwHzB6CcPXtkZxTjwL5hE,1237
 infinity/table.py,sha256=ByoGtbY-3kdya197TeEsHfJU-Ov986dXnFdtMlV7hGA,2427
 infinity/utils.py,sha256=-IDma0UnER_vgvCdIm48Omfal5fd_i7HP9iEx83lXcc,1391
 infinity/remote_thrift/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-infinity/remote_thrift/client.py,sha256=_KFbkTE2wWg1MZtMUUvCBIcKEs3CecPewQrCIqp6nRo,13944
+infinity/remote_thrift/client.py,sha256=GKoKiFMgDq0n-jnV7n7ZK-lfMuIev8fjbz7vnfwToYc,13663
 infinity/remote_thrift/common.py,sha256=4eyCmKtUP3dNyZmtIPoCc05AAseuJsfqgfTQ6aY9iag,680
 infinity/remote_thrift/db.py,sha256=o-lCmXs6bTEkwDcnYG0s__2xpWLldOOtCeLnhrFmj-s,12738
-infinity/remote_thrift/infinity.py,sha256=rLgV2jdnDfIotM7B3Lnf9CkOMFT7IOcahdML2AyFR50,4498
+infinity/remote_thrift/infinity.py,sha256=r9Y7wQqs2GrXE9GFcbXhO0A3HMCRJUX8Lr1no0zrBQs,4176
 infinity/remote_thrift/query_builder.py,sha256=aM9qJqbt59jDH5AZ7iIADUNBRwYE5qeWGoEJ0EEXfZU,9938
 infinity/remote_thrift/table.py,sha256=vYtCCRxMMjPVQeFq0kwK2WNuFpnAZDUo5VAAIWRJ4aI,18182
 infinity/remote_thrift/types.py,sha256=FCd4FTQnxYDMK22jUgYPtvgfkboTYtLbLYUp7DU4xJs,10297
 infinity/remote_thrift/utils.py,sha256=6B1M5J5Yg69m1wyFLcivdk5I57mF89MMuUSEVrf57WE,7204
-infinity/remote_thrift/infinity_thrift_rpc/InfinityService.py,sha256=Qt9SYNZZMe4qtASYYZo4O_lQUBVvuRpp306eDO7kZH4,183820
+infinity/remote_thrift/infinity_thrift_rpc/InfinityService.py,sha256=vf4nFV_ZxkBgrhFzHPREuhN2ziLvBSmWX0ywHVUeJVw,177661
 infinity/remote_thrift/infinity_thrift_rpc/__init__.py,sha256=ezRvowu7Yojw8xly58EOLQ3_40IK5XUqusB8XPoRlF4,53
 infinity/remote_thrift/infinity_thrift_rpc/constants.py,sha256=fEiYY_X50Lqtkoew_h1qWBH5QmDiygExYB-6WRsifqg,366
-infinity/remote_thrift/infinity_thrift_rpc/ttypes.py,sha256=AimSVt5PaTX0a79pONx5k3b1s7vP-JTlK_YNHcnB9EY,275131
-infinity_sdk-0.1.1.dist-info/METADATA,sha256=dD7MbyQFatfMAIAXBn3uhr0-VYS639-mYAwSUO47ax0,2022
-infinity_sdk-0.1.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-infinity_sdk-0.1.1.dist-info/top_level.txt,sha256=I5UhBoCrOOXaJN_xGXGoA73npSJ-IRiqYdRL8NYf5VY,9
-infinity_sdk-0.1.1.dist-info/RECORD,,
+infinity/remote_thrift/infinity_thrift_rpc/ttypes.py,sha256=9yoewv6CuCsesyg5ojXU_aoj_EV9cy7qDzgb_A5OSXE,272498
+infinity_sdk-0.2.0.dev1.dist-info/METADATA,sha256=i-LiJ_q6MGaF42p04szJJ_wO1PdeW9MBctLxMgoMeYA,2027
+infinity_sdk-0.2.0.dev1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+infinity_sdk-0.2.0.dev1.dist-info/top_level.txt,sha256=I5UhBoCrOOXaJN_xGXGoA73npSJ-IRiqYdRL8NYf5VY,9
+infinity_sdk-0.2.0.dev1.dist-info/RECORD,,
```

