# Comparing `tmp/vnfaker-0.0.2.tar.gz` & `tmp/vnfaker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnfaker-0.0.2.tar", last modified: Mon May  1 03:23:22 2023, max compression
+gzip compressed data, was "vnfaker-0.0.3.tar", last modified: Thu May  4 08:39:49 2023, max compression
```

## Comparing `vnfaker-0.0.2.tar` & `vnfaker-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.345397 vnfaker-0.0.2/
--rw-r--r--   0 ducquang   (501) admin       (80)     1056 2023-04-15 03:22:43.000000 vnfaker-0.0.2/LICENSE.txt
--rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-01 03:23:22.345156 vnfaker-0.0.2/PKG-INFO
--rw-r--r--   0 ducquang   (501) admin       (80)     1177 2023-04-22 08:57:04.000000 vnfaker-0.0.2/README.md
--rw-r--r--   0 ducquang   (501) admin       (80)       38 2023-05-01 03:23:22.345492 vnfaker-0.0.2/setup.cfg
--rw-r--r--   0 ducquang   (501) admin       (80)     1006 2023-05-01 03:22:48.000000 vnfaker-0.0.2/setup.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.313522 vnfaker-0.0.2/src/
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.318135 vnfaker-0.0.2/src/vnfaker/
--rw-r--r--   0 ducquang   (501) admin       (80)       70 2023-04-22 07:54:20.000000 vnfaker-0.0.2/src/vnfaker/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     3000 2023-04-22 07:28:33.000000 vnfaker-0.0.2/src/vnfaker/commonUtils.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.320354 vnfaker-0.0.2/src/vnfaker/data/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.2/src/vnfaker/data/__init__.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.321060 vnfaker-0.0.2/src/vnfaker/data/company/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.2/src/vnfaker/data/company/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     4748 2023-04-11 01:32:31.000000 vnfaker-0.0.2/src/vnfaker/data/company/company.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.322197 vnfaker-0.0.2/src/vnfaker/data/occupation/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.2/src/vnfaker/data/occupation/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)    34962 2023-04-11 06:57:16.000000 vnfaker-0.0.2/src/vnfaker/data/occupation/occupation.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.328016 vnfaker-0.0.2/src/vnfaker/data/person/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.2/src/vnfaker/data/person/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     1136 2023-04-11 08:39:50.000000 vnfaker-0.0.2/src/vnfaker/data/person/female.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1089 2023-04-11 08:42:28.000000 vnfaker-0.0.2/src/vnfaker/data/person/female_middle.name
--rw-r--r--   0 ducquang   (501) admin       (80)      111 2023-04-10 17:26:37.000000 vnfaker-0.0.2/src/vnfaker/data/person/first.name
--rw-r--r--   0 ducquang   (501) admin       (80)      148 2023-04-11 08:43:12.000000 vnfaker-0.0.2/src/vnfaker/data/person/last.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1782 2023-04-25 12:45:47.000000 vnfaker-0.0.2/src/vnfaker/data/person/male.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1178 2023-04-11 08:38:25.000000 vnfaker-0.0.2/src/vnfaker/data/person/male_middle.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.335864 vnfaker-0.0.2/src/vnfaker/data/provinces/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.2/src/vnfaker/data/provinces/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)  3512185 2023-04-10 17:48:23.000000 vnfaker-0.0.2/src/vnfaker/data/provinces/flat-divisions.json
--rw-r--r--   0 ducquang   (501) admin       (80)  2404923 2023-04-10 17:48:23.000000 vnfaker-0.0.2/src/vnfaker/data/provinces/nested-divisions.json
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.341188 vnfaker-0.0.2/src/vnfaker/data/sentence/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.2/src/vnfaker/data/sentence/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)   244103 2023-04-12 08:52:12.000000 vnfaker-0.0.2/src/vnfaker/data/sentence/sentence.txt
--rw-r--r--   0 ducquang   (501) admin       (80)     9052 2023-05-01 03:22:48.000000 vnfaker-0.0.2/src/vnfaker/generator.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.320002 vnfaker-0.0.2/src/vnfaker.egg-info/
--rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/PKG-INFO
--rw-r--r--   0 ducquang   (501) admin       (80)      939 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/SOURCES.txt
--rw-r--r--   0 ducquang   (501) admin       (80)        1 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/dependency_links.txt
--rw-r--r--   0 ducquang   (501) admin       (80)       15 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/requires.txt
--rw-r--r--   0 ducquang   (501) admin       (80)        8 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/top_level.txt
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.559720 vnfaker-0.0.3/
+-rw-r--r--   0 ducquang   (501) admin       (80)     1056 2023-04-15 03:22:43.000000 vnfaker-0.0.3/LICENSE.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-04 08:39:49.559206 vnfaker-0.0.3/PKG-INFO
+-rw-r--r--   0 ducquang   (501) admin       (80)     1177 2023-04-22 08:57:04.000000 vnfaker-0.0.3/README.md
+-rw-r--r--   0 ducquang   (501) admin       (80)       38 2023-05-04 08:39:49.559939 vnfaker-0.0.3/setup.cfg
+-rw-r--r--   0 ducquang   (501) admin       (80)     1033 2023-05-04 08:23:44.000000 vnfaker-0.0.3/setup.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.515515 vnfaker-0.0.3/src/
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.520598 vnfaker-0.0.3/src/vnfaker/
+-rw-r--r--   0 ducquang   (501) admin       (80)       70 2023-04-22 07:54:20.000000 vnfaker-0.0.3/src/vnfaker/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     3102 2023-05-04 08:37:58.000000 vnfaker-0.0.3/src/vnfaker/commonUtils.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.524644 vnfaker-0.0.3/src/vnfaker/data/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.3/src/vnfaker/data/__init__.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.525374 vnfaker-0.0.3/src/vnfaker/data/company/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.3/src/vnfaker/data/company/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)    14530 2023-05-01 04:39:51.000000 vnfaker-0.0.3/src/vnfaker/data/company/company.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.526574 vnfaker-0.0.3/src/vnfaker/data/occupation/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.3/src/vnfaker/data/occupation/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)    34962 2023-04-11 06:57:16.000000 vnfaker-0.0.3/src/vnfaker/data/occupation/occupation.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.532832 vnfaker-0.0.3/src/vnfaker/data/person/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.3/src/vnfaker/data/person/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     1132 2023-05-01 04:04:14.000000 vnfaker-0.0.3/src/vnfaker/data/person/female.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1089 2023-05-01 04:04:55.000000 vnfaker-0.0.3/src/vnfaker/data/person/female_middle.name
+-rw-r--r--   0 ducquang   (501) admin       (80)      439 2023-05-02 10:33:11.000000 vnfaker-0.0.3/src/vnfaker/data/person/last.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1778 2023-05-01 03:46:35.000000 vnfaker-0.0.3/src/vnfaker/data/person/male.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1172 2023-05-01 04:09:43.000000 vnfaker-0.0.3/src/vnfaker/data/person/male_middle.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.543090 vnfaker-0.0.3/src/vnfaker/data/provinces/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.3/src/vnfaker/data/provinces/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)  3512185 2023-04-10 17:48:23.000000 vnfaker-0.0.3/src/vnfaker/data/provinces/flat-divisions.json
+-rw-r--r--   0 ducquang   (501) admin       (80)  2404923 2023-04-10 17:48:23.000000 vnfaker-0.0.3/src/vnfaker/data/provinces/nested-divisions.json
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.553657 vnfaker-0.0.3/src/vnfaker/data/religion/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-05-04 08:18:11.000000 vnfaker-0.0.3/src/vnfaker/data/religion/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)      363 2023-05-04 08:20:57.000000 vnfaker-0.0.3/src/vnfaker/data/religion/religion.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.555331 vnfaker-0.0.3/src/vnfaker/data/sentence/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.3/src/vnfaker/data/sentence/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)   244103 2023-04-12 08:52:12.000000 vnfaker-0.0.3/src/vnfaker/data/sentence/sentence.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)     9682 2023-05-04 08:32:39.000000 vnfaker-0.0.3/src/vnfaker/generator.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.524177 vnfaker-0.0.3/src/vnfaker.egg-info/
+-rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/PKG-INFO
+-rw-r--r--   0 ducquang   (501) admin       (80)      982 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/SOURCES.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)        1 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/dependency_links.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)       32 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/requires.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)        8 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/top_level.txt
```

### Comparing `vnfaker-0.0.2/LICENSE.txt` & `vnfaker-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.2/PKG-INFO` & `vnfaker-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnfaker
-Version: 0.0.2
+Version: 0.0.3
 Summary: vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.
 Home-page: https://github.com/phanducquang/vnfaker
 Author: Phan Duc Quang
 Author-email: phanducquang07@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/phanducquang/vnfaker/issues
 Platform: UNKNOWN
