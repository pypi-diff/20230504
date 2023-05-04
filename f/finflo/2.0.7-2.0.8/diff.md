# Comparing `tmp/finflo-2.0.7.tar.gz` & `tmp/finflo-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finflo-2.0.7.tar", last modified: Thu Apr 27 14:34:31 2023, max compression
+gzip compressed data, was "finflo-2.0.8.tar", last modified: Thu May  4 12:09:42 2023, max compression
```

## Comparing `finflo-2.0.7.tar` & `finflo-2.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 14:34:31.357445 finflo-2.0.7/
--rw-rw-rw-   0        0        0       19 2022-11-21 10:05:01.000000 finflo-2.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5488 2023-04-27 14:34:31.358437 finflo-2.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 14:34:31.306440 finflo-2.0.7/finflo/
--rw-rw-rw-   0        0        0        0 2022-11-21 10:05:02.000000 finflo-2.0.7/finflo/__init__.py
--rw-rw-rw-   0        0        0     1230 2022-12-21 07:25:04.000000 finflo-2.0.7/finflo/admin.py
--rw-rw-rw-   0        0        0     8907 2023-03-12 17:35:11.000000 finflo-2.0.7/finflo/api.py
--rw-rw-rw-   0        0        0      205 2023-02-27 08:45:47.000000 finflo-2.0.7/finflo/apps.py
--rw-rw-rw-   0        0        0      386 2022-11-24 13:02:42.000000 finflo-2.0.7/finflo/base_enum.py
--rw-rw-rw-   0        0        0      301 2022-12-15 05:39:52.000000 finflo-2.0.7/finflo/compatability.py
--rw-rw-rw-   0        0        0     1035 2023-02-20 05:36:29.000000 finflo-2.0.7/finflo/exception.py
--rw-rw-rw-   0        0        0     1460 2023-03-31 06:16:55.000000 finflo-2.0.7/finflo/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:34:31.354437 finflo-2.0.7/finflo/migrations/
--rw-rw-rw-   0        0        0    11825 2023-04-27 14:33:17.000000 finflo-2.0.7/finflo/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1489 2023-02-28 10:26:38.000000 finflo-2.0.7/finflo/migrations/0002_remigrate.py
--rw-rw-rw-   0        0        0        0 2022-11-21 10:05:02.000000 finflo-2.0.7/finflo/migrations/__init__.py
--rw-rw-rw-   0        0        0     8277 2023-04-27 14:32:20.000000 finflo-2.0.7/finflo/models.py
--rw-rw-rw-   0        0        0     4090 2023-02-21 05:58:43.000000 finflo-2.0.7/finflo/serializer.py
--rw-rw-rw-   0        0        0     2785 2023-03-24 10:04:31.000000 finflo-2.0.7/finflo/signals.py
--rw-rw-rw-   0        0        0        2 2023-03-06 12:26:54.000000 finflo-2.0.7/finflo/tests.py
--rw-rw-rw-   0        0        0    13841 2023-04-06 10:53:25.000000 finflo-2.0.7/finflo/transition.py
--rw-rw-rw-   0        0        0      907 2023-02-01 11:16:37.000000 finflo-2.0.7/finflo/urls.py
--rw-rw-rw-   0        0        0      293 2022-11-21 10:05:02.000000 finflo-2.0.7/finflo/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:34:31.335443 finflo-2.0.7/finflo.egg-info/
--rw-rw-rw-   0        0        0     5488 2023-04-27 14:34:29.000000 finflo-2.0.7/finflo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-04-27 14:34:31.000000 finflo-2.0.7/finflo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 14:34:29.000000 finflo-2.0.7/finflo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 14:34:30.000000 finflo-2.0.7/finflo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5089 2022-12-19 10:56:18.000000 finflo-2.0.7/readme.md
--rw-rw-rw-   0        0        0      421 2023-04-27 14:34:31.365444 finflo-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-03-26 08:52:21.000000 finflo-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:09:42.702130 finflo-2.0.8/
+-rw-rw-rw-   0        0        0       19 2022-11-21 10:05:01.000000 finflo-2.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5488 2023-05-04 12:09:42.703130 finflo-2.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 12:09:42.638130 finflo-2.0.8/finflo/
+-rw-rw-rw-   0        0        0        0 2022-11-21 10:05:02.000000 finflo-2.0.8/finflo/__init__.py
+-rw-rw-rw-   0        0        0     1230 2022-12-21 07:25:04.000000 finflo-2.0.8/finflo/admin.py
+-rw-rw-rw-   0        0        0    14178 2023-05-04 12:03:05.000000 finflo-2.0.8/finflo/api.py
+-rw-rw-rw-   0        0        0      205 2023-02-27 08:45:47.000000 finflo-2.0.8/finflo/apps.py
+-rw-rw-rw-   0        0        0      386 2022-11-24 13:02:42.000000 finflo-2.0.8/finflo/base_enum.py
+-rw-rw-rw-   0        0        0      301 2022-12-15 05:39:52.000000 finflo-2.0.8/finflo/compatability.py
+-rw-rw-rw-   0        0        0     1035 2023-02-20 05:36:29.000000 finflo-2.0.8/finflo/exception.py
+-rw-rw-rw-   0        0        0     1460 2023-03-31 06:16:55.000000 finflo-2.0.8/finflo/middleware.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:09:42.696135 finflo-2.0.8/finflo/migrations/
+-rw-rw-rw-   0        0        0    11825 2023-04-27 14:33:17.000000 finflo-2.0.8/finflo/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1489 2023-02-28 10:26:38.000000 finflo-2.0.8/finflo/migrations/0002_remigrate.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 10:05:02.000000 finflo-2.0.8/finflo/migrations/__init__.py
+-rw-rw-rw-   0        0        0     8277 2023-04-27 14:32:20.000000 finflo-2.0.8/finflo/models.py
+-rw-rw-rw-   0        0        0     3873 2023-05-04 12:00:46.000000 finflo-2.0.8/finflo/serializer.py
+-rw-rw-rw-   0        0        0     2917 2023-05-04 11:48:54.000000 finflo-2.0.8/finflo/signals.py
+-rw-rw-rw-   0        0        0        2 2023-03-06 12:26:54.000000 finflo-2.0.8/finflo/tests.py
+-rw-rw-rw-   0        0        0    13841 2023-04-06 10:53:25.000000 finflo-2.0.8/finflo/transition.py
+-rw-rw-rw-   0        0        0     1400 2023-05-04 12:07:18.000000 finflo-2.0.8/finflo/urls.py
+-rw-rw-rw-   0        0        0      293 2022-11-21 10:05:02.000000 finflo-2.0.8/finflo/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:09:42.675120 finflo-2.0.8/finflo.egg-info/
+-rw-rw-rw-   0        0        0     5488 2023-05-04 12:09:39.000000 finflo-2.0.8/finflo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-05-04 12:09:42.000000 finflo-2.0.8/finflo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 12:09:40.000000 finflo-2.0.8/finflo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 12:09:41.000000 finflo-2.0.8/finflo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5089 2022-12-19 10:56:18.000000 finflo-2.0.8/readme.md
+-rw-rw-rw-   0        0        0      421 2023-05-04 12:09:42.712132 finflo-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-03-26 08:52:21.000000 finflo-2.0.8/setup.py
```

### Comparing `finflo-2.0.7/PKG-INFO` & `finflo-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finflo
-Version: 2.0.7
+Version: 2.0.8
 Author: AnandRaj
 Author-email: anandrajb@venzotechnologies.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
