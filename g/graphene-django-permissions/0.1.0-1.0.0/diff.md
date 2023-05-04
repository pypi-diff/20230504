# Comparing `tmp/graphene-django-permissions-0.1.0.tar.gz` & `tmp/graphene_django_permissions-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-permissions-0.1.0.tar", max compression
+gzip compressed data, was "graphene_django_permissions-1.0.0.tar", max compression
```

## Comparing `graphene-django-permissions-0.1.0.tar` & `graphene_django_permissions-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1073 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/LICENSE
--rw-r--r--   0        0        0      741 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/README.md
--rw-r--r--   0        0        0       58 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/graphene_django_permissions/__init__.py
--rw-r--r--   0        0        0     4057 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/graphene_django_permissions/middleware.py
--rw-r--r--   0        0        0     2317 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1028 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/factories.py
--rwxr-xr-x   0        0        0      655 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/manage.py
--rw-r--r--   0        0        0     1337 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/migrations/__init__.py
--rw-r--r--   0        0        0      536 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/models.py
--rw-r--r--   0        0        0     3143 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/schema.py
--rw-r--r--   0        0        0     1092 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/settings.py
--rw-r--r--   0        0        0    41569 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/test_middleware.py
--rw-r--r--   0        0        0      185 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/urls.py
--rw-r--r--   0        0        0     1715 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/utils.py
--rw-r--r--   0        0        0      381 2022-05-10 20:55:40.915317 graphene-django-permissions-0.1.0/tests/wsgi.py
--rw-r--r--   0        0        0     1554 2022-05-10 20:55:50.378665 graphene-django-permissions-0.1.0/setup.py
--rw-r--r--   0        0        0     1656 2022-05-10 20:55:50.378971 graphene-django-permissions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/LICENSE
+-rw-r--r--   0        0        0     9442 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/README.md
+-rw-r--r--   0        0        0       58 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/graphene_django_permissions/__init__.py
+-rw-r--r--   0        0        0     4015 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/graphene_django_permissions/middleware.py
+-rw-r--r--   0        0        0     3754 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1028 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/factories.py
+-rwxr-xr-x   0        0        0      655 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/manage.py
+-rw-r--r--   0        0        0     1337 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      536 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/models.py
+-rw-r--r--   0        0        0     3224 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/schema.py
+-rw-r--r--   0        0        0     1098 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/settings.py
+-rw-r--r--   0        0        0    41264 2023-05-04 01:37:14.987015 graphene_django_permissions-1.0.0/tests/test_middleware.py
+-rw-r--r--   0        0        0      138 2023-05-04 01:37:14.991015 graphene_django_permissions-1.0.0/tests/urls.py
+-rw-r--r--   0        0        0     1715 2023-05-04 01:37:14.991015 graphene_django_permissions-1.0.0/tests/utils.py
+-rw-r--r--   0        0        0      381 2023-05-04 01:37:14.991015 graphene_django_permissions-1.0.0/tests/wsgi.py
+-rw-r--r--   0        0        0    10700 1970-01-01 00:00:00.000000 graphene_django_permissions-1.0.0/PKG-INFO
```

### Comparing `graphene-django-permissions-0.1.0/LICENSE` & `graphene_django_permissions-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-permissions-0.1.0/graphene_django_permissions/middleware.py` & `graphene_django_permissions-1.0.0/graphene_django_permissions/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     """
 
     def resolve(self, next, root, info, **args):
         # First, get the result for this node in the response
         result = next(root, info, **args)
 
         # Given the resulting value, check whether the current user has view access
-        if isinstance(result.value, models.Model):
-            if not has_permission_to_view_model_object(info.context.user, result.value):
+        if isinstance(result, models.Model):
+            if not has_permission_to_view_model_object(info.context.user, result):
                 # The user does not have access to all objects for this model, nor this
                 # specific object. As such, return null for this field.
 
                 if isinstance(info.return_type, graphql.GraphQLNonNull):
                     # If this field the client requested (but doesn't have access to) is
                     # non-nullable in the GraphQL schema, then we're forced to raise an
                     # error, since we can't circumvent the schema at the authorization
@@ -51,39 +51,39 @@
                     # GQL schema will still be returned and appear as normal.
                     raise PermissionDenied(
                         "You do not have permission to access this field"
                     )
 
                 return None
 
-        elif isinstance(result.value, models.QuerySet):
-            model = result.value.model
+        elif isinstance(result, models.QuerySet):
+            model = result.model
             permission = get_view_permission_for_model(model)
             if not info.context.user.has_perm(permission):
                 # The user does not have access to all objects for this model, so we'll
                 # filter to only the specific objects the user can access. Note that we
                 # are implicitly converting the queryset to a list by doing so. This is
                 # intentional, since the query will already have been evaluated and
                 # optimized from the top-level (if graphene_django_optimizer is used),
                 # so we effectively pay no SQL cost by iterating through the results
                 # here, unlike if we were to use a `filter` on the queryset or similar.
                 return [
                     obj
-                    for obj in result.value
+                    for obj in result
                     if info.context.user.has_perm(permission, obj=obj)
                 ]
 
-        elif isinstance(result.value, (list, tuple, set)):
+        elif isinstance(result, (list, tuple, set)):
             # Sometimes queries may return a list or other iterable of models, rather
             # than a QuerySet of models (e.g., if they performed some in-memory
             # filtering on a queryset and implicitly converted to a list themselves). In
             # this case, we should still attempt to check permissions on the individual
             # objects. We'll allow (1) any object that isn't a model object or (2) any
             # model object that the user has permission to view.
             return [
                 obj
-                for obj in result.value
+                for obj in result
                 if not isinstance(obj, models.Model)
                 or has_permission_to_view_model_object(info.context.user, obj)
             ]
 
         return result
```

### Comparing `graphene-django-permissions-0.1.0/tests/factories.py` & `graphene_django_permissions-1.0.0/tests/factories.py`

 * *Files identical despite different names*

### Comparing `graphene-django-permissions-0.1.0/tests/manage.py` & `graphene_django_permissions-1.0.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `graphene-django-permissions-0.1.0/tests/migrations/0001_initial.py` & `graphene_django_permissions-1.0.0/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `graphene-django-permissions-0.1.0/tests/models.py` & `graphene_django_permissions-1.0.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `graphene-django-permissions-0.1.0/tests/schema.py` & `graphene_django_permissions-1.0.0/tests/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 
 # Types
 
 
 class Project(DjangoObjectType):
     class Meta:
         model = models.Project
+        fields = "__all__"
 
 
 class Expense(DjangoObjectType):
     class Meta:
         model = models.Expense
+        fields = "__all__"
 
 
 class User(DjangoObjectType):
     class Meta:
         model = UserModel
+        fields = "__all__"
 
 
 # Queries
 
 
 class Query(graphene.ObjectType):
     project = graphene.Field(Project, id=graphene.ID())
```

### Comparing `graphene-django-permissions-0.1.0/tests/settings.py` & `graphene_django_permissions-1.0.0/tests/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 
 DATABASES = {
     "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": BASE_DIR / "db.sqlite3"}
 }
 
 GRAPHENE = {
-    "SCHEMA": "schema.schema",
+    "SCHEMA": "tests.schema.schema",
     "MIDDLEWARE": [
         "graphene_django_permissions.middleware.GrapheneAuthorizationMiddleware",
     ],
 }
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
```

### Comparing `graphene-django-permissions-0.1.0/tests/test_middleware.py` & `graphene_django_permissions-1.0.0/tests/test_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import re
 
 import pytest
 from django.contrib.auth.backends import BaseBackend
 from django.test.client import Client
 from graphene_django.utils.testing import graphql_query
 
@@ -39,15 +38,15 @@
 def use_owner_permitted_auth_backend(settings):
     """
     Add the object-level permissioning authorization backend to the configured backends
     in Django.
     """
     settings.AUTHENTICATION_BACKENDS = [
         *settings.AUTHENTICATION_BACKENDS,
-        "test_middleware.OwnerPermittedAuthBackend",
+        "tests.test_middleware.OwnerPermittedAuthBackend",
     ]
 
 
 class TestGrapheneAuthorizationMiddleware:
     """
     Test that the Graphene authorization middleware properly restricts read access
     depending on user permissions.
