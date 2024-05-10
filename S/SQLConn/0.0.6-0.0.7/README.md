# Comparing `tmp/SQLConn-0.0.6.tar.gz` & `tmp/SQLConn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLConn-0.0.6.tar", last modified: Mon May  6 10:06:30 2024, max compression
+gzip compressed data, was "SQLConn-0.0.7.tar", last modified: Fri May 10 05:38:09 2024, max compression
```

## Comparing `SQLConn-0.0.6.tar` & `SQLConn-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 10:06:30.788059 SQLConn-0.0.6/
--rw-rw-rw-   0        0        0     9260 2024-05-06 10:06:30.786041 SQLConn-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8818 2024-05-06 08:56:32.000000 SQLConn-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 10:06:30.757758 SQLConn-0.0.6/SQLConn/
--rw-rw-rw-   0        0        0     5323 2024-05-06 10:06:19.000000 SQLConn-0.0.6/SQLConn/SQLConn.py
--rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.6/SQLConn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:06:30.783535 SQLConn-0.0.6/SQLConn.egg-info/
--rw-rw-rw-   0        0        0     9260 2024-05-06 10:06:30.000000 SQLConn-0.0.6/SQLConn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-05-06 10:06:30.000000 SQLConn-0.0.6/SQLConn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 10:06:30.000000 SQLConn-0.0.6/SQLConn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-06 10:06:30.000000 SQLConn-0.0.6/SQLConn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 10:06:30.000000 SQLConn-0.0.6/SQLConn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 10:06:30.788059 SQLConn-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-06 10:06:25.000000 SQLConn-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:38:09.232230 SQLConn-0.0.7/
+-rw-rw-rw-   0        0        0    10415 2024-05-10 05:38:09.231228 SQLConn-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9975 2024-05-10 05:36:53.000000 SQLConn-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 05:38:09.226233 SQLConn-0.0.7/SQLConn/
+-rw-rw-rw-   0        0        0     5583 2024-05-06 10:21:39.000000 SQLConn-0.0.7/SQLConn/SQLConn.py
+-rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.7/SQLConn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:38:09.230234 SQLConn-0.0.7/SQLConn.egg-info/
+-rw-rw-rw-   0        0        0    10415 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 05:38:09.232230 SQLConn-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-10 04:21:28.000000 SQLConn-0.0.7/setup.py
```

### Comparing `SQLConn-0.0.6/PKG-INFO` & `SQLConn-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,190 +1,225 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: mysqlclient
 Requires-Dist: pandas
 Requires-Dist: cx_oracle
 Requires-Dist: psycopg2
 Requires-Dist: pymssql
 Requires-Dist: sqlalchemy
 
 # SQLConn
+
 ## 한국어 버전(Korean Version)
+
 SQLConn은 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하여 데이터를 쉽게 조작하고 관리할 수 있는 Python 패키지입니다. 이 패키지는 MySQL, PostgreSQL, Microsoft SQL Server, Oracle 및 SQLite 데이터베이스에 대한 지원을 포함합니다.
 
 ### 기능
 
 - 여러 데이터베이스에 대한 통합된 인터페이스 제공
 - 데이터 조회 및 조작을 위한 간편한 함수 제공
 - 데이터베이스 쿼리 결과를 DataFrame으로 변환
 - CSV, Excel, TSV 파일로의 데이터 출력 지원
 - 다른 데이터베이스로의 데이터 이동 지원
 
 ### 연결가능한 데이터베이스
+
 - MySQL
 - PostgreSQL
 - Microsoft SQL Server
 - Oracle
 - SQLite
 
 ### 설치 방법
 
 파이썬과 pip가 설치된 환경에서 다음 명령어를 통해 `SQLConn` 패키지를 설치할 수 있습니다:
 
 ```bash
 pip install SQLConn
 ```
+
 ### 클래스 소개
