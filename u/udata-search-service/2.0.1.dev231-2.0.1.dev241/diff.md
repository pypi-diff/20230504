# Comparing `tmp/udata-search-service-2.0.1.dev231.tar.gz` & `tmp/udata-search-service-2.0.1.dev241.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udata-search-service-2.0.1.dev231.tar", last modified: Mon Jan  9 13:43:31 2023, max compression
+gzip compressed data, was "udata-search-service-2.0.1.dev241.tar", last modified: Thu May  4 12:12:59 2023, max compression
```

## Comparing `udata-search-service-2.0.1.dev231.tar` & `udata-search-service-2.0.1.dev241.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2409 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/.circleci/config.yml
--rw-r--r--   0        0        0      763 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/.gitignore
--rw-r--r--   0        0        0     1413 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/CHANGELOG.md
--rw-r--r--   0        0        0      173 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/Dockerfiles/Dockerfile.app
--rw-r--r--   0        0        0      494 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/Makefile
--rw-r--r--   0        0        0     3776 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/README.md
--rw-r--r--   0        0        0      394 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/bumpr.rc
--rw-r--r--   0        0        0      329 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/docker-compose.test.yml
--rw-r--r--   0        0        0      560 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/docker-compose.yml
--rw-r--r--   0        0        0    18532 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/docs/udata-search-service-schema.png
--rw-r--r--   0        0        0      831 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/tests/__init__.py
--rw-r--r--   0        0        0      769 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/tests/conftest.py
--rw-r--r--   0        0        0    27744 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/tests/test_api.py
--rw-r--r--   0        0        0     6046 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/tests/test_consumers.py
--rw-r--r--   0        0        0    12407 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/tests/test_search_client.py
--rw-r--r--   0        0        0      202 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/__init__.py
--rw-r--r--   0        0        0      807 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/app.py
--rw-r--r--   0        0        0      703 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/config.py
--rw-r--r--   0        0        0      767 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/container.py
--rw-r--r--   0        0        0        0 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/domain/__init__.py
--rw-r--r--   0        0        0     2524 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/domain/entities.py
--rw-r--r--   0        0        0     2439 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/domain/factories.py
--rw-r--r--   0        0        0     1343 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/domain/interfaces.py
--rw-r--r--   0        0        0        0 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/__init__.py
--rw-r--r--   0        0        0     2641 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/consumers.py
--rw-r--r--   0        0        0     2063 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/migrate.py
--rw-r--r--   0        0        0    15928 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/search_clients.py
--rw-r--r--   0        0        0     5699 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/services.py
--rw-r--r--   0        0        0     1402 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/utils.py
--rw-r--r--   0        0        0        0 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/presentation/__init__.py
--rw-r--r--   0        0        0    14216 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/presentation/api.py
--rw-r--r--   0        0        0      952 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/presentation/commands.py
--rw-r--r--   0        0        0       76 2023-01-09 13:40:30.000000 udata-search-service-2.0.1.dev231/udata_search_service/wsgi.py
--rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 udata-search-service-2.0.1.dev231/PKG-INFO
+-rw-r--r--   0        0        0     2409 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/.circleci/config.yml
+-rw-r--r--   0        0        0      763 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/.gitignore
+-rw-r--r--   0        0        0     1579 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/CHANGELOG.md
+-rw-r--r--   0        0        0      173 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/Dockerfiles/Dockerfile.app
+-rw-r--r--   0        0        0      494 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/Makefile
+-rw-r--r--   0        0        0     3776 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/README.md
+-rw-r--r--   0        0        0      394 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/bumpr.rc
+-rw-r--r--   0        0        0      329 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/docker-compose.test.yml
+-rw-r--r--   0        0        0      560 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/docker-compose.yml
+-rw-r--r--   0        0        0    18532 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/docs/udata-search-service-schema.png
+-rw-r--r--   0        0        0      831 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/__init__.py
+-rw-r--r--   0        0        0      769 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/conftest.py
+-rw-r--r--   0        0        0    27860 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/test_api.py
+-rw-r--r--   0        0        0     6164 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/test_consumers.py
+-rw-r--r--   0        0        0    13254 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/test_search_client.py
+-rw-r--r--   0        0        0      202 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/app.py
+-rw-r--r--   0        0        0      703 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/config.py
+-rw-r--r--   0        0        0      767 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/container.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/domain/__init__.py
+-rw-r--r--   0        0        0     2666 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/domain/entities.py
+-rw-r--r--   0        0        0     2501 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/domain/factories.py
+-rw-r--r--   0        0        0     1343 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/domain/interfaces.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2641 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/consumers.py
+-rw-r--r--   0        0        0     2063 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/migrate.py
+-rw-r--r--   0        0        0    15953 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/search_clients.py
+-rw-r--r--   0        0        0     5699 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/services.py
+-rw-r--r--   0        0        0     1402 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/utils.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/presentation/__init__.py
+-rw-r--r--   0        0        0    14252 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/presentation/api.py
+-rw-r--r--   0        0        0      952 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/presentation/commands.py
+-rw-r--r--   0        0        0       76 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/wsgi.py
+-rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 udata-search-service-2.0.1.dev241/PKG-INFO
```

### Comparing `udata-search-service-2.0.1.dev231/.circleci/config.yml` & `udata-search-service-2.0.1.dev241/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/.gitignore` & `udata-search-service-2.0.1.dev241/.gitignore`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/CHANGELOG.md` & `udata-search-service-2.0.1.dev241/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Changelog
 
 ## Current (in progress)
 
-- Nothing yet
+- Add `last_update` field to dataset entity. All datasets need to be reindexed to take last_update into account [#40](https://github.com/opendatateam/udata-search-service/pull/40)
 
 ## 2.0.0 (2023-01-09)
 
 - Use redpanda instead of Kafka [#34](https://github.com/opendatateam/udata-search-service/pull/34)
 - Remove Kafka integration and use HTTP calls instead [#35](https://github.com/opendatateam/udata-search-service/pull/35)
 
 ## 1.0.3 (2022-07-11)
```