@@ -229,15 +228,15 @@
         response = graphql_query(
             query=self._projects_with_expenses_query(),
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projects"]
 
         # All of the projects and expenses should be visible, with their associated user
         # data
         assert len(projects_in_response) == 2
         assert {project["id"] for project in projects_in_response} == {
             str(project1.id),
@@ -276,15 +275,15 @@
         response = graphql_query(
             query=self._projects_with_expenses_query(),
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projects"]
 
         # All of the projects and expenses should be visible
         assert len(projects_in_response) == 2
         assert {project["id"] for project in projects_in_response} == {
             str(project1.id),
             str(project2.id),
@@ -326,15 +325,15 @@
         response = graphql_query(
             self._projects_with_expenses_query(),
             client=client,
         )
 
         # There should be no errors, but the top-level list should be empty
         assert_graphql_response_has_no_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         assert len(content["data"]["projects"]) == 0
 
     @pytest.mark.usefixtures("use_owner_permitted_auth_backend")
     def test_top_level_list_field_contains_owned_objects_with_object_level_permissions(
         self, client: Client
     ):
         """
@@ -362,15 +361,15 @@
 
         response = graphql_query(
             self._projects_with_expenses_query(),
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         assert len(content["data"]["projects"]) == 1
         assert content["data"]["projects"][0]["id"] == str(project3.id)
         assert len(content["data"]["projects"][0]["expenses"]) == 2
 
     def test_top_level_list_field_is_empty_for_anonymous_user_without_permission(
         self, client: Client
     ):
@@ -387,15 +386,15 @@
         response = graphql_query(
             self._projects_with_expenses_query(),
             client=client,
         )
 
         # There should be no errors, but the top-level list should be empty
         assert_graphql_response_has_no_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         assert len(content["data"]["projects"]) == 0
 
     def test_top_level_object_field_is_non_empty_with_permission(self, client: Client):
         """
         When querying for a single object field, it should be returned if the user has
         permission to that model.
         """
@@ -417,15 +416,15 @@
                 "id": project.id,
             },
             client=client,
         )
 
         # There should be no errors, but the top-level object should be empty
         assert_graphql_response_has_no_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         project_in_response = content["data"]["project"]
         assert project_in_response is not None
         assert project_in_response["id"] == str(project.id)
         assert project_in_response["owner"] is not None
         assert len(project_in_response["expenses"]) == 2
         assert project_in_response["expenses"][0]["owner"] is not None
 
@@ -452,15 +451,15 @@
                 "id": project.id,
             },
             client=client,
         )
 
         # There should be no errors, but the top-level object should be empty
         assert_graphql_response_has_no_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         assert content["data"]["project"] is None
 
     def test_nested_related_model_list_is_empty_when_missing_permissions(
         self, client: Client
     ):
         """
         When a user doesn't have permission for a nested model that's returned as a
@@ -483,15 +482,15 @@
         response = graphql_query(
             query=self._projects_with_expenses_query(),
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projects"]
 
         # The projects should show up, but expenses should be empty
         assert len(projects_in_response) == 2
         assert {project["id"] for project in projects_in_response} == {
             str(project1.id),
             str(project2.id),
@@ -534,15 +533,15 @@
         response = graphql_query(
             query=self._projects_with_expenses_query(),
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projects"]
 
         # The projects should show up, and the list of expenses should match the ones
         # owned by the user
         assert len(projects_in_response) == 2
         assert {project["id"] for project in projects_in_response} == {
             str(project1.id),
@@ -598,15 +597,15 @@
                 "id": project.id,
             },
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         project_in_response = content["data"]["project"]
         assert project_in_response is not None
         assert project_in_response["id"] == str(project.id)
         # The owner and their expenses should show up, since the user has permission to
         # view both
         assert project_in_response["owner"] is not None
         assert project_in_response["owner"]["id"] == str(project.owner.id)
@@ -639,15 +638,15 @@
                 "id": project.id,
             },
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         project_in_response = content["data"]["project"]
         assert project_in_response is not None
         assert project_in_response["id"] == str(project.id)
         # The owner should still show up, but its list of expenses should be empty since
         # the user does not have permission to view those
         assert project_in_response["owner"] is not None
         assert project_in_response["owner"]["id"] == str(project.owner.id)
@@ -679,15 +678,15 @@
                 "id": expense.id,
             },
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         expense_in_response = content["data"]["expense"]
         assert expense_in_response["id"] == str(expense.id)
         assert expense_in_response["amount"] == expense.amount
         assert expense_in_response["project"] is not None
         assert expense_in_response["project"]["id"] == str(expense.project.id)
         assert expense_in_response["project"]["owner"]["id"] == str(
             expense.project.owner.id
@@ -723,15 +722,15 @@
             },
             client=client,
         )
 
         # Verify that an error showed up for the expense's project owner (User), since
         # the user doesn't have permission
         assert_graphql_response_has_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         assert (
             "You do not have permission to access this field"
             in content["errors"][0]["message"]
         )
         assert content["errors"][0]["path"] == [
             "expense",
             "project",
@@ -773,15 +772,15 @@
                 "id": expense.id,
             },
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         expense_in_response = content["data"]["expense"]
         assert expense_in_response["id"] == str(expense.id)
         assert expense_in_response["project"] is not None
         assert expense_in_response["project"]["id"] == str(project.id)
 
     def test_nullable_foreign_key_appears_empty_without_permission_to_model(
         self, client: Client
@@ -812,15 +811,15 @@
             client=client,
         )
 
         # The project should show up as null, but there should be no errors in the
         # response, since we can safely omit it and still satisfy the GQL schema
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         expense_in_response = content["data"]["expense"]
         assert expense_in_response["id"] == str(expense.id)
         assert expense_in_response["project"] is None
 
     def test_field_returning_list_instead_of_queryset_is_not_empty_with_permission(
         self, client: Client
     ):
@@ -846,15 +845,15 @@
             self._projects_returning_list_query(),
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
         # All of the projects should show up
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projectsList"]
 
         assert len(projects_in_response) == 2
         assert {project["id"] for project in projects_in_response} == {
             str(project1.id),
             str(project2.id),
         }
@@ -889,15 +888,15 @@
         response = graphql_query(
             self._projects_returning_list_query(),
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projectsList"]
 
         assert len(projects_in_response) == 2
         assert {project["id"] for project in projects_in_response} == {
             str(project1.id),
             str(project2.id),
         }
@@ -926,15 +925,15 @@
         response = graphql_query(
             self._projects_returning_list_query(),
             client=client,
         )
 
         assert_graphql_response_has_no_errors(response)
 
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projectsList"]
 
         # Since the user doesn't have permission to view projects, none should be
         # returned (even though this query resolver returns a list and not a QuerySet)
         assert len(projects_in_response) == 0
 
     def test_mutation_response_is_complete_with_permissions(self, client: Client):
@@ -967,15 +966,15 @@
         # The mutation should've been performed successfully
         assert_graphql_response_has_no_errors(response)
         project.refresh_from_db()
         assert project.name == new_name
 
         # The response should contain all of the requested data, including the nested
         # user and expense data fields
-        content = json.loads(response.content)
+        content = response.json()
         project_in_response = content["data"]["projectUpdate"]["project"]
         assert project_in_response["id"] == str(project.id)
         assert project_in_response["name"] == new_name
         assert project_in_response["owner"] is not None
         assert project_in_response["owner"]["id"] == str(project.owner.id)
         assert len(project_in_response["expenses"]) == 2
         assert project_in_response["expenses"][0]["owner"] is not None
@@ -1009,15 +1008,15 @@
 
         # The mutation itself should've been performed successfully, with no errors
         assert_graphql_response_has_no_errors(response)
         project.refresh_from_db()
         assert project.name == new_name
 
         # The response, however, should omit the unauthorized expenses data
-        content = json.loads(response.content)
+        content = response.json()
         project_in_response = content["data"]["projectUpdate"]["project"]
         assert project_in_response["id"] == str(project.id)
         assert project_in_response["name"] == new_name
         assert project_in_response["owner"] is not None
         assert project_in_response["owner"]["id"] == str(project.owner.id)
         assert len(project_in_response["expenses"]) == 0
 
@@ -1082,15 +1081,15 @@
             response = graphql_query(
                 query=self._projects_with_expenses_query(),
                 client=client,
             )
 
         # Sanity-check that the response was valid
         assert_graphql_response_has_no_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projects"]
         assert len(projects_in_response) == 2
         assert len(projects_in_response[0]["expenses"]) > 0
 
         self._assert_projects_with_expenses_sql_queries_match_expected(captured)
 
     def test_sql_queries_are_still_optimized_when_user_is_missing_permissions(
@@ -1117,15 +1116,15 @@
             response = graphql_query(
                 query=self._projects_with_expenses_query(),
                 client=client,
             )
 
         # Sanity-check that the response was valid
         assert_graphql_response_has_no_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projects"]
         assert len(projects_in_response) == 2
         # Expenses should be empty since the user does not have permission to view them
         assert len(projects_in_response[0]["expenses"]) == 0
 
         # The SQL query performance should be the same as when a user has all
         # permission, still optimized
@@ -1161,15 +1160,15 @@
             response = graphql_query(
                 query=self._projects_with_expenses_query(),
                 client=client,
             )
 
         # Sanity-check that the response was valid
         assert_graphql_response_has_no_errors(response)
-        content = json.loads(response.content)
+        content = response.json()
         projects_in_response = content["data"]["projects"]
         assert len(projects_in_response) == 2
         # Expenses should contain only the ones owned by the user
         assert len(projects_in_response[0]["expenses"]) == 2
         assert len(projects_in_response[1]["expenses"]) == 2
 
         # The SQL query performance should be the same as when a user has all
```

### Comparing `graphene-django-permissions-0.1.0/tests/utils.py` & `graphene_django_permissions-1.0.0/tests/utils.py`

 * *Files identical despite different names*