```

### Comparing `vnfaker-0.0.2/README.md` & `vnfaker-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.2/setup.py` & `vnfaker-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     README = fh.read()
 
 setuptools.setup(
     name="vnfaker",
-    version="0.0.2",
+    version="0.0.3",
     author="Phan Duc Quang",
     author_email="phanducquang07@gmail.com",
     description="vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/phanducquang/vnfaker",
     project_urls={
@@ -22,9 +22,10 @@
     ],
     package_dir={"": "src"},
     package_data={"": ["data/*/*.name", "data/*/*.json", "data/*/*.txt"],},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
     install_requires=[
         "orjson>=3.8.10",
+        "unidecode>=1.3.6"
     ],
 )
```

### Comparing `vnfaker-0.0.2/src/vnfaker/commonUtils.py` & `vnfaker-0.0.3/src/vnfaker/commonUtils.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,22 +62,24 @@
     female_filename = "female.name"
     male_mid_filename = "male_middle.name"
     female_mid_filename = "female_middle.name"
     company_filename = "company.name"
     provinces_filename = "flat-divisions.json"
     occupation_filename = "occupation.name"
     sentence_filename = "sentence.txt"
+    religion_filename = "religion.name"
 
     lastNames = _read_file(lastname_filename, "person")
     maleNames = _read_file(male_filename, "person")
     femaleNames = _read_file(female_filename, "person")
     maleMidNames = _read_file(male_mid_filename, "person")
     femaleMidNames = _read_file(female_mid_filename, "person")
     companyNames = _read_file(company_filename, "company")
     occupationNames = _read_file(occupation_filename, "occupation")