### Comparing `udata-search-service-2.0.1.dev231/README.md` & `udata-search-service-2.0.1.dev241/README.md`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/docker-compose.yml` & `udata-search-service-2.0.1.dev241/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/docs/udata-search-service-schema.png` & `udata-search-service-2.0.1.dev241/docs/udata-search-service-schema.png`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/pyproject.toml` & `udata-search-service-2.0.1.dev241/pyproject.toml`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/tests/conftest.py` & `udata-search-service-2.0.1.dev241/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/tests/test_api.py` & `udata-search-service-2.0.1.dev241/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     dataset = {
         'id': faker.md5(),
         'title': faker.sentence(),
         'description': faker.text(),
         'acronym': faker.company_suffix(),
         'url': faker.url(),
         'created_at': faker.past_datetime().isoformat(),
+        'last_update': faker.past_datetime().isoformat(),
         'views': faker.random_int(),
         'followers': faker.random_int(),
         'reuses': faker.random_int(),
         'featured': faker.random_int(min=0, max=1),
         'resources_count': faker.random_int(min=1, max=15),
         'organization': {
             'id': faker.md5(),
@@ -93,14 +94,15 @@
     dataset = {
         'id': faker.md5(),
         'title': faker.sentence(),
         'description': faker.text(),
         'acronym': faker.company_suffix(),
         'url': faker.url(),
         'created_at': faker.past_datetime().isoformat(),
+        'last_update': faker.past_datetime().isoformat(),
         'views': faker.random_int(),
         'followers': faker.random_int(),
         'reuses': faker.random_int(),
         'featured': faker.random_int(min=0, max=1),
         'resources_count': faker.random_int(min=1, max=15),
         'organization': {
             'id': faker.md5(),
```

### Comparing `udata-search-service-2.0.1.dev231/tests/test_consumers.py` & `udata-search-service-2.0.1.dev241/tests/test_consumers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         'acronym': 'DVF',
         'url': '/fr/datasets/demandes-de-valeurs-foncieres/',
         'tags': ['foncier', 'foncier-sol-mutation-fonciere', 'fonciere', 'valeur-fonciere'],
         'license': 'notspecified',
         'badges': [],
         'frequency': 'semiannual',
         'created_at': '2019-01-25T11:30:50',
+        'last_update': '2020-02-27T12:32:50',
         'views': 7806,
         'followers': 72,
         'reuses': 45,
         'featured': 0,
         'resources_count': 10,
         'organization': {
             'id': '534fff8ea3a7292c64a77f02',
@@ -54,14 +55,15 @@
     # Make sure that these fields are log2p-normalized
     for key in ['views', 'followers', 'reuses']:
         assert document[key] == log2p(obj[key])
 
     # Make sure that all other particular fields are treated accordingly
     assert document['concat_title_org'] == get_concat_title_org(document['title'], document['acronym'], document['organization_name'])
     assert document['created_at'].date() == datetime.date(2019, 1, 25)
+    assert document['last_update'].date() == datetime.date(2020, 2, 27)
     assert document['temporal_coverage_start'].date() == datetime.date(2016, 7, 1)
     assert document['temporal_coverage_end'].date() == datetime.date(2021, 6, 30)
     assert document['granularity'] == 'fr:commune'
     assert document['geozones'] == ['fr:arrondissement:353', 'country-group:world', 'country:fr', 'country-group:ue']
     assert document['organization'] == obj['organization']['id']
     assert document['organization_name'] == obj['organization']['name']
     assert document['orga_followers'] == log2p(401)
```

### Comparing `udata-search-service-2.0.1.dev231/tests/test_search_client.py` & `udata-search-service-2.0.1.dev241/tests/test_search_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,14 +305,36 @@
     assert res[0]['title'] == 'data-test-2'
     results_number, res = search_client.query_organizations(None, 0, 20, {}, sort='-followers')
     assert res[0]['name'] == 'org-test-2'
     results_number, res = search_client.query_reuses(None, 0, 20, {}, sort='-followers')
     assert res[0]['title'] == 'reuse-test-2'
 
 
+def test_general_search_with_sorting_last_update(app, client, search_client, faker):
+    search_client.index_dataset(DatasetFactory(
+        title='data-test-1',
+        last_update=datetime.date(2021, 12, 2)
+    ))
+    search_client.index_dataset(DatasetFactory(
+        title='data-test-2',
+        last_update=datetime.date(2022, 12, 2)
+    ))
+    search_client.index_dataset(DatasetFactory(
+        title='data-test-3',
+        last_update=datetime.date(2023, 12, 2)
+    ))
+    # Without this, ElasticSearch does not seem to have the time to index.
+    time.sleep(2)
+
+    results_number, res = search_client.query_datasets(None, 0, 20, {}, sort='-last_update')
+    assert res[0]['title'] == 'data-test-3'
+    results_number, res = search_client.query_datasets(None, 0, 20, {}, sort='last_update')
+    assert res[0]['title'] == 'data-test-1'
+
+
 def test_search_dataset_with_synonym(app, client, search_client, faker):
     search_client.index_dataset(DatasetFactory(
         title='rp',
     ))
 
     # Without this, ElasticSearch does not seem to have the time to index.
     time.sleep(2)
```

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/app.py` & `udata-search-service-2.0.1.dev241/udata_search_service/app.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/config.py` & `udata-search-service-2.0.1.dev241/udata_search_service/config.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/container.py` & `udata-search-service-2.0.1.dev241/udata_search_service/container.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/domain/entities.py` & `udata-search-service-2.0.1.dev241/udata_search_service/domain/entities.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     followers: int
     reuses: int
     featured: int
     resources_count: int
     concat_title_org: str
     description: str
 
+    last_update: datetime.date = None
     acronym: str = None
     badges: List[str] = None
     tags: List[str] = None
     license: str = None
     temporal_coverage_start: datetime.date = None
     temporal_coverage_end: datetime.date = None
     granularity: str = None
@@ -69,14 +70,16 @@
     organization: str = None
     organization_name: str = None
     owner: str = None
 
     def __post_init__(self):
         if isinstance(self.created_at, str):
             self.created_at = isoparse(self.created_at)
+        if isinstance(self.last_update, str):
+            self.last_update = isoparse(self.last_update)
         if isinstance(self.temporal_coverage_start, str):
             self.temporal_coverage_start = isoparse(self.temporal_coverage_start)
         if isinstance(self.temporal_coverage_end, str):
             self.temporal_coverage_end = isoparse(self.temporal_coverage_end)
 
 
 @dataclasses.dataclass
```

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/domain/factories.py` & `udata-search-service-2.0.1.dev241/udata_search_service/domain/factories.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     id = factory.Faker('md5')
     title = factory.Faker('sentence')
     description = factory.Faker('text')
     acronym = factory.Faker('company_suffix')
     url = factory.Faker('url')
     created_at = factory.LazyFunction(datetime.datetime.now)
+    last_update = factory.LazyFunction(datetime.datetime.now)
     orga_sp = 4
     orga_followers = factory.Faker('random_int')
     views = factory.Faker('random_int')
     followers = factory.Faker('random_int')
     reuses = factory.Faker('random_int')
     featured = factory.Faker('random_int')
     resources_count = factory.Faker('random_int', min=1, max=15)
```

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/domain/interfaces.py` & `udata-search-service-2.0.1.dev241/udata_search_service/domain/interfaces.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/consumers.py` & `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/consumers.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/migrate.py` & `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/migrate.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/search_clients.py` & `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/search_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 
 
 class SearchableDataset(IndexDocument):
     title = Text(analyzer=dgv_analyzer)
     acronym = Text()
     url = Text()
     created_at = Date()
+    last_update = Date()
     tags = Keyword(multi=True)
     license = Keyword()
     badges = Keyword(multi=True)
     frequency = Text()
     format = Keyword(multi=True)
     orga_sp = Integer()
     orga_followers = Float()
```

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/services.py` & `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/services.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/infrastructure/utils.py` & `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/presentation/api.py` & `udata-search-service-2.0.1.dev241/udata_search_service/presentation/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         if not pattern.match(value):
             raise ValueError('Temporal coverage does not match the right pattern.')
         return value
 
     @validator('sort')
     def sort_validate(cls, value):
         sorts = [
-            'created', 'reuses', 'followers', 'views'
+            'created', 'last_update', 'reuses', 'followers', 'views'
         ]
         choices = sorts + ['-' + k for k in sorts]
         if value not in choices:
             raise ValueError('Temporal coverage does not match the right pattern.')
         return value
 
 
@@ -111,14 +111,15 @@
     acronym: Optional[str] = None
     url: Optional[str] = None
     tags: Optional[list] = []
     license: Optional[str] = None
     badges: Optional[list] = []
     frequency: Optional[str] = None
     created_at: str
+    last_update: str
     organization: Optional[dict] = None
     owner: Optional[str] = None
     views: int
     followers: int
     reuses: int
     resources_count: Optional[int] = 0
     featured: Optional[int] = 0
```

### Comparing `udata-search-service-2.0.1.dev231/udata_search_service/presentation/commands.py` & `udata-search-service-2.0.1.dev241/udata_search_service/presentation/commands.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev231/PKG-INFO` & `udata-search-service-2.0.1.dev241/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udata-search-service
-Version: 2.0.1.dev231
+Version: 2.0.1.dev241
 Summary: udata search service
 Author-email: Opendata Team <opendatateam@data.gouv.fr>
 Description-Content-Type: text/markdown
 Requires-Dist: dependency-injector==4.36.0
 Requires-Dist: elasticsearch==7.15.0
 Requires-Dist: elasticsearch_dsl==7.4.0
 Requires-Dist: factory-boy==3.2.1
```

