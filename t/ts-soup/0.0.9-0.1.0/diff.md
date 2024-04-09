# Comparing `tmp/ts-soup-0.0.9.tar.gz` & `tmp/ts-soup-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-_ntpj_yd\ts-soup-0.0.9.tar", last modified: Sun Apr  7 06:47:24 2024, max compression
+gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-gejmd28n\ts-soup-0.1.0.tar", last modified: Tue Apr  9 03:14:10 2024, max compression
```

## Comparing `ts-soup-0.0.9.tar` & `ts-soup-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 06:47:24.520920 ts-soup-0.0.9/
--rw-rw-rw-   0        0        0     1028 2024-04-07 06:47:24.519919 ts-soup-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts-soup-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 06:47:24.520920 ts-soup-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      607 2024-04-07 06:47:13.000000 ts-soup-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:47:24.506431 ts-soup-0.0.9/ts_soup/
--rw-rw-rw-   0        0        0      307 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/app.py
--rw-rw-rw-   0        0        0    18009 2024-04-07 06:46:03.000000 ts-soup-0.0.9/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:47:24.516559 ts-soup-0.0.9/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     5793 2024-04-07 01:22:11.000000 ts-soup-0.0.9/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-07 06:47:24.518559 ts-soup-0.0.9/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-07 06:47:24.000000 ts-soup-0.0.9/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-07 06:47:24.000000 ts-soup-0.0.9/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 06:47:24.000000 ts-soup-0.0.9/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 06:47:24.000000 ts-soup-0.0.9/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 03:14:10.901619 ts-soup-0.1.0/
+-rw-rw-rw-   0        0        0     1028 2024-04-09 03:14:10.900617 ts-soup-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts-soup-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 03:14:10.901619 ts-soup-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-09 03:12:51.000000 ts-soup-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:14:10.887588 ts-soup-0.1.0/ts_soup/
+-rw-rw-rw-   0        0        0      411 2024-04-09 03:12:17.000000 ts-soup-0.1.0/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts-soup-0.1.0/ts_soup/app.py
+-rw-rw-rw-   0        0        0    15530 2024-04-09 03:12:17.000000 ts-soup-0.1.0/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:14:10.896665 ts-soup-0.1.0/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts-soup-0.1.0/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-07 01:22:11.000000 ts-soup-0.1.0/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     3955 2024-04-09 03:12:17.000000 ts-soup-0.1.0/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:14:10.899116 ts-soup-0.1.0/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-09 03:14:10.000000 ts-soup-0.1.0/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-09 03:14:10.000000 ts-soup-0.1.0/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:14:10.000000 ts-soup-0.1.0/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 03:14:10.000000 ts-soup-0.1.0/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.0.9/PKG-INFO` & `ts-soup-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.9
+Version: 0.1.0
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.0.9/README.md` & `ts-soup-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.9/setup.py` & `ts-soup-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.0.9",
+  version="0.1.0",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts-soup-0.0.9/ts_soup/app.py` & `ts-soup-0.1.0/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.9/ts_soup/common.py` & `ts-soup-0.1.0/ts_soup/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import pandas as pd
 from functools import wraps
 import traceback
 
 import pymysql
 from sqlalchemy import create_engine
 
-"""
-"""
 
 warnings.filterwarnings('ignore')
 
+# 注册形成的数据库连接
 USABLE_DBS = {}
 
 CURRENT_DATE = None
 SYNC_FROM_DATE = None
+
+# 同步程序执行情况
 EXECUTE_STATE = True
-"""
-记录每个表的更新状况的矩阵，全局对象
-"""
+
+# 记录每个表的更新状况的矩阵，全局对象
 DATA_UPDATED_STATE = None
 
 
 def query_in_sql(list_):
     return ','.join(list(map(lambda x: '"' + x + '"', list_)))
 
 
