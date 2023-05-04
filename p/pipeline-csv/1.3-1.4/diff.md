# Comparing `tmp/pipeline_csv-1.3.tar.gz` & `tmp/pipeline_csv-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_csv-1.3.tar", last modified: Fri Apr 14 08:12:18 2023, max compression
+gzip compressed data, was "pipeline_csv-1.4.tar", last modified: Thu May  4 09:46:50 2023, max compression
```

## Comparing `pipeline_csv-1.3.tar` & `pipeline_csv-1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:12:18.635825 pipeline_csv-1.3/
--rw-rw-rw-   0        0        0     1094 2023-03-13 10:59:03.000000 pipeline_csv-1.3/LICENSE
--rw-rw-rw-   0        0        0       60 2023-03-14 17:31:18.000000 pipeline_csv-1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9222 2023-04-14 08:12:18.651449 pipeline_csv-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6634 2023-03-30 05:04:13.000000 pipeline_csv-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 08:12:18.588945 pipeline_csv-1.3/pipeline_csv/
--rw-rw-rw-   0        0        0      701 2023-03-15 17:59:16.000000 pipeline_csv-1.3/pipeline_csv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:12:18.620198 pipeline_csv-1.3/pipeline_csv/csvfile/
--rw-rw-rw-   0        0        0    10771 2023-03-14 17:31:18.000000 pipeline_csv-1.3/pipeline_csv/csvfile/README.md
--rw-rw-rw-   0        0        0     9651 2023-03-30 11:58:25.000000 pipeline_csv-1.3/pipeline_csv/csvfile/__init__.py
--rw-rw-rw-   0        0        0    15597 2023-03-30 11:58:25.000000 pipeline_csv-1.3/pipeline_csv/csvfile/row.py
--rw-rw-rw-   0        0        0     4461 2023-03-23 18:46:32.000000 pipeline_csv-1.3/pipeline_csv/csvfile/tubes.py
--rw-rw-rw-   0        0        0     5965 2023-03-29 13:25:05.000000 pipeline_csv-1.3/pipeline_csv/oegiv.py
--rw-rw-rw-   0        0        0     2267 2023-04-14 04:49:03.000000 pipeline_csv-1.3/pipeline_csv/orientation.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:12:18.604573 pipeline_csv-1.3/pipeline_csv.egg-info/
--rw-rw-rw-   0        0        0     9222 2023-04-14 08:12:18.000000 pipeline_csv-1.3/pipeline_csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-04-14 08:12:18.000000 pipeline_csv-1.3/pipeline_csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:12:18.000000 pipeline_csv-1.3/pipeline_csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 08:12:18.000000 pipeline_csv-1.3/pipeline_csv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-03-14 17:31:18.000000 pipeline_csv-1.3/pyproject.toml
--rw-rw-rw-   0        0        0      664 2023-04-14 08:12:18.651449 pipeline_csv-1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 09:46:50.290238 pipeline_csv-1.4/
+-rw-rw-rw-   0        0        0     1094 2023-03-13 10:59:03.000000 pipeline_csv-1.4/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-03-14 17:31:18.000000 pipeline_csv-1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7171 2023-05-04 09:46:50.290238 pipeline_csv-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6634 2023-05-04 09:42:35.000000 pipeline_csv-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 09:46:50.274612 pipeline_csv-1.4/pipeline_csv/
+-rw-rw-rw-   0        0        0      701 2023-03-15 17:59:16.000000 pipeline_csv-1.4/pipeline_csv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:46:50.290238 pipeline_csv-1.4/pipeline_csv/csvfile/
+-rw-rw-rw-   0        0        0    13051 2023-05-04 09:42:35.000000 pipeline_csv-1.4/pipeline_csv/csvfile/README.md
+-rw-rw-rw-   0        0        0    10055 2023-05-04 09:42:35.000000 pipeline_csv-1.4/pipeline_csv/csvfile/__init__.py
+-rw-rw-rw-   0        0        0    16783 2023-05-04 09:42:35.000000 pipeline_csv-1.4/pipeline_csv/csvfile/row.py
+-rw-rw-rw-   0        0        0     4765 2023-05-04 09:42:35.000000 pipeline_csv-1.4/pipeline_csv/csvfile/tubes.py
+-rw-rw-rw-   0        0        0     5965 2023-03-29 13:25:05.000000 pipeline_csv-1.4/pipeline_csv/oegiv.py
+-rw-rw-rw-   0        0        0     2267 2023-04-14 04:49:03.000000 pipeline_csv-1.4/pipeline_csv/orientation.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:46:50.290238 pipeline_csv-1.4/pipeline_csv.egg-info/
+-rw-rw-rw-   0        0        0     7171 2023-05-04 09:46:50.000000 pipeline_csv-1.4/pipeline_csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-04 09:46:50.000000 pipeline_csv-1.4/pipeline_csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:46:50.000000 pipeline_csv-1.4/pipeline_csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 09:46:50.000000 pipeline_csv-1.4/pipeline_csv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-03-14 17:31:18.000000 pipeline_csv-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      664 2023-05-04 09:46:50.305864 pipeline_csv-1.4/setup.cfg
```

### Comparing `pipeline_csv-1.3/LICENSE` & `pipeline_csv-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.3/README.md` & `pipeline_csv-1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PipelineCsv library
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/pipeline.csv/pep257.yml?label=Pep257&style=plastic&branch=main)](https://github.com/vb64/pipeline.csv/actions?query=workflow%3Apep257)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/pipeline.csv/py3.yml?label=Python%203.7-3.10&style=plastic&branch=main)](https://github.com/vb64/pipeline.csv/actions?query=workflow%3Apy3)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/pipeline.csv/py3.yml?label=Python%203.7-3.11&style=plastic&branch=main)](https://github.com/vb64/pipeline.csv/actions?query=workflow%3Apy3)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/031838411159440885e8c4a28f233c4e)](https://www.codacy.com/gh/vb64/pipeline.csv/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vb64/pipeline.csv&amp;utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/031838411159440885e8c4a28f233c4e)](https://www.codacy.com/gh/vb64/pipeline.csv/dashboard?utm_source=github.com&utm_medium=referral&utm_content=vb64/pipeline.csv&utm_campaign=Badge_Coverage)
 
 [In Russian](READMEru.md)
 
 The free, open source PipelineCsv library is designed to work with the results of analysis of in-line flaw detection data in the form of a CSV file.
```

### Comparing `pipeline_csv-1.3/pipeline_csv/__init__.py` & `pipeline_csv-1.4/pipeline_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.3/pipeline_csv/csvfile/README.md` & `pipeline_csv-1.4/pipeline_csv/csvfile/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Формат файла экспорта/импорта
 
 Файл в кодировке, указанной в атрибуте `ENCODING` класса `File` с разделителем колонок ';' и первой строкой, содержащей заголовки колонок данных.
 Файл содержит 27 колонок. Часть колонок интерпретируется одинаково для всех типов обьектов.
-Для другой части колонок их данные интерпретируются в запвисимости от типа обьекта в конкретной строке.
+Для другой части колонок их данные интерпретируются в зависимости от типа обьекта в конкретной строке.
 
 ## Общие колонки для всех типов обьектов
 
 ### Дистанция по одометру
 
 Номер колонки '01' заголовок 'DistOd'
 
@@ -45,14 +45,20 @@
 
 -   25 Latitude Широта
 -   26 Longtitude Долгота
 -   27 Altitude Высота
 
 Числа с плавающей точкой, представляющие  гео-координаты обьекта.
 
+### Опциональный идентификатор
+
+Номер колонки '16' заголовок 'DistML'
+
+Если задано, то должно содержать уникальный для данной колонки идентификатор обьекта (строка).
+
 ### Колонки, используемые для привязки обьектов к маркерам и швам в экспресс-отчете InspectionViewer
 
 -   04 ObjectName Текст до 20 символов длиной.
 -   16 DistML Дистанция до маркера слева в мм.
 -   17 DistMR Дистанция до маркера справа в мм.
 -   18 DistStL Дистанция до стыка слева в мм.
 -   19 DistStR Дистанция до стыка справа в мм.
@@ -83,15 +89,17 @@
 
 Если значение колонки 02 TypeObject установлено в 0 (Шов)
 
 Колонка 03 Object_Code должна содержать код 0, а колонка 05 Object_Code_T должна содержать текст 'Шов'.
 
 Колонка 04 ObjectName может содержать пользовательский номер трубы (произвольная строка в кодировке win-1251).
 
-Колонка  09 Depth_min может содержать радиус изгиба трубы в ее диаметрах (с плавающей точкой).
+Колонка 09 Depth_min может содержать радиус изгиба трубы в ее диаметрах (с плавающей точкой).
+
+Колонка 10 Depth_max может содержать минимальное проходное сечение трубы в мм (строка).
 
 Остальные колонки должны быть пустыми.
 
 ### Маркеры
 
 Если значение колонки 02 TypeObject установлено в 1 (Маркер)
 
@@ -190,7 +198,40 @@
 Если значение колонки 02 TypeObject установлено в 5 (Категория трубопровода)
 
 Колонка 03 Object_Code должна содержать код 0, а колонка 05 Object_Code_T должна содержать текст 'Категория трубопровода'.
 
 Колонка 10 Depth_max должна содержать код категории трубопровода.
 
 Остальные колонки должны быть пустыми.
+
+## Схема использования колонок по типам обьектов
+
+```
+                                   All  Weld  Mark  Defect  Wall  Seam  Category
+01 DistOd                          +    +     +     +       +     +     +
+02 TypeObject                      +    +     +     +       +     +     +
+03 Object_Code                          +     +     +       +     +     +
+04 ObjectName                           +     
+05 Object_Code_T                        +     +     +       +           +
+06 Marker                          +    +     +     +       +     +     +
+07 Length                                           +
+08 Width                                            +
+09 Depth_min                            +           +
+10 Depth_max                            +           +       +           +
+11 OrientTD                                         +             +
+12 OrientBD                                         +             +
+13 MPoint_Orient                                    +
+14 MPoint_Dist                                      +
+15 Type_Def                                         +
+16 DistML                          +    +     +     +       +     +     +
+17 DistMR                          -     
+18 DistStL                         -      
+19 DistStR                         -      
+20 LinkStL                         -      
+21 LinkStR                         -      
+22 LinkML                          -     
+23 LinkMR                          -     
+24 Comments                        +    +     +     +       +     +     +
+25 Latitude                        +    +     +     +       +     +     +
+26 Longtitude                      +    +     +     +       +     +     +
+27 Altitude                        +    +     +     +       +     +     +
+```
```

### Comparing `pipeline_csv-1.3/pipeline_csv/csvfile/__init__.py` & `pipeline_csv-1.4/pipeline_csv/csvfile/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     return table_index, pos
 
 
 class Stream:
     """Holds current state of data stream."""
 
     def __init__(self):
-        """Inital data stream state."""
+        """Init data stream state."""
         self.thick = None
         self.category = None
 
 
 class FloatDelimiter:
     """Possible float delimiter for output csv."""
 
@@ -134,14 +134,15 @@
 
     def __init__(self, float_delimiter=FloatDelimiter.Point):
         """Create empty csv file object."""
         self.data = []
         self.thicks = []
         self.categories = []
         self.float_delimiter = float_delimiter
+        self.ids = set()
         self.stream = Stream()
 
     @classmethod
     def open_file(cls, file_path, mode):
         """Open file wrapper."""
         return open(file_path, mode + 't', encoding=cls.ENCODING)
 
@@ -158,22 +159,31 @@
         next(reader)  # skip column titles row
         for row in reader:
 
             if not row:
                 continue
 
             item = cls.RowCls.from_csv_row(row)
+            obj.check_id_unique(item)
             obj.data.append(item)
+
             if item.is_category:
                 obj.categories.append(item)
             elif item.is_thick:
                 obj.thicks.append(item)
 
         return obj
 
+    def check_id_unique(self, row):
+        """Check for row ID property is unique."""
+        if row.obj_id:
+            if row.obj_id in self.ids:
+                raise Error("Duplicate object ID: '{}'".format(row.obj_id))
+            self.ids.add(row.obj_id)
+
     @property
     def total_length(self):
         """Reckord total length."""
         return int(self.data[-1].dist_od)
 
     def make_distances_unique(self, dist_shift_mm=1):
         """Make distances of rows unique, by increasing values of duplicate distances."""
@@ -185,20 +195,22 @@
                 shift_count += 1
             dist_list.append(row.dist_od)
 
         return shift_count
 
     def to_file(self, file_path):
         """Save csv to file."""
+        self.ids.clear()
         output = self.open_file(file_path, 'w')
         writer = csv.writer(output, delimiter=self.DELIMETER, lineterminator='\n')
 
         writer.writerow(self.COLUMN_HEADS)
         for row in sorted(self.data, key=lambda val: int(val.dist_od)):
             if int(row.type_object) >= 0:
+                self.check_id_unique(row)
                 writer.writerow(format_floats(row.values(), self.float_delimiter))
 
         output.close()
 
     def append(self, csv_file):
         """Append data from csv file."""
         length = self.total_length
```

### Comparing `pipeline_csv-1.3/pipeline_csv/csvfile/row.py` & `pipeline_csv-1.4/pipeline_csv/csvfile/row.py`

 * *Files 8% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         self.link_mr = ''
         self.comments = ''
         self.latitude = ''
         self.longtitude = ''
         self.altitude = ''
 
     def __str__(self):
-        """String representation for row object."""
+        """As text."""
         return ';'.join([str(i) for i in self.values()])
 
     @property
     def marker(self):
         """Return string for marker feature."""
         return self.get_bool(self.is_marker_int)
 
@@ -174,14 +174,34 @@
         return self.is_lineobj and self.is_marker_int
 
     @property
     def dist(self):
         """Return object distance as integer mm."""
         return int(self.dist_od)
 
+    @property
+    def obj_id(self):
+        """Return optional object ID as string."""
+        return self.dist_ml
+
+    @obj_id.setter
+    def obj_id(self, value):
+        """Set optional object ID as string."""
+        self.dist_ml = str(value).strip()
+
+    @property
+    def min_diam(self):
+        """Return optional minimal pipe diameter as string (mm)."""
+        return self.depth_max
+
+    @min_diam.setter
+    def min_diam(self, value):
+        """Set optional minimal pipe diameter as string (mm)."""
+        self.depth_max = value
+
     @staticmethod
     def get_minutes(text):
         """Restore full integer minute from text 'hours,minites'."""
         val = Orientation.from_csv(text)
 
         if val is None:
             return None
@@ -204,102 +224,119 @@
             self.latitude = latitude
             self.longtitude = longtitude
             self.altitude = altitude
 
         return self
 
     @classmethod
-    def with_dist(cls, distanse, latitude='', longtitude='', altitude=''):
+    def with_dist(cls, distanse, obj_id='', latitude='', longtitude='', altitude=''):
         """Construct row as common object with dist and geo."""
         obj = cls()
         obj.dist_od = int(distanse)
+        obj.obj_id = obj_id
 
         return obj.set_geo(latitude, longtitude, altitude)
 
     @classmethod
-    def as_common(cls, distanse, typ, latitude='', longtitude='', altitude=''):
+    def as_common(cls, distanse, typ, obj_id='', latitude='', longtitude='', altitude=''):
         """Construct row as common object."""
-        obj = cls.with_dist(distanse, latitude, longtitude, altitude)
+        obj = cls.with_dist(distanse, obj_id=obj_id, latitude=latitude, longtitude=longtitude, altitude=altitude)
         obj.type_object = typ
         obj.object_code_t = cls.name_object(obj.type_object)
 
         return obj
 
     @classmethod
-    def as_weld(cls, distanse, custom_number='', latitude='', longtitude='', altitude=''):
+    def as_weld(cls, distanse, min_diam=None, obj_id='', custom_number='', latitude='', longtitude='', altitude=''):
         """Construct row as weld object."""
-        obj = cls.as_common(distanse, ObjectClass.WELD, latitude, longtitude, altitude)
+        obj = cls.as_common(
+          distanse, ObjectClass.WELD,
+          obj_id=obj_id,
+          latitude=latitude, longtitude=longtitude, altitude=altitude
+        )
+
         if custom_number:
             obj.object_name = custom_number
 
+        if min_diam:
+            obj.min_diam = min_diam
+
         return obj
 
     @classmethod
-    def as_thick(cls, distanse, thick, latitude='', longtitude='', altitude=''):
+    def as_thick(cls, distanse, thick, obj_id='', latitude='', longtitude='', altitude=''):
         """Construct row as thickness change object."""
-        obj = cls.as_common(distanse, ObjectClass.THICK, latitude, longtitude, altitude)
+        obj = cls.as_common(
+          distanse, ObjectClass.THICK,
+          obj_id=obj_id,
+          latitude=latitude, longtitude=longtitude, altitude=altitude
+        )
         obj.depth_max = thick
         return obj
 
     @classmethod
-    def as_category(cls, distanse, category, latitude='', longtitude='', altitude=''):
+    def as_category(cls, distanse, category, obj_id='', latitude='', longtitude='', altitude=''):
         """Construct row as pipeline category object."""
-        obj = cls.as_common(distanse, ObjectClass.PIPELINE_CATEGORY, latitude, longtitude, altitude)
+        obj = cls.as_common(
+          distanse, ObjectClass.PIPELINE_CATEGORY,
+          obj_id=obj_id,
+          latitude=latitude, longtitude=longtitude, altitude=altitude
+        )
         obj.depth_max = category
         return obj
 
     @classmethod
-    def as_seam(cls, distanse, typ, orient1, orient2):
+    def as_seam(cls, distanse, typ, orient1, orient2, obj_id=''):
         """Construct row as seam object with given typ."""
         if typ not in SEAM:
             raise Error("Wrong seam type: {}".format(typ))
 
-        obj = cls.with_dist(distanse, '', '', '')
+        obj = cls.with_dist(distanse, obj_id=obj_id, latitude='', longtitude='', altitude='')
         obj.type_object = ObjectClass.HOR_WELD
         obj.object_code = typ
         obj.object_code_t = cls.name_seam(obj.object_code)
 
         if obj.object_code in [TypeHorWeld.HORIZONTAL, TypeHorWeld.SPIRAL, TypeHorWeld.SECOND]:
             obj.orient_td = str(orient1)
 
         if obj.object_code in [TypeHorWeld.SECOND]:
             obj.orient_bd = str(orient2)
 
         return obj
 
     @classmethod
-    def as_lineobj(cls, distanse, typ, name, is_marker, comment, latitude='', longtitude='', altitude=''):
+    def as_lineobj(cls, distanse, typ, name, is_marker, comment, obj_id='', latitude='', longtitude='', altitude=''):
         """Construct row as line object."""
         lineobj = cls.lineobj_dict()
         if typ not in lineobj:
             raise Error("Wrong lineobj type: {}".format(typ))
 
-        obj = cls.with_dist(distanse, latitude, longtitude, altitude)
+        obj = cls.with_dist(distanse, obj_id=obj_id, latitude=latitude, longtitude=longtitude, altitude=altitude)
         obj.type_object = ObjectClass.MARKER
         obj.object_code = typ
         obj.object_code_t = lineobj[obj.object_code]
         obj.object_name = name
         obj.is_marker_int = is_marker
         obj.comments = comment
 
         return obj
 
     @classmethod
-    def as_defekt(  # pylint: disable=too-many-locals
+    def as_defekt(  # pylint: disable=too-many-locals,too-many-arguments
       cls, distanse, typ, side, length, width, depth, orient1, orient2, mp_orient, mp_dist, comment,
-      latitude='', longtitude='', altitude=''
+      obj_id='', latitude='', longtitude='', altitude=''
     ):
         """Construct row as defekt object."""
         defekts = cls.defekts_dict()
         if typ not in defekts:
             raise Error("Wrong defekt type: {}".format(typ))
 
         depth_int = to_int(depth)
 
-        obj = cls.with_dist(distanse, latitude, longtitude, altitude)
+        obj = cls.with_dist(distanse, obj_id=obj_id, latitude=latitude, longtitude=longtitude, altitude=altitude)
         obj.type_object = ObjectClass.DEFEKT
         obj.object_code = typ
         obj.object_code_t = defekts[obj.object_code]
 
         if orient1:
             obj.orient_td = str(orient1)
         if orient2:
```

### Comparing `pipeline_csv-1.3/pipeline_csv/csvfile/tubes.py` & `pipeline_csv-1.4/pipeline_csv/csvfile/tubes.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,24 @@
         return self.row.depth_min
 
     def set_radius(self, val):
         """Set tube curve radius."""
         self.row.depth_min = val
 
     @property
+    def min_diam(self):
+        """Return optional minimal pipe diameter as string (mm)."""
+        return self.row.depth_max
+
+    @min_diam.setter
+    def min_diam(self, value):
+        """Set optional minimal pipe diameter as string (mm)."""
+        self.row.depth_max = value
+
+    @property
     def number(self):
         """Tube custom or auto number."""
         num = self.row.object_name.strip()
         if not num:
             num = self.auto_number
         return num
```

### Comparing `pipeline_csv-1.3/pipeline_csv/oegiv.py` & `pipeline_csv-1.4/pipeline_csv/oegiv.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.3/pipeline_csv/orientation.py` & `pipeline_csv-1.4/pipeline_csv/orientation.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.3/setup.cfg` & `pipeline_csv-1.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6970 656c 696e 655f 6373 760d   = pipeline_csv.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e33 0d0a  .version = 1.3..
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e34 0d0a  .version = 1.4..
 00000030: 6175 7468 6f72 203d 2056 6974 616c 7920  author = Vitaly 
 00000040: 426f 676f 6d6f 6c6f 760d 0a61 7574 686f  Bogomolov..autho
 00000050: 725f 656d 6169 6c20 3d20 6d61 696c 4076  r_email = mail@v
 00000060: 6974 616c 792d 626f 676f 6d6f 6c6f 762e  italy-bogomolov.
 00000070: 7275 0d0a 6465 7363 7269 7074 696f 6e20  ru..description 
 00000080: 3d20 5069 7065 6c69 6e65 2069 6e6c 696e  = Pipeline inlin
 00000090: 6520 696e 7370 6563 7469 6f6e 2064 6174  e inspection dat
```