```

### Comparing `finflo-2.0.7/finflo/admin.py` & `finflo-2.0.8/finflo/admin.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.7/finflo/api.py` & `finflo-2.0.8/finflo/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.permissions import IsAuthenticated
 from .transition import FinFlotransition
 from rest_framework.generics import (
     ListAPIView,
     ListCreateAPIView,
-    RetrieveUpdateAPIView
+    RetrieveUpdateAPIView,
+    RetrieveUpdateDestroyAPIView
 )
 from django.shortcuts import get_object_or_404
 from django.conf import settings
 from .serializer import  (
     StatesSerializer,
     TransitionManagerserializer,
     Actionseriaizer,
@@ -167,14 +168,38 @@
         serializer = Actionseriaizer(data=request.data)
         if serializer.is_valid():
             serializer.save()
             return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
         return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
 
 
+
+
+class ActionRetrieveUpdateApi(RetrieveUpdateDestroyAPIView):
+    queryset = Action.objects.all()
+    serializer_class = Actionseriaizer
+    permission_classes = [IsAuthenticated]
+
+    def retrieve(self, request, pk=None):
+        queryset = Action.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = Actionseriaizer(user)
+        return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+
+    def update(self, request, pk=None):
+        queryset = Action.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = Actionseriaizer(user, data=request.data)
+        if serializer.is_valid():
+            serializer.save()
+            return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+        return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
+
+
+
 # STATES API 
 
 
 class statesListCreateApi(ListCreateAPIView):
     queryset = States.objects.all()
     serializer_class = StatesSerializer
     permission_classes = [IsAuthenticated]
@@ -190,27 +215,80 @@
         if serializer.is_valid():
             serializer.save()
             return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
         return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
 
 
 
+class StatesRetrieveUpdateApi(RetrieveUpdateDestroyAPIView):
+    queryset = States.objects.all()
+    serializer_class = StatesSerializer
+    permission_classes = [IsAuthenticated]
+
+    def retrieve(self, request, pk=None):
+        queryset = States.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = StatesSerializer(user)
+        return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+
+    def update(self, request, pk=None):
+        queryset = States.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = StatesSerializer(user, data=request.data)
+        if serializer.is_valid():
+            serializer.save()
+            return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+        return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
+
+
+
+
 # FLOW MODEL GET API 
 
 class FlowModelGetApi(ListCreateAPIView):
     queryset = Flowmodel.objects.all()
     serializer_class = FlowmodelsSerializer
     permission_classes = [IsAuthenticated]
 
     def list(self, request):
         queryset = Flowmodel.objects.all()
         serializer = FlowmodelsSerializer(queryset, many=True)
         return Response({"status": "success" , "data": serializer.data}, status=status.HTTP_200_OK)
 
 
+    def post(self, request):
+        serializer = FlowmodelsSerializer(data=request.data)
+        if serializer.is_valid():
+            serializer.save()
+            return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+        return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
+
+
+
+class FlowModelRetrieveUpdateApi(RetrieveUpdateDestroyAPIView):
+    queryset = Flowmodel.objects.all()
+    serializer_class = FlowmodelsSerializer
+    permission_classes = [IsAuthenticated]
+
+    def retrieve(self, request, pk=None):
+        queryset = Flowmodel.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = FlowmodelsSerializer(user)
+        return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+
+    def update(self, request, pk=None):
+        queryset = Flowmodel.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = FlowmodelsSerializer(user, data=request.data)
+        if serializer.is_valid():
+            serializer.save()
+            return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+        return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
+
+
 
 # PARTY TYPE API 
 
 class PartyTypeListCreateApi(ListCreateAPIView):
     queryset = Party.objects.all()
     serializer_class = partytypeserializer
     permission_classes = [IsAuthenticated]
@@ -226,14 +304,37 @@
         if serializer.is_valid():
             serializer.save()
             return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
         return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
 
 
 
+class PartyTypeRetrieveUpdateApi(RetrieveUpdateDestroyAPIView):
+    queryset = Party.objects.all()
+    serializer_class = partytypeserializer
+    permission_classes = [IsAuthenticated]
+
+    def retrieve(self, request, pk=None):
+        queryset = Party.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = partytypeserializer(user)
+        return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+
+    def update(self, request, pk=None):
+        queryset = Party.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = partytypeserializer(user, data=request.data)
+        if serializer.is_valid():
+            serializer.save()
+            return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+        return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
+
+
+
+
 # SIGN LIST API 
 
 
 class SignListListCreateApi(ListCreateAPIView):
     queryset = SignList.objects.all()
     serializer_class = signlistserialzier
     permission_classes = [IsAuthenticated]
@@ -244,8 +345,32 @@
         return Response({"status": "success" , "data": serializer.data}, status=status.HTTP_200_OK)
 
     def post(self, request):
         serializer = signlistserialzier(data=request.data)
         if serializer.is_valid():
             serializer.save()
             return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+        return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
+
+
+
+
+
+class SignListRetrieveUpdateApi(RetrieveUpdateDestroyAPIView):
+    queryset = SignList.objects.all()
+    serializer_class = signlistserialzier
+    permission_classes = [IsAuthenticated]
+
+    def retrieve(self, request, pk=None):
+        queryset = SignList.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = signlistserialzier(user)
+        return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
+
+    def update(self, request, pk=None):
+        queryset = SignList.objects.all()
+        user = get_object_or_404(queryset, pk=pk)
+        serializer = signlistserialzier(user, data=request.data)
+        if serializer.is_valid():
+            serializer.save()
+            return Response({"status": "success", "data": serializer.data}, status=status.HTTP_201_CREATED)
         return Response({"status": "failure", "data": serializer.errors},status=status.HTTP_204_NO_CONTENT)
```

### Comparing `finflo-2.0.7/finflo/exception.py` & `finflo-2.0.8/finflo/exception.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.7/finflo/middleware.py` & `finflo-2.0.8/finflo/middleware.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.7/finflo/migrations/0001_initial.py` & `finflo-2.0.8/finflo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.7/finflo/migrations/0002_remigrate.py` & `finflo-2.0.8/finflo/migrations/0002_remigrate.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.7/finflo/models.py` & `finflo-2.0.8/finflo/models.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.7/finflo/serializer.py` & `finflo-2.0.8/finflo/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,24 +113,15 @@
         return obj.workflowitems.id
 
 
 
 class Actionseriaizer(serializers.ModelSerializer):
     class Meta:
         model = Action
-        fields = [
-            'description',
-            'model',
-            'from_state',
-            'to_state',
-            'intermediator',
-            'from_party',
-            'to_party',
-            'stage_required'
-        ]
+        fields = '__all__'
 
 
 
 class StatesSerializer(serializers.ModelSerializer):
     class Meta:
         model = States
         fields = '__all__'
```

### Comparing `finflo-2.0.7/finflo/signals.py` & `finflo-2.0.8/finflo/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.db.models.signals import post_save, post_delete
 from .exception import DefaultsNotFoundError, PartyLengthError
 from .middleware import get_current_user
 from .models import States, TransitionManager, workevents, workflowitems
 from django.conf import settings
 from .transition import  DefaultModelValues
 from .compatability import check_version_compatibility
-
+from .middleware import get_current_user
 
 # MAIN SIGNAL RECEIVER FOR TRANSITION HANDLING - 4/8/2022 by anand
 
 Base_link = "https://pypi.org/project/finflo/"
 
 
 # CORE LIST ITERATED FROM THE DEFAULT SETTINGS -- PRODUCTION : 27/10/2022
@@ -53,21 +53,23 @@
         model = sender._meta.label_lower
         states = States.objects.get(id=1)
         obj = TransitionManager.objects.create(type=model, t_id=instance.id)
         obj2 = workflowitems.objects.create(
             transitionmanager=obj,
             model_type=model,
             record_datas=DefaultModelValues(model_type = obj.type , id = obj.t_id).get_record_Datas(),
+            event_user = get_current_user(),
             initial_state=states.description,
             interim_state=states.description,
             final_state=states.description,
         )
         workevents.objects.create(
             workflowitems=obj2,
             model_type=model,
+            event_user = get_current_user(),
             record_datas = DefaultModelValues(model_type =  obj.type , id = obj.t_id).get_record_Datas(),
             initial_state=states.description,
             interim_state=states.description,
             final_state=states.description,
         )
```

### Comparing `finflo-2.0.7/finflo/transition.py` & `finflo-2.0.8/finflo/transition.py`

 * *Files identical despite different names*

### Comparing `finflo-2.0.7/finflo.egg-info/PKG-INFO` & `finflo-2.0.8/finflo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finflo
-Version: 2.0.7
+Version: 2.0.8
 Author: AnandRaj
 Author-email: anandrajb@venzotechnologies.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
```

### Comparing `finflo-2.0.7/finflo.egg-info/SOURCES.txt` & `finflo-2.0.8/finflo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finflo-2.0.7/readme.md` & `finflo-2.0.8/readme.md`

 * *Files identical despite different names*