+    religionNames = _read_file(religion_filename, "religion")
     sentencesValue = _read_file(sentence_filename, "sentence")
     FLAT_DIVISIONS_JSON_PATH = Path(__file__).parent / 'data' / 'provinces' / 'flat-divisions.json'
 
     address = orjson.loads(FLAT_DIVISIONS_JSON_PATH.read_bytes())
     domainEmail = ['gmail.com', 'outlook.com', 'yandex.com', 'hotmail.com', 'icloud.com', 'yahoo.com']
```

### Comparing `vnfaker-0.0.2/src/vnfaker/data/occupation/occupation.name` & `vnfaker-0.0.3/src/vnfaker/data/occupation/occupation.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.2/src/vnfaker/data/person/female.name` & `vnfaker-0.0.3/src/vnfaker/data/person/female.name`

 * *Files 12% similar despite different names*

```diff
@@ -1,191 +1,190 @@
-Chi
+Ái
+An
+Ân
+Anh
+Ánh
+Bạch Thảo
+Băng
+Bằng
+Bảo
+Bích
 Bình
-Di
-Hạ
-Hằng
-Khê
-Nhiên
-Nhàn
+Ca
+Cầm
+Cát
+Châu
 Chi
-Hương
-Mai
-Phương
-Thi
-Thy
-Thơ
-Thư
-Thảo
-Vũ
-Ðào
-Minh
-Yên
 Chiêu
-Châu
+Chinh
+Chung
+Cúc
+Cương
+Dạ
+Ðài
+Dân
+Đan
+Ðan
+Ðàn
+Đăng
+Dao
+Đào
+Ðào
+Di
+Diễm
+Diệp
+Ðiệp
+Diệu
+Ðình
+Ðoan
+Du
+Dung
+Dương
+Ðường
 Duyên
-Hiền
-Huệ
+Giang
+Giao
 Hà
-Hạnh
+Hạ
 Hải
+Hân
+Hằng
+Hạnh
 Hảo
 Hậu
+Hiền
+Hiệp
+Hiếu
+Hoa
+Hòa
+Hoài
+Hoan
+Hoàn
 Hồng
 Hợp
+Huệ
+Hương
+Hường
+Hưởng
+Huyền
+Kê
+Khai
+Khanh
+Khánh
+Khê
+Khôi
+Khuê
+Khuyên
+Kiều
+Kim
 Lam
+Lâm
+Lan
+Lăng
+Lễ
+Lệ
 Liên
+Liễu
+Linh
 Loan
+Lộc
+Lợi
+Ly
+Lý
+Mai
+Mẫn
+Mi
+Miên
+Minh
+My
+Mỹ
 Nga
 Ngà
 Ngân
+Nghi
 Ngọc
+Ngôn
+Nguyên
+Nguyệt
+Nhã
+Nhàn
+Nhân
+Nhạn
+Nhi
+Nhiên
+Nhơn
 Như
+Nhung
+Nữ
+Nương
+Oanh
+Phi
+Phong
+Phúc
+Phụng
+Phước
+Phương
 Phượng
-Quyên
 Quân
+Quế
+Quyên
+Quỳnh
+Sa
 San
-Thoa
-Thu
-Thủy
-Trang
-Trâm
-Ty
-Vân
-Ðiệp
-Băng
+Sinh
+Sương
 Tâm
-Cúc
-Hoa
-Kim
-Quỳnh
-Trà
-Tuyết
-Yến
-Anh
-Hân
-Lan
-Lễ
-Thúy
-Tiên
-Trân
-Trúc
-Uyên
-Vy
-Linh
-Dương
-Cát
-Ly
-Tường
-Hường
-Nhi
-Nhung
-Tú
-Vỹ
-Khuê
-Kiều
-Lộc
-My
-Phúc
-Phước
-Trinh
-Huyền
-Nương
-Thiện
-Ái
-Mỹ
-Lâm
-Nguyệt
-Khanh
+Thắm
 Thanh
+Thảo
+Thêu
+Thi
 Thiên
-Hưởng
-Giang
-Chung
-Hòa
+Thiện
+Thơ
+Thoa
+Thoại
+Thông
+Thu
+Thư
+Thuần
+Thuận
 Thục