-| 클래스명       | 소개                                                         | 특이 사항          |
-| -------------- | ------------------------------------------------------------ | ---------------- |
-| `SQLConn`      | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다. |
-| `MySQLConn`    | MySQL 데이터베이스와의 연결을 관리합니다.                     | SQLConn에게 상속 받았습니다 |
-| `MSSQLConn`    | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.       | SQLConn에게 상속 받았습니다 |
-| `PostgreSQLConn` | PostgreSQL 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
-| `OracleConn`   | Oracle 데이터베이스와의 연결을 관리합니다.                     | SQLConn에게 상속 받았습니다 |
-| `SQLiteConn`   | SQLite 파일 기반 데이터베이스와의 연결을 관리합니다.           | SQLConn에게 상속 받았습니다 |
+
+| 클래스명           | 소개                                                                    | 특이 사항                   |
+| ------------------ | ----------------------------------------------------------------------- | --------------------------- |
+| `SQLConn`        | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다.          |
+| `MYSQLConn`      | MySQL 데이터베이스와의 연결을 관리합니다.                               | SQLConn에게 상속 받았습니다 |
+| `MSSQLConn`      | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
+| `PostgreSQLConn` | PostgreSQL 데이터베이스와의 연결을 관리합니다.                          | SQLConn에게 상속 받았습니다 |
+| `OracleConn`     | Oracle 데이터베이스와의 연결을 관리합니다.                              | SQLConn에게 상속 받았습니다 |
+| `SQLiteConn`     | SQLite 파일 기반 데이터베이스와의 연결을 관리합니다.                    | SQLConn에게 상속 받았습니다 |
 
 ### 메소드 소개
-| 메소드명       | 소개                                                  | 특이사항                      |
-|--------------|--------------------------------------------------------------|------------------------------|
-| `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다. | Show, Select 커맨드만 가능    |
-| `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
-| `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
-| `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                     | Show, Select 커맨드만 가능    |
-| `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
-| `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.              | Show, Select 커맨드만 가능    |
-| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 읽기용 프로퍼티               |
-| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 읽기용 프로퍼티               |
 
+| 메소드명         | 소개                                                           | 특이사항                        |
+| ---------------- | -------------------------------------------------------------- | ------------------------------- |
+| `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다.    | Show, Select 커맨드만 가능      |
+| `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
+| `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                         | Show, Select 커맨드만 가능      |
+| `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                       | Show, Select 커맨드만 가능      |
+| `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                         | Show, Select 커맨드만 가능      |
+| `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.                | Show, Select 커맨드만 가능      |
+| `URL`          | 데이터베이스 연결 URL을 제공합니다.                            | 읽기용 프로퍼티                 |
+| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.         | 읽기용 프로퍼티                 |
 
 ### 사용예제
+
 각 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn, SQLiteConn
 
 # MySQL 데이터베이스에 연결
-mysql_conn = MySQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
+mysql_conn = MYSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # MsSQL 데이터베이스에 연결
 mssql_conn = MSSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # PostgreSQL 데이터베이스에 연결
 postgresql_conn = PostgreSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # SQLite 데이터베이스에 연결
 mssql_conn = SQLiteConn('your-host')
 
 # 데이터 조회 예제
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
 ### 로컬호스트에서 사용하기
+
 로컬 호스트 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn
 
 # MySQL 데이터베이스에 연결