@@ -50,14 +50,17 @@
     USABLE_DBS[db_info['alias'] + '_pym'] = engine
     if db_info['default']:
         USABLE_DBS[f'{db_type}_default_pym'] = engine
 
 
 def __init(customized_table, customized_time, sync_start, sync_end, db_infos):
     """
+    整个同步程序的初始化程序，并处理命令行参数 1、读取之前更新状态，形成updated_state矩阵。
+                                        2、确定需要更新的table
+    形成策略：
      1、指定时间，未指定表格:
         data_updated_state: 第四类转换完成的data_updated_state,对应时间的行 state列全部赋值为 0
         to_update_tables: 返回查询结果
      2、指定表格，未指定时间：
         data_updated_state: 第四类转换完成的data_updated_state
         to_update_tables: 返回指定表格
      3、指定时间，指定表格:
@@ -84,14 +87,15 @@
                         get_sqlalchemy_engine(db_info, db_type)
                     else:
                         get_pymsql_engine(db_info, db_type)
 
             else:
                 raise ValueError('未配置engine类型')
 
+
     SYNC_FROM_DATE = sync_start
     CURRENT_DATE = sync_end
     to_update_tables = pd.read_sql('select * from to_update_tables', con=USABLE_DBS['targets_default'])['table_name']
     with USABLE_DBS['targets_default'].begin() as conn:
         conn.execute("""
         CREATE TABLE if not exists `updated_state`  (
                       `update_date` date DEFAULT NULL,
@@ -136,82 +140,86 @@
 
     else:
         DATA_UPDATED_STATE = state_table  # 4、未指定时间，未指定表格:
         return to_update_tables
 
 
 class BaseSource(ABC):
-    def __init__(self, db, index_field, empty_check):
+    """
+    定义需要使用在入口函数中注册的数据库连接的source的基类，即 如果需要使用数据库连接，则需要继承BaseSource
+    """
+    def __init__(self,
+                 db:str=None,
+                 index_field: str = 'date',
+                 empty_check: bool = True):
         """
         :param db: 数据库名
         :param index_field: 数据源筛选日期的字段，如果不提供则默认"date",如果需要查询全表，则index_field需要设置为 None。
         :param empty_check: 是否为当前方法主要数据源（除了配置信息的数据源），判空时使用，若不想使当前数据源参与判空，可设为 False
         """
         self.empty_check = empty_check
         if db:
             self.db = USABLE_DBS[db]
         else:
             self.db = USABLE_DBS['sources_default']
         self.index_field = index_field
 
     @abstractmethod
     def build_source(self, to_update_date):
+        """
+        :param to_update_date:
+        :return: yyyy-mm-dd 格式日期列表
+        """
         pass
 
 
 class BaseTarget(ABC):
-    def __init__(self, tb, index_field, db, user_def_pro, drop_axis, drop_na_subset, drop_na_thresh, has_unique_idx,
-                 is_seperated):
-        self.tb = tb
-        self.user_def_pro = user_def_pro
-        if user_def_pro is None:
-            self.user_def_pro = []
-
+    """
+    定义需要使用在入口函数中注册的数据库连接的target的基类，即 如果需要使用数据库连接，则需要继承BaseTarget
+    """
+    def __init__(self,db: str = None):
         if db:
             self.db = USABLE_DBS[db]
             self.db_pym = USABLE_DBS[f'{db}_pym']
             self.db_str = db
         else:
             self.db = USABLE_DBS['targets_default']
             self.db_pym = USABLE_DBS['targets_default_pym']
             self.db_str = 'targets_default'
 
-        self.is_seperated = is_seperated
-        self.drop_axis = drop_axis
-        self.drop_na_subset = drop_na_subset
-        self.drop_na_thresh = drop_na_thresh
-        self.has_unique_idx = has_unique_idx
-        self.index_field = index_field
-
     @abstractmethod
     def build_output(self, cur_result):
+        """
+        :param to_update_date:
+        :return: yyyy-mm-dd 格式日期列表
+        """
         pass
 
 
 class Executor:
     """
     数据处理原则：
         n2one: 数据源配置为is_data=True的对应日期查询结果只要存在一个全为空，则视当天的所有数据都为空，不更新数据表，也不更新操作记录表(updated_state)
         one2n:
                如果数据结果存在一个 None或者 emptyDataframe ，则当次调用 updated_state 表不更新
                如果数据结果全都有值，但是存在个别天数的行中存在空数据，则会删除空数据对应的行，updated_state更新取每个数据结果的交集作为日期
     """
 
-    def __init__(self, sources, targets, executed_table):
+    def __init__(self, sources, targets, executed_table,customized_updated_state=None):
         """
         数据库的操作器，负责从源表读取数据 _make_source_data，以及写入目标表 _handle_result
         """
         self.any_source_empty = False
         self.value = []
         self.sources = sources
         self.targets = targets
         self.source_data = []
         self.executed_table = executed_table
         self.to_update_date = self.__get_update_date()
-        self.customized_updated_state = None
+
 
     def __get_update_date(self):
         return DATA_UPDATED_STATE.loc[~(DATA_UPDATED_STATE[self.executed_table] == 1), 'update_date']
 
     def make_source_data(self):
         """
         产生数据源source_data的方法，按照TargetInfo顺序写入 source_data中
@@ -235,134 +243,80 @@
             else:
                 raise ValueError("source.empty_check未设置")
 
             self.source_data.append(data)
 
     def handle_result(self):
         """
-        处理结果的方法
-        1.有分表的处理：
-            将value和target_info顺序展开 ，得到对应处理完的df，根据df的日期取出分表的suffix，
-            再根据suffix选择需要插入的数据进行数据插入，同时删除对应日期的数据
-        2.无分表的处理：
-            将value和target_info顺序展开 ，得到对应处理完的df，删除对应日期的数据，进行数据插入
-        3.update_state处理：
-            在依次遍历value时选择各数据目标df最小的索引集合（取交集），以使得多个数据目标时，如果多个表的对应
-            索引值存在缺失，可以在下一次同步时进行同步。
+        调用各target处理对应返回结果的方法，并取得各target执行后需要更新的日期，updated_date
+        update_state处理：
+            在依次遍历value时选择各数据目标df最小的日期集合（取交集），以使得多个target时，如果多个target的对应
+            日期缺失，则updated_state依旧为0 。
         :return:
         """
         update_state_date = None
         func_update_flag = True
         for index, target in enumerate(self.targets):
             cur_result = self.value[index]
 
-            if len(target.user_def_pro) > 0:  # 获取在funcs里传入的额外属性（target未定义的）
-                for pro in target.user_def_pro:
-                    setattr(target, pro, getattr(self, pro))
-
             """
              处理返回值整个为none，如有一个返回结果为none，则整个方法的 这段to_update_date时间都应视为无数据，防止下文
              转str和合并索引时产生keyError
              """
             if cur_result is None:
                 func_update_flag = False
                 print(f'{target.tb} 无数据同步')
                 continue
 
-            # 处理返回值部分为空的情况
-            params = {'axis': target.drop_axis, 'how': 'all', 'thresh': target.drop_na_thresh}
-            if target.drop_na_subset:
-                params['subset'] = target.drop_na_subset
-            cur_result = cur_result.dropna(**params)
-
-            # 处理经过dropna以后如果全为空的情况，视为全为空，原理同上
-            if cur_result.empty:
-                func_update_flag = False
-                print(f'{target.tb} 无数据同步')
+            # 调用统一接口完成成果产出，返回每个target更新的日期，最后取交集作为该func的完成同步的日期
+            # 先统一转datetime，再转str
+            updated_date = target.build_output(cur_result)
+            if updated_date is None:
                 continue
-
-            """统一把index_field字段转为str类型，防止后面在insert_update_state 和各表插入数据时 使用datetime64 或 int等类型"""
-            # datetime.date 在dataframe中有可能是Object类型
-            if str(cur_result[target.index_field].dtypes) == 'datetime64' or str(
-                    cur_result[target.index_field].dtypes).lower() == 'object':
-                cur_result[target.index_field] = pd.to_datetime(cur_result[target.index_field]).apply(
-                    lambda x: x.strftime('%Y-%m-%d'))
-            else:
-                # 碰到其他情况再继续完善，例如此处是inheritId，则把int或float转str
-                cur_result[target.index_field] = cur_result[target.index_field].astype(str).apply(
-                    lambda x: x.split('.')[0])
-
-            # 调用统一接口完成成果产出
-            target.build_output(cur_result)
+            date_df = pd.to_datetime(updated_date)
+            updated_date = pd.DataFrame(date_df, columns=['update_date']).drop_duplicates().applymap(lambda x:x.strftime('%Y-%m-%d'))
 
             # 如果未传入自定义更新日期，则取数据日期作为 处理操作表的更新日期，取各数据结果交集
-            if (update_state_date is not None) and (self.customized_updated_state is None):
+            if update_state_date is not None:
                 update_state_date = update_state_date.merge(
-                    cur_result[[target.index_field]].drop_duplicates(),
-                    left_on='update_date',
-                    right_on=target.index_field,
+                    pd.DataFrame(updated_date,columns=['update_date']).drop_duplicates(),
+                    on='update_date',
                     how='inner'
                 )[['update_date']]
-            elif (update_state_date is None) and (self.customized_updated_state is None):
-                update_state_date = pd.DataFrame(
-                    cur_result[target.index_field].drop_duplicates().values,
-                    columns=['update_date']
-                )
+            else:
+                update_state_date = pd.DataFrame(updated_date,columns=['update_date']).drop_duplicates()
 
         # 将方法的操作记录写入数据库
         if func_update_flag:
             if update_state_date is not None and not update_state_date.empty:
                 self.__handle_insert_update_state(update_state_date)
-            # 如果update_state_date无值，则说明传了customized值，更新日期在二者中选其一有值的
-            else:
-                if self.customized_updated_state is not None and not self.customized_updated_state.empty:
-                    self.__handle_insert_update_state(self.customized_updated_state)
 
     def __handle_insert_update_state(self, update_state):
-        """
-        为update_state可能分表做准备
-        :param update_state:
-        :return:
-        """
         update_state['table_name'] = self.executed_table
         with USABLE_DBS['targets_default'].begin() as conn:
             conn.execute(
                 f'delete from updated_state where table_name = "{self.executed_table}" and update_date in ({query_in_sql(update_state["update_date"].values.tolist())})')
             update_state.to_sql('updated_state', con=conn, index=False, if_exists='append')
 
 
-"""
-数据库装饰器 按数据流向类型区分，向数据库写入数据
-one2one:
-表示数据仅从一张表导入另一张表
-n2one:
-表示数据从多张表取汇聚成一张表
-one2n:
-数据从一张表导出分多张表导入
-n2n:
-_seperate: 采用了分表策略的表
-...
-"""
-
-
 def db_operator(sources: list, targets: list):
     """
     数据库操作器，包括源表与目标表，在funcs中需按照target_info顺序将结果添加到 executor.value中
     使用三个类来完成工作  1. Executor   方法层面，对应funcs模块中每个方法
                        2. Source 数据源层面，对应装饰器中定义的数据源
                        3. Target 目标表层面，对应装饰器中配置的目标表
     :param sources: 源表信息，list类型:
     [
-        Source(db=源表所在库名(默认ALI_DATA),tb=源表名,query_field=查询源表字段名(默认*),date_field=源表日期字段名(默认'date'，如果查全表则为None)，other_condition=其他查询条件),
-        Source(db=源表所在库名,tb=源表名,query_field=查询源表字段名,date_field=源表日期字段名，other_condition=其他查询条件) ...
+        Source(db=源表所在库名(默认ALI_DATA),tb=源表名,...),
+        Source(db=源表所在库名,tb=源表名,...) ...
     ]
     :param targets:目标表信息，list类型:
     [
-        Target(db=目标数据库，tb=目标表名,date_field=目标表日期字段名),
-        Target(db=目标数据库，tb=目标表名,date_field=目标表日期字段名) ...
+        Target(db=目标数据库，tb=目标表名,...),
+        Target(db=目标数据库，tb=目标表名,....) ...
     ]
     :return:
     """
 
     def wrapper(func):
         @wraps(func)
         def inner_wrapper():
```

### Comparing `ts-soup-0.0.9/ts_soup/workers/sources.py` & `ts-soup-0.1.0/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.9/ts_soup.egg-info/PKG-INFO` & `ts-soup-0.1.0/ts_soup.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.9
+Version: 0.1.0
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