-Lý
-Tranh
-An
 Thương
-Vi
-Miên
-Nguyên
-Oanh
-Sa
-Xuân
-Mi
-Diệu
-Thoại
-Ân
-Nghi
-Ý
-Dung
-Nhơn
-Sinh
+Thường
+Thúy
+Thùy
+Thủy
 Thụy
-Ðường
-Diệp
-Bạch Thảo
-Diễm
-Khôi
-Nhạn
-Quế
-Thắm
-Đăng
+Thy
+Tiên
+Trà
+Trâm
+Trầm
+Trân
+Trang
+Tranh
+Trinh
+Trúc
 Trung
-Giao
-Ca
-Cương
-Khuyên
-Khánh
-Thông
+Tú
+Tuệ
+Tường
 Tuyến
 Tuyền
-Xuyến
-Ánh
-Đan
-Ðan
+Tuyết
+Ty
+Uyên
 Uyển
-Khai
-Tuệ
-Liễu
-Hiệp
-Hoàn
-Lệ
-Lợi
-Nhân
-Phụng
-Thuần
-Thuận
-Cầm
-Bích
-Hoan
-Nữ
-Sương
-Ðàn
-Bảo
-Dạ
-Phi
-Thùy
-Dao
-Kê
-Dân
-Hiếu
-Mẫn
-Nhã
-Ngôn
-Thêu
-Hoài
-Phong
+Vân
+Vi
 Việt
 Vọng
-Ðoan
-Ðình
-Du
-Ðài
-Đào
-Trầm
-Chinh
-Thường
+Vũ
+Vy
+Vỹ
 xanh
-Bằng
-Lăng
+Xuân
+Xuyến
+Ý
+Yên
+Yến
```

### Comparing `vnfaker-0.0.2/src/vnfaker/data/person/female_middle.name` & `vnfaker-0.0.3/src/vnfaker/data/person/female_middle.name`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-Phương
+Ái
 An
 Anh
+Ánh
+Ấu
+Bạch
 Ban
-Bình
-Bích
 Băng
-Bạch
 Bảo
+Bích
+Bình
 Bội
 Cam
+Cẩm
+Cát
 Chi
 Chiêu
-Cát
-Cẩm
+Dã
+Dạ
+Đài
+Ðài
+Đan
+Ðan
 Di
-Diên
 Diễm
+Diên
 Diệp
 Diệu
+Đinh
+Ðinh
+Đoan
+Ðoan
+Đơn
+Đông
+Ðông
+Ðồng
+Đức
 Duy
 Duyên
-Dã
-Dạ
 Gia
 Giang
-Giao
 Giáng
-Hiếu
+Giao
+Hà
+Hạ
+Hạc
+Hải
+Hàm
+Hằng
+Hạnh
+Hảo
 Hiền
+Hiếu
 Hiểu
+Hồ
 Hoa
+Hoạ
+Họa
 Hoài
 Hoàn
 Hoàng
-Hoạ
-Huyền
+Hồng
 Huệ
-Huỳnh
-Hà
-Hàm
 Hương
 Hướng
-Hạ
-Hạc
-Hạnh
-Hải
-Hảo
-Hằng
-Họa
-Hồ
-Hồng
-Khiết
-Khuê
-Khánh
-Khúc
+Huyền
+Huỳnh
 Khả
 Khải
-Kim
+Khánh
+Khiết
+Khúc
+Khuê
 Kiết
 Kiều
+Kim
 Kỳ
 Lam
+Lâm
 Lan
-Linh
+Lê
+Lệ
 Liên
 Liễu
+Linh
 Loan
-Ly
-Lâm
-Lê
-Lưu
-Lệ
 Lộc
 Lục
+Lưu
+Ly
 Mai
-Minh
 Mậu
+Minh
 Mộc
 Mộng
 Mỹ
+Ngân
 Nghi
+Ngọc
 Nguyên
 Nguyết
 Nguyệt
-Ngân
-Ngọc
-Nhan
 Nhã
-Như
+Nhan
 Nhất
 Nhật
+Như
 Oanh
 Phi
 Phong
+Phụng
 Phước
+Phương
 Phượng
-Phụng
 Quế
 Quỳnh
 Sao
+Sơn
 Song
 Sông
-Sơn
 Sương
+Tâm
+Thạch
+Thái
 Thanh
+Thảo
 Thi
 Thiên
+Thiện
 Thiếu
 Thiều
-Thiện
-Thu
-Thuần
-Thy
-Thái
-Thùy
-Thúy
 Thơ
+Thu
 Thư
+Thuần
+Thục
 Thương
 Thường
-Thạch
-Thảo
-Thục
-Thụy
+Thúy
+Thùy
 Thủy
-Tinh
+Thụy
+Thy
 Tiên
 Tiểu
-Trang
-Triều
-Triệu
-Trung
+Tinh
+Tịnh
+Tố
 Trà
 Trâm
+Trầm
 Trân
+Trang
+Triều
+Triệu
 Trúc
-Trầm
-Tuyết
-Tuyền
+Trung
+Tú
+Từ
 Tuệ
-Tâm
 Tùng
-Tùy
-Tú
-Túy
 Tường
-Tịnh
-Tố
-Từ
+Túy
+Tùy
+Tuyền
+Tuyết
 Uyên
 Uyển
-Vi
-Vinh
-Việt
-Vy
+Vân
 Vàng
 Vành
-Vân
+Vi
+Việt
+Vinh
 Vũ
-Xuyến
+Vy
 Xuân
-Yên
-Yến
-Ái
-Ánh
-Ðan
-Ðinh
-Ðoan
-Ðài
-Ðông
-Ðồng
+Xuyến
 Ý
-Đan
-Đinh
-Đoan
-Đài
-Đông
-Đơn
-Đức
-Ấu
+Yên
+Yến
```