-mysql_conn = MySQLConn('your-password')
+mysql_conn = MYSQLConn('your-password')
 
 # MsSQL 데이터베이스에 연결
 mssql_conn = MSSQLConn('your-password')
 
 # PostgreSQL 데이터베이스에 연결
 postgresql_conn = PostgreSQLConn('your-password')
 
 # 데이터 조회 예제
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
+### 패키지 주소
+
+- [github](https://github.com/janyoungjin/SQLConn)
+- [pypi](https://pypi.org/project/SQLConn/)
+
 ## English Version
+
 SQLConn is a Python package that connects to various SQL database management systems (DBMS) to easily manipulate and manage data. This package includes support for MySQL, PostgreSQL, Microsoft SQL Server, Oracle, and SQLite databases.
 
 ### function
 
 - Provides a unified interface to multiple databases
 - Provides simple functions for data inquiry and manipulation
 - Convert database query results to DataFrame
 - Supports data output to CSV, Excel, TSV files
 - Support for data movement to other databases
+
 ### Support database
+
 - MySQL
 - PostgreSQL
 - Microsoft SQL Server
 - Oracle
 - SQLite
 
 ### How to install
 
 In an environment where Python and pip are installed, you can install the `SQLConn` package using the following command:
 
 ```bash
 pip install SQLConn
 ```
+
 ### class info
-| class name | info | significant |
-| -------------- | ----------------------------------------------- | ---------------- |
-| `SQLConn` | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
-| `MySQLConn` | Manages MySQL database relationships. | protected  SQLConn |
-| `MSSQLConn` | Manages connections to Microsoft SQL Server databases. | protected  SQLConn |
-| `PostgreSQLConn` | Manages connections to PostgreSQL databases. | protected  SQLConn |
-| `OracleCon` | Manages Oracle database relationships. | protected  SQLConn |
-| `SQLiteConn` | Manages SQLite file-based database relationships. | protected  SQLConn |
+
+| class name         | info                                                                    | significant              |
+| ------------------ | ----------------------------------------------------------------------- | ------------------------ |
+| `SQLConn`        | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
+| `MYSQLConn`      | Manages MySQL database relationships.                                   | protected  SQLConn       |
+| `MSSQLConn`      | Manages connections to Microsoft SQL Server databases.                  | protected  SQLConn       |
+| `PostgreSQLConn` | Manages connections to PostgreSQL databases.                            | protected  SQLConn       |
+| `OracleCon`      | Manages Oracle database relationships.                                  | protected  SQLConn       |
+| `SQLiteConn`     | Manages SQLite file-based database relationships.                       | protected  SQLConn       |
 
 ### method info
-| method name       | info                                                  | significant                      |
-|--------------|--------------------------------------------------------------|------------------------------|
-| `to_DataFrame` | Executes a SQL query and returns the results as a pandas DataFrame. | Show, Select commands only |
-| `execute` | Executes a SQL query on a database but returns no results. | Show, Select command not available |
-| `to_csv` | Save the SQL query results as a CSV file. | Show, Select commands only |
-| `to_excel` | Save the SQL query results as an Excel file. | Show, Select commands only |
-| `to_tsv` | Save the SQL query results as a TSV file. | Show, Select commands only |
-| `to_sql` | Store SQL query results in another database. | Show, Select commands only |
-| `URL` | Provide the database connection URL. | get property |
-| `engine` | Provides SQLAlchemy engine for database connection. | get property |
+
+| method name      | info                                                                | significant                        |
+| ---------------- | ------------------------------------------------------------------- | ---------------------------------- |
+| `to_DataFrame` | Executes a SQL query and returns the results as a pandas DataFrame. | Show, Select commands only         |
+| `execute`      | Executes a SQL query on a database but returns no results.          | Show, Select command not available |
+| `to_csv`       | Save the SQL query results as a CSV file.                           | Show, Select commands only         |
+| `to_excel`     | Save the SQL query results as an Excel file.                        | Show, Select commands only         |
+| `to_tsv`       | Save the SQL query results as a TSV file.                           | Show, Select commands only         |
+| `to_sql`       | Store SQL query results in another database.                        | Show, Select commands only         |
+| `URL`          | Provide the database connection URL.                                | get property                       |
+| `engine`       | Provides SQLAlchemy engine for database connection.                 | get property                       |
 
 ### Example of use
+
 The basic way to create and use each database connection object is as follows:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn, SQLiteConn
 
 # Connect to MySQL database
-mysql_conn = MySQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
+mysql_conn = MYSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to MsSQL database
 mssql_conn = MSSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to PostgreSQL database
 postgresql_conn = PostgreSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to SQLite database
 mssql_conn = SQLiteConn('your-host')
 
 # Data query example
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
 ### Using on local host
+
 The basic way to create and use a localhost database connection object is as follows:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn
 
 # Connect to MySQL database
-mysql_conn = MySQLConn('your-password')
+mysql_conn = MYSQLConn('your-password')
 
 # Connect to MsSQL database
 mssql_conn = MSSQLConn('your-password')
 
 # Connect to PostgreSQL database
 postgresql_conn = PostgreSQLConn('your-password')
 
 # Data query example
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
+### package address
+
+- [github](https://github.com/janyoungjin/SQLConn)
+
+- [pypi](https://pypi.org/project/SQLConn/)
+
 ### warning
+
 This document was converted from the Korean version to English through a translator, so the meaning may be strange.
```

### Comparing `SQLConn-0.0.6/README.md` & `SQLConn-0.0.7/SQLConn.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,175 +1,225 @@
+Metadata-Version: 2.1
+Name: SQLConn
+Version: 0.0.7
+Summary: This package facilitates easy SQL database integration.
+Home-page: https://github.com/janyoungjin/SQLConn
+Author: janyoungjin
+Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
+Description-Content-Type: text/markdown
+Requires-Dist: mysqlclient
+Requires-Dist: pandas
+Requires-Dist: cx_oracle
+Requires-Dist: psycopg2
+Requires-Dist: pymssql
+Requires-Dist: sqlalchemy
+
 # SQLConn
+
 ## 한국어 버전(Korean Version)
+
 SQLConn은 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하여 데이터를 쉽게 조작하고 관리할 수 있는 Python 패키지입니다. 이 패키지는 MySQL, PostgreSQL, Microsoft SQL Server, Oracle 및 SQLite 데이터베이스에 대한 지원을 포함합니다.
 
 ### 기능
 
 - 여러 데이터베이스에 대한 통합된 인터페이스 제공
 - 데이터 조회 및 조작을 위한 간편한 함수 제공
 - 데이터베이스 쿼리 결과를 DataFrame으로 변환
 - CSV, Excel, TSV 파일로의 데이터 출력 지원
 - 다른 데이터베이스로의 데이터 이동 지원
 
 ### 연결가능한 데이터베이스
+
 - MySQL
 - PostgreSQL
 - Microsoft SQL Server
 - Oracle
 - SQLite
 
 ### 설치 방법
 
 파이썬과 pip가 설치된 환경에서 다음 명령어를 통해 `SQLConn` 패키지를 설치할 수 있습니다:
 
 ```bash
 pip install SQLConn
 ```
+
 ### 클래스 소개
-| 클래스명       | 소개                                                         | 특이 사항          |
-| -------------- | ------------------------------------------------------------ | ---------------- |
-| `SQLConn`      | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다. |
-| `MySQLConn`    | MySQL 데이터베이스와의 연결을 관리합니다.                     | SQLConn에게 상속 받았습니다 |
-| `MSSQLConn`    | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.       | SQLConn에게 상속 받았습니다 |
-| `PostgreSQLConn` | PostgreSQL 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
-| `OracleConn`   | Oracle 데이터베이스와의 연결을 관리합니다.                     | SQLConn에게 상속 받았습니다 |
-| `SQLiteConn`   | SQLite 파일 기반 데이터베이스와의 연결을 관리합니다.           | SQLConn에게 상속 받았습니다 |
+
+| 클래스명           | 소개                                                                    | 특이 사항                   |
+| ------------------ | ----------------------------------------------------------------------- | --------------------------- |
+| `SQLConn`        | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다.          |
+| `MYSQLConn`      | MySQL 데이터베이스와의 연결을 관리합니다.                               | SQLConn에게 상속 받았습니다 |
+| `MSSQLConn`      | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
+| `PostgreSQLConn` | PostgreSQL 데이터베이스와의 연결을 관리합니다.                          | SQLConn에게 상속 받았습니다 |
+| `OracleConn`     | Oracle 데이터베이스와의 연결을 관리합니다.                              | SQLConn에게 상속 받았습니다 |
+| `SQLiteConn`     | SQLite 파일 기반 데이터베이스와의 연결을 관리합니다.                    | SQLConn에게 상속 받았습니다 |
 
 ### 메소드 소개
-| 메소드명       | 소개                                                  | 특이사항                      |
-|--------------|--------------------------------------------------------------|------------------------------|
-| `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다. | Show, Select 커맨드만 가능    |
-| `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
-| `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
-| `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                     | Show, Select 커맨드만 가능    |
-| `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
-| `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.              | Show, Select 커맨드만 가능    |
-| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 읽기용 프로퍼티               |
-| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 읽기용 프로퍼티               |
 
+| 메소드명         | 소개                                                           | 특이사항                        |
+| ---------------- | -------------------------------------------------------------- | ------------------------------- |
+| `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다.    | Show, Select 커맨드만 가능      |
+| `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
+| `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                         | Show, Select 커맨드만 가능      |
+| `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                       | Show, Select 커맨드만 가능      |
+| `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                         | Show, Select 커맨드만 가능      |
+| `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.                | Show, Select 커맨드만 가능      |
+| `URL`          | 데이터베이스 연결 URL을 제공합니다.                            | 읽기용 프로퍼티                 |
+| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.         | 읽기용 프로퍼티                 |
 
 ### 사용예제
+
 각 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn, SQLiteConn
 
 # MySQL 데이터베이스에 연결
-mysql_conn = MySQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
+mysql_conn = MYSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # MsSQL 데이터베이스에 연결
 mssql_conn = MSSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # PostgreSQL 데이터베이스에 연결
 postgresql_conn = PostgreSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # SQLite 데이터베이스에 연결
 mssql_conn = SQLiteConn('your-host')
 
 # 데이터 조회 예제
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
 ### 로컬호스트에서 사용하기
+
 로컬 호스트 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn
 
 # MySQL 데이터베이스에 연결
-mysql_conn = MySQLConn('your-password')
+mysql_conn = MYSQLConn('your-password')
 
 # MsSQL 데이터베이스에 연결
 mssql_conn = MSSQLConn('your-password')
 
 # PostgreSQL 데이터베이스에 연결
 postgresql_conn = PostgreSQLConn('your-password')
 
 # 데이터 조회 예제
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
+### 패키지 주소
+
+- [github](https://github.com/janyoungjin/SQLConn)
+- [pypi](https://pypi.org/project/SQLConn/)
+
 ## English Version
+
 SQLConn is a Python package that connects to various SQL database management systems (DBMS) to easily manipulate and manage data. This package includes support for MySQL, PostgreSQL, Microsoft SQL Server, Oracle, and SQLite databases.
 
 ### function
 
 - Provides a unified interface to multiple databases
 - Provides simple functions for data inquiry and manipulation
 - Convert database query results to DataFrame
 - Supports data output to CSV, Excel, TSV files
 - Support for data movement to other databases
+
 ### Support database
+
 - MySQL
 - PostgreSQL
 - Microsoft SQL Server
 - Oracle
 - SQLite
 
 ### How to install
 
 In an environment where Python and pip are installed, you can install the `SQLConn` package using the following command:
 
 ```bash
 pip install SQLConn
 ```
+
 ### class info
-| class name | info | significant |
-| -------------- | ----------------------------------------------- | ---------------- |
-| `SQLConn` | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
-| `MySQLConn` | Manages MySQL database relationships. | protected  SQLConn |
-| `MSSQLConn` | Manages connections to Microsoft SQL Server databases. | protected  SQLConn |
-| `PostgreSQLConn` | Manages connections to PostgreSQL databases. | protected  SQLConn |
-| `OracleCon` | Manages Oracle database relationships. | protected  SQLConn |
-| `SQLiteConn` | Manages SQLite file-based database relationships. | protected  SQLConn |
+
+| class name         | info                                                                    | significant              |
+| ------------------ | ----------------------------------------------------------------------- | ------------------------ |
+| `SQLConn`        | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
+| `MYSQLConn`      | Manages MySQL database relationships.                                   | protected  SQLConn       |
+| `MSSQLConn`      | Manages connections to Microsoft SQL Server databases.                  | protected  SQLConn       |
+| `PostgreSQLConn` | Manages connections to PostgreSQL databases.                            | protected  SQLConn       |
+| `OracleCon`      | Manages Oracle database relationships.                                  | protected  SQLConn       |
+| `SQLiteConn`     | Manages SQLite file-based database relationships.                       | protected  SQLConn       |
 
 ### method info
-| method name       | info                                                  | significant                      |
-|--------------|--------------------------------------------------------------|------------------------------|
-| `to_DataFrame` | Executes a SQL query and returns the results as a pandas DataFrame. | Show, Select commands only |
-| `execute` | Executes a SQL query on a database but returns no results. | Show, Select command not available |
-| `to_csv` | Save the SQL query results as a CSV file. | Show, Select commands only |
-| `to_excel` | Save the SQL query results as an Excel file. | Show, Select commands only |
-| `to_tsv` | Save the SQL query results as a TSV file. | Show, Select commands only |
-| `to_sql` | Store SQL query results in another database. | Show, Select commands only |
-| `URL` | Provide the database connection URL. | get property |
-| `engine` | Provides SQLAlchemy engine for database connection. | get property |
+
+| method name      | info                                                                | significant                        |
+| ---------------- | ------------------------------------------------------------------- | ---------------------------------- |
+| `to_DataFrame` | Executes a SQL query and returns the results as a pandas DataFrame. | Show, Select commands only         |
+| `execute`      | Executes a SQL query on a database but returns no results.          | Show, Select command not available |
+| `to_csv`       | Save the SQL query results as a CSV file.                           | Show, Select commands only         |
+| `to_excel`     | Save the SQL query results as an Excel file.                        | Show, Select commands only         |
+| `to_tsv`       | Save the SQL query results as a TSV file.                           | Show, Select commands only         |
+| `to_sql`       | Store SQL query results in another database.                        | Show, Select commands only         |
+| `URL`          | Provide the database connection URL.                                | get property                       |
+| `engine`       | Provides SQLAlchemy engine for database connection.                 | get property                       |
 
 ### Example of use
+
 The basic way to create and use each database connection object is as follows:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn, SQLiteConn
 
 # Connect to MySQL database
-mysql_conn = MySQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
+mysql_conn = MYSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to MsSQL database
 mssql_conn = MSSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to PostgreSQL database
 postgresql_conn = PostgreSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to SQLite database
 mssql_conn = SQLiteConn('your-host')
 
 # Data query example
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
 ### Using on local host
+
 The basic way to create and use a localhost database connection object is as follows:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn
 
 # Connect to MySQL database
-mysql_conn = MySQLConn('your-password')
+mysql_conn = MYSQLConn('your-password')
 
 # Connect to MsSQL database
 mssql_conn = MSSQLConn('your-password')
 
 # Connect to PostgreSQL database
 postgresql_conn = PostgreSQLConn('your-password')
 
 # Data query example
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
+### package address
+
+- [github](https://github.com/janyoungjin/SQLConn)
+
+- [pypi](https://pypi.org/project/SQLConn/)
+
 ### warning
-This document was converted from the Korean version to English through a translator, so the meaning may be strange.
+
+This document was converted from the Korean version to English through a translator, so the meaning may be strange.
```

### Comparing `SQLConn-0.0.6/SQLConn/SQLConn.py` & `SQLConn-0.0.7/SQLConn/SQLConn.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,18 @@
         if not (cmd.lower().startswith('select') or cmd.lower().startswith('show')):
             raise ValueError("to_sql does only supports 'select' or 'show' commands.")
         try:
             with other.engine.connect() as conn:
                 self.to_DataFrame(cmd).to_sql(name,conn,index=False,if_exists="replace")
         except Exception as e:
             warnings.warn(str(e))
+    def to_HTML(self,cmd:str):
+        if not (cmd.lower().startswith('select') or cmd.lower().startswith('show')):
+            raise ValueError("to_HTML does only supports 'select' or 'show' commands.")
+        self.to_DataFrame(cmd).to_html(index=False)
 class MYSQLConn(SQLConn):
     def __init__(self,password:str,host:str='127.0.0.1',user:str="root",database:str="mysql",port:str|int=3306) -> None:
         super().__init__()
         self.__host=host
         self.__user=user
         self.__password=password
         self.__database=database
```

### Comparing `SQLConn-0.0.6/SQLConn.egg-info/PKG-INFO` & `SQLConn-0.0.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,190 +1,210 @@
-Metadata-Version: 2.1
-Name: SQLConn
-Version: 0.0.6
-Summary: This package facilitates easy SQL database integration.
-Home-page: https://github.com/janyoungjin/SQLConn
-Author: janyoungjin
-Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
-Description-Content-Type: text/markdown
-Requires-Dist: mysqlclient
-Requires-Dist: pandas
-Requires-Dist: cx_oracle
-Requires-Dist: psycopg2
-Requires-Dist: pymssql
-Requires-Dist: sqlalchemy
-
 # SQLConn
+
 ## 한국어 버전(Korean Version)
+
 SQLConn은 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하여 데이터를 쉽게 조작하고 관리할 수 있는 Python 패키지입니다. 이 패키지는 MySQL, PostgreSQL, Microsoft SQL Server, Oracle 및 SQLite 데이터베이스에 대한 지원을 포함합니다.
 
 ### 기능
 
 - 여러 데이터베이스에 대한 통합된 인터페이스 제공
 - 데이터 조회 및 조작을 위한 간편한 함수 제공
 - 데이터베이스 쿼리 결과를 DataFrame으로 변환
 - CSV, Excel, TSV 파일로의 데이터 출력 지원
 - 다른 데이터베이스로의 데이터 이동 지원
 
 ### 연결가능한 데이터베이스
+
 - MySQL
 - PostgreSQL
 - Microsoft SQL Server
 - Oracle
 - SQLite
 
 ### 설치 방법
 
 파이썬과 pip가 설치된 환경에서 다음 명령어를 통해 `SQLConn` 패키지를 설치할 수 있습니다:
 
 ```bash
 pip install SQLConn
 ```
+
 ### 클래스 소개
-| 클래스명       | 소개                                                         | 특이 사항          |
-| -------------- | ------------------------------------------------------------ | ---------------- |
-| `SQLConn`      | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다. |
-| `MySQLConn`    | MySQL 데이터베이스와의 연결을 관리합니다.                     | SQLConn에게 상속 받았습니다 |
-| `MSSQLConn`    | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.       | SQLConn에게 상속 받았습니다 |
-| `PostgreSQLConn` | PostgreSQL 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
-| `OracleConn`   | Oracle 데이터베이스와의 연결을 관리합니다.                     | SQLConn에게 상속 받았습니다 |
-| `SQLiteConn`   | SQLite 파일 기반 데이터베이스와의 연결을 관리합니다.           | SQLConn에게 상속 받았습니다 |
+
+| 클래스명           | 소개                                                                    | 특이 사항                   |
+| ------------------ | ----------------------------------------------------------------------- | --------------------------- |
+| `SQLConn`        | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다.          |
+| `MYSQLConn`      | MySQL 데이터베이스와의 연결을 관리합니다.                               | SQLConn에게 상속 받았습니다 |
+| `MSSQLConn`      | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
+| `PostgreSQLConn` | PostgreSQL 데이터베이스와의 연결을 관리합니다.                          | SQLConn에게 상속 받았습니다 |
+| `OracleConn`     | Oracle 데이터베이스와의 연결을 관리합니다.                              | SQLConn에게 상속 받았습니다 |
+| `SQLiteConn`     | SQLite 파일 기반 데이터베이스와의 연결을 관리합니다.                    | SQLConn에게 상속 받았습니다 |
 
 ### 메소드 소개
-| 메소드명       | 소개                                                  | 특이사항                      |
-|--------------|--------------------------------------------------------------|------------------------------|
-| `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다. | Show, Select 커맨드만 가능    |
-| `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
-| `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
-| `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                     | Show, Select 커맨드만 가능    |
-| `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
-| `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.              | Show, Select 커맨드만 가능    |
-| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 읽기용 프로퍼티               |
-| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 읽기용 프로퍼티               |
 
+| 메소드명         | 소개                                                           | 특이사항                        |
+| ---------------- | -------------------------------------------------------------- | ------------------------------- |
+| `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다.    | Show, Select 커맨드만 가능      |
+| `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
+| `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                         | Show, Select 커맨드만 가능      |
+| `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                       | Show, Select 커맨드만 가능      |
+| `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                         | Show, Select 커맨드만 가능      |
+| `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.                | Show, Select 커맨드만 가능      |
+| `URL`          | 데이터베이스 연결 URL을 제공합니다.                            | 읽기용 프로퍼티                 |
+| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.         | 읽기용 프로퍼티                 |
 
 ### 사용예제
+
 각 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn, SQLiteConn
 
 # MySQL 데이터베이스에 연결
-mysql_conn = MySQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
+mysql_conn = MYSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # MsSQL 데이터베이스에 연결
 mssql_conn = MSSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # PostgreSQL 데이터베이스에 연결
 postgresql_conn = PostgreSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # SQLite 데이터베이스에 연결
 mssql_conn = SQLiteConn('your-host')
 
 # 데이터 조회 예제
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
 ### 로컬호스트에서 사용하기
+
 로컬 호스트 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn
 
 # MySQL 데이터베이스에 연결
-mysql_conn = MySQLConn('your-password')
+mysql_conn = MYSQLConn('your-password')
 
 # MsSQL 데이터베이스에 연결
 mssql_conn = MSSQLConn('your-password')
 
 # PostgreSQL 데이터베이스에 연결
 postgresql_conn = PostgreSQLConn('your-password')
 
 # 데이터 조회 예제
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
+### 패키지 주소
+
+- [github](https://github.com/janyoungjin/SQLConn)
+- [pypi](https://pypi.org/project/SQLConn/)
+
 ## English Version
+
 SQLConn is a Python package that connects to various SQL database management systems (DBMS) to easily manipulate and manage data. This package includes support for MySQL, PostgreSQL, Microsoft SQL Server, Oracle, and SQLite databases.
 
 ### function
 
 - Provides a unified interface to multiple databases
 - Provides simple functions for data inquiry and manipulation
 - Convert database query results to DataFrame
 - Supports data output to CSV, Excel, TSV files
 - Support for data movement to other databases
+
 ### Support database
+
 - MySQL
 - PostgreSQL
 - Microsoft SQL Server
 - Oracle
 - SQLite
 
 ### How to install
 
 In an environment where Python and pip are installed, you can install the `SQLConn` package using the following command:
 
 ```bash
 pip install SQLConn
 ```
+
 ### class info
-| class name | info | significant |
-| -------------- | ----------------------------------------------- | ---------------- |
-| `SQLConn` | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
-| `MySQLConn` | Manages MySQL database relationships. | protected  SQLConn |
-| `MSSQLConn` | Manages connections to Microsoft SQL Server databases. | protected  SQLConn |
-| `PostgreSQLConn` | Manages connections to PostgreSQL databases. | protected  SQLConn |
-| `OracleCon` | Manages Oracle database relationships. | protected  SQLConn |
-| `SQLiteConn` | Manages SQLite file-based database relationships. | protected  SQLConn |
+
+| class name         | info                                                                    | significant              |
+| ------------------ | ----------------------------------------------------------------------- | ------------------------ |
+| `SQLConn`        | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
+| `MYSQLConn`      | Manages MySQL database relationships.                                   | protected  SQLConn       |
+| `MSSQLConn`      | Manages connections to Microsoft SQL Server databases.                  | protected  SQLConn       |
+| `PostgreSQLConn` | Manages connections to PostgreSQL databases.                            | protected  SQLConn       |
+| `OracleCon`      | Manages Oracle database relationships.                                  | protected  SQLConn       |
+| `SQLiteConn`     | Manages SQLite file-based database relationships.                       | protected  SQLConn       |
 
 ### method info
-| method name       | info                                                  | significant                      |
-|--------------|--------------------------------------------------------------|------------------------------|
-| `to_DataFrame` | Executes a SQL query and returns the results as a pandas DataFrame. | Show, Select commands only |
-| `execute` | Executes a SQL query on a database but returns no results. | Show, Select command not available |
-| `to_csv` | Save the SQL query results as a CSV file. | Show, Select commands only |
-| `to_excel` | Save the SQL query results as an Excel file. | Show, Select commands only |
-| `to_tsv` | Save the SQL query results as a TSV file. | Show, Select commands only |
-| `to_sql` | Store SQL query results in another database. | Show, Select commands only |
-| `URL` | Provide the database connection URL. | get property |
-| `engine` | Provides SQLAlchemy engine for database connection. | get property |
+
+| method name      | info                                                                | significant                        |
+| ---------------- | ------------------------------------------------------------------- | ---------------------------------- |
+| `to_DataFrame` | Executes a SQL query and returns the results as a pandas DataFrame. | Show, Select commands only         |
+| `execute`      | Executes a SQL query on a database but returns no results.          | Show, Select command not available |
+| `to_csv`       | Save the SQL query results as a CSV file.                           | Show, Select commands only         |
+| `to_excel`     | Save the SQL query results as an Excel file.                        | Show, Select commands only         |
+| `to_tsv`       | Save the SQL query results as a TSV file.                           | Show, Select commands only         |
+| `to_sql`       | Store SQL query results in another database.                        | Show, Select commands only         |
+| `URL`          | Provide the database connection URL.                                | get property                       |
+| `engine`       | Provides SQLAlchemy engine for database connection.                 | get property                       |
 
 ### Example of use
+
 The basic way to create and use each database connection object is as follows:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn, SQLiteConn
 
 # Connect to MySQL database
-mysql_conn = MySQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
+mysql_conn = MYSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to MsSQL database
 mssql_conn = MSSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to PostgreSQL database
 postgresql_conn = PostgreSQLConn(host='your-host', user='your-user', password='your-password', database='your-database',port='your-port')
 
 # Connect to SQLite database
 mssql_conn = SQLiteConn('your-host')
 
 # Data query example
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
 ### Using on local host
+
 The basic way to create and use a localhost database connection object is as follows:
+
 ```py
-from SQLConn import MySQLConn, PostgreSQLConn
+from SQLConn import MYSQLConn, PostgreSQLConn, MSSQLConn
 
 # Connect to MySQL database
-mysql_conn = MySQLConn('your-password')
+mysql_conn = MYSQLConn('your-password')
 
 # Connect to MsSQL database
 mssql_conn = MSSQLConn('your-password')
 
 # Connect to PostgreSQL database
 postgresql_conn = PostgreSQLConn('your-password')
 
 # Data query example
 df = mysql_conn.to_DataFrame("SELECT * FROM your_table")
 print(df)
 ```
+
+### package address
+
+- [github](https://github.com/janyoungjin/SQLConn)
+
+- [pypi](https://pypi.org/project/SQLConn/)
+
 ### warning
+
 This document was converted from the Korean version to English through a translator, so the meaning may be strange.
```

### Comparing `SQLConn-0.0.6/setup.py` & `SQLConn-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='SQLConn',
-    version='0.0.6',
+    version='0.0.7',
     description='This package facilitates easy SQL database integration.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='janyoungjin',
     install_requires=['mysqlclient', 'pandas', 'cx_oracle', 'psycopg2', 'pymssql','sqlalchemy'],
     packages=find_packages(exclude=[]),
     url='https://github.com/janyoungjin/SQLConn',
```