### Comparing `vnfaker-0.0.2/src/vnfaker/data/person/male.name` & `vnfaker-0.0.3/src/vnfaker/data/person/male.name`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 An
 Án
 Ân
 Ẩn
 Anh
+Ánh
 Bắc
 Bạch
 Bằng
 Bào
 Bảo
 Bảo Long
 Bình
@@ -52,15 +53,14 @@
 Ðoàn
 Doanh
 Ðôn
 Ðông
 Ðồng
 Du
 Đức
-Ðức
 Duệ
 Dũng
 Dụng
 Dương
 Duy
 Duyệt
 Gia
@@ -87,25 +87,25 @@
 Hoài
 Hoán
 Hoàn
 Hoàng
 Hoạt
 Học
 Hội
-Hồng
 Hợp
 Huấn
 Hùng
 Hưng
 Hữu
 Huy
 Huynh
 Huỳnh
 Hỷ
 Kha
+Khá
 Khải
 Khang
 Khanh
 Khánh
 Khiêm
 Khiếu
 Khoa
```

### Comparing `vnfaker-0.0.2/src/vnfaker/data/person/male_middle.name` & `vnfaker-0.0.3/src/vnfaker/data/person/male_middle.name`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 An
 Ân
 Anh
 Bá
 Bách
 Bằng
 Bảo
-Bích
 Bình
-Bửu
 Bữu
+Bửu
 Cảnh
 Cao
 Cát
 Chấn
 Chánh
 Chế
 Chí
 Chiến
 Chiêu
 Chính
 Chuẩn
 Chung
 Công
-Cường
 Cương
+Cường
 Ðắc
 Ðại
 Dân
 Ðan
-Ðăng
 Đăng
+Ðăng
 Danh
 Ðạt
-Ðình
 Ðinh
+Ðình
 Ðịnh
 Ðoàn
-Ðồng
 Ðông
-Ðức
+Ðồng
 Đức
+Ðức
 Dũng
 Dương
 Duy
 Gia
 Giang
 Hà
 Hải
@@ -64,58 +63,58 @@
 Huân
 Hùng
 Hưng
 Hướng
 Hữu
 Huy
 Khắc
-Khải
 Khai
+Khải
 Khang
 Khánh
 Khoa
 Khôi
 Khởi
 Khương
 Khuyến
 Kiên
 Kiến
 Kiệt
 Kim
 Kỳ
 Lạc
-Lâm
 Lam
+Lâm
 Lập
 Liên
 Long
 Lương
 Mạnh
 Minh
 Mộng
 Nam
 Nghị
 Nghĩa
 Ngọc
 Nguyên
 Nguyễn
 Nhân
-Nhật
 Nhất
+Nhật
 Như
 Niệm
 Phi
 Phong
 Phú
 Phúc
 Phục
 Phụng
 Phước
-Phượng
 Phương
+Phượng
 Quân
 Quang
 Quảng
 Quốc
 Quý
 Quyết
 Sĩ
@@ -126,59 +125,59 @@
 Tài
 Tâm
 Tân
 Tấn
 Tất
 Thạch
 Thái
-Thắng
 Thăng
-Thành
+Thắng
 Thanh
+Thành
 Thất
 Thế
 Thiên
 Thiện
 Thiếu
 Thiệu
 Thịnh
 Thời
 Thông
 Thống
-Thụ
 Thu
+Thụ
 Thuận
-Thượng
 Thường
+Thượng
 Thụy
 Tích
 Tiến
 Tiền
 Tiểu
 Toàn
 Tôn
 Trí
 Triển
-Triệu
 Triều
+Triệu
 Trọng
 Trúc
 Trung
 Trường
 Từ
 Tuấn
 Tùng
 Tường
 Tuyền
 Uy
-Vạn
 Văn
 Vân
+Vạn
 Viễn
-Việt
 Viết
-Vĩnh
+Việt
 Vinh
+Vĩnh
 Vũ
 Vương
 Xuân
 Yên
```

### Comparing `vnfaker-0.0.2/src/vnfaker/data/provinces/flat-divisions.json` & `vnfaker-0.0.3/src/vnfaker/data/provinces/flat-divisions.json`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.2/src/vnfaker/data/provinces/nested-divisions.json` & `vnfaker-0.0.3/src/vnfaker/data/provinces/nested-divisions.json`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.2/src/vnfaker/data/sentence/sentence.txt` & `vnfaker-0.0.3/src/vnfaker/data/sentence/sentence.txt`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.2/src/vnfaker/generator.py` & `vnfaker-0.0.3/src/vnfaker/generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,116 +8,122 @@
 
 from .commonUtils import CommonUtils, str_clean, change_year, date_time_ad
 
 
 class Generator:
 
     def __init__(self):
-        self.username_value = None
-        self.email_value = None
-        self.district_name = None
-        self.ward_name = None
-        self.province_name = None
-        self.known_location_value = None
-        self.name_value = None
-        self.last_name_value = None
-        self.mid_name_value = None
-        self.nickname_value = None
-        self.sentences_value = None
-        self.id_number_value = None
-        self.occupation_value = None
-        self.company_value = None
-        self.birth_date = None
-        self.gender_value = None
-        self.address_value = None
-        self.phone = None
-        self.full_name = None
+        self.__religion_value = None
+        self.__username_value = None
+        self.__email_value = None
+        self.__district_name = None
+        self.__ward_name = None
+        self.__province_name = None
+        self.__known_location_value = None
+        self.__name_value = None
+        self.__last_name_value = None
+        self.__mid_name_value = None
+        self.__nickname_value = None
+        self.__sentences_value = None
+        self.__id_number_value = None
+        self.__occupation_value = None
+        self.__company_value = None
+        self.__birth_date = None
+        self.__gender_value = None
+        self.__address_value = None
+        self.__phone = None
+        self.__full_name = None
 
     def gender(self):
-        if self.gender_value is None:
-            self.gender_value = random.choice([1, 2])
-        return self.gender_value
+        if self.__gender_value is None:
+            self.__gender_value = random.choice([1, 2])
+        return self.__gender_value
 
     def fullname(self):
-        if self.full_name is None:
-            if self.gender_value is None:
+        if self.__full_name is None:
+            if self.__gender_value is None:
                 self.gender()
-            self.last_name_value = random.choice(CommonUtils.lastNames)
-            if self.gender_value:  # man
-                self.mid_name_value = random.choice(CommonUtils.maleMidNames)
-                self.name_value = random.choice(CommonUtils.maleNames)
-                self.full_name = "{} {} {}".format(self.last_name_value, self.mid_name_value, self.name_value)
+            self.__last_name_value = random.choice(CommonUtils.lastNames)
+            if self.__gender_value:  # man
+                self.__mid_name_value = random.choice(CommonUtils.maleMidNames)
+                self.__name_value = random.choice(CommonUtils.maleNames)
+                self.__full_name = "{} {} {}".format(self.__last_name_value, self.__mid_name_value, self.__name_value)
             else:
-                self.mid_name_value = random.choice(CommonUtils.femaleMidNames)
-                self.name_value = random.choice(CommonUtils.femaleNames)
-                self.full_name = "{} {} {}".format(self.last_name_value, self.mid_name_value, self.name_value)
-        return self.full_name
+                self.__mid_name_value = random.choice(CommonUtils.femaleMidNames)
+                self.__name_value = random.choice(CommonUtils.femaleNames)
+                self.__full_name = "{} {} {}".format(self.__last_name_value, self.__mid_name_value, self.__name_value)
+        return self.__full_name
 
     def middle_name(self):
-        if self.full_name is None:
+        if self.__full_name is None:
             self.fullname()
-        return self.mid_name_value
+        return self.__mid_name_value
 
     def last_name(self):
-        if self.full_name is None:
+        if self.__full_name is None:
             self.fullname()
-        return self.last_name_value
+        return self.__last_name_value
 
     def name(self):
-        if self.full_name is None:
+        if self.__full_name is None:
             self.fullname()
-        return self.name_value
+        return self.__name_value
 
     def nickname(self, number_of_nick: int = 3):
-        if self.nickname_value is None:
+        if self.__nickname_value is None:
             if number_of_nick > 10:
                 number_of_nick = 10
-            if self.full_name is None:
+            if self.__full_name is None:
                 self.fullname()
-            nickname = ["{} {}".format(self.mid_name_value, self.name_value),
-                        "{} {}".format(self.name_value, self.last_name_value),
-                        "{} {}".format(self.last_name_value, self.name_value),
-                        unidecode(str_clean(self.name_value)).lower(),
-                        unidecode(str_clean(self.mid_name_value + self.name_value)).lower(),
-                        unidecode(str_clean(self.mid_name_value + self.name_value + random.randint(1, 999).__str__())).lower(),
-                        unidecode(str_clean(self.name_value + self.last_name_value)).lower(),
-                        unidecode(str_clean(self.name_value + self.last_name_value + random.randint(1, 999).__str__())).lower(),
-                        unidecode(str_clean(self.last_name_value + self.name_value)).lower(),
-                        unidecode(str_clean(self.last_name_value + self.name_value + random.randint(1, 999).__str__())).lower(),
-                        unidecode(str_clean(self.name_value + self.name_value + random.randint(1, 999).__str__())).lower()]
+            nickname = ["{} {}".format(self.__mid_name_value, self.__name_value),
+                        "{} {}".format(self.__name_value, self.__last_name_value),
+                        "{} {}".format(self.__last_name_value, self.__name_value),
+                        unidecode(str_clean(self.__name_value)).lower(),
+                        unidecode(str_clean(self.__mid_name_value + self.__name_value)).lower(),
+                        unidecode(str_clean(
+                            self.__mid_name_value + self.__name_value + random.randint(1, 999).__str__())).lower(),
+                        unidecode(str_clean(self.__name_value + self.__last_name_value)).lower(),
+                        unidecode(str_clean(
+                            self.__name_value + self.__last_name_value + random.randint(1, 999).__str__())).lower(),
+                        unidecode(str_clean(self.__last_name_value + self.__name_value)).lower(),
+                        unidecode(str_clean(
+                            self.__last_name_value + self.__name_value + random.randint(1, 999).__str__())).lower(),
+                        unidecode(str_clean(
+                            self.__name_value + self.__name_value + random.randint(1, 999).__str__())).lower()]
             nickname_value_set = [random.choice(nickname) for _ in range(random.randint(1, number_of_nick))]
-            self.nickname_value = list(set(nickname_value_set))
-        return self.nickname_value
+            self.__nickname_value = list(set(nickname_value_set))
+        return self.__nickname_value
 
     def email(self):
-        if self.email_value is None:
-            if self.full_name is None:
+        if self.__email_value is None:
+            if self.__full_name is None:
                 self.fullname()
-            self.email_value = "{}@{}".format(unidecode(str_clean(self.full_name)).lower(), random.choice(CommonUtils.domainEmail))
-        return self.email_value
+            self.__email_value = "{}@{}".format(unidecode(str_clean(self.__full_name)).lower(),
+                                                random.choice(CommonUtils.domainEmail))
+        return self.__email_value
 
     def username(self):
-        if self.username_value is None:
-            if self.nickname_value is None:
+        if self.__username_value is None:
+            if self.__nickname_value is None:
                 self.nickname()
-            self.username_value = random.choice(self.nickname_value)
-        return self.username_value
+            self.__username_value = random.choice(self.__nickname_value)
+        return self.__username_value
 
     def mobile_phone(self):
-        if self.phone is None:
+        if self.__phone is None:
             list_phone_start = [
                 '086', '096', '097', '098', '032', '033', '034', '035', '036', '037', '038', '039', '090', '093', '091',
                 '094',
                 '083', '084', '085',
             ]
             start = random.choice(list_phone_start)
             # random 7 number from 0000000 to 9999999
             end = random.randint(0000000, 9999999)
-            self.phone = start + str(end)
-        return self.phone
+            self.__phone = start + str(end)
+        return self.__phone
 
     def date_of_birth(
             self,
             tz_info: Optional[tzinfo] = None,
             minimum_age: int = 0,
             maximum_age: int = 115,
             timestamp: bool = True,
@@ -131,15 +137,15 @@
         :param minimum_age: Defaults to 0.
         :param maximum_age: Defaults to 115.
         :param timestamp: Defaults to True.
 
         :example: 852051600000 Or Date('1997-01-01')
         :return: Timestamp(Default) Or Date
         """
-        if self.birth_date is None:
+        if self.__birth_date is None:
             if not isinstance(minimum_age, int):
                 raise TypeError("minimum_age must be an integer.")
 
             if not isinstance(maximum_age, int):
                 raise TypeError("maximum_age must be an integer.")
 
             if maximum_age < 0:
@@ -157,65 +163,70 @@
 
             now = datetime.now(tz_info).date()
             start_date = change_year(now, -(maximum_age + 1))
             end_date = change_year(now, -minimum_age)
 
             dob_temp = date_time_ad(tzinfo=tz_info, start_datetime=start_date, end_datetime=end_date).date()
 
-            self.birth_date = dob_temp if dob_temp != start_date else dob_temp + timedelta(days=1)
+            self.__birth_date = dob_temp if dob_temp != start_date else dob_temp + timedelta(days=1)
         if timestamp:
-            return datetime.fromisoformat(self.birth_date.isoformat()).timestamp() * 1000
-        return self.birth_date
+            return datetime.fromisoformat(self.__birth_date.isoformat()).timestamp() * 1000
+        return self.__birth_date
 
     def address(self):
-        if self.address_value is None:
+        if self.__address_value is None:
             address_value_obj = random.choice(CommonUtils.address)
-            self.province_name = address_value_obj.get("province_name")
-            self.ward_name = address_value_obj.get("ward_name")
-            self.district_name = address_value_obj.get("district_name")
-            self.address_value = "{}, {}, {}".format(self.ward_name,
-                                                     self.district_name,
-                                                     self.province_name)
-        return self.address_value
+            self.__province_name = address_value_obj.get("__province_name")
+            self.__ward_name = address_value_obj.get("__ward_name")
+            self.__district_name = address_value_obj.get("__district_name")
+            self.__address_value = "{}, {}, {}".format(self.__ward_name,
+                                                       self.__district_name,
+                                                       self.__province_name)
+        return self.__address_value
 
     def address_province(self):
-        if self.address_value is None:
+        if self.__address_value is None:
             self.address()
-        return self.province_name
+        return self.__province_name
 
     def address_district(self):
-        if self.address_value is None:
+        if self.__address_value is None:
             self.address()
-        return self.district_name
+        return self.__district_name
 
     def address_ward(self):
-        if self.address_value is None:
+        if self.__address_value is None:
             self.address()
-        return self.ward_name
+        return self.__ward_name
 
     def company(self):
-        if self.company_value is None:
-            self.company_value = random.choice(CommonUtils.companyNames)
-        return self.company_value
+        if self.__company_value is None:
+            self.__company_value = random.choice(CommonUtils.companyNames)
+        return self.__company_value
 
     def known_location(self):
-        if self.known_location_value is None:
-            self.known_location_value = [random.choice(CommonUtils.address).get("province_name") for _ in
-                                         range(random.randint(1, 5))]
-        return self.known_location_value
+        if self.__known_location_value is None:
+            self.__known_location_value = [random.choice(CommonUtils.address).get("__province_name") for _ in
+                                           range(random.randint(1, 5))]
+        return self.__known_location_value
 
     def occupation(self):
-        if self.occupation_value is None:
-            self.occupation_value = random.choice(CommonUtils.occupationNames)
-        return self.occupation_value
+        if self.__occupation_value is None:
+            self.__occupation_value = random.choice(CommonUtils.occupationNames)
+        return self.__occupation_value
 
     def id_number(self, number_of_id):
-        if self.id_number_value is None:
+        if self.__id_number_value is None:
             number = '0123456789'
-            self.id_number_value = "".join([random.choice(number) for _ in range(number_of_id)])
-        return self.id_number_value
+            self.__id_number_value = "".join([random.choice(number) for _ in range(number_of_id)])
+        return self.__id_number_value
 
     def sentences(self):
-        if self.sentences_value is None:
+        if self.__sentences_value is None:
             sentences_value_temp = [random.choice(CommonUtils.sentencesValue) for _ in range(random.randint(1, 3))]
-            self.sentences_value = ". ".join(sentences_value_temp) + "."
-        return self.sentences_value
+            self.__sentences_value = ". ".join(sentences_value_temp) + "."
+        return self.__sentences_value
+
+    def religion(self):
+        if self.__religion_value is None:
+            self.__religion_value = random.choice(CommonUtils.religionNames)
+        return self.__religion_value
```

### Comparing `vnfaker-0.0.2/src/vnfaker.egg-info/PKG-INFO` & `vnfaker-0.0.3/src/vnfaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnfaker
-Version: 0.0.2
+Version: 0.0.3
 Summary: vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.
 Home-page: https://github.com/phanducquang/vnfaker
 Author: Phan Duc Quang
 Author-email: phanducquang07@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/phanducquang/vnfaker/issues
 Platform: UNKNOWN
```

### Comparing `vnfaker-0.0.2/src/vnfaker.egg-info/SOURCES.txt` & `vnfaker-0.0.3/src/vnfaker.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 src/vnfaker/data/company/__init__.py
 src/vnfaker/data/company/company.name
 src/vnfaker/data/occupation/__init__.py
 src/vnfaker/data/occupation/occupation.name
 src/vnfaker/data/person/__init__.py
 src/vnfaker/data/person/female.name
 src/vnfaker/data/person/female_middle.name
-src/vnfaker/data/person/first.name
 src/vnfaker/data/person/last.name
 src/vnfaker/data/person/male.name
 src/vnfaker/data/person/male_middle.name
 src/vnfaker/data/provinces/__init__.py
 src/vnfaker/data/provinces/flat-divisions.json
 src/vnfaker/data/provinces/nested-divisions.json
+src/vnfaker/data/religion/__init__.py
+src/vnfaker/data/religion/religion.name
 src/vnfaker/data/sentence/__init__.py
 src/vnfaker/data/sentence/sentence.txt
```

