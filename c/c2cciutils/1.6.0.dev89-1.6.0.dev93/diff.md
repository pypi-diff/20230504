# Comparing `tmp/c2cciutils-1.6.0.dev89.tar.gz` & `tmp/c2cciutils-1.6.0.dev93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2cciutils-1.6.0.dev89.tar", max compression
+gzip compressed data, was "c2cciutils-1.6.0.dev93.tar", max compression
```

## Comparing `c2cciutils-1.6.0.dev89.tar` & `c2cciutils-1.6.0.dev93.tar`

### file list

```diff
@@ -1,603 +1,592 @@
--rw-r--r--   0        0        0     1307 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/LICENSE
--rw-r--r--   0        0        0    14776 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/README.md
--rw-r--r--   0        0        0    18066 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/__init__.py
--rw-r--r--   0        0        0      178 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/applications-versions.yaml
--rw-r--r--   0        0        0      283 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/applications.yaml
--rw-r--r--   0        0        0     1232 2023-05-03 12:36:28.729092 c2cciutils-1.6.0.dev89/c2cciutils/applications_definition.py
--rw-r--r--   0        0        0     9028 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/audit.py
--rw-r--r--   0        0        0      358 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/branches.graphql
--rw-r--r--   0        0        0      308 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/commits.graphql
--rw-r--r--   0        0        0    22063 2023-05-03 12:36:26.160920 c2cciutils-1.6.0.dev89/c2cciutils/configuration.py
--rw-r--r--   0        0        0      131 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/default_branch.graphql
--rw-r--r--   0        0        0     3425 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/env.py
--rw-r--r--   0        0        0     5485 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/lib/docker.py
--rw-r--r--   0        0        0    14824 2023-05-03 12:35:25.288529 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/.package-lock.json
--rw-r--r--   0        0        0     2973 2023-05-03 12:35:22.944355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/api.js
--rw-r--r--   0        0        0    20649 2023-05-03 12:35:22.976358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/baseclient.js
--rw-r--r--   0        0        0      196 2023-05-03 12:35:22.980358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/constants.js
--rw-r--r--   0        0        0     2792 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/envelope.js
--rw-r--r--   0        0        0     6114 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/exports.js
--rw-r--r--   0        0        0    13557 2023-05-03 12:35:23.020361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/hub.js
--rw-r--r--   0        0        0     3921 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/index.js
--rw-r--r--   0        0        0     4142 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/integration.js
--rw-r--r--   0        0        0     1017 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/integrations/functiontostring.js
--rw-r--r--   0        0        0     6540 2023-05-03 12:35:23.040362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/integrations/inboundfilters.js
--rw-r--r--   0        0        0      333 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/integrations/index.js
--rw-r--r--   0        0        0    13560 2023-05-03 12:35:23.060364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/scope.js
--rw-r--r--   0        0        0     1161 2023-05-03 12:35:23.064364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/sdk.js
--rw-r--r--   0        0        0     5052 2023-05-03 12:35:23.064364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/session.js
--rw-r--r--   0        0        0     3819 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/sessionflusher.js
--rw-r--r--   0        0        0     1220 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/errors.js
--rw-r--r--   0        0        0     8922 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/hubextensions.js
--rw-r--r--   0        0        0    12457 2023-05-03 12:35:23.036362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/idletransaction.js
--rw-r--r--   0        0        0     8967 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/span.js
--rw-r--r--   0        0        0     2669 2023-05-03 12:35:23.076365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/spanstatus.js
--rw-r--r--   0        0        0     1877 2023-05-03 12:35:23.076365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/trace.js
--rw-r--r--   0        0        0     7741 2023-05-03 12:35:23.080366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/transaction.js
--rw-r--r--   0        0        0      623 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/utils.js
--rw-r--r--   0        0        0     3433 2023-05-03 12:35:22.952356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/transports/base.js
--rw-r--r--   0        0        0     3513 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/transports/offline.js
--rw-r--r--   0        0        0      796 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js
--rw-r--r--   0        0        0     8185 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/utils/prepareEvent.js
--rw-r--r--   0        0        0      166 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/version.js
--rw-r--r--   0        0        0     2845 2023-05-03 12:35:22.948356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/api.js
--rw-r--r--   0        0        0    20562 2023-05-03 12:35:22.976358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/baseclient.js
--rw-r--r--   0        0        0      113 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/constants.js
--rw-r--r--   0        0        0     2723 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/envelope.js
--rw-r--r--   0        0        0     5734 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/exports.js
--rw-r--r--   0        0        0    13310 2023-05-03 12:35:23.024361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/hub.js
--rw-r--r--   0        0        0     1833 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/index.js
--rw-r--r--   0        0        0     3983 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/integration.js
--rw-r--r--   0        0        0      944 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/integrations/functiontostring.js
--rw-r--r--   0        0        0     6350 2023-05-03 12:35:23.040362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/integrations/inboundfilters.js
--rw-r--r--   0        0        0      146 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/integrations/index.js
--rw-r--r--   0        0        0    13506 2023-05-03 12:35:23.060364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/scope.js
--rw-r--r--   0        0        0     1079 2023-05-03 12:35:23.064364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/sdk.js
--rw-r--r--   0        0        0     4938 2023-05-03 12:35:23.068364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/session.js
--rw-r--r--   0        0        0     3751 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/sessionflusher.js
--rw-r--r--   0        0        0     1141 2023-05-03 12:35:22.992359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/errors.js
--rw-r--r--   0        0        0     8723 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/hubextensions.js
--rw-r--r--   0        0        0    12223 2023-05-03 12:35:23.036362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/idletransaction.js
--rw-r--r--   0        0        0     8832 2023-05-03 12:35:23.076365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/span.js
--rw-r--r--   0        0        0     2600 2023-05-03 12:35:23.076365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/spanstatus.js
--rw-r--r--   0        0        0     1803 2023-05-03 12:35:23.080366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/trace.js
--rw-r--r--   0        0        0     7640 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/transaction.js
--rw-r--r--   0        0        0      417 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/utils.js
--rw-r--r--   0        0        0     3404 2023-05-03 12:35:22.956356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/transports/base.js
--rw-r--r--   0        0        0     3418 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/transports/offline.js
--rw-r--r--   0        0        0      720 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/utils/hasTracingEnabled.js
--rw-r--r--   0        0        0     8067 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/utils/prepareEvent.js
--rw-r--r--   0        0        0       91 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/version.js
--rw-r--r--   0        0        0      943 2023-05-03 12:35:22.816346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/modules/index.js
--rw-r--r--   0        0        0       26 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      915 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/package.json
--rw-r--r--   0        0        0      824 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
--rw-r--r--   0        0        0       71 2023-05-03 12:35:22.888351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0    10274 2023-05-03 12:35:22.852348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/tslib.es6.js
--rw-r--r--   0        0        0    13204 2023-05-03 12:35:22.872350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/tslib.js
--rw-r--r--   0        0        0      627 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/package.json
--rw-r--r--   0        0        0     5887 2023-05-03 12:35:22.848348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/client.js
--rw-r--r--   0        0        0     3247 2023-05-03 12:35:22.928354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/eventbuilder.js
--rw-r--r--   0        0        0    12033 2023-05-03 12:35:22.940355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/handlers.js
--rw-r--r--   0        0        0     2961 2023-05-03 12:35:22.980358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/index.js
--rw-r--r--   0        0        0     1462 2023-05-03 12:35:22.868350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/console.js
--rw-r--r--   0        0        0    11763 2023-05-03 12:35:22.896352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/context.js
--rw-r--r--   0        0        0     5626 2023-05-03 12:35:22.908353 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/contextlines.js
--rw-r--r--   0        0        0    10395 2023-05-03 12:35:22.948356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/http.js
--rw-r--r--   0        0        0     1151 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/index.js
--rw-r--r--   0        0        0     3071 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/linkederrors.js
--rw-r--r--   0        0        0    12254 2023-05-03 12:35:23.020361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/localvariables.js
--rw-r--r--   0        0        0     2184 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/modules.js
--rw-r--r--   0        0        0     6512 2023-05-03 12:35:23.036362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/onuncaughtexception.js
--rw-r--r--   0        0        0     2505 2023-05-03 12:35:23.040362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/onunhandledrejection.js
--rw-r--r--   0        0        0     6635 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/requestdata.js
--rw-r--r--   0        0        0     6051 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/undici/index.js
--rw-r--r--   0        0        0     1296 2023-05-03 12:35:22.924354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/errorhandling.js
--rw-r--r--   0        0        0     8607 2023-05-03 12:35:22.952356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/http.js
--rw-r--r--   0        0        0     1696 2023-05-03 12:35:23.024361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/module.js
--rw-r--r--   0        0        0     1606 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/requestDataDeprecated.js
--rw-r--r--   0        0        0     8798 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/requestdata.js
--rw-r--r--   0        0        0     9782 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/sdk.js
--rw-r--r--   0        0        0     1019 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/tracing/index.js
--rw-r--r--   0        0        0      396 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/tracing/integrations.js
--rw-r--r--   0        0        0     4786 2023-05-03 12:35:22.956356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/transports/http.js
--rw-r--r--   0        0        0     1629 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/utils.js
--rw-r--r--   0        0        0     5836 2023-05-03 12:35:22.856349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/client.js
--rw-r--r--   0        0        0     3157 2023-05-03 12:35:22.928354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/eventbuilder.js
--rw-r--r--   0        0        0    11895 2023-05-03 12:35:22.944355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/handlers.js
--rw-r--r--   0        0        0     1717 2023-05-03 12:35:22.996359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/index.js
--rw-r--r--   0        0        0     1400 2023-05-03 12:35:22.880351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/console.js
--rw-r--r--   0        0        0    11588 2023-05-03 12:35:22.904352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/context.js
--rw-r--r--   0        0        0     5541 2023-05-03 12:35:22.920354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/contextlines.js
--rw-r--r--   0        0        0    10385 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/http.js
--rw-r--r--   0        0        0      564 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/index.js
--rw-r--r--   0        0        0     3001 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/linkederrors.js
--rw-r--r--   0        0        0    12131 2023-05-03 12:35:23.020361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/localvariables.js
--rw-r--r--   0        0        0     2122 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/modules.js
--rw-r--r--   0        0        0     6396 2023-05-03 12:35:23.040362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/onuncaughtexception.js
--rw-r--r--   0        0        0     2409 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/onunhandledrejection.js
--rw-r--r--   0        0        0     6570 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/requestdata.js
--rw-r--r--   0        0        0     6024 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/undici/index.js
--rw-r--r--   0        0        0     1200 2023-05-03 12:35:22.924354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/errorhandling.js
--rw-r--r--   0        0        0     8385 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/http.js
--rw-r--r--   0        0        0     1618 2023-05-03 12:35:23.024361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/module.js
--rw-r--r--   0        0        0     1532 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/requestDataDeprecated.js
--rw-r--r--   0        0        0     8640 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/requestdata.js
--rw-r--r--   0        0        0     9460 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/sdk.js
--rw-r--r--   0        0        0      931 2023-05-03 12:35:23.008360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/tracing/index.js
--rw-r--r--   0        0        0      142 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/tracing/integrations.js
--rw-r--r--   0        0        0     4667 2023-05-03 12:35:22.976358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/transports/http.js
--rw-r--r--   0        0        0     1550 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/utils.js
--rw-r--r--   0        0        0      943 2023-05-03 12:35:22.816346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/node_modules/tslib/modules/index.js
--rw-r--r--   0        0        0       26 2023-05-03 12:35:22.872350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      915 2023-05-03 12:35:22.880351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/node_modules/tslib/package.json
--rw-r--r--   0        0        0      824 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
--rw-r--r--   0        0        0       71 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0    10274 2023-05-03 12:35:22.852348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/node_modules/tslib/tslib.es6.js
--rw-r--r--   0        0        0    13204 2023-05-03 12:35:22.860349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/node_modules/tslib/tslib.js
--rw-r--r--   0        0        0      970 2023-05-03 12:35:23.060364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/package.json
--rw-r--r--   0        0        0       35 2023-05-03 12:35:22.808345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/types/cjs/index.js
--rw-r--r--   0        0        0       35 2023-05-03 12:35:22.824346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/types/esm/index.js
--rw-r--r--   0        0        0      506 2023-05-03 12:35:22.828347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/types/package.json
--rw-r--r--   0        0        0     5903 2023-05-03 12:35:22.952356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/baggage.js
--rw-r--r--   0        0        0     4527 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/browser.js
--rw-r--r--   0        0        0     1291 2023-05-03 12:35:22.828347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncNullishCoalesce.js
--rw-r--r--   0        0        0     2210 2023-05-03 12:35:22.848348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChain.js
--rw-r--r--   0        0        0     1749 2023-05-03 12:35:22.872350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChainDelete.js
--rw-r--r--   0        0        0      824 2023-05-03 12:35:22.880351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createNamedExportFrom.js
--rw-r--r--   0        0        0      882 2023-05-03 12:35:22.888351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createStarExport.js
--rw-r--r--   0        0        0      660 2023-05-03 12:35:22.900352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopDefault.js
--rw-r--r--   0        0        0     1002 2023-05-03 12:35:22.908353 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespace.js
--rw-r--r--   0        0        0      743 2023-05-03 12:35:22.920354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespaceDefaultOnly.js
--rw-r--r--   0        0        0      773 2023-05-03 12:35:22.924354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireDefault.js
--rw-r--r--   0        0        0     1100 2023-05-03 12:35:22.928354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireWildcard.js
--rw-r--r--   0        0        0     2325 2023-05-03 12:35:22.932355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_nullishCoalesce.js
--rw-r--r--   0        0        0     2078 2023-05-03 12:35:22.940355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChain.js
--rw-r--r--   0        0        0     1752 2023-05-03 12:35:22.944355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChainDelete.js
--rw-r--r--   0        0        0     1941 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/index.js
--rw-r--r--   0        0        0      727 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/clientreport.js
--rw-r--r--   0        0        0     3180 2023-05-03 12:35:22.976358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/dsn.js
--rw-r--r--   0        0        0     1613 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/env.js
--rw-r--r--   0        0        0     6945 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/envelope.js
--rw-r--r--   0        0        0      819 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/error.js
--rw-r--r--   0        0        0     8328 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/index.js
--rw-r--r--   0        0        0    18001 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/instrument.js
--rw-r--r--   0        0        0     4878 2023-05-03 12:35:23.040362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/is.js
--rw-r--r--   0        0        0     2403 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/logger.js
--rw-r--r--   0        0        0     1096 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/memo.js
--rw-r--r--   0        0        0     7809 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/misc.js
--rw-r--r--   0        0        0     2703 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/node-stack-trace.js
--rw-r--r--   0        0        0     2267 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/node.js
--rw-r--r--   0        0        0     9477 2023-05-03 12:35:23.060364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/normalize.js
--rw-r--r--   0        0        0     9449 2023-05-03 12:35:23.064364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/object.js
--rw-r--r--   0        0        0     5629 2023-05-03 12:35:23.068364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/path.js
--rw-r--r--   0        0        0     3592 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/promisebuffer.js
--rw-r--r--   0        0        0     3349 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/ratelimit.js
--rw-r--r--   0        0        0     9445 2023-05-03 12:35:23.076365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/requestdata.js
--rw-r--r--   0        0        0     1725 2023-05-03 12:35:23.080366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/severity.js
--rw-r--r--   0        0        0     4558 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/stacktrace.js
--rw-r--r--   0        0        0     3764 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/string.js
--rw-r--r--   0        0        0     4591 2023-05-03 12:35:23.088366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/supports.js
--rw-r--r--   0        0        0     4495 2023-05-03 12:35:23.088366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/syncpromise.js
--rw-r--r--   0        0        0     7759 2023-05-03 12:35:23.092366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/time.js
--rw-r--r--   0        0        0     1094 2023-05-03 12:35:23.092366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/tracing.js
--rw-r--r--   0        0        0     1632 2023-05-03 12:35:23.096367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/url.js
--rw-r--r--   0        0        0     3919 2023-05-03 12:35:23.096367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/userIntegrations.js
--rw-r--r--   0        0        0     2198 2023-05-03 12:35:23.008360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/vendor/escapeStringForRegex.js
--rw-r--r--   0        0        0     1235 2023-05-03 12:35:23.088366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/vendor/supportsHistory.js
--rw-r--r--   0        0        0     3202 2023-05-03 12:35:23.100367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/worldwide.js
--rw-r--r--   0        0        0     5598 2023-05-03 12:35:22.956356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/baggage.js
--rw-r--r--   0        0        0     4394 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/browser.js
--rw-r--r--   0        0        0     1188 2023-05-03 12:35:22.844348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncNullishCoalesce.js
--rw-r--r--   0        0        0     2127 2023-05-03 12:35:22.860349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChain.js
--rw-r--r--   0        0        0     1639 2023-05-03 12:35:22.880351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChainDelete.js
--rw-r--r--   0        0        0      738 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createNamedExportFrom.js
--rw-r--r--   0        0        0      801 2023-05-03 12:35:22.896352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createStarExport.js
--rw-r--r--   0        0        0      577 2023-05-03 12:35:22.904352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopDefault.js
--rw-r--r--   0        0        0      917 2023-05-03 12:35:22.912353 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespace.js
--rw-r--r--   0        0        0      647 2023-05-03 12:35:22.924354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespaceDefaultOnly.js
--rw-r--r--   0        0        0      687 2023-05-03 12:35:22.924354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireDefault.js
--rw-r--r--   0        0        0     1013 2023-05-03 12:35:22.928354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireWildcard.js
--rw-r--r--   0        0        0     2245 2023-05-03 12:35:22.936355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_nullishCoalesce.js
--rw-r--r--   0        0        0     2000 2023-05-03 12:35:22.940355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChain.js
--rw-r--r--   0        0        0     1652 2023-05-03 12:35:22.944355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChainDelete.js
--rw-r--r--   0        0        0      890 2023-05-03 12:35:23.020361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/index.js
--rw-r--r--   0        0        0      645 2023-05-03 12:35:22.976358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/clientreport.js
--rw-r--r--   0        0        0     3038 2023-05-03 12:35:22.980358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/dsn.js
--rw-r--r--   0        0        0     1511 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/env.js
--rw-r--r--   0        0        0     6547 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/envelope.js
--rw-r--r--   0        0        0      744 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/error.js
--rw-r--r--   0        0        0     3382 2023-05-03 12:35:23.024361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/index.js
--rw-r--r--   0        0        0    17819 2023-05-03 12:35:23.036362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/instrument.js
--rw-r--r--   0        0        0     4529 2023-05-03 12:35:23.040362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/is.js
--rw-r--r--   0        0        0     2259 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/logger.js
--rw-r--r--   0        0        0     1021 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/memo.js
--rw-r--r--   0        0        0     7523 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/misc.js
--rw-r--r--   0        0        0     2635 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/node-stack-trace.js
--rw-r--r--   0        0        0     2155 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/node.js
--rw-r--r--   0        0        0     9377 2023-05-03 12:35:23.060364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/normalize.js
--rw-r--r--   0        0        0     9181 2023-05-03 12:35:23.064364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/object.js
--rw-r--r--   0        0        0     5442 2023-05-03 12:35:23.068364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/path.js
--rw-r--r--   0        0        0     3515 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/promisebuffer.js
--rw-r--r--   0        0        0     3159 2023-05-03 12:35:23.076365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/ratelimit.js
--rw-r--r--   0        0        0     9276 2023-05-03 12:35:23.076365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/requestdata.js
--rw-r--r--   0        0        0     1579 2023-05-03 12:35:23.080366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/severity.js
--rw-r--r--   0        0        0     4313 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/stacktrace.js
--rw-r--r--   0        0        0     3597 2023-05-03 12:35:23.084366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/string.js
--rw-r--r--   0        0        0     4291 2023-05-03 12:35:23.088366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/supports.js
--rw-r--r--   0        0        0     4364 2023-05-03 12:35:23.092366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/syncpromise.js
--rw-r--r--   0        0        0     7544 2023-05-03 12:35:23.092366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/time.js
--rw-r--r--   0        0        0      979 2023-05-03 12:35:23.096367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/tracing.js
--rw-r--r--   0        0        0     1492 2023-05-03 12:35:23.096367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/url.js
--rw-r--r--   0        0        0     3833 2023-05-03 12:35:23.100367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/userIntegrations.js
--rw-r--r--   0        0        0     2114 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/vendor/escapeStringForRegex.js
--rw-r--r--   0        0        0     1151 2023-05-03 12:35:23.088366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/vendor/supportsHistory.js
--rw-r--r--   0        0        0     3073 2023-05-03 12:35:23.100367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/worldwide.js
--rw-r--r--   0        0        0      943 2023-05-03 12:35:22.804345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/node_modules/tslib/modules/index.js
--rw-r--r--   0        0        0       26 2023-05-03 12:35:22.868350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      915 2023-05-03 12:35:22.872350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/node_modules/tslib/package.json
--rw-r--r--   0        0        0      824 2023-05-03 12:35:22.828347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
--rw-r--r--   0        0        0       71 2023-05-03 12:35:22.876350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0    10274 2023-05-03 12:35:22.844348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/node_modules/tslib/tslib.es6.js
--rw-r--r--   0        0        0    13204 2023-05-03 12:35:22.856349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/node_modules/tslib/tslib.js
--rw-r--r--   0        0        0      720 2023-05-03 12:35:23.100367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/package.json
--rw-r--r--   0        0        0     1549 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/backgroundtab.js
--rw-r--r--   0        0        0     9662 2023-05-03 12:35:22.940355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/browsertracing.js
--rw-r--r--   0        0        0    16045 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/index.js
--rw-r--r--   0        0        0      839 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/utils.js
--rw-r--r--   0        0        0     9245 2023-05-03 12:35:23.064364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/request.js
--rw-r--r--   0        0        0     2510 2023-05-03 12:35:23.068364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/router.js
--rw-r--r--   0        0        0      199 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/types.js
--rw-r--r--   0        0        0     3902 2023-05-03 12:35:22.980358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getCLS.js
--rw-r--r--   0        0        0     2257 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getFID.js
--rw-r--r--   0        0        0     3094 2023-05-03 12:35:22.996359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getLCP.js
--rw-r--r--   0        0        0      843 2023-05-03 12:35:22.920354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/bindReporter.js
--rw-r--r--   0        0        0     1031 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/generateUniqueID.js
--rw-r--r--   0        0        0      973 2023-05-03 12:35:22.968357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getActivationStart.js
--rw-r--r--   0        0        0     1851 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getNavigationEntry.js
--rw-r--r--   0        0        0     1795 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getVisibilityWatcher.js
--rw-r--r--   0        0        0     1563 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/initMetric.js
--rw-r--r--   0        0        0      943 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/observe.js
--rw-r--r--   0        0        0     1379 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/onHidden.js
--rw-r--r--   0        0        0     1753 2023-05-03 12:35:22.952356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/extensions.js
--rw-r--r--   0        0        0     2074 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/index.js
--rw-r--r--   0        0        0     5368 2023-05-03 12:35:22.840348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/apollo.js
--rw-r--r--   0        0        0    12006 2023-05-03 12:35:22.948356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/express.js
--rw-r--r--   0        0        0     2405 2023-05-03 12:35:23.008360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/graphql.js
--rw-r--r--   0        0        0     1184 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/lazy.js
--rw-r--r--   0        0        0     9496 2023-05-03 12:35:23.036362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mongo.js
--rw-r--r--   0        0        0     2580 2023-05-03 12:35:23.040362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mysql.js
--rw-r--r--   0        0        0     3387 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/postgres.js
--rw-r--r--   0        0        0     2441 2023-05-03 12:35:23.060364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/prisma.js
--rw-r--r--   0        0        0      793 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/utils/node-utils.js
--rw-r--r--   0        0        0     1429 2023-05-03 12:35:22.904352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/backgroundtab.js
--rw-r--r--   0        0        0     9706 2023-05-03 12:35:22.940355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/browsertracing.js
--rw-r--r--   0        0        0    15585 2023-05-03 12:35:23.024361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/index.js
--rw-r--r--   0        0        0      735 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/utils.js
--rw-r--r--   0        0        0     9060 2023-05-03 12:35:23.064364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/request.js
--rw-r--r--   0        0        0     2420 2023-05-03 12:35:23.068364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/router.js
--rw-r--r--   0        0        0      127 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/types.js
--rw-r--r--   0        0        0     3788 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getCLS.js
--rw-r--r--   0        0        0     2121 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getFID.js
--rw-r--r--   0        0        0     2938 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getLCP.js
--rw-r--r--   0        0        0      767 2023-05-03 12:35:22.928354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/bindReporter.js
--rw-r--r--   0        0        0      951 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/generateUniqueID.js
--rw-r--r--   0        0        0      871 2023-05-03 12:35:22.976358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getActivationStart.js
--rw-r--r--   0        0        0     1739 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getNavigationEntry.js
--rw-r--r--   0        0        0     1689 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getVisibilityWatcher.js
--rw-r--r--   0        0        0     1425 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/initMetric.js
--rw-r--r--   0        0        0      872 2023-05-03 12:35:23.052363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/observe.js
--rw-r--r--   0        0        0     1301 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/onHidden.js
--rw-r--r--   0        0        0     1686 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/extensions.js
--rw-r--r--   0        0        0     1047 2023-05-03 12:35:23.024361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/index.js
--rw-r--r--   0        0        0     5248 2023-05-03 12:35:22.868350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/apollo.js
--rw-r--r--   0        0        0    11942 2023-05-03 12:35:22.948356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/express.js
--rw-r--r--   0        0        0     2340 2023-05-03 12:35:23.008360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/graphql.js
--rw-r--r--   0        0        0     1039 2023-05-03 12:35:23.036362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/lazy.js
--rw-r--r--   0        0        0     9433 2023-05-03 12:35:23.040362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mongo.js
--rw-r--r--   0        0        0     2511 2023-05-03 12:35:23.044363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mysql.js
--rw-r--r--   0        0        0     3315 2023-05-03 12:35:23.056364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/postgres.js
--rw-r--r--   0        0        0     2365 2023-05-03 12:35:23.060364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js
--rw-r--r--   0        0        0      693 2023-05-03 12:35:23.048363 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js
--rw-r--r--   0        0        0      943 2023-05-03 12:35:22.816346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/node_modules/tslib/modules/index.js
--rw-r--r--   0        0        0       26 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      915 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/node_modules/tslib/package.json
--rw-r--r--   0        0        0      824 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
--rw-r--r--   0        0        0       71 2023-05-03 12:35:22.888351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0    10274 2023-05-03 12:35:22.852348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/node_modules/tslib/tslib.es6.js
--rw-r--r--   0        0        0    13204 2023-05-03 12:35:22.872350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/node_modules/tslib/tslib.js
--rw-r--r--   0        0        0      699 2023-05-03 12:35:23.072365 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/package.json
--rw-r--r--   0        0        0     7910 2023-05-03 12:35:22.804345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/agent-base/dist/src/index.js
--rw-r--r--   0        0        0      495 2023-05-03 12:35:22.824346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/agent-base/dist/src/promisify.js
--rw-r--r--   0        0        0     1635 2023-05-03 12:35:22.828347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/agent-base/package.json
--rw-r--r--   0        0        0       27 2023-05-03 12:35:22.816346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/.eslintrc.json
--rw-r--r--   0        0        0       60 2023-05-03 12:35:22.824346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/.npmpackagejsonlintrc.json
--rw-r--r--   0        0        0       50 2023-05-03 12:35:22.828347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/.releaserc.json
--rw-r--r--   0        0        0      539 2023-05-03 12:35:22.744341 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/build/lib/boolean.js
--rw-r--r--   0        0        0      463 2023-05-03 12:35:22.784344 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/build/lib/index.js
--rw-r--r--   0        0        0      646 2023-05-03 12:35:22.804345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/build/lib/isBooleanable.js
--rw-r--r--   0        0        0      228 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/licenseCheck.json
--rw-r--r--   0        0        0      982 2023-05-03 12:35:22.840348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/package.json
--rw-r--r--   0        0        0      323 2023-05-03 12:35:22.844348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/tsconfig.json
--rw-r--r--   0        0        0     4047 2023-05-03 12:35:22.728339 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/cookie/index.js
--rw-r--r--   0        0        0     1104 2023-05-03 12:35:22.744341 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/cookie/package.json
--rw-r--r--   0        0        0     1419 2023-05-03 12:35:22.860349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/package.json
--rw-r--r--   0        0        0     6010 2023-05-03 12:35:22.804345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/src/browser.js
--rw-r--r--   0        0        0     6289 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/src/common.js
--rw-r--r--   0        0        0      314 2023-05-03 12:35:22.840348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/src/index.js
--rw-r--r--   0        0        0     4685 2023-05-03 12:35:22.848348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/src/node.js
--rw-r--r--   0        0        0     1429 2023-05-03 12:35:22.804345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/define-properties/index.js
--rw-r--r--   0        0        0     2245 2023-05-03 12:35:22.824346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/define-properties/package.json
--rw-r--r--   0        0        0       25 2023-05-03 12:35:22.728339 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/detect-node/browser.js
--rw-r--r--   0        0        0      184 2023-05-03 12:35:22.744341 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/detect-node/index.esm.js
--rw-r--r--   0        0        0      186 2023-05-03 12:35:22.784344 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/detect-node/index.js
--rw-r--r--   0        0        0      607 2023-05-03 12:35:22.804345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/detect-node/package.json
--rw-r--r--   0        0        0     2582 2023-05-03 12:35:22.828347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/es6-error/es6/index.js
--rw-r--r--   0        0        0     2703 2023-05-03 12:35:22.840348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/es6-error/lib/index.js
--rw-r--r--   0        0        0     1404 2023-05-03 12:35:22.708338 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/es6-error/package.json
--rw-r--r--   0        0        0      461 2023-05-03 12:35:22.708338 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/escape-string-regexp/index.js
--rw-r--r--   0        0        0      686 2023-05-03 12:35:22.728339 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     4140 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/.jscs.json
--rw-r--r--   0        0        0     1463 2023-05-03 12:35:22.784344 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/implementation.js
--rw-r--r--   0        0        0      126 2023-05-03 12:35:22.804345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/index.js
--rw-r--r--   0        0        0     1498 2023-05-03 12:35:22.676335 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/package.json
--rw-r--r--   0        0        0     8991 2023-05-03 12:35:22.844348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/test/index.js
--rw-r--r--   0        0        0    13145 2023-05-03 12:35:22.848348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/get-intrinsic/index.js
--rw-r--r--   0        0        0     2349 2023-05-03 12:35:22.856349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/get-intrinsic/package.json
--rw-r--r--   0        0        0     8767 2023-05-03 12:35:22.824346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/get-intrinsic/test/GetIntrinsic.js
--rw-r--r--   0        0        0       37 2023-05-03 12:35:22.956356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/bootstrap.js
--rw-r--r--   0        0        0      414 2023-05-03 12:35:23.024361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/Logger.js
--rw-r--r--   0        0        0     6510 2023-05-03 12:35:22.940355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/classes/Agent.js
--rw-r--r--   0        0        0      905 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/classes/HttpProxyAgent.js
--rw-r--r--   0        0        0     1542 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/classes/HttpsProxyAgent.js
--rw-r--r--   0        0        0      814 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/classes/index.js
--rw-r--r--   0        0        0      575 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/errors.js
--rw-r--r--   0        0        0     6002 2023-05-03 12:35:22.976358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/factories/createGlobalProxyAgent.js
--rw-r--r--   0        0        0     1086 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/factories/createProxyController.js
--rw-r--r--   0        0        0      694 2023-05-03 12:35:23.008360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/factories/index.js
--rw-r--r--   0        0        0      476 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/index.js
--rw-r--r--   0        0        0      759 2023-05-03 12:35:22.956356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/routines/bootstrap.js
--rw-r--r--   0        0        0      402 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/routines/index.js
--rw-r--r--   0        0        0      165 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/types.js
--rw-r--r--   0        0        0     1479 2023-05-03 12:35:22.948356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/utilities/bindHttpMethod.js
--rw-r--r--   0        0        0      866 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/utilities/index.js
--rw-r--r--   0        0        0     1341 2023-05-03 12:35:23.020361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/utilities/isUrlMatchingNoProxy.js
--rw-r--r--   0        0        0     1065 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/utilities/parseProxyUrl.js
--rw-r--r--   0        0        0     2585 2023-05-03 12:35:23.036362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/package.json
--rw-r--r--   0        0        0      129 2023-05-03 12:35:23.024361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/Logger.js
--rw-r--r--   0        0        0     6762 2023-05-03 12:35:22.948356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/classes/Agent.js
--rw-r--r--   0        0        0      733 2023-05-03 12:35:23.000360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/classes/HttpProxyAgent.js
--rw-r--r--   0        0        0     1346 2023-05-03 12:35:23.004360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/classes/HttpsProxyAgent.js
--rw-r--r--   0        0        0      174 2023-05-03 12:35:23.012360 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/classes/index.js
--rw-r--r--   0        0        0      299 2023-05-03 12:35:22.996359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/errors.js
--rw-r--r--   0        0        0     5715 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/factories/createGlobalProxyAgent.js
--rw-r--r--   0        0        0      882 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/factories/createProxyController.js
--rw-r--r--   0        0        0      160 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/factories/index.js
--rw-r--r--   0        0        0      100 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/index.js
--rw-r--r--   0        0        0      550 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/routines/bootstrap.js
--rw-r--r--   0        0        0       60 2023-05-03 12:35:23.016361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/routines/index.js
--rw-r--r--   0        0        0     1567 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/types.js
--rw-r--r--   0        0        0     1197 2023-05-03 12:35:22.956356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/utilities/bindHttpMethod.js
--rw-r--r--   0        0        0      200 2023-05-03 12:35:23.020361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/utilities/index.js
--rw-r--r--   0        0        0     1022 2023-05-03 12:35:23.020361 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/utilities/isUrlMatchingNoProxy.js
--rw-r--r--   0        0        0      874 2023-05-03 12:35:23.032362 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/utilities/parseProxyUrl.js
--rw-r--r--   0        0        0       36 2023-05-03 12:35:22.740340 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/auto.js
--rw-r--r--   0        0        0      254 2023-05-03 12:35:22.784344 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/implementation.browser.js
--rw-r--r--   0        0        0       40 2023-05-03 12:35:22.800345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/implementation.js
--rw-r--r--   0        0        0      408 2023-05-03 12:35:22.828347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/index.js
--rw-r--r--   0        0        0     2418 2023-05-03 12:35:22.876350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/package.json
--rw-r--r--   0        0        0      251 2023-05-03 12:35:22.844348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/polyfill.js
--rw-r--r--   0        0        0      722 2023-05-03 12:35:22.848348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/shim.js
--rw-r--r--   0        0        0      213 2023-05-03 12:35:22.824346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/test/implementation.js
--rw-r--r--   0        0        0      196 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/test/index.js
--rw-r--r--   0        0        0      767 2023-05-03 12:35:22.840348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/test/native.js
--rw-r--r--   0        0        0      900 2023-05-03 12:35:22.852348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/test/shimmed.js
--rw-r--r--   0        0        0     1399 2023-05-03 12:35:22.864349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/test/tests.js
--rw-r--r--   0        0        0     1011 2023-05-03 12:35:22.676335 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has/package.json
--rw-r--r--   0        0        0      129 2023-05-03 12:35:22.816346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has/src/index.js
--rw-r--r--   0        0        0      331 2023-05-03 12:35:22.828347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has/test/index.js
--rw-r--r--   0        0        0      817 2023-05-03 12:35:22.800345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-property-descriptors/index.js
--rw-r--r--   0        0        0     1933 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-property-descriptors/package.json
--rw-r--r--   0        0        0     1405 2023-05-03 12:35:22.820346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-property-descriptors/test/index.js
--rw-r--r--   0        0        0      420 2023-05-03 12:35:22.820346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/index.js
--rw-r--r--   0        0        0     2648 2023-05-03 12:35:22.852348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/package.json
--rw-r--r--   0        0        0     1761 2023-05-03 12:35:22.844348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/shams.js
--rw-r--r--   0        0        0      654 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/test/index.js
--rw-r--r--   0        0        0      723 2023-05-03 12:35:22.772343 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/test/shams/core-js.js
--rw-r--r--   0        0        0      686 2023-05-03 12:35:22.812346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/test/shams/get-own-property-symbols.js
--rw-r--r--   0        0        0     2021 2023-05-03 12:35:22.848348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/test/tests.js
--rw-r--r--   0        0        0     7841 2023-05-03 12:35:22.724339 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/https-proxy-agent/dist/agent.js
--rw-r--r--   0        0        0      579 2023-05-03 12:35:22.740340 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/https-proxy-agent/dist/index.js
--rw-r--r--   0        0        0     2460 2023-05-03 12:35:22.784344 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/https-proxy-agent/dist/parse-proxy-response.js
--rw-r--r--   0        0        0     1405 2023-05-03 12:35:22.816346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/https-proxy-agent/package.json
--rw-r--r--   0        0        0      796 2023-05-03 12:35:22.620331 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/json-stringify-safe/package.json
--rw-r--r--   0        0        0      907 2023-05-03 12:35:22.772343 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/json-stringify-safe/stringify.js
--rw-r--r--   0        0        0     7550 2023-05-03 12:35:22.840348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/json-stringify-safe/test/stringify_test.js
--rw-r--r--   0        0        0     8186 2023-05-03 12:35:22.672335 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru-cache/index.js
--rw-r--r--   0        0        0      705 2023-05-03 12:35:22.724339 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru-cache/package.json
--rw-r--r--   0        0        0     4625 2023-05-03 12:35:22.800345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/benchmark.js
--rw-r--r--   0        0        0     7934 2023-05-03 12:35:22.832347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/lru.js
--rw-r--r--   0        0        0      901 2023-05-03 12:35:22.652334 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/package.json
--rw-r--r--   0        0        0     7366 2023-05-03 12:35:22.844348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/test.js
--rw-r--r--   0        0        0      227 2023-05-03 12:35:22.876350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/tsconfig.json
--rw-r--r--   0        0        0     1785 2023-05-03 12:35:22.620331 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/matcher/index.js
--rw-r--r--   0        0        0      871 2023-05-03 12:35:22.648333 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/matcher/package.json
--rw-r--r--   0        0        0     3023 2023-05-03 12:35:22.672335 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/ms/index.js
--rw-r--r--   0        0        0      705 2023-05-03 12:35:22.620331 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/ms/package.json
--rw-r--r--   0        0        0     3218 2023-05-03 12:35:22.812346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/object-keys/implementation.js
--rw-r--r--   0        0        0      823 2023-05-03 12:35:22.820346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/object-keys/index.js
--rw-r--r--   0        0        0      422 2023-05-03 12:35:22.824346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/object-keys/isArguments.js
--rw-r--r--   0        0        0     1903 2023-05-03 12:35:22.652334 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/object-keys/package.json
--rw-r--r--   0        0        0       61 2023-05-03 12:35:22.848348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/object-keys/test/index.js
--rw-r--r--   0        0        0      274 2023-05-03 12:35:22.864349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/constants.js
--rw-r--r--   0        0        0     6377 2023-05-03 12:35:22.868350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/createLogger.js
--rw-r--r--   0        0        0     1103 2023-05-03 12:35:22.876350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/createMockLogger.js
--rw-r--r--   0        0        0      629 2023-05-03 12:35:22.880351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/createNodeWriter.js
--rw-r--r--   0        0        0     2493 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/createRoarrInititialGlobalState.js
--rw-r--r--   0        0        0      914 2023-05-03 12:35:22.888351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/index.js
--rw-r--r--   0        0        0     1186 2023-05-03 12:35:22.892351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/log.js
--rw-r--r--   0        0        0       47 2023-05-03 12:35:22.896352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/types.js
--rw-r--r--   0        0        0     2350 2023-05-03 12:35:22.904352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/package.json
--rwxr-xr-x   0        0        0     4426 2023-05-03 12:35:22.956356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/bin/semver.js
--rw-r--r--   0        0        0     3610 2023-05-03 12:35:22.772343 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/classes/comparator.js
--rw-r--r--   0        0        0      129 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/classes/index.js
--rw-r--r--   0        0        0    14139 2023-05-03 12:35:22.944355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/classes/range.js
--rw-r--r--   0        0        0     8008 2023-05-03 12:35:22.964357 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/classes/semver.js
--rw-r--r--   0        0        0      191 2023-05-03 12:35:22.672335 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/clean.js
--rw-r--r--   0        0        0      947 2023-05-03 12:35:22.700337 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/cmp.js
--rw-r--r--   0        0        0     1505 2023-05-03 12:35:22.720339 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/coerce.js
--rw-r--r--   0        0        0      267 2023-05-03 12:35:22.800345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/compare-build.js
--rw-r--r--   0        0        0      118 2023-05-03 12:35:22.812346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/compare-loose.js
--rw-r--r--   0        0        0      156 2023-05-03 12:35:22.820346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/compare.js
--rw-r--r--   0        0        0      634 2023-05-03 12:35:22.840348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/diff.js
--rw-r--r--   0        0        0      112 2023-05-03 12:35:22.848348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/eq.js
--rw-r--r--   0        0        0      110 2023-05-03 12:35:22.852348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/gt.js
--rw-r--r--   0        0        0      113 2023-05-03 12:35:22.856349 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/gte.js
--rw-r--r--   0        0        0      400 2023-05-03 12:35:22.880351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/inc.js
--rw-r--r--   0        0        0      110 2023-05-03 12:35:22.896352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/lt.js
--rw-r--r--   0        0        0      113 2023-05-03 12:35:22.900352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/lte.js
--rw-r--r--   0        0        0      122 2023-05-03 12:35:22.908353 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/major.js
--rw-r--r--   0        0        0      122 2023-05-03 12:35:22.920354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/minor.js
--rw-r--r--   0        0        0      114 2023-05-03 12:35:22.924354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/neq.js
--rw-r--r--   0        0        0      662 2023-05-03 12:35:22.928354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/parse.js
--rw-r--r--   0        0        0      122 2023-05-03 12:35:22.928354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/patch.js
--rw-r--r--   0        0        0      220 2023-05-03 12:35:22.936355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/prerelease.js
--rw-r--r--   0        0        0      118 2023-05-03 12:35:22.944355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/rcompare.js
--rw-r--r--   0        0        0      149 2023-05-03 12:35:22.952356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/rsort.js
--rw-r--r--   0        0        0      233 2023-05-03 12:35:22.952356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/satisfies.js
--rw-r--r--   0        0        0      147 2023-05-03 12:35:22.980358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/sort.js
--rw-r--r--   0        0        0      162 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/valid.js
--rw-r--r--   0        0        0     2574 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/index.js
--rw-r--r--   0        0        0      467 2023-05-03 12:35:22.832347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/internal/constants.js
--rw-r--r--   0        0        0      226 2023-05-03 12:35:22.836347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/internal/debug.js
--rw-r--r--   0        0        0      410 2023-05-03 12:35:22.876350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/internal/identifiers.js
--rw-r--r--   0        0        0      383 2023-05-03 12:35:22.924354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/internal/parse-options.js
--rw-r--r--   0        0        0     6672 2023-05-03 12:35:22.948356 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/internal/re.js
--rw-r--r--   0        0        0     1731 2023-05-03 12:35:22.992359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/package.json
--rw-r--r--   0        0        0       69 2023-05-03 12:35:22.932355 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/preload.js
--rw-r--r--   0        0        0      217 2023-05-03 12:35:22.868350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/gtr.js
--rw-r--r--   0        0        0      201 2023-05-03 12:35:22.892351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/intersects.js
--rw-r--r--   0        0        0      213 2023-05-03 12:35:22.904352 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/ltr.js
--rw-r--r--   0        0        0      579 2023-05-03 12:35:22.908353 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/max-satisfying.js
--rw-r--r--   0        0        0      577 2023-05-03 12:35:22.912353 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/min-satisfying.js
--rw-r--r--   0        0        0     1500 2023-05-03 12:35:22.920354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/min-version.js
--rw-r--r--   0        0        0     2190 2023-05-03 12:35:22.924354 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/outside.js
--rw-r--r--   0        0        0     1341 2023-05-03 12:35:22.976358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/simplify.js
--rw-r--r--   0        0        0     7418 2023-05-03 12:35:22.980358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/subset.js
--rw-r--r--   0        0        0      268 2023-05-03 12:35:22.984358 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/to-comparators.js
--rw-r--r--   0        0        0      312 2023-05-03 12:35:22.988359 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/valid.js
--rw-r--r--   0        0        0      210 2023-05-03 12:35:22.800345 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver-compare/example/cmp.js
--rw-r--r--   0        0        0      181 2023-05-03 12:35:22.812346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver-compare/example/lex.js
--rw-r--r--   0        0        0      372 2023-05-03 12:35:22.724339 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver-compare/index.js
--rw-r--r--   0        0        0      659 2023-05-03 12:35:22.620331 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver-compare/package.json
--rw-r--r--   0        0        0      444 2023-05-03 12:35:22.832347 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver-compare/test/cmp.js
--rw-r--r--   0        0        0     2235 2023-05-03 12:35:22.652334 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/serialize-error/index.js
--rw-r--r--   0        0        0      743 2023-05-03 12:35:22.672335 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/serialize-error/package.json
--rwxr-xr-x   0        0        0       57 2023-05-03 12:35:22.892351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/bin/snyk
--rw-r--r--   0        0        0      150 2023-05-03 12:35:23.456393 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/config.default.json
--rw-r--r--   0        0        0     1838 2023-05-03 12:35:23.068364 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/110.index.js
--rw-r--r--   0        0        0   103302 2023-05-03 12:35:23.088366 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/213.index.js
--rw-r--r--   0        0        0   133844 2023-05-03 12:35:23.096367 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/31.index.js
--rw-r--r--   0        0        0   173511 2023-05-03 12:35:23.116368 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/38.index.js
--rw-r--r--   0        0        0   161488 2023-05-03 12:35:23.128369 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/384.index.js
--rw-r--r--   0        0        0   128289 2023-05-03 12:35:23.144370 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/395.index.js
--rw-r--r--   0        0        0     2969 2023-05-03 12:35:23.144370 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/477.index.js
--rw-r--r--   0        0        0   557584 2023-05-03 12:35:23.184373 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/503.index.js
--rw-r--r--   0        0        0    22931 2023-05-03 12:35:23.184373 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/519.index.js
--rw-r--r--   0        0        0      612 2023-05-03 12:35:23.188373 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/522.index.js
--rw-r--r--   0        0        0   569531 2023-05-03 12:35:23.224376 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/535.index.js
--rw-r--r--   0        0        0     7242 2023-05-03 12:35:23.224376 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/542.index.js
--rw-r--r--   0        0        0     1061 2023-05-03 12:35:23.224376 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/575.index.js
--rw-r--r--   0        0        0    32497 2023-05-03 12:35:23.228376 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/663.index.js
--rw-r--r--   0        0        0    18697 2023-05-03 12:35:23.228376 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/726.index.js
--rw-r--r--   0        0        0   106008 2023-05-03 12:35:23.240377 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/741.index.js
--rw-r--r--   0        0        0   280086 2023-05-03 12:35:23.260379 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/784.index.js
--rw-r--r--   0        0        0   265629 2023-05-03 12:35:23.276380 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/790.index.js
--rw-r--r--   0        0        0     3295 2023-05-03 12:35:23.276380 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/831.index.js
--rw-r--r--   0        0        0    11175 2023-05-03 12:35:23.284381 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/85.index.js
--rw-r--r--   0        0        0     1445 2023-05-03 12:35:23.288381 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/855.index.js
--rw-r--r--   0        0        0      523 2023-05-03 12:35:23.288381 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/875.index.js
--rw-r--r--   0        0        0   267291 2023-05-03 12:35:23.292381 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/895.index.js
--rw-r--r--   0        0        0   227159 2023-05-03 12:35:23.296382 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/905.index.js
--rw-r--r--   0        0        0  4489688 2023-05-03 12:35:23.348385 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/917.index.js
--rw-r--r--   0        0        0  8653273 2023-05-03 12:35:23.428391 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/95.index.js
--rw-r--r--   0        0        0      592 2023-05-03 12:35:23.428391 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/959.index.js
--rw-r--r--   0        0        0    93818 2023-05-03 12:35:23.432392 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/970.index.js
--rw-r--r--   0        0        0    20674 2023-05-03 12:35:23.432392 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/974.index.js
--rw-r--r--   0        0        0    14335 2023-05-03 12:35:23.432392 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/989.index.js
--rw-r--r--   0        0        0  1682422 2023-05-03 12:35:23.452393 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/index.js
--rw-r--r--   0        0        0   613426 2023-05-03 12:35:23.792418 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/sql-wasm.wasm
--rw-r--r--   0        0        0   614892 2023-05-03 12:35:23.460394 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/thirdPartyNotice.json
--rw-r--r--   0        0        0      140 2023-05-03 12:35:23.452393 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/jest.config.js
--rw-r--r--   0        0        0     1094 2023-05-03 12:35:23.456393 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/package.json
--rw-r--r--   0        0        0     1203 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/distPackage.py
--rw-r--r--   0        0        0      844 2023-05-03 12:35:23.676410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/package.py
--rw-r--r--   0        0        0      726 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/__about__.py
--rw-r--r--   0        0        0      562 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/_compat.py
--rw-r--r--   0        0        0     2022 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/_structures.py
--rw-r--r--   0        0        0     1812 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/_typing.py
--rw-r--r--   0        0        0     9460 2023-05-03 12:35:23.676410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/markers.py
--rw-r--r--   0        0        0     5098 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/requirements.py
--rw-r--r--   0        0        0    32208 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/specifiers.py
--rw-r--r--   0        0        0    29561 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/tags.py
--rw-r--r--   0        0        0     4385 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/utils.py
--rw-r--r--   0        0        0    15974 2023-05-03 12:35:23.684410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/version.py
--rw-r--r--   0        0        0    13551 2023-05-03 12:35:23.676410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pip_resolve.py
--rw-r--r--   0        0        0     1788 2023-05-03 12:35:23.676410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pipfile.py
--rw-r--r--   0        0        0   273365 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pyparsing.py
--rw-r--r--   0        0        0       92 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pytoml/__init__.py
--rw-r--r--   0        0        0      509 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pytoml/core.py
--rw-r--r--   0        0        0    11254 2023-05-03 12:35:23.676410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pytoml/parser.py
--rw-r--r--   0        0        0     3815 2023-05-03 12:35:23.684410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pytoml/writer.py
--rw-r--r--   0        0        0     1508 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/reqPackage.py
--rw-r--r--   0        0        0      353 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/requirements/__init__.py
--rw-r--r--   0        0        0     1352 2023-05-03 12:35:23.672409 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/requirements/fragment.py
--rw-r--r--   0        0        0     3092 2023-05-03 12:35:23.676410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/requirements/parser.py
--rw-r--r--   0        0        0    10020 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/requirements/requirement.py
--rw-r--r--   0        0        0      405 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/requirements/vcs.py
--rw-r--r--   0        0        0     1427 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/setup_file.py
--rw-r--r--   0        0        0     6291 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/test_pip_resolve.py
--rw-r--r--   0        0        0     2258 2023-05-03 12:35:23.680410 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/utils.py
--rw-r--r--   0        0        0      246 2023-05-03 12:35:23.456393 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/src/generated/binary-deployments.json
--rw-r--r--   0        0        0      186 2023-05-03 12:35:23.460394 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/tsconfig.json
--rw-r--r--   0        0        0      843 2023-05-03 12:35:23.432392 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/wrapper_dist/bootstrap.js
--rw-r--r--   0        0        0    11438 2023-05-03 12:35:23.432392 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/wrapper_dist/common.js
--rw-r--r--   0        0        0      246 2023-05-03 12:35:23.456393 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/wrapper_dist/generated/binary-deployments.json
--rw-r--r--   0        0        0     2017 2023-05-03 12:35:23.452393 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/wrapper_dist/index.js
--rw-r--r--   0        0        0      498 2023-05-03 12:35:22.824346 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/dist/angular-sprintf.min.js
--rw-r--r--   0        0        0     3675 2023-05-03 12:35:22.844348 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/dist/sprintf.min.js
--rw-r--r--   0        0        0      818 2023-05-03 12:35:22.652334 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/package.json
--rw-r--r--   0        0        0      663 2023-05-03 12:35:22.876350 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/src/angular-sprintf.js
--rw-r--r--   0        0        0     9250 2023-05-03 12:35:22.884351 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/src/sprintf.js
--rw-r--r--   0        0        0      782 2023-05-03 12:35:22.620331 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/type-fest/package.json
--rw-r--r--   0        0        0      207 2023-05-03 12:35:22.616331 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/yallist/iterator.js
--rw-r--r--   0        0        0      652 2023-05-03 12:35:22.720339 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/yallist/package.json
--rw-r--r--   0        0        0     8411 2023-05-03 12:35:22.672335 c2cciutils-1.6.0.dev89/c2cciutils/node_modules/yallist/yallist.js
--rw-r--r--   0        0        0    27102 2023-05-03 12:35:25.276528 c2cciutils-1.6.0.dev89/c2cciutils/package-lock.json
--rw-r--r--   0        0        0      134 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/package.json
--rw-r--r--   0        0        0    10112 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/pr_checks.py
--rw-r--r--   0        0        0    17707 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/publish.py
--rw-r--r--   0        0        0     1548 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/schema-applications.json
--rw-r--r--   0        0        0    22561 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/schema.json
--rw-r--r--   0        0        0       36 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/__init__.py
--rw-r--r--   0        0        0     1104 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/audit.py
--rw-r--r--   0        0        0     3039 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/clean.py
--rw-r--r--   0        0        0     1712 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/docker_logs.py
--rw-r--r--   0        0        0     1316 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/docker_versions_gen.py
--rw-r--r--   0        0        0     4385 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/download_applications.py
--rw-r--r--   0        0        0      375 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/env.py
--rw-r--r--   0        0        0       69 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/__init__.py
--rw-r--r--   0        0        0     3274 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/db.py
--rw-r--r--   0        0        0      921 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/install.py
--rw-r--r--   0        0        0     2655 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/logs.py
--rw-r--r--   0        0        0     5661 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/wait.py
--rw-r--r--   0        0        0     1162 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/main.py
--rw-r--r--   0        0        0     2150 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/pin_pipenv.py
--rw-r--r--   0        0        0     2182 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/pr_checks.py
--rw-r--r--   0        0        0    18016 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/publish.py
--rw-r--r--   0        0        0     2804 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/scripts/trigger_image_update.py
--rw-r--r--   0        0        0     1517 2023-05-03 12:35:09.663336 c2cciutils-1.6.0.dev89/c2cciutils/security.py
--rw-r--r--   0        0        0     4334 2023-05-03 12:41:51.502555 c2cciutils-1.6.0.dev89/pyproject.toml
--rw-r--r--   0        0        0   356964 1970-01-01 00:00:00.000000 c2cciutils-1.6.0.dev89/setup.py
--rw-r--r--   0        0        0    16769 1970-01-01 00:00:00.000000 c2cciutils-1.6.0.dev89/PKG-INFO
+-rw-r--r--   0        0        0     1307 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/LICENSE
+-rw-r--r--   0        0        0    14776 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/README.md
+-rw-r--r--   0        0        0    18066 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/applications-versions.yaml
+-rw-r--r--   0        0        0      283 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/applications.yaml
+-rw-r--r--   0        0        0     1232 2023-05-03 13:43:32.034405 c2cciutils-1.6.0.dev93/c2cciutils/applications_definition.py
+-rw-r--r--   0        0        0     9028 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/audit.py
+-rw-r--r--   0        0        0      358 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/branches.graphql
+-rw-r--r--   0        0        0      308 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/commits.graphql
+-rw-r--r--   0        0        0    22063 2023-05-03 13:43:29.886381 c2cciutils-1.6.0.dev93/c2cciutils/configuration.py
+-rw-r--r--   0        0        0      131 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/default_branch.graphql
+-rw-r--r--   0        0        0     3425 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/env.py
+-rw-r--r--   0        0        0     5485 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/lib/docker.py
+-rw-r--r--   0        0        0    13951 2023-05-03 13:42:52.338002 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/.package-lock.json
+-rw-r--r--   0        0        0     2973 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/api.js
+-rw-r--r--   0        0        0    20649 2023-05-03 13:42:50.285978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/baseclient.js
+-rw-r--r--   0        0        0      196 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/constants.js
+-rw-r--r--   0        0        0     2792 2023-05-03 13:42:50.305978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/envelope.js
+-rw-r--r--   0        0        0     6114 2023-05-03 13:42:50.325978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/exports.js
+-rw-r--r--   0        0        0    14525 2023-05-03 13:42:50.345978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/hub.js
+-rw-r--r--   0        0        0     4225 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/index.js
+-rw-r--r--   0        0        0     4142 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/integration.js
+-rw-r--r--   0        0        0     1305 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/integrations/functiontostring.js
+-rw-r--r--   0        0        0     6540 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/integrations/inboundfilters.js
+-rw-r--r--   0        0        0      333 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/integrations/index.js
+-rw-r--r--   0        0        0    13782 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/scope.js
+-rw-r--r--   0        0        0     1161 2023-05-03 13:42:50.401979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/sdk.js
+-rw-r--r--   0        0        0     5052 2023-05-03 13:42:50.405979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/session.js
+-rw-r--r--   0        0        0     3819 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/sessionflusher.js
+-rw-r--r--   0        0        0     1220 2023-05-03 13:42:50.313978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/errors.js
+-rw-r--r--   0        0        0     8922 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/hubextensions.js
+-rw-r--r--   0        0        0    12257 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/idletransaction.js
+-rw-r--r--   0        0        0     8973 2023-05-03 13:42:50.413979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/span.js
+-rw-r--r--   0        0        0     2669 2023-05-03 13:42:50.417979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/spanstatus.js
+-rw-r--r--   0        0        0     1877 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/trace.js
+-rw-r--r--   0        0        0     7741 2023-05-03 13:42:50.425979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/transaction.js
+-rw-r--r--   0        0        0      623 2023-05-03 13:42:50.429979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/utils.js
+-rw-r--r--   0        0        0     3433 2023-05-03 13:42:50.249977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/transports/base.js
+-rw-r--r--   0        0        0     2021 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/transports/multiplexed.js
+-rw-r--r--   0        0        0     3513 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/transports/offline.js
+-rw-r--r--   0        0        0      796 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js
+-rw-r--r--   0        0        0     8963 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/utils/prepareEvent.js
+-rw-r--r--   0        0        0      166 2023-05-03 13:42:50.433979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/version.js
+-rw-r--r--   0        0        0     2845 2023-05-03 13:42:50.237977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/api.js
+-rw-r--r--   0        0        0    20562 2023-05-03 13:42:50.289978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/baseclient.js
+-rw-r--r--   0        0        0      113 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/constants.js
+-rw-r--r--   0        0        0     2723 2023-05-03 13:42:50.309978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/envelope.js
+-rw-r--r--   0        0        0     5734 2023-05-03 13:42:50.329978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/exports.js
+-rw-r--r--   0        0        0    14180 2023-05-03 13:42:50.345978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/hub.js
+-rw-r--r--   0        0        0     1971 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/index.js
+-rw-r--r--   0        0        0     3983 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/integration.js
+-rw-r--r--   0        0        0     1232 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/integrations/functiontostring.js
+-rw-r--r--   0        0        0     6350 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/integrations/inboundfilters.js
+-rw-r--r--   0        0        0      146 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/integrations/index.js
+-rw-r--r--   0        0        0    13728 2023-05-03 13:42:50.397979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/scope.js
+-rw-r--r--   0        0        0     1079 2023-05-03 13:42:50.401979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/sdk.js
+-rw-r--r--   0        0        0     4938 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/session.js
+-rw-r--r--   0        0        0     3751 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/sessionflusher.js
+-rw-r--r--   0        0        0     1141 2023-05-03 13:42:50.317978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/errors.js
+-rw-r--r--   0        0        0     8723 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/hubextensions.js
+-rw-r--r--   0        0        0    12026 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/idletransaction.js
+-rw-r--r--   0        0        0     8841 2023-05-03 13:42:50.413979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/span.js
+-rw-r--r--   0        0        0     2600 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/spanstatus.js
+-rw-r--r--   0        0        0     1803 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/trace.js
+-rw-r--r--   0        0        0     7640 2023-05-03 13:42:50.429979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/transaction.js
+-rw-r--r--   0        0        0      417 2023-05-03 13:42:50.429979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/utils.js
+-rw-r--r--   0        0        0     3404 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/transports/base.js
+-rw-r--r--   0        0        0     1978 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/transports/multiplexed.js
+-rw-r--r--   0        0        0     3418 2023-05-03 13:42:50.377979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/transports/offline.js
+-rw-r--r--   0        0        0      720 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/utils/hasTracingEnabled.js
+-rw-r--r--   0        0        0     8845 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/utils/prepareEvent.js
+-rw-r--r--   0        0        0       91 2023-05-03 13:42:50.433979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/version.js
+-rw-r--r--   0        0        0      627 2023-05-03 13:42:50.433979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/package.json
+-rw-r--r--   0        0        0     1705 2023-05-03 13:42:50.313978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/async/domain.js
+-rw-r--r--   0        0        0     1318 2023-05-03 13:42:50.341978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/async/hooks.js
+-rw-r--r--   0        0        0      652 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/async/index.js
+-rw-r--r--   0        0        0     5887 2023-05-03 13:42:50.237977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/client.js
+-rw-r--r--   0        0        0     3247 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/eventbuilder.js
+-rw-r--r--   0        0        0    11931 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/handlers.js
+-rw-r--r--   0        0        0     2534 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/index.js
+-rw-r--r--   0        0        0     1462 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/console.js
+-rw-r--r--   0        0        0    11763 2023-05-03 13:42:50.289978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/context.js
+-rw-r--r--   0        0        0     5626 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/contextlines.js
+-rw-r--r--   0        0        0    10377 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/http.js
+-rw-r--r--   0        0        0     1151 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/index.js
+-rw-r--r--   0        0        0     3071 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/linkederrors.js
+-rw-r--r--   0        0        0    12718 2023-05-03 13:42:50.401979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/localvariables.js
+-rw-r--r--   0        0        0     2184 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/modules.js
+-rw-r--r--   0        0        0     6512 2023-05-03 13:42:50.417979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/onuncaughtexception.js
+-rw-r--r--   0        0        0     2505 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/onunhandledrejection.js
+-rw-r--r--   0        0        0     6635 2023-05-03 13:42:50.425979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/requestdata.js
+-rw-r--r--   0        0        0     6064 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/undici/index.js
+-rw-r--r--   0        0        0     1296 2023-05-03 13:42:50.325978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/errorhandling.js
+-rw-r--r--   0        0        0     8752 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/http.js
+-rw-r--r--   0        0        0     1696 2023-05-03 13:42:50.405979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/module.js
+-rw-r--r--   0        0        0      246 2023-05-03 13:42:50.413979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/nodeVersion.js
+-rw-r--r--   0        0        0     1606 2023-05-03 13:42:50.437979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/requestDataDeprecated.js
+-rw-r--r--   0        0        0     8798 2023-05-03 13:42:50.425979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/requestdata.js
+-rw-r--r--   0        0        0     9675 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/sdk.js
+-rw-r--r--   0        0        0     1019 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/tracing/index.js
+-rw-r--r--   0        0        0      396 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/tracing/integrations.js
+-rw-r--r--   0        0        0     4786 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/transports/http.js
+-rw-r--r--   0        0        0     1644 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/utils.js
+-rw-r--r--   0        0        0     1645 2023-05-03 13:42:50.317978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/async/domain.js
+-rw-r--r--   0        0        0     1262 2023-05-03 13:42:50.345978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/async/hooks.js
+-rw-r--r--   0        0        0      568 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/async/index.js
+-rw-r--r--   0        0        0     5836 2023-05-03 13:42:50.249977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/client.js
+-rw-r--r--   0        0        0     3157 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/eventbuilder.js
+-rw-r--r--   0        0        0    11809 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/handlers.js
+-rw-r--r--   0        0        0     1244 2023-05-03 13:42:50.377979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/index.js
+-rw-r--r--   0        0        0     1400 2023-05-03 13:42:50.265977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/console.js
+-rw-r--r--   0        0        0    11588 2023-05-03 13:42:50.293978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/context.js
+-rw-r--r--   0        0        0     5541 2023-05-03 13:42:50.305978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/contextlines.js
+-rw-r--r--   0        0        0    10336 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/http.js
+-rw-r--r--   0        0        0      564 2023-05-03 13:42:50.377979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/index.js
+-rw-r--r--   0        0        0     3001 2023-05-03 13:42:50.397979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/linkederrors.js
+-rw-r--r--   0        0        0    12577 2023-05-03 13:42:50.401979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/localvariables.js
+-rw-r--r--   0        0        0     2122 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/modules.js
+-rw-r--r--   0        0        0     6396 2023-05-03 13:42:50.417979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/onuncaughtexception.js
+-rw-r--r--   0        0        0     2409 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/onunhandledrejection.js
+-rw-r--r--   0        0        0     6570 2023-05-03 13:42:50.429979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/requestdata.js
+-rw-r--r--   0        0        0     6006 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/undici/index.js
+-rw-r--r--   0        0        0     1200 2023-05-03 13:42:50.329978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/errorhandling.js
+-rw-r--r--   0        0        0     8507 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/http.js
+-rw-r--r--   0        0        0     1618 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/module.js
+-rw-r--r--   0        0        0      169 2023-05-03 13:42:50.413979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/nodeVersion.js
+-rw-r--r--   0        0        0     1532 2023-05-03 13:42:50.437979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/requestDataDeprecated.js
+-rw-r--r--   0        0        0     8640 2023-05-03 13:42:50.433979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/requestdata.js
+-rw-r--r--   0        0        0     9353 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/sdk.js
+-rw-r--r--   0        0        0      931 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/tracing/index.js
+-rw-r--r--   0        0        0      142 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/tracing/integrations.js
+-rw-r--r--   0        0        0     4667 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/transports/http.js
+-rw-r--r--   0        0        0     1565 2023-05-03 13:42:50.445979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/utils.js
+-rw-r--r--   0        0        0      994 2023-05-03 13:42:50.445979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/package.json
+-rw-r--r--   0        0        0       35 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/types/cjs/index.js
+-rw-r--r--   0        0        0       35 2023-05-03 13:42:50.241977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/types/esm/index.js
+-rw-r--r--   0        0        0      506 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/types/package.json
+-rw-r--r--   0        0        0     5903 2023-05-03 13:42:50.341978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/baggage.js
+-rw-r--r--   0        0        0     4527 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/browser.js
+-rw-r--r--   0        0        0     1291 2023-05-03 13:42:50.237977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncNullishCoalesce.js
+-rw-r--r--   0        0        0     2210 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChain.js
+-rw-r--r--   0        0        0     1749 2023-05-03 13:42:50.269977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChainDelete.js
+-rw-r--r--   0        0        0      824 2023-05-03 13:42:50.285978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createNamedExportFrom.js
+-rw-r--r--   0        0        0      882 2023-05-03 13:42:50.289978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createStarExport.js
+-rw-r--r--   0        0        0      660 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopDefault.js
+-rw-r--r--   0        0        0     1002 2023-05-03 13:42:50.305978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespace.js
+-rw-r--r--   0        0        0      743 2023-05-03 13:42:50.309978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespaceDefaultOnly.js
+-rw-r--r--   0        0        0      773 2023-05-03 13:42:50.313978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireDefault.js
+-rw-r--r--   0        0        0     1100 2023-05-03 13:42:50.325978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireWildcard.js
+-rw-r--r--   0        0        0     2325 2023-05-03 13:42:50.329978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_nullishCoalesce.js
+-rw-r--r--   0        0        0     2078 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChain.js
+-rw-r--r--   0        0        0     1752 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChainDelete.js
+-rw-r--r--   0        0        0     1941 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/index.js
+-rw-r--r--   0        0        0      727 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/clientreport.js
+-rw-r--r--   0        0        0     3180 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/dsn.js
+-rw-r--r--   0        0        0     1613 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/env.js
+-rw-r--r--   0        0        0     6925 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/envelope.js
+-rw-r--r--   0        0        0      819 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/error.js
+-rw-r--r--   0        0        0     8501 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/index.js
+-rw-r--r--   0        0        0    19360 2023-05-03 13:42:50.397979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/instrument.js
+-rw-r--r--   0        0        0     4878 2023-05-03 13:42:50.405979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/is.js
+-rw-r--r--   0        0        0     2403 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/logger.js
+-rw-r--r--   0        0        0     1096 2023-05-03 13:42:50.413979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/memo.js
+-rw-r--r--   0        0        0     7809 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/misc.js
+-rw-r--r--   0        0        0     2703 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/node-stack-trace.js
+-rw-r--r--   0        0        0     2267 2023-05-03 13:42:50.425979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/node.js
+-rw-r--r--   0        0        0     9677 2023-05-03 13:42:50.433979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/normalize.js
+-rw-r--r--   0        0        0     9449 2023-05-03 13:42:50.437979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/object.js
+-rw-r--r--   0        0        0     5629 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/path.js
+-rw-r--r--   0        0        0     3592 2023-05-03 13:42:50.445979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/promisebuffer.js
+-rw-r--r--   0        0        0     3349 2023-05-03 13:42:50.445979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/ratelimit.js
+-rw-r--r--   0        0        0     9445 2023-05-03 13:42:50.449980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/requestdata.js
+-rw-r--r--   0        0        0     1725 2023-05-03 13:42:50.453980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/severity.js
+-rw-r--r--   0        0        0     4725 2023-05-03 13:42:50.453980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/stacktrace.js
+-rw-r--r--   0        0        0     3764 2023-05-03 13:42:50.457980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/string.js
+-rw-r--r--   0        0        0     4591 2023-05-03 13:42:50.457980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/supports.js
+-rw-r--r--   0        0        0     4495 2023-05-03 13:42:50.461980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/syncpromise.js
+-rw-r--r--   0        0        0     7845 2023-05-03 13:42:50.465980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/time.js
+-rw-r--r--   0        0        0     1094 2023-05-03 13:42:50.465980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/tracing.js
+-rw-r--r--   0        0        0     2341 2023-05-03 13:42:50.465980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/url.js
+-rw-r--r--   0        0        0     3919 2023-05-03 13:42:50.469980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/userIntegrations.js
+-rw-r--r--   0        0        0     2198 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/vendor/escapeStringForRegex.js
+-rw-r--r--   0        0        0     1235 2023-05-03 13:42:50.461980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/vendor/supportsHistory.js
+-rw-r--r--   0        0        0     3202 2023-05-03 13:42:50.473980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/worldwide.js
+-rw-r--r--   0        0        0     5598 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/baggage.js
+-rw-r--r--   0        0        0     4394 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/browser.js
+-rw-r--r--   0        0        0     1188 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncNullishCoalesce.js
+-rw-r--r--   0        0        0     2127 2023-05-03 13:42:50.265977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChain.js
+-rw-r--r--   0        0        0     1639 2023-05-03 13:42:50.277978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChainDelete.js
+-rw-r--r--   0        0        0      738 2023-05-03 13:42:50.289978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createNamedExportFrom.js
+-rw-r--r--   0        0        0      801 2023-05-03 13:42:50.293978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createStarExport.js
+-rw-r--r--   0        0        0      577 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopDefault.js
+-rw-r--r--   0        0        0      917 2023-05-03 13:42:50.305978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespace.js
+-rw-r--r--   0        0        0      647 2023-05-03 13:42:50.309978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespaceDefaultOnly.js
+-rw-r--r--   0        0        0      687 2023-05-03 13:42:50.317978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireDefault.js
+-rw-r--r--   0        0        0     1013 2023-05-03 13:42:50.325978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireWildcard.js
+-rw-r--r--   0        0        0     2245 2023-05-03 13:42:50.329978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_nullishCoalesce.js
+-rw-r--r--   0        0        0     2000 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChain.js
+-rw-r--r--   0        0        0     1652 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChainDelete.js
+-rw-r--r--   0        0        0      890 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/index.js
+-rw-r--r--   0        0        0      645 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/clientreport.js
+-rw-r--r--   0        0        0     3038 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/dsn.js
+-rw-r--r--   0        0        0     1511 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/env.js
+-rw-r--r--   0        0        0     6527 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/envelope.js
+-rw-r--r--   0        0        0      744 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/error.js
+-rw-r--r--   0        0        0     3442 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/index.js
+-rw-r--r--   0        0        0    19108 2023-05-03 13:42:50.401979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/instrument.js
+-rw-r--r--   0        0        0     4529 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/is.js
+-rw-r--r--   0        0        0     2259 2023-05-03 13:42:50.413979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/logger.js
+-rw-r--r--   0        0        0     1021 2023-05-03 13:42:50.417979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/memo.js
+-rw-r--r--   0        0        0     7523 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/misc.js
+-rw-r--r--   0        0        0     2635 2023-05-03 13:42:50.425979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/node-stack-trace.js
+-rw-r--r--   0        0        0     2155 2023-05-03 13:42:50.429979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/node.js
+-rw-r--r--   0        0        0     9577 2023-05-03 13:42:50.433979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/normalize.js
+-rw-r--r--   0        0        0     9181 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/object.js
+-rw-r--r--   0        0        0     5442 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/path.js
+-rw-r--r--   0        0        0     3515 2023-05-03 13:42:50.445979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/promisebuffer.js
+-rw-r--r--   0        0        0     3159 2023-05-03 13:42:50.445979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/ratelimit.js
+-rw-r--r--   0        0        0     9276 2023-05-03 13:42:50.449980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/requestdata.js
+-rw-r--r--   0        0        0     1579 2023-05-03 13:42:50.453980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/severity.js
+-rw-r--r--   0        0        0     4480 2023-05-03 13:42:50.453980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/stacktrace.js
+-rw-r--r--   0        0        0     3597 2023-05-03 13:42:50.457980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/string.js
+-rw-r--r--   0        0        0     4291 2023-05-03 13:42:50.461980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/supports.js
+-rw-r--r--   0        0        0     4364 2023-05-03 13:42:50.461980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/syncpromise.js
+-rw-r--r--   0        0        0     7630 2023-05-03 13:42:50.465980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/time.js
+-rw-r--r--   0        0        0      979 2023-05-03 13:42:50.465980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/tracing.js
+-rw-r--r--   0        0        0     2169 2023-05-03 13:42:50.469980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/url.js
+-rw-r--r--   0        0        0     3833 2023-05-03 13:42:50.469980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/userIntegrations.js
+-rw-r--r--   0        0        0     2114 2023-05-03 13:42:50.377979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/vendor/escapeStringForRegex.js
+-rw-r--r--   0        0        0     1151 2023-05-03 13:42:50.461980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/vendor/supportsHistory.js
+-rw-r--r--   0        0        0     3073 2023-05-03 13:42:50.473980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/worldwide.js
+-rw-r--r--   0        0        0      720 2023-05-03 13:42:50.473980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/package.json
+-rw-r--r--   0        0        0     1549 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/backgroundtab.js
+-rw-r--r--   0        0        0     9662 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/browsertracing.js
+-rw-r--r--   0        0        0    16045 2023-05-03 13:42:50.393979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/index.js
+-rw-r--r--   0        0        0      839 2023-05-03 13:42:50.453980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/utils.js
+-rw-r--r--   0        0        0     9441 2023-05-03 13:42:50.445979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/request.js
+-rw-r--r--   0        0        0     2597 2023-05-03 13:42:50.449980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/router.js
+-rw-r--r--   0        0        0      199 2023-05-03 13:42:50.449980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/types.js
+-rw-r--r--   0        0        0     3902 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getCLS.js
+-rw-r--r--   0        0        0     2257 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getFID.js
+-rw-r--r--   0        0        0     3094 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getLCP.js
+-rw-r--r--   0        0        0      843 2023-05-03 13:42:50.317978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/bindReporter.js
+-rw-r--r--   0        0        0     1031 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/generateUniqueID.js
+-rw-r--r--   0        0        0      973 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getActivationStart.js
+-rw-r--r--   0        0        0     1851 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getNavigationEntry.js
+-rw-r--r--   0        0        0     1795 2023-05-03 13:42:50.377979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getVisibilityWatcher.js
+-rw-r--r--   0        0        0     1563 2023-05-03 13:42:50.405979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/initMetric.js
+-rw-r--r--   0        0        0      943 2023-05-03 13:42:50.433979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/observe.js
+-rw-r--r--   0        0        0     1379 2023-05-03 13:42:50.437979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/onHidden.js
+-rw-r--r--   0        0        0     1735 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/extensions.js
+-rw-r--r--   0        0        0     2157 2023-05-03 13:42:50.397979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/index.js
+-rw-r--r--   0        0        0     5368 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/apollo.js
+-rw-r--r--   0        0        0    12006 2023-05-03 13:42:50.341978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/express.js
+-rw-r--r--   0        0        0     2405 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/graphql.js
+-rw-r--r--   0        0        0     1184 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/lazy.js
+-rw-r--r--   0        0        0     9526 2023-05-03 13:42:50.413979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mongo.js
+-rw-r--r--   0        0        0     2645 2023-05-03 13:42:50.417979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mysql.js
+-rw-r--r--   0        0        0     3457 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/postgres.js
+-rw-r--r--   0        0        0     1883 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/prisma.js
+-rw-r--r--   0        0        0      793 2023-05-03 13:42:50.425979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/utils/node-utils.js
+-rw-r--r--   0        0        0     1429 2023-05-03 13:42:50.309978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/backgroundtab.js
+-rw-r--r--   0        0        0     9706 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/browsertracing.js
+-rw-r--r--   0        0        0    15585 2023-05-03 13:42:50.401979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/index.js
+-rw-r--r--   0        0        0      735 2023-05-03 13:42:50.453980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/utils.js
+-rw-r--r--   0        0        0     9229 2023-05-03 13:42:50.445979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/request.js
+-rw-r--r--   0        0        0     2501 2023-05-03 13:42:50.449980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/router.js
+-rw-r--r--   0        0        0      127 2023-05-03 13:42:50.453980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/types.js
+-rw-r--r--   0        0        0     3788 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getCLS.js
+-rw-r--r--   0        0        0     2121 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getFID.js
+-rw-r--r--   0        0        0     2938 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getLCP.js
+-rw-r--r--   0        0        0      767 2023-05-03 13:42:50.329978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/bindReporter.js
+-rw-r--r--   0        0        0      951 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/generateUniqueID.js
+-rw-r--r--   0        0        0      871 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getActivationStart.js
+-rw-r--r--   0        0        0     1739 2023-05-03 13:42:50.377979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getNavigationEntry.js
+-rw-r--r--   0        0        0     1689 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getVisibilityWatcher.js
+-rw-r--r--   0        0        0     1425 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/initMetric.js
+-rw-r--r--   0        0        0      872 2023-05-03 13:42:50.433979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/observe.js
+-rw-r--r--   0        0        0     1301 2023-05-03 13:42:50.437979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/onHidden.js
+-rw-r--r--   0        0        0     1668 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/extensions.js
+-rw-r--r--   0        0        0     1080 2023-05-03 13:42:50.405979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/index.js
+-rw-r--r--   0        0        0     5248 2023-05-03 13:42:50.285978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/apollo.js
+-rw-r--r--   0        0        0    11942 2023-05-03 13:42:50.341978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/express.js
+-rw-r--r--   0        0        0     2340 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/graphql.js
+-rw-r--r--   0        0        0     1039 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/lazy.js
+-rw-r--r--   0        0        0     9463 2023-05-03 13:42:50.413979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mongo.js
+-rw-r--r--   0        0        0     2576 2023-05-03 13:42:50.421979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mysql.js
+-rw-r--r--   0        0        0     3385 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/postgres.js
+-rw-r--r--   0        0        0     1802 2023-05-03 13:42:50.441980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js
+-rw-r--r--   0        0        0      693 2023-05-03 13:42:50.429979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js
+-rw-r--r--   0        0        0      723 2023-05-03 13:42:50.453980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/package.json
+-rw-r--r--   0        0        0     7910 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/agent-base/dist/src/index.js
+-rw-r--r--   0        0        0      495 2023-05-03 13:42:50.241977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/agent-base/dist/src/promisify.js
+-rw-r--r--   0        0        0     1635 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/agent-base/package.json
+-rw-r--r--   0        0        0       27 2023-05-03 13:42:50.237977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/.eslintrc.json
+-rw-r--r--   0        0        0       60 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/.npmpackagejsonlintrc.json
+-rw-r--r--   0        0        0       50 2023-05-03 13:42:50.249977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/.releaserc.json
+-rw-r--r--   0        0        0      539 2023-05-03 13:42:50.225977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/build/lib/boolean.js
+-rw-r--r--   0        0        0      463 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/build/lib/index.js
+-rw-r--r--   0        0        0      646 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/build/lib/isBooleanable.js
+-rw-r--r--   0        0        0      228 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/licenseCheck.json
+-rw-r--r--   0        0        0      982 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/package.json
+-rw-r--r--   0        0        0      323 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/tsconfig.json
+-rw-r--r--   0        0        0     4047 2023-05-03 13:42:50.193976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/cookie/index.js
+-rw-r--r--   0        0        0     1104 2023-05-03 13:42:50.225977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/cookie/package.json
+-rw-r--r--   0        0        0     1419 2023-05-03 13:42:50.269977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/package.json
+-rw-r--r--   0        0        0     6010 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/src/browser.js
+-rw-r--r--   0        0        0     6289 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/src/common.js
+-rw-r--r--   0        0        0      314 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/src/index.js
+-rw-r--r--   0        0        0     4685 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/src/node.js
+-rw-r--r--   0        0        0     1429 2023-05-03 13:42:50.221977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/define-properties/index.js
+-rw-r--r--   0        0        0     2245 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/define-properties/package.json
+-rw-r--r--   0        0        0       25 2023-05-03 13:42:50.177976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/detect-node/browser.js
+-rw-r--r--   0        0        0      184 2023-05-03 13:42:50.193976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/detect-node/index.esm.js
+-rw-r--r--   0        0        0      186 2023-05-03 13:42:50.221977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/detect-node/index.js
+-rw-r--r--   0        0        0      607 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/detect-node/package.json
+-rw-r--r--   0        0        0     2582 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/es6-error/es6/index.js
+-rw-r--r--   0        0        0     2703 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/es6-error/lib/index.js
+-rw-r--r--   0        0        0     1404 2023-05-03 13:42:50.161976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/es6-error/package.json
+-rw-r--r--   0        0        0      461 2023-05-03 13:42:50.177976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/escape-string-regexp/index.js
+-rw-r--r--   0        0        0      686 2023-05-03 13:42:50.193976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     4140 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/.jscs.json
+-rw-r--r--   0        0        0     1463 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/implementation.js
+-rw-r--r--   0        0        0      126 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/index.js
+-rw-r--r--   0        0        0     1498 2023-05-03 13:42:50.161976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/package.json
+-rw-r--r--   0        0        0     8991 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/test/index.js
+-rw-r--r--   0        0        0    13145 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/get-intrinsic/index.js
+-rw-r--r--   0        0        0     2349 2023-05-03 13:42:50.265977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/get-intrinsic/package.json
+-rw-r--r--   0        0        0     8767 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/get-intrinsic/test/GetIntrinsic.js
+-rw-r--r--   0        0        0       37 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/bootstrap.js
+-rw-r--r--   0        0        0      414 2023-05-03 13:42:50.397979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/Logger.js
+-rw-r--r--   0        0        0     6510 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/classes/Agent.js
+-rw-r--r--   0        0        0      905 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/classes/HttpProxyAgent.js
+-rw-r--r--   0        0        0     1542 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/classes/HttpsProxyAgent.js
+-rw-r--r--   0        0        0      814 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/classes/index.js
+-rw-r--r--   0        0        0      575 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/errors.js
+-rw-r--r--   0        0        0     6002 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/factories/createGlobalProxyAgent.js
+-rw-r--r--   0        0        0     1086 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/factories/createProxyController.js
+-rw-r--r--   0        0        0      694 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/factories/index.js
+-rw-r--r--   0        0        0      476 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/index.js
+-rw-r--r--   0        0        0      759 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/routines/bootstrap.js
+-rw-r--r--   0        0        0      402 2023-05-03 13:42:50.385979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/routines/index.js
+-rw-r--r--   0        0        0      165 2023-05-03 13:42:50.405979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/types.js
+-rw-r--r--   0        0        0     1479 2023-05-03 13:42:50.345978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/utilities/bindHttpMethod.js
+-rw-r--r--   0        0        0      866 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/utilities/index.js
+-rw-r--r--   0        0        0     1341 2023-05-03 13:42:50.397979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/utilities/isUrlMatchingNoProxy.js
+-rw-r--r--   0        0        0     1065 2023-05-03 13:42:50.405979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/utilities/parseProxyUrl.js
+-rw-r--r--   0        0        0     2585 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/package.json
+-rw-r--r--   0        0        0      129 2023-05-03 13:42:50.401979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/Logger.js
+-rw-r--r--   0        0        0     6762 2023-05-03 13:42:50.341978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/classes/Agent.js
+-rw-r--r--   0        0        0      733 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/classes/HttpProxyAgent.js
+-rw-r--r--   0        0        0     1346 2023-05-03 13:42:50.377979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/classes/HttpsProxyAgent.js
+-rw-r--r--   0        0        0      174 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/classes/index.js
+-rw-r--r--   0        0        0      299 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/errors.js
+-rw-r--r--   0        0        0     5715 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/factories/createGlobalProxyAgent.js
+-rw-r--r--   0        0        0      882 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/factories/createProxyController.js
+-rw-r--r--   0        0        0      160 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/factories/index.js
+-rw-r--r--   0        0        0      100 2023-05-03 13:42:50.389979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/index.js
+-rw-r--r--   0        0        0      550 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/routines/bootstrap.js
+-rw-r--r--   0        0        0       60 2023-05-03 13:42:50.393979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/routines/index.js
+-rw-r--r--   0        0        0     1567 2023-05-03 13:42:50.409979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/types.js
+-rw-r--r--   0        0        0     1197 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/utilities/bindHttpMethod.js
+-rw-r--r--   0        0        0      200 2023-05-03 13:42:50.393979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/utilities/index.js
+-rw-r--r--   0        0        0     1022 2023-05-03 13:42:50.397979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/utilities/isUrlMatchingNoProxy.js
+-rw-r--r--   0        0        0      874 2023-05-03 13:42:50.405979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/utilities/parseProxyUrl.js
+-rw-r--r--   0        0        0       36 2023-05-03 13:42:50.225977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/auto.js
+-rw-r--r--   0        0        0      254 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/implementation.browser.js
+-rw-r--r--   0        0        0       40 2023-05-03 13:42:50.237977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/implementation.js
+-rw-r--r--   0        0        0      408 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/index.js
+-rw-r--r--   0        0        0     2418 2023-05-03 13:42:50.289978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/package.json
+-rw-r--r--   0        0        0      251 2023-05-03 13:42:50.265977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/polyfill.js
+-rw-r--r--   0        0        0      722 2023-05-03 13:42:50.269977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/shim.js
+-rw-r--r--   0        0        0      213 2023-05-03 13:42:50.249977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/test/implementation.js
+-rw-r--r--   0        0        0      196 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/test/index.js
+-rw-r--r--   0        0        0      767 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/test/native.js
+-rw-r--r--   0        0        0      900 2023-05-03 13:42:50.273977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/test/shimmed.js
+-rw-r--r--   0        0        0     1399 2023-05-03 13:42:50.281978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/test/tests.js
+-rw-r--r--   0        0        0     1011 2023-05-03 13:42:50.133976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has/package.json
+-rw-r--r--   0        0        0      129 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has/src/index.js
+-rw-r--r--   0        0        0      331 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has/test/index.js
+-rw-r--r--   0        0        0      817 2023-05-03 13:42:50.225977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-property-descriptors/index.js
+-rw-r--r--   0        0        0     1933 2023-05-03 13:42:50.249977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-property-descriptors/package.json
+-rw-r--r--   0        0        0     1405 2023-05-03 13:42:50.237977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-property-descriptors/test/index.js
+-rw-r--r--   0        0        0      420 2023-05-03 13:42:50.249977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/index.js
+-rw-r--r--   0        0        0     2648 2023-05-03 13:42:50.281978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/package.json
+-rw-r--r--   0        0        0     1761 2023-05-03 13:42:50.265977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/shams.js
+-rw-r--r--   0        0        0      654 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/test/index.js
+-rw-r--r--   0        0        0      723 2023-05-03 13:42:50.237977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/test/shams/core-js.js
+-rw-r--r--   0        0        0      686 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/test/shams/get-own-property-symbols.js
+-rw-r--r--   0        0        0     2021 2023-05-03 13:42:50.269977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/test/tests.js
+-rw-r--r--   0        0        0     7841 2023-05-03 13:42:50.189977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/https-proxy-agent/dist/agent.js
+-rw-r--r--   0        0        0      579 2023-05-03 13:42:50.221977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/https-proxy-agent/dist/index.js
+-rw-r--r--   0        0        0     2460 2023-05-03 13:42:50.225977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/https-proxy-agent/dist/parse-proxy-response.js
+-rw-r--r--   0        0        0     1405 2023-05-03 13:42:50.233977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/https-proxy-agent/package.json
+-rw-r--r--   0        0        0      796 2023-05-03 13:42:50.081975 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/json-stringify-safe/package.json
+-rw-r--r--   0        0        0      907 2023-05-03 13:42:50.221977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/json-stringify-safe/stringify.js
+-rw-r--r--   0        0        0     7550 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/json-stringify-safe/test/stringify_test.js
+-rw-r--r--   0        0        0     8186 2023-05-03 13:42:50.177976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru-cache/index.js
+-rw-r--r--   0        0        0      705 2023-05-03 13:42:50.221977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru-cache/package.json
+-rw-r--r--   0        0        0     4625 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/benchmark.js
+-rw-r--r--   0        0        0     7934 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/lru.js
+-rw-r--r--   0        0        0      901 2023-05-03 13:42:50.081975 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/package.json
+-rw-r--r--   0        0        0     7366 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/test.js
+-rw-r--r--   0        0        0      227 2023-05-03 13:42:50.293978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/tsconfig.json
+-rw-r--r--   0        0        0     1785 2023-05-03 13:42:50.101975 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/matcher/index.js
+-rw-r--r--   0        0        0      871 2023-05-03 13:42:50.133976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/matcher/package.json
+-rw-r--r--   0        0        0     3023 2023-05-03 13:42:50.133976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/ms/index.js
+-rw-r--r--   0        0        0      705 2023-05-03 13:42:50.081975 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/ms/package.json
+-rw-r--r--   0        0        0     3218 2023-05-03 13:42:50.225977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/object-keys/implementation.js
+-rw-r--r--   0        0        0      823 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/object-keys/index.js
+-rw-r--r--   0        0        0      422 2023-05-03 13:42:50.237977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/object-keys/isArguments.js
+-rw-r--r--   0        0        0     1903 2023-05-03 13:42:50.077975 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/object-keys/package.json
+-rw-r--r--   0        0        0       61 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/object-keys/test/index.js
+-rw-r--r--   0        0        0      274 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/constants.js
+-rw-r--r--   0        0        0     6377 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/createLogger.js
+-rw-r--r--   0        0        0     1103 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/createMockLogger.js
+-rw-r--r--   0        0        0      629 2023-05-03 13:42:50.265977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/createNodeWriter.js
+-rw-r--r--   0        0        0     2493 2023-05-03 13:42:50.269977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/createRoarrInititialGlobalState.js
+-rw-r--r--   0        0        0      914 2023-05-03 13:42:50.273977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/index.js
+-rw-r--r--   0        0        0     1186 2023-05-03 13:42:50.285978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/log.js
+-rw-r--r--   0        0        0       47 2023-05-03 13:42:50.293978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/types.js
+-rw-r--r--   0        0        0     2350 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/package.json
+-rwxr-xr-x   0        0        0     4823 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/bin/semver.js
+-rw-r--r--   0        0        0     3563 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/classes/comparator.js
+-rw-r--r--   0        0        0      129 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/classes/index.js
+-rw-r--r--   0        0        0    14283 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/classes/range.js
+-rw-r--r--   0        0        0     8673 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/classes/semver.js
+-rw-r--r--   0        0        0      191 2023-05-03 13:42:50.157976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/clean.js
+-rw-r--r--   0        0        0      947 2023-05-03 13:42:50.177976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/cmp.js
+-rw-r--r--   0        0        0     1505 2023-05-03 13:42:50.185976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/coerce.js
+-rw-r--r--   0        0        0      267 2023-05-03 13:42:50.241977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/compare-build.js
+-rw-r--r--   0        0        0      118 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/compare-loose.js
+-rw-r--r--   0        0        0      156 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/compare.js
+-rw-r--r--   0        0        0     1303 2023-05-03 13:42:50.269977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/diff.js
+-rw-r--r--   0        0        0      112 2023-05-03 13:42:50.273977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/eq.js
+-rw-r--r--   0        0        0      110 2023-05-03 13:42:50.277978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/gt.js
+-rw-r--r--   0        0        0      113 2023-05-03 13:42:50.285978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/gte.js
+-rw-r--r--   0        0        0      464 2023-05-03 13:42:50.297978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/inc.js
+-rw-r--r--   0        0        0      110 2023-05-03 13:42:50.313978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/lt.js
+-rw-r--r--   0        0        0      113 2023-05-03 13:42:50.313978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/lte.js
+-rw-r--r--   0        0        0      122 2023-05-03 13:42:50.325978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/major.js
+-rw-r--r--   0        0        0      122 2023-05-03 13:42:50.329978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/minor.js
+-rw-r--r--   0        0        0      114 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/neq.js
+-rw-r--r--   0        0        0      317 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/parse.js
+-rw-r--r--   0        0        0      122 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/patch.js
+-rw-r--r--   0        0        0      220 2023-05-03 13:42:50.341978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/prerelease.js
+-rw-r--r--   0        0        0      118 2023-05-03 13:42:50.349978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/rcompare.js
+-rw-r--r--   0        0        0      149 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/rsort.js
+-rw-r--r--   0        0        0      233 2023-05-03 13:42:50.357978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/satisfies.js
+-rw-r--r--   0        0        0      147 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/sort.js
+-rw-r--r--   0        0        0      162 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/valid.js
+-rw-r--r--   0        0        0     2616 2023-05-03 13:42:50.305978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/index.js
+-rw-r--r--   0        0        0      657 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/internal/constants.js
+-rw-r--r--   0        0        0      226 2023-05-03 13:42:50.265977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/internal/debug.js
+-rw-r--r--   0        0        0      410 2023-05-03 13:42:50.293978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/internal/identifiers.js
+-rw-r--r--   0        0        0      324 2023-05-03 13:42:50.337978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/internal/parse-options.js
+-rw-r--r--   0        0        0     6672 2023-05-03 13:42:50.353978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/internal/re.js
+-rw-r--r--   0        0        0     1748 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/package.json
+-rw-r--r--   0        0        0       69 2023-05-03 13:42:50.341978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/preload.js
+-rw-r--r--   0        0        0      217 2023-05-03 13:42:50.293978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/gtr.js
+-rw-r--r--   0        0        0      210 2023-05-03 13:42:50.309978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/intersects.js
+-rw-r--r--   0        0        0      213 2023-05-03 13:42:50.317978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/ltr.js
+-rw-r--r--   0        0        0      579 2023-05-03 13:42:50.325978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/max-satisfying.js
+-rw-r--r--   0        0        0      577 2023-05-03 13:42:50.325978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/min-satisfying.js
+-rw-r--r--   0        0        0     1500 2023-05-03 13:42:50.329978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/min-version.js
+-rw-r--r--   0        0        0     2190 2023-05-03 13:42:50.333978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/outside.js
+-rw-r--r--   0        0        0     1341 2023-05-03 13:42:50.361978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/simplify.js
+-rw-r--r--   0        0        0     7510 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/subset.js
+-rw-r--r--   0        0        0      268 2023-05-03 13:42:50.365979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/to-comparators.js
+-rw-r--r--   0        0        0      312 2023-05-03 13:42:50.369979 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/valid.js
+-rw-r--r--   0        0        0      210 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver-compare/example/cmp.js
+-rw-r--r--   0        0        0      181 2023-05-03 13:42:50.249977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver-compare/example/lex.js
+-rw-r--r--   0        0        0      372 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver-compare/index.js
+-rw-r--r--   0        0        0      659 2023-05-03 13:42:50.161976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver-compare/package.json
+-rw-r--r--   0        0        0      444 2023-05-03 13:42:50.261977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver-compare/test/cmp.js
+-rw-r--r--   0        0        0     2235 2023-05-03 13:42:50.133976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/serialize-error/index.js
+-rw-r--r--   0        0        0      743 2023-05-03 13:42:50.161976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/serialize-error/package.json
+-rwxr-xr-x   0        0        0       57 2023-05-03 13:42:50.293978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/bin/snyk
+-rw-r--r--   0        0        0      150 2023-05-03 13:42:50.781983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/config.default.json
+-rw-r--r--   0        0        0     1838 2023-05-03 13:42:50.449980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/110.index.js
+-rw-r--r--   0        0        0   103302 2023-05-03 13:42:50.461980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/213.index.js
+-rw-r--r--   0        0        0   133844 2023-05-03 13:42:50.473980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/31.index.js
+-rw-r--r--   0        0        0   173511 2023-05-03 13:42:50.485980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/38.index.js
+-rw-r--r--   0        0        0   161488 2023-05-03 13:42:50.497980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/384.index.js
+-rw-r--r--   0        0        0   128289 2023-05-03 13:42:50.501980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/395.index.js
+-rw-r--r--   0        0        0     2969 2023-05-03 13:42:50.513980 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/477.index.js
+-rw-r--r--   0        0        0   557584 2023-05-03 13:42:50.537981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/503.index.js
+-rw-r--r--   0        0        0    22931 2023-05-03 13:42:50.541981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/519.index.js
+-rw-r--r--   0        0        0      612 2023-05-03 13:42:50.541981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/522.index.js
+-rw-r--r--   0        0        0   569531 2023-05-03 13:42:50.581981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/535.index.js
+-rw-r--r--   0        0        0     7242 2023-05-03 13:42:50.581981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/542.index.js
+-rw-r--r--   0        0        0     1061 2023-05-03 13:42:50.581981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/575.index.js
+-rw-r--r--   0        0        0    32497 2023-05-03 13:42:50.585981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/663.index.js
+-rw-r--r--   0        0        0    18697 2023-05-03 13:42:50.585981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/726.index.js
+-rw-r--r--   0        0        0   106008 2023-05-03 13:42:50.593981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/741.index.js
+-rw-r--r--   0        0        0   280086 2023-05-03 13:42:50.601981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/784.index.js
+-rw-r--r--   0        0        0   265629 2023-05-03 13:42:50.613982 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/790.index.js
+-rw-r--r--   0        0        0     3295 2023-05-03 13:42:50.613982 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/831.index.js
+-rw-r--r--   0        0        0    11175 2023-05-03 13:42:50.617982 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/85.index.js
+-rw-r--r--   0        0        0     1445 2023-05-03 13:42:50.621981 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/855.index.js
+-rw-r--r--   0        0        0      523 2023-05-03 13:42:50.625982 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/875.index.js
+-rw-r--r--   0        0        0   267291 2023-05-03 13:42:50.629982 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/895.index.js
+-rw-r--r--   0        0        0   227159 2023-05-03 13:42:50.637982 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/905.index.js
+-rw-r--r--   0        0        0  4489688 2023-05-03 13:42:50.673982 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/917.index.js
+-rw-r--r--   0        0        0  8653273 2023-05-03 13:42:50.765983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/95.index.js
+-rw-r--r--   0        0        0      592 2023-05-03 13:42:50.765983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/959.index.js
+-rw-r--r--   0        0        0    93818 2023-05-03 13:42:50.765983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/970.index.js
+-rw-r--r--   0        0        0    20674 2023-05-03 13:42:50.765983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/974.index.js
+-rw-r--r--   0        0        0    14335 2023-05-03 13:42:50.765983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/989.index.js
+-rw-r--r--   0        0        0  1682422 2023-05-03 13:42:50.781983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/index.js
+-rw-r--r--   0        0        0   613426 2023-05-03 13:42:51.085987 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/sql-wasm.wasm
+-rw-r--r--   0        0        0   614892 2023-05-03 13:42:50.785983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/thirdPartyNotice.json
+-rw-r--r--   0        0        0      140 2023-05-03 13:42:50.781983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/jest.config.js
+-rw-r--r--   0        0        0     1094 2023-05-03 13:42:50.781983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/package.json
+-rw-r--r--   0        0        0     1203 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/distPackage.py
+-rw-r--r--   0        0        0      844 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/package.py
+-rw-r--r--   0        0        0      726 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/_typing.py
+-rw-r--r--   0        0        0     9460 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/markers.py
+-rw-r--r--   0        0        0     5098 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/requirements.py
+-rw-r--r--   0        0        0    32208 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/specifiers.py
+-rw-r--r--   0        0        0    29561 2023-05-03 13:42:50.981986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/tags.py
+-rw-r--r--   0        0        0     4385 2023-05-03 13:42:50.981986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/utils.py
+-rw-r--r--   0        0        0    15974 2023-05-03 13:42:50.985986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/version.py
+-rw-r--r--   0        0        0    13551 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pip_resolve.py
+-rw-r--r--   0        0        0     1788 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pipfile.py
+-rw-r--r--   0        0        0   273365 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pyparsing.py
+-rw-r--r--   0        0        0       92 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pytoml/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pytoml/core.py
+-rw-r--r--   0        0        0    11254 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pytoml/parser.py
+-rw-r--r--   0        0        0     3815 2023-05-03 13:42:50.985986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pytoml/writer.py
+-rw-r--r--   0        0        0     1508 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/reqPackage.py
+-rw-r--r--   0        0        0      353 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/requirements/__init__.py
+-rw-r--r--   0        0        0     1352 2023-05-03 13:42:50.969986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/requirements/fragment.py
+-rw-r--r--   0        0        0     3092 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/requirements/parser.py
+-rw-r--r--   0        0        0    10020 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/requirements/requirement.py
+-rw-r--r--   0        0        0      405 2023-05-03 13:42:50.985986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/requirements/vcs.py
+-rw-r--r--   0        0        0     1427 2023-05-03 13:42:50.973986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/setup_file.py
+-rw-r--r--   0        0        0     6291 2023-05-03 13:42:50.981986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/test_pip_resolve.py
+-rw-r--r--   0        0        0     2258 2023-05-03 13:42:50.981986 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/utils.py
+-rw-r--r--   0        0        0      246 2023-05-03 13:42:50.781983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/src/generated/binary-deployments.json
+-rw-r--r--   0        0        0      186 2023-05-03 13:42:50.785983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/tsconfig.json
+-rw-r--r--   0        0        0      843 2023-05-03 13:42:50.765983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/wrapper_dist/bootstrap.js
+-rw-r--r--   0        0        0    11438 2023-05-03 13:42:50.769983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/wrapper_dist/common.js
+-rw-r--r--   0        0        0      246 2023-05-03 13:42:50.781983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/wrapper_dist/generated/binary-deployments.json
+-rw-r--r--   0        0        0     2017 2023-05-03 13:42:50.781983 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/wrapper_dist/index.js
+-rw-r--r--   0        0        0      498 2023-05-03 13:42:50.245977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/dist/angular-sprintf.min.js
+-rw-r--r--   0        0        0     3675 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/dist/sprintf.min.js
+-rw-r--r--   0        0        0      818 2023-05-03 13:42:50.101975 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/package.json
+-rw-r--r--   0        0        0      663 2023-05-03 13:42:50.285978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/src/angular-sprintf.js
+-rw-r--r--   0        0        0     9250 2023-05-03 13:42:50.293978 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/src/sprintf.js
+-rw-r--r--   0        0        0      943 2023-05-03 13:42:50.133976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/modules/index.js
+-rw-r--r--   0        0        0       26 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0      915 2023-05-03 13:42:50.253977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/package.json
+-rw-r--r--   0        0        0      824 2023-05-03 13:42:50.185976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
+-rw-r--r--   0        0        0       71 2023-05-03 13:42:50.257977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
+-rw-r--r--   0        0        0    10274 2023-05-03 13:42:50.229977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/tslib.es6.js
+-rw-r--r--   0        0        0    13204 2023-05-03 13:42:50.241977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/tslib.js
+-rw-r--r--   0        0        0      782 2023-05-03 13:42:50.077975 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/type-fest/package.json
+-rw-r--r--   0        0        0      207 2023-05-03 13:42:50.133976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/yallist/iterator.js
+-rw-r--r--   0        0        0      652 2023-05-03 13:42:50.221977 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/yallist/package.json
+-rw-r--r--   0        0        0     8411 2023-05-03 13:42:50.177976 c2cciutils-1.6.0.dev93/c2cciutils/node_modules/yallist/yallist.js
+-rw-r--r--   0        0        0    25304 2023-05-03 13:42:52.334002 c2cciutils-1.6.0.dev93/c2cciutils/package-lock.json
+-rw-r--r--   0        0        0      134 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/package.json
+-rw-r--r--   0        0        0    10112 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/pr_checks.py
+-rw-r--r--   0        0        0    17707 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/publish.py
+-rw-r--r--   0        0        0     1548 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/schema-applications.json
+-rw-r--r--   0        0        0    22561 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/schema.json
+-rw-r--r--   0        0        0       36 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/__init__.py
+-rw-r--r--   0        0        0     1104 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/audit.py
+-rw-r--r--   0        0        0     3039 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/clean.py
+-rw-r--r--   0        0        0     1712 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/docker_logs.py
+-rw-r--r--   0        0        0     1316 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/docker_versions_gen.py
+-rw-r--r--   0        0        0     4385 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/download_applications.py
+-rw-r--r--   0        0        0      375 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/env.py
+-rw-r--r--   0        0        0       69 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/__init__.py
+-rw-r--r--   0        0        0     3274 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/db.py
+-rw-r--r--   0        0        0      921 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/install.py
+-rw-r--r--   0        0        0     2655 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/logs.py
+-rw-r--r--   0        0        0     5661 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/wait.py
+-rw-r--r--   0        0        0     1162 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/main.py
+-rw-r--r--   0        0        0     2150 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/pin_pipenv.py
+-rw-r--r--   0        0        0     2182 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/pr_checks.py
+-rw-r--r--   0        0        0    18222 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/publish.py
+-rw-r--r--   0        0        0     2804 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/scripts/trigger_image_update.py
+-rw-r--r--   0        0        0     1517 2023-05-03 13:42:34.377791 c2cciutils-1.6.0.dev93/c2cciutils/security.py
+-rw-r--r--   0        0        0     4334 2023-05-03 13:48:12.933481 c2cciutils-1.6.0.dev93/pyproject.toml
+-rw-r--r--   0        0        0   358583 1970-01-01 00:00:00.000000 c2cciutils-1.6.0.dev93/setup.py
+-rw-r--r--   0        0        0    16769 1970-01-01 00:00:00.000000 c2cciutils-1.6.0.dev93/PKG-INFO
```

### Comparing `c2cciutils-1.6.0.dev89/LICENSE` & `c2cciutils-1.6.0.dev93/LICENSE`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/README.md` & `c2cciutils-1.6.0.dev93/README.md`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/__init__.py` & `c2cciutils-1.6.0.dev93/c2cciutils/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/applications_definition.py` & `c2cciutils-1.6.0.dev93/c2cciutils/applications_definition.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/audit.py` & `c2cciutils-1.6.0.dev93/c2cciutils/audit.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/configuration.py` & `c2cciutils-1.6.0.dev93/c2cciutils/configuration.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/env.py` & `c2cciutils-1.6.0.dev93/c2cciutils/env.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/lib/docker.py` & `c2cciutils-1.6.0.dev93/c2cciutils/lib/docker.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/.package-lock.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/.package-lock.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9850677083333335%*

 * *Differences: {"'packages'": "{'node_modules/@sentry-internal/tracing': {'version': '7.50.0', 'resolved': "*

 * *               "'https://registry.npmjs.org/@sentry-internal/tracing/-/tracing-7.50.0.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-4TQ4vN0aMBWsUXfJWk2xbe4x7fKfwCXgXKTtHC/ocwwKM+0EefV5Iw9YFG8IrIQN4vMtuRzktqcs9q0/Sbv7tg==', "*

 * *               "'dependencies': {'@sentry/core': '7.50.0', '@sentry/types': '7.50.0', "*

 * *               "'@sentry/utils': '7.50.0'}}, 'node_modules/@sentry/core': {'version': '7 […]*

```diff
@@ -1,95 +1,75 @@
 {
     "lockfileVersion": 3,
     "name": "c2ccicheck",
     "packages": {
         "node_modules/@sentry-internal/tracing": {
             "dependencies": {
-                "@sentry/core": "7.46.0",
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry/core": "7.50.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "tslib": "^1.9.3"
             },
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-KYoppa7PPL8Er7bdPoxTNUfIY804JL7hhOEomQHYD22rLynwQ4AaLm3YEY75QWwcGb0B7ZDMV+tSumW7Rxuwuw==",
-            "resolved": "https://registry.npmjs.org/@sentry-internal/tracing/-/tracing-7.46.0.tgz",
-            "version": "7.46.0"
-        },
-        "node_modules/@sentry-internal/tracing/node_modules/tslib": {
-            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-4TQ4vN0aMBWsUXfJWk2xbe4x7fKfwCXgXKTtHC/ocwwKM+0EefV5Iw9YFG8IrIQN4vMtuRzktqcs9q0/Sbv7tg==",
+            "resolved": "https://registry.npmjs.org/@sentry-internal/tracing/-/tracing-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/@sentry/core": {
             "dependencies": {
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "tslib": "^1.9.3"
             },
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-BnNHGh/ZTztqQedFko7vb2u6yLs/kWesOQNivav32ZbsEpVCjcmG1gOJXh2YmGIvj3jXOC9a4xfIuh+lYFcA6A==",
-            "resolved": "https://registry.npmjs.org/@sentry/core/-/core-7.46.0.tgz",
-            "version": "7.46.0"
-        },
-        "node_modules/@sentry/core/node_modules/tslib": {
-            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-6oD1a3fYs4aiNK7tuJSd88LHjYJAetd7ZK/AfJniU7zWKj4jxIYfO8nhm0qdnhEDs81RcweVDmPhWm3Kwrzzsg==",
+            "resolved": "https://registry.npmjs.org/@sentry/core/-/core-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/@sentry/node": {
             "dependencies": {
-                "@sentry-internal/tracing": "7.46.0",
-                "@sentry/core": "7.46.0",
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry-internal/tracing": "7.50.0",
+                "@sentry/core": "7.50.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "cookie": "^0.4.1",
                 "https-proxy-agent": "^5.0.0",
                 "lru_map": "^0.3.3",
                 "tslib": "^1.9.3"
             },
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-+GrgJMCye2WXGarRiU5IJHCK27xg7xbPc2XjGojBKbBoZfqxVAWbXEK4bnBQgRGP1pCmrU/M6ZhVgR3dP580xA==",
-            "resolved": "https://registry.npmjs.org/@sentry/node/-/node-7.46.0.tgz",
-            "version": "7.46.0"
-        },
-        "node_modules/@sentry/node/node_modules/tslib": {
-            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-11UJBKoQFMp7f8sbzeO2gENsKIUkVCNBTzuPRib7l2K1HMjSfacXmwwma7ZEs0mc3ofIZ1UYuyONAXmI1lK9cQ==",
+            "resolved": "https://registry.npmjs.org/@sentry/node/-/node-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/@sentry/types": {
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-2FMEMgt2h6u7AoELhNhu9L54GAh67KKfK2pJ1kEXJHmWxM9FSCkizjLs/t+49xtY7jEXr8qYq8bV967VfDPQ9g==",
-            "resolved": "https://registry.npmjs.org/@sentry/types/-/types-7.46.0.tgz",
-            "version": "7.46.0"
+            "integrity": "sha512-Zo9vyI98QNeYT0K0y57Rb4JRWDaPEgmp+QkQ4CRQZFUTWetO5fvPZ4Gb/R7TW16LajuHZlbJBHmvmNj2pkL2kw==",
+            "resolved": "https://registry.npmjs.org/@sentry/types/-/types-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/@sentry/utils": {
             "dependencies": {
-                "@sentry/types": "7.46.0",
+                "@sentry/types": "7.50.0",
                 "tslib": "^1.9.3"
             },
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-elRezDAF84guMG0OVIIZEWm6wUpgbda4HGks98CFnPsrnMm3N1bdBI9XdlxYLtf+ir5KsGR5YlEIf/a0kRUwAQ==",
-            "resolved": "https://registry.npmjs.org/@sentry/utils/-/utils-7.46.0.tgz",
-            "version": "7.46.0"
-        },
-        "node_modules/@sentry/utils/node_modules/tslib": {
-            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-iyPwwC6fwJsiPhH27ZbIiSsY5RaccHBqADS2zEjgKYhmP4P9WGgHRDrvLEnkOjqQyKNb6c0yfmv83n0uxYnolw==",
+            "resolved": "https://registry.npmjs.org/@sentry/utils/-/utils-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/agent-base": {
             "dependencies": {
                 "debug": "4"
             },
             "engines": {
                 "node": ">= 6.0.0"
@@ -323,17 +303,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-NB1ctGL5rlHrPJtFDVIVzTyQylMLu9N9VICA6HSFJo8MCGVTMW6gfpicwKmmK/dAjTOrqu5l63JJOpDSrAis3A==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.3.8.tgz",
-            "version": "7.3.8"
+            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+            "version": "7.5.0"
         },
         "node_modules/semver-compare": {
             "integrity": "sha512-YM3/ITh2MJ5MtzaM429anh+x2jiLVjqILF4m4oyQB18W7Ggea7BfqdH/wGMK7dDiMghv/6WG7znWMwUDzJiXow==",
             "resolved": "https://registry.npmjs.org/semver-compare/-/semver-compare-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/serialize-error": {
@@ -367,14 +347,19 @@
             "version": "1.1150.0"
         },
         "node_modules/sprintf-js": {
             "integrity": "sha512-VE0SOVEHCk7Qc8ulkWw3ntAzXuqf7S2lvwQaDLRnUeIEaKNQJzV6BwmLKhOqT61aGhfUMrXeaBk+oDGCzvhcug==",
             "resolved": "https://registry.npmjs.org/sprintf-js/-/sprintf-js-1.1.2.tgz",
             "version": "1.1.2"
         },
+        "node_modules/tslib": {
+            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
+            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
+            "version": "1.14.1"
+        },
         "node_modules/type-fest": {
             "engines": {
                 "node": ">=10"
             },
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/api.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/api.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/baseclient.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/baseclient.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/envelope.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/envelope.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/exports.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/exports.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/hub.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/hub.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,26 @@
-Object.defineProperty(exports, '__esModule', {
-    value: true
-});
-
-const utils = require('@sentry/utils');
-const constants = require('./constants.js');
-const scope = require('./scope.js');
-const session = require('./session.js');
+import {
+    uuid4,
+    dateTimestampInSeconds,
+    consoleSandbox,
+    logger,
+    GLOBAL_OBJ,
+    getGlobalSingleton
+} from '@sentry/utils';
+import {
+    DEFAULT_ENVIRONMENT
+} from './constants.js';
+import {
+    Scope
+} from './scope.js';
+import {
+    closeSession,
+    makeSession,
+    updateSession
+} from './session.js';
 
 /**
  * API compatibility version of this hub.
  *
  * WARNING: This number should only be increased when the global interface
  * changes and new methods are introduced.
  *
@@ -20,19 +31,14 @@
 /**
  * Default maximum number of breadcrumbs added to an event. Can be overwritten
  * with {@link Options.maxBreadcrumbs}.
  */
 const DEFAULT_BREADCRUMBS = 100;
 
 /**
- * A layer in the process stack.
- * @hidden
- */
-
-/**
  * @inheritDoc
  */
 class Hub {
     /** Is a {@link Layer}[] containing the client and scope */
 
     /** Contains the last event id of a captured event.  */
 
@@ -40,18 +46,18 @@
      * Creates a new instance of the hub, will push one {@link Layer} into the
      * internal stack on creation.
      *
      * @param client bound to the hub.
      * @param scope bound to the hub.
      * @param version number, higher number means higher priority.
      */
-    constructor(client, scope$1 = new scope.Scope(), _version = API_VERSION) {
+    constructor(client, scope = new Scope(), _version = API_VERSION) {
         this._version = _version;
         this._stack = [{
-            scope: scope$1
+            scope
         }];
         if (client) {
             this.bindClient(client);
         }
     }
 
     /**
@@ -73,20 +79,20 @@
     }
 
     /**
      * @inheritDoc
      */
     pushScope() {
         // We want to clone the content of prev scope
-        const scope$1 = scope.Scope.clone(this.getScope());
+        const scope = Scope.clone(this.getScope());
         this.getStack().push({
             client: this.getClient(),
-            scope: scope$1,
+            scope,
         });
-        return scope$1;
+        return scope;
     }
 
     /**
      * @inheritDoc
      */
     popScope() {
         if (this.getStack().length <= 1) return false;
@@ -127,15 +133,15 @@
         return this._stack[this._stack.length - 1];
     }
 
     /**
      * @inheritDoc
      */
     captureException(exception, hint) {
-        const eventId = (this._lastEventId = hint && hint.event_id ? hint.event_id : utils.uuid4());
+        const eventId = (this._lastEventId = hint && hint.event_id ? hint.event_id : uuid4());
         const syntheticException = new Error('Sentry syntheticException');
         this._withClient((client, scope) => {
             client.captureException(
                 exception, {
                     originalException: exception,
                     syntheticException,
                     ...hint,
@@ -152,15 +158,15 @@
      */
     captureMessage(
         message,
         // eslint-disable-next-line deprecation/deprecation
         level,
         hint,
     ) {
-        const eventId = (this._lastEventId = hint && hint.event_id ? hint.event_id : utils.uuid4());
+        const eventId = (this._lastEventId = hint && hint.event_id ? hint.event_id : uuid4());
         const syntheticException = new Error(message);
         this._withClient((client, scope) => {
             client.captureMessage(
                 message,
                 level, {
                     originalException: message,
                     syntheticException,
@@ -173,15 +179,15 @@
         return eventId;
     }
 
     /**
      * @inheritDoc
      */
     captureEvent(event, hint) {
-        const eventId = hint && hint.event_id ? hint.event_id : utils.uuid4();
+        const eventId = hint && hint.event_id ? hint.event_id : uuid4();
         if (!event.type) {
             this._lastEventId = eventId;
         }
 
         this._withClient((client, scope) => {
             client.captureEvent(event, {
                 ...hint,
@@ -212,21 +218,21 @@
         const {
             beforeBreadcrumb = null, maxBreadcrumbs = DEFAULT_BREADCRUMBS
         } =
         (client.getOptions && client.getOptions()) || {};
 
         if (maxBreadcrumbs <= 0) return;
 
-        const timestamp = utils.dateTimestampInSeconds();
+        const timestamp = dateTimestampInSeconds();
         const mergedBreadcrumb = {
             timestamp,
             ...breadcrumb
         };
         const finalBreadcrumb = beforeBreadcrumb ?
-            (utils.consoleSandbox(() => beforeBreadcrumb(mergedBreadcrumb, hint))) :
+            (consoleSandbox(() => beforeBreadcrumb(mergedBreadcrumb, hint))) :
             mergedBreadcrumb;
 
         if (finalBreadcrumb === null) return;
 
         if (client.emit) {
             client.emit('beforeAddBreadcrumb', finalBreadcrumb, hint);
         }
@@ -307,24 +313,34 @@
      */
     getIntegration(integration) {
         const client = this.getClient();
         if (!client) return null;
         try {
             return client.getIntegration(integration);
         } catch (_oO) {
-            (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.warn(`Cannot retrieve integration ${integration.id} from the current Hub`);
+            (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.warn(`Cannot retrieve integration ${integration.id} from the current Hub`);
             return null;
         }
     }
 
     /**
      * @inheritDoc
      */
     startTransaction(context, customSamplingContext) {
-        return this._callExtensionMethod('startTransaction', context, customSamplingContext);
+        const result = this._callExtensionMethod('startTransaction', context, customSamplingContext);
+
+        if ((typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && !result) {
+            // eslint-disable-next-line no-console
+            console.warn(`Tracing extension 'startTransaction' has not been added. Call 'addTracingExtensions' before calling 'init':
+Sentry.addTracingExtensions();
+Sentry.init({...});
+`);
+        }
+
+        return result;
     }
 
     /**
      * @inheritDoc
      */
     traceHeaders() {
         return this._callExtensionMethod('traceHeaders');
@@ -345,17 +361,17 @@
 
     /**
      * @inheritDoc
      */
     endSession() {
         const layer = this.getStackTop();
         const scope = layer.scope;
-        const session$1 = scope.getSession();
-        if (session$1) {
-            session.closeSession(session$1);
+        const session = scope.getSession();
+        if (session) {
+            closeSession(session);
         }
         this._sendSessionUpdate();
 
         // the session is over; take it off of the scope
         scope.setSession();
     }
 
@@ -365,45 +381,45 @@
     startSession(context) {
         const {
             scope,
             client
         } = this.getStackTop();
         const {
             release,
-            environment = constants.DEFAULT_ENVIRONMENT
+            environment = DEFAULT_ENVIRONMENT
         } = (client && client.getOptions()) || {};
 
         // Will fetch userAgent if called from browser sdk
         const {
             userAgent
-        } = utils.GLOBAL_OBJ.navigator || {};
+        } = GLOBAL_OBJ.navigator || {};
 
-        const session$1 = session.makeSession({
+        const session = makeSession({
             release,
             environment,
             user: scope.getUser(),
             ...(userAgent && {
                 userAgent
             }),
             ...context,
         });
 
         // End existing session if there's one
         const currentSession = scope.getSession && scope.getSession();
         if (currentSession && currentSession.status === 'ok') {
-            session.updateSession(currentSession, {
+            updateSession(currentSession, {
                 status: 'exited'
             });
         }
         this.endSession();
 
         // Afterwards we set the new session on the scope
-        scope.setSession(session$1);
+        scope.setSession(session);
 
-        return session$1;
+        return session;
     }
 
     /**
      * Returns if default PII should be sent to Sentry and propagated in ourgoing requests
      * when Tracing is used.
      */
     shouldSendDefaultPii() {
@@ -416,21 +432,18 @@
      * Sends the current Session on the scope
      */
     _sendSessionUpdate() {
         const {
             scope,
             client
         } = this.getStackTop();
-        if (!scope) return;
 
         const session = scope.getSession();
-        if (session) {
-            if (client && client.captureSession) {
-                client.captureSession(session);
-            }
+        if (session && client && client.captureSession) {
+            client.captureSession(session);
         }
     }
 
     /**
      * Internal helper function to call a method on the top client if it exists.
      *
      * @param method The method to call on the client.
@@ -453,31 +466,31 @@
     // eslint-disable-next-line @typescript-eslint/no-explicit-any
     _callExtensionMethod(method, ...args) {
         const carrier = getMainCarrier();
         const sentry = carrier.__SENTRY__;
         if (sentry && sentry.extensions && typeof sentry.extensions[method] === 'function') {
             return sentry.extensions[method].apply(this, args);
         }
-        (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.warn(`Extension method ${method} couldn't be found, doing nothing.`);
+        (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.warn(`Extension method ${method} couldn't be found, doing nothing.`);
     }
 }
 
 /**
  * Returns the global shim registry.
  *
  * FIXME: This function is problematic, because despite always returning a valid Carrier,
  * it has an optional `__SENTRY__` property, which then in turn requires us to always perform an unnecessary check
  * at the call-site. We always access the carrier through this function, so we can guarantee that `__SENTRY__` is there.
  **/
 function getMainCarrier() {
-    utils.GLOBAL_OBJ.__SENTRY__ = utils.GLOBAL_OBJ.__SENTRY__ || {
+    GLOBAL_OBJ.__SENTRY__ = GLOBAL_OBJ.__SENTRY__ || {
         extensions: {},
         hub: undefined,
     };
-    return utils.GLOBAL_OBJ;
+    return GLOBAL_OBJ;
 }
 
 /**
  * Replaces the current main hub with the passed one on the global object
  *
  * @returns The old replaced hub
  */
@@ -495,53 +508,77 @@
  * contains a more recent version, it replaces the registered version.
  * Otherwise, the currently registered hub will be returned.
  */
 function getCurrentHub() {
     // Get main carrier (global for every environment)
     const registry = getMainCarrier();
 
+    if (registry.__SENTRY__ && registry.__SENTRY__.acs) {
+        const hub = registry.__SENTRY__.acs.getCurrentHub();
+
+        if (hub) {
+            return hub;
+        }
+    }
+
+    // Return hub that lives on a global object
+    return getGlobalHub(registry);
+}
+
+function getGlobalHub(registry = getMainCarrier()) {
     // If there's no hub, or its an old API, assign a new one
     if (!hasHubOnCarrier(registry) || getHubFromCarrier(registry).isOlderThan(API_VERSION)) {
         setHubOnCarrier(registry, new Hub());
     }
 
-    // Prefer domains over global if they are there (applicable only to Node environment)
-    if (utils.isNodeEnv()) {
-        return getHubFromActiveDomain(registry);
-    }
     // Return hub that lives on a global object
     return getHubFromCarrier(registry);
 }
 
 /**
- * Try to read the hub from an active domain, and fallback to the registry if one doesn't exist
- * @returns discovered hub
+ * @private Private API with no semver guarantees!
+ *
+ * If the carrier does not contain a hub, a new hub is created with the global hub client and scope.
+ */
+function ensureHubOnCarrier(carrier, parent = getGlobalHub()) {
+    // If there's no hub on current domain, or it's an old API, assign a new one
+    if (!hasHubOnCarrier(carrier) || getHubFromCarrier(carrier).isOlderThan(API_VERSION)) {
+        const globalHubTopStack = parent.getStackTop();
+        setHubOnCarrier(carrier, new Hub(globalHubTopStack.client, Scope.clone(globalHubTopStack.scope)));
+    }
+}
+
+/**
+ * @private Private API with no semver guarantees!
+ *
+ * Sets the global async context strategy
+ */
+function setAsyncContextStrategy(strategy) {
+    // Get main carrier (global for every environment)
+    const registry = getMainCarrier();
+    registry.__SENTRY__ = registry.__SENTRY__ || {};
+    registry.__SENTRY__.acs = strategy;
+}
+
+/**
+ * Runs the supplied callback in its own async context. Async Context strategies are defined per SDK.
+ *
+ * @param callback The callback to run in its own async context
+ * @param options Options to pass to the async context strategy
+ * @returns The result of the callback
  */
-function getHubFromActiveDomain(registry) {
-    try {
-        const sentry = getMainCarrier().__SENTRY__;
-        const activeDomain = sentry && sentry.extensions && sentry.extensions.domain && sentry.extensions.domain.active;
-
-        // If there's no active domain, just return global hub
-        if (!activeDomain) {
-            return getHubFromCarrier(registry);
-        }
-
-        // If there's no hub on current domain, or it's an old API, assign a new one
-        if (!hasHubOnCarrier(activeDomain) || getHubFromCarrier(activeDomain).isOlderThan(API_VERSION)) {
-            const registryHubTopStack = getHubFromCarrier(registry).getStackTop();
-            setHubOnCarrier(activeDomain, new Hub(registryHubTopStack.client, scope.Scope.clone(registryHubTopStack.scope)));
-        }
-
-        // Return hub that lives on a domain
-        return getHubFromCarrier(activeDomain);
-    } catch (_Oo) {
-        // Return hub that lives on a global object
-        return getHubFromCarrier(registry);
+function runWithAsyncContext(callback, options = {}) {
+    const registry = getMainCarrier();
+
+    if (registry.__SENTRY__ && registry.__SENTRY__.acs) {
+        return registry.__SENTRY__.acs.runWithAsyncContext(callback, options);
     }
+
+    // if there was no strategy, fallback to just calling the callback
+    return callback();
 }
 
 /**
  * This will tell whether a carrier has a hub on it or not
  * @param carrier object
  */
 function hasHubOnCarrier(carrier) {
@@ -551,15 +588,15 @@
 /**
  * This will create a new {@link Hub} and add to the passed object on
  * __SENTRY__.hub.
  * @param carrier object
  * @hidden
  */
 function getHubFromCarrier(carrier) {
-    return utils.getGlobalSingleton('hub', () => new Hub(), carrier);
+    return getGlobalSingleton('hub', () => new Hub(), carrier);
 }
 
 /**
  * This will set passed {@link Hub} on the passed object's __SENTRY__.hub attribute
  * @param carrier object
  * @param hub Hub
  * @returns A boolean indicating success or failure
@@ -567,15 +604,20 @@
 function setHubOnCarrier(carrier, hub) {
     if (!carrier) return false;
     const __SENTRY__ = (carrier.__SENTRY__ = carrier.__SENTRY__ || {});
     __SENTRY__.hub = hub;
     return true;
 }
 
-exports.API_VERSION = API_VERSION;
-exports.Hub = Hub;
-exports.getCurrentHub = getCurrentHub;
-exports.getHubFromCarrier = getHubFromCarrier;
-exports.getMainCarrier = getMainCarrier;
-exports.makeMain = makeMain;
-exports.setHubOnCarrier = setHubOnCarrier;
+export {
+    API_VERSION,
+    Hub,
+    ensureHubOnCarrier,
+    getCurrentHub,
+    getHubFromCarrier,
+    getMainCarrier,
+    makeMain,
+    runWithAsyncContext,
+    setAsyncContextStrategy,
+    setHubOnCarrier
+};
 //# sourceMappingURL=hub.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/index.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -15,14 +15,15 @@
 const sessionflusher = require('./sessionflusher.js');
 const scope = require('./scope.js');
 const api = require('./api.js');
 const baseclient = require('./baseclient.js');
 const sdk = require('./sdk.js');
 const base = require('./transports/base.js');
 const offline = require('./transports/offline.js');
+const multiplexed = require('./transports/multiplexed.js');
 const version = require('./version.js');
 const integration = require('./integration.js');
 const index = require('./integrations/index.js');
 const prepareEvent = require('./utils/prepareEvent.js');
 const hasTracingEnabled = require('./utils/hasTracingEnabled.js');
 const constants = require('./constants.js');
 const functiontostring = require('./integrations/functiontostring.js');
@@ -54,31 +55,35 @@
 exports.setExtras = exports$1.setExtras;
 exports.setTag = exports$1.setTag;
 exports.setTags = exports$1.setTags;
 exports.setUser = exports$1.setUser;
 exports.startTransaction = exports$1.startTransaction;
 exports.withScope = exports$1.withScope;
 exports.Hub = hub.Hub;
+exports.ensureHubOnCarrier = hub.ensureHubOnCarrier;
 exports.getCurrentHub = hub.getCurrentHub;
 exports.getHubFromCarrier = hub.getHubFromCarrier;
 exports.getMainCarrier = hub.getMainCarrier;
 exports.makeMain = hub.makeMain;
+exports.runWithAsyncContext = hub.runWithAsyncContext;
+exports.setAsyncContextStrategy = hub.setAsyncContextStrategy;
 exports.setHubOnCarrier = hub.setHubOnCarrier;
 exports.closeSession = session.closeSession;
 exports.makeSession = session.makeSession;
 exports.updateSession = session.updateSession;
 exports.SessionFlusher = sessionflusher.SessionFlusher;
 exports.Scope = scope.Scope;
 exports.addGlobalEventProcessor = scope.addGlobalEventProcessor;
 exports.getEnvelopeEndpointWithUrlEncodedAuth = api.getEnvelopeEndpointWithUrlEncodedAuth;
 exports.getReportDialogEndpoint = api.getReportDialogEndpoint;
 exports.BaseClient = baseclient.BaseClient;
 exports.initAndBind = sdk.initAndBind;
 exports.createTransport = base.createTransport;
 exports.makeOfflineTransport = offline.makeOfflineTransport;
+exports.makeMultiplexedTransport = multiplexed.makeMultiplexedTransport;
 exports.SDK_VERSION = version.SDK_VERSION;
 exports.getIntegrationsToSetup = integration.getIntegrationsToSetup;
 exports.Integrations = index;
 exports.prepareEvent = prepareEvent.prepareEvent;
 exports.hasTracingEnabled = hasTracingEnabled.hasTracingEnabled;
 exports.DEFAULT_ENVIRONMENT = constants.DEFAULT_ENVIRONMENT;
 exports.FunctionToString = functiontostring.FunctionToString;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/integration.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/integration.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/integrations/functiontostring.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/integrations/functiontostring.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,10 @@
-Object.defineProperty(exports, '__esModule', {
-    value: true
-});
-
-const utils = require('@sentry/utils');
+import {
+    getOriginalFunction
+} from '@sentry/utils';
 
 let originalFunctionToString;
 
 /** Patch toString calls to return proper name for wrapped functions */
 class FunctionToString {
     constructor() {
         FunctionToString.prototype.__init.call(this);
@@ -28,18 +26,26 @@
     /**
      * @inheritDoc
      */
     setupOnce() {
         // eslint-disable-next-line @typescript-eslint/unbound-method
         originalFunctionToString = Function.prototype.toString;
 
-        // eslint-disable-next-line @typescript-eslint/no-explicit-any
-        Function.prototype.toString = function(...args) {
-            const context = utils.getOriginalFunction(this) || this;
-            return originalFunctionToString.apply(context, args);
-        };
+        // intrinsics (like Function.prototype) might be immutable in some environments
+        // e.g. Node with --frozen-intrinsics, XS (an embedded JavaScript engine) or SES (a JavaScript proposal)
+        try {
+            // eslint-disable-next-line @typescript-eslint/no-explicit-any
+            Function.prototype.toString = function(...args) {
+                const context = getOriginalFunction(this) || this;
+                return originalFunctionToString.apply(context, args);
+            };
+        } catch (e) {
+            // ignore errors here, just don't patch this
+        }
     }
 }
 FunctionToString.__initStatic();
 
-exports.FunctionToString = FunctionToString;
+export {
+    FunctionToString
+};
 //# sourceMappingURL=functiontostring.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/integrations/inboundfilters.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/integrations/inboundfilters.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/scope.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/scope.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -483,20 +483,27 @@
         // a trace context on the event. There is a product feature in place where we link
         // errors with transaction and it relies on that.
         if (this._span) {
             event.contexts = {
                 trace: this._span.getTraceContext(),
                 ...event.contexts
             };
-            const transactionName = this._span.transaction && this._span.transaction.name;
-            if (transactionName) {
-                event.tags = {
-                    transaction: transactionName,
-                    ...event.tags
+            const transaction = this._span.transaction;
+            if (transaction) {
+                event.sdkProcessingMetadata = {
+                    dynamicSamplingContext: transaction.getDynamicSamplingContext(),
+                    ...event.sdkProcessingMetadata,
                 };
+                const transactionName = transaction.name;
+                if (transactionName) {
+                    event.tags = {
+                        transaction: transactionName,
+                        ...event.tags
+                    };
+                }
             }
         }
 
         this._applyFingerprint(event);
 
         event.breadcrumbs = [...(event.breadcrumbs || []), ...this._breadcrumbs];
         event.breadcrumbs = event.breadcrumbs.length > 0 ? event.breadcrumbs : undefined;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/sdk.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/sdk.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/session.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/session.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/sessionflusher.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/sessionflusher.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/errors.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/errors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/hubextensions.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/hubextensions.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/idletransaction.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/idletransaction.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -44,15 +44,15 @@
      */
     add(span) {
         // We should make sure we do not push and pop activities for
         // the transaction that this span recorder belongs to.
         if (span.spanId !== this.transactionSpanId) {
             // We patch span.finish() to pop an activity after setting an endTimestamp.
             span.finish = (endTimestamp) => {
-                span.endTimestamp = typeof endTimestamp === 'number' ? endTimestamp : utils.timestampWithMs();
+                span.endTimestamp = typeof endTimestamp === 'number' ? endTimestamp : utils.timestampInSeconds();
                 this._popActivity(span.spanId);
             };
 
             // We should only push new activities if the span does not have an end timestamp.
             if (span.endTimestamp === undefined) {
                 this._pushActivity(span.spanId);
             }
@@ -127,17 +127,14 @@
         IdleTransaction.prototype.__init.call(this);
         IdleTransaction.prototype.__init2.call(this);
         IdleTransaction.prototype.__init3.call(this);
         IdleTransaction.prototype.__init4.call(this);
         IdleTransaction.prototype.__init5.call(this);
         IdleTransaction.prototype.__init6.call(this);
         if (_onScope) {
-            // There should only be one active transaction on the scope
-            clearActiveTransaction(_idleHub);
-
             // We set the transaction here on the scope so error events pick up the trace
             // context and attach it to the error.
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.log(`Setting idle transaction on scope. Span ID: ${this.spanId}`);
             _idleHub.configureScope(scope => scope.setSpan(this));
         }
 
         this._restartIdleTimeout();
@@ -147,15 +144,15 @@
                 this._finishReason = IDLE_TRANSACTION_FINISH_REASONS[3];
                 this.finish();
             }
         }, this._finalTimeout);
     }
 
     /** {@inheritDoc} */
-    finish(endTimestamp = utils.timestampWithMs()) {
+    finish(endTimestamp = utils.timestampInSeconds()) {
         this._finished = true;
         this.activities = {};
 
         if (this.op === 'ui.action.click') {
             this.setTag(FINISH_REASON_TAG, this._finishReason);
         }
 
@@ -195,15 +192,18 @@
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.log('[Tracing] flushing IdleTransaction');
         } else {
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.log('[Tracing] No active IdleTransaction');
         }
 
         // if `this._onScope` is `true`, the transaction put itself on the scope when it started
         if (this._onScope) {
-            clearActiveTransaction(this._idleHub);
+            const scope = this._idleHub.getScope();
+            if (scope.getTransaction() === this) {
+                scope.setSpan(undefined);
+            }
         }
 
         return super.finish(endTimestamp);
     }
 
     /**
      * Register a callback function that gets excecuted before the transaction finishes.
@@ -318,21 +318,21 @@
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.log(`[Tracing] popActivity ${spanId}`);
             // eslint-disable-next-line @typescript-eslint/no-dynamic-delete
             delete this.activities[spanId];
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.log('[Tracing] new activities count', Object.keys(this.activities).length);
         }
 
         if (Object.keys(this.activities).length === 0) {
-            const endTimestamp = utils.timestampWithMs();
+            const endTimestamp = utils.timestampInSeconds();
             if (this._idleTimeoutCanceledPermanently) {
                 this._finishReason = IDLE_TRANSACTION_FINISH_REASONS[5];
                 this.finish(endTimestamp);
             } else {
                 // We need to add the timeout here to have the real endtimestamp of the transaction
-                // Remember timestampWithMs is in seconds, timeout is in ms
+                // Remember timestampInSeconds is in seconds, timeout is in ms
                 this._restartIdleTimeout(endTimestamp + this._idleTimeout / 1000);
             }
         }
     }
 
     /**
      * Checks when entries of this.activities are not changing for 3 beats.
@@ -371,21 +371,11 @@
         (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.log(`pinging Heartbeat -> current counter: ${this._heartbeatCounter}`);
         setTimeout(() => {
             this._beat();
         }, this._heartbeatInterval);
     }
 }
 
-/**
- * Reset transaction on scope to `undefined`
- */
-function clearActiveTransaction(hub) {
-    const scope = hub.getScope();
-    if (scope.getTransaction()) {
-        scope.setSpan(undefined);
-    }
-}
-
 exports.IdleTransaction = IdleTransaction;
 exports.IdleTransactionSpanRecorder = IdleTransactionSpanRecorder;
 exports.TRACING_DEFAULTS = TRACING_DEFAULTS;
 //# sourceMappingURL=idletransaction.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/span.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/span.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -65,15 +65,15 @@
      * @inheritDoc
      */
 
     /**
      * Timestamp in seconds when the span was created.
      */
     __init4() {
-        this.startTimestamp = utils.timestampWithMs();
+        this.startTimestamp = utils.timestampInSeconds();
     }
 
     /**
      * Timestamp in seconds when the span ended.
      */
 
     /**
@@ -269,15 +269,15 @@
                 logMessage
             } = this.transaction.metadata.spanMetadata[this.spanId];
             if (logMessage) {
                 utils.logger.log((logMessage).replace('Starting', 'Finishing'));
             }
         }
 
-        this.endTimestamp = typeof endTimestamp === 'number' ? endTimestamp : utils.timestampWithMs();
+        this.endTimestamp = typeof endTimestamp === 'number' ? endTimestamp : utils.timestampInSeconds();
     }
 
     /**
      * @inheritDoc
      */
     toTraceparent() {
         let sampledString = '';
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/spanstatus.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/spanstatus.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/trace.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/trace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/transaction.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/transaction.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/tracing/utils.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/tracing/utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/transports/base.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/transports/base.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/transports/offline.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/transports/offline.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/cjs/utils/prepareEvent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/utils/prepareEvent.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -37,15 +37,19 @@
         event_id: event.event_id || hint.event_id || utils.uuid4(),
         timestamp: event.timestamp || utils.dateTimestampInSeconds(),
     };
     const integrations = hint.integrations || options.integrations.map(i => i.name);
 
     applyClientOptions(prepared, options);
     applyIntegrationsMetadata(prepared, integrations);
-    applyDebugMetadata(prepared, options.stackParser);
+
+    // Only apply debug metadata to error events.
+    if (event.type === undefined) {
+        applyDebugMetadata(prepared, options.stackParser);
+    }
 
     // If we have scope given to us, use it as the base for further modifications.
     // This allows us to prevent unnecessary copying of data if `captureContext` is not provided.
     let finalScope = scope$1;
     if (hint.captureContext) {
         finalScope = scope.Scope.clone(finalScope).update(hint.captureContext);
     }
@@ -119,28 +123,48 @@
 
     const request = event.request;
     if (request && request.url) {
         request.url = utils.truncate(request.url, maxValueLength);
     }
 }
 
+const debugIdStackParserCache = new WeakMap();
+
 /**
  * Applies debug metadata images to the event in order to apply source maps by looking up their debug ID.
  */
 function applyDebugMetadata(event, stackParser) {
     const debugIdMap = utils.GLOBAL_OBJ._sentryDebugIds;
 
     if (!debugIdMap) {
         return;
     }
 
+    let debugIdStackFramesCache;
+    const cachedDebugIdStackFrameCache = debugIdStackParserCache.get(stackParser);
+    if (cachedDebugIdStackFrameCache) {
+        debugIdStackFramesCache = cachedDebugIdStackFrameCache;
+    } else {
+        debugIdStackFramesCache = new Map();
+        debugIdStackParserCache.set(stackParser, debugIdStackFramesCache);
+    }
+
     // Build a map of filename -> debug_id
     const filenameDebugIdMap = Object.keys(debugIdMap).reduce((acc, debugIdStackTrace) => {
-        const parsedStack = stackParser(debugIdStackTrace);
-        for (const stackFrame of parsedStack) {
+        let parsedStack;
+        const cachedParsedStack = debugIdStackFramesCache.get(debugIdStackTrace);
+        if (cachedParsedStack) {
+            parsedStack = cachedParsedStack;
+        } else {
+            parsedStack = stackParser(debugIdStackTrace);
+            debugIdStackFramesCache.set(debugIdStackTrace, parsedStack);
+        }
+
+        for (let i = parsedStack.length - 1; i >= 0; i--) {
+            const stackFrame = parsedStack[i];
             if (stackFrame.filename) {
                 acc[stackFrame.filename] = debugIdMap[debugIdStackTrace];
                 break;
             }
         }
         return acc;
     }, {});
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/api.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/api.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/baseclient.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/baseclient.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/envelope.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/envelope.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/exports.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/exports.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/hub.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/cjs/hub.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,15 @@
-import {
-    uuid4,
-    dateTimestampInSeconds,
-    consoleSandbox,
-    logger,
-    GLOBAL_OBJ,
-    isNodeEnv,
-    getGlobalSingleton
-} from '@sentry/utils';
-import {
-    DEFAULT_ENVIRONMENT
-} from './constants.js';
-import {
-    Scope
-} from './scope.js';
-import {
-    closeSession,
-    makeSession,
-    updateSession
-} from './session.js';
+Object.defineProperty(exports, '__esModule', {
+    value: true
+});
+
+const utils = require('@sentry/utils');
+const constants = require('./constants.js');
+const scope = require('./scope.js');
+const session = require('./session.js');
 
 /**
  * API compatibility version of this hub.
  *
  * WARNING: This number should only be increased when the global interface
  * changes and new methods are introduced.
  *
@@ -32,19 +20,14 @@
 /**
  * Default maximum number of breadcrumbs added to an event. Can be overwritten
  * with {@link Options.maxBreadcrumbs}.
  */
 const DEFAULT_BREADCRUMBS = 100;
 
 /**
- * A layer in the process stack.
- * @hidden
- */
-
-/**
  * @inheritDoc
  */
 class Hub {
     /** Is a {@link Layer}[] containing the client and scope */
 
     /** Contains the last event id of a captured event.  */
 
@@ -52,18 +35,18 @@
      * Creates a new instance of the hub, will push one {@link Layer} into the
      * internal stack on creation.
      *
      * @param client bound to the hub.
      * @param scope bound to the hub.
      * @param version number, higher number means higher priority.
      */
-    constructor(client, scope = new Scope(), _version = API_VERSION) {
+    constructor(client, scope$1 = new scope.Scope(), _version = API_VERSION) {
         this._version = _version;
         this._stack = [{
-            scope
+            scope: scope$1
         }];
         if (client) {
             this.bindClient(client);
         }
     }
 
     /**
@@ -85,20 +68,20 @@
     }
 
     /**
      * @inheritDoc
      */
     pushScope() {
         // We want to clone the content of prev scope
-        const scope = Scope.clone(this.getScope());
+        const scope$1 = scope.Scope.clone(this.getScope());
         this.getStack().push({
             client: this.getClient(),
-            scope,
+            scope: scope$1,
         });
-        return scope;
+        return scope$1;
     }
 
     /**
      * @inheritDoc
      */
     popScope() {
         if (this.getStack().length <= 1) return false;
@@ -139,15 +122,15 @@
         return this._stack[this._stack.length - 1];
     }
 
     /**
      * @inheritDoc
      */
     captureException(exception, hint) {
-        const eventId = (this._lastEventId = hint && hint.event_id ? hint.event_id : uuid4());
+        const eventId = (this._lastEventId = hint && hint.event_id ? hint.event_id : utils.uuid4());
         const syntheticException = new Error('Sentry syntheticException');
         this._withClient((client, scope) => {
             client.captureException(
                 exception, {
                     originalException: exception,
                     syntheticException,
                     ...hint,
@@ -164,15 +147,15 @@
      */
     captureMessage(
         message,
         // eslint-disable-next-line deprecation/deprecation
         level,
         hint,
     ) {
-        const eventId = (this._lastEventId = hint && hint.event_id ? hint.event_id : uuid4());
+        const eventId = (this._lastEventId = hint && hint.event_id ? hint.event_id : utils.uuid4());
         const syntheticException = new Error(message);
         this._withClient((client, scope) => {
             client.captureMessage(
                 message,
                 level, {
                     originalException: message,
                     syntheticException,
@@ -185,15 +168,15 @@
         return eventId;
     }
 
     /**
      * @inheritDoc
      */
     captureEvent(event, hint) {
-        const eventId = hint && hint.event_id ? hint.event_id : uuid4();
+        const eventId = hint && hint.event_id ? hint.event_id : utils.uuid4();
         if (!event.type) {
             this._lastEventId = eventId;
         }
 
         this._withClient((client, scope) => {
             client.captureEvent(event, {
                 ...hint,
@@ -224,21 +207,21 @@
         const {
             beforeBreadcrumb = null, maxBreadcrumbs = DEFAULT_BREADCRUMBS
         } =
         (client.getOptions && client.getOptions()) || {};
 
         if (maxBreadcrumbs <= 0) return;
 
-        const timestamp = dateTimestampInSeconds();
+        const timestamp = utils.dateTimestampInSeconds();
         const mergedBreadcrumb = {
             timestamp,
             ...breadcrumb
         };
         const finalBreadcrumb = beforeBreadcrumb ?
-            (consoleSandbox(() => beforeBreadcrumb(mergedBreadcrumb, hint))) :
+            (utils.consoleSandbox(() => beforeBreadcrumb(mergedBreadcrumb, hint))) :
             mergedBreadcrumb;
 
         if (finalBreadcrumb === null) return;
 
         if (client.emit) {
             client.emit('beforeAddBreadcrumb', finalBreadcrumb, hint);
         }
@@ -319,24 +302,34 @@
      */
     getIntegration(integration) {
         const client = this.getClient();
         if (!client) return null;
         try {
             return client.getIntegration(integration);
         } catch (_oO) {
-            (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.warn(`Cannot retrieve integration ${integration.id} from the current Hub`);
+            (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.warn(`Cannot retrieve integration ${integration.id} from the current Hub`);
             return null;
         }
     }
 
     /**
      * @inheritDoc
      */
     startTransaction(context, customSamplingContext) {
-        return this._callExtensionMethod('startTransaction', context, customSamplingContext);
+        const result = this._callExtensionMethod('startTransaction', context, customSamplingContext);
+
+        if ((typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && !result) {
+            // eslint-disable-next-line no-console
+            console.warn(`Tracing extension 'startTransaction' has not been added. Call 'addTracingExtensions' before calling 'init':
+Sentry.addTracingExtensions();
+Sentry.init({...});
+`);
+        }
+
+        return result;
     }
 
     /**
      * @inheritDoc
      */
     traceHeaders() {
         return this._callExtensionMethod('traceHeaders');
@@ -357,17 +350,17 @@
 
     /**
      * @inheritDoc
      */
     endSession() {
         const layer = this.getStackTop();
         const scope = layer.scope;
-        const session = scope.getSession();
-        if (session) {
-            closeSession(session);
+        const session$1 = scope.getSession();
+        if (session$1) {
+            session.closeSession(session$1);
         }
         this._sendSessionUpdate();
 
         // the session is over; take it off of the scope
         scope.setSession();
     }
 
@@ -377,45 +370,45 @@
     startSession(context) {
         const {
             scope,
             client
         } = this.getStackTop();
         const {
             release,
-            environment = DEFAULT_ENVIRONMENT
+            environment = constants.DEFAULT_ENVIRONMENT
         } = (client && client.getOptions()) || {};
 
         // Will fetch userAgent if called from browser sdk
         const {
             userAgent
-        } = GLOBAL_OBJ.navigator || {};
+        } = utils.GLOBAL_OBJ.navigator || {};
 
-        const session = makeSession({
+        const session$1 = session.makeSession({
             release,
             environment,
             user: scope.getUser(),
             ...(userAgent && {
                 userAgent
             }),
             ...context,
         });
 
         // End existing session if there's one
         const currentSession = scope.getSession && scope.getSession();
         if (currentSession && currentSession.status === 'ok') {
-            updateSession(currentSession, {
+            session.updateSession(currentSession, {
                 status: 'exited'
             });
         }
         this.endSession();
 
         // Afterwards we set the new session on the scope
-        scope.setSession(session);
+        scope.setSession(session$1);
 
-        return session;
+        return session$1;
     }
 
     /**
      * Returns if default PII should be sent to Sentry and propagated in ourgoing requests
      * when Tracing is used.
      */
     shouldSendDefaultPii() {
@@ -428,21 +421,18 @@
      * Sends the current Session on the scope
      */
     _sendSessionUpdate() {
         const {
             scope,
             client
         } = this.getStackTop();
-        if (!scope) return;
 
         const session = scope.getSession();
-        if (session) {
-            if (client && client.captureSession) {
-                client.captureSession(session);
-            }
+        if (session && client && client.captureSession) {
+            client.captureSession(session);
         }
     }
 
     /**
      * Internal helper function to call a method on the top client if it exists.
      *
      * @param method The method to call on the client.
@@ -465,31 +455,31 @@
     // eslint-disable-next-line @typescript-eslint/no-explicit-any
     _callExtensionMethod(method, ...args) {
         const carrier = getMainCarrier();
         const sentry = carrier.__SENTRY__;
         if (sentry && sentry.extensions && typeof sentry.extensions[method] === 'function') {
             return sentry.extensions[method].apply(this, args);
         }
-        (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.warn(`Extension method ${method} couldn't be found, doing nothing.`);
+        (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.warn(`Extension method ${method} couldn't be found, doing nothing.`);
     }
 }
 
 /**
  * Returns the global shim registry.
  *
  * FIXME: This function is problematic, because despite always returning a valid Carrier,
  * it has an optional `__SENTRY__` property, which then in turn requires us to always perform an unnecessary check
  * at the call-site. We always access the carrier through this function, so we can guarantee that `__SENTRY__` is there.
  **/
 function getMainCarrier() {
-    GLOBAL_OBJ.__SENTRY__ = GLOBAL_OBJ.__SENTRY__ || {
+    utils.GLOBAL_OBJ.__SENTRY__ = utils.GLOBAL_OBJ.__SENTRY__ || {
         extensions: {},
         hub: undefined,
     };
-    return GLOBAL_OBJ;
+    return utils.GLOBAL_OBJ;
 }
 
 /**
  * Replaces the current main hub with the passed one on the global object
  *
  * @returns The old replaced hub
  */
@@ -507,71 +497,95 @@
  * contains a more recent version, it replaces the registered version.
  * Otherwise, the currently registered hub will be returned.
  */
 function getCurrentHub() {
     // Get main carrier (global for every environment)
     const registry = getMainCarrier();
 
+    if (registry.__SENTRY__ && registry.__SENTRY__.acs) {
+        const hub = registry.__SENTRY__.acs.getCurrentHub();
+
+        if (hub) {
+            return hub;
+        }
+    }
+
+    // Return hub that lives on a global object
+    return getGlobalHub(registry);
+}
+
+function getGlobalHub(registry = getMainCarrier()) {
     // If there's no hub, or its an old API, assign a new one
     if (!hasHubOnCarrier(registry) || getHubFromCarrier(registry).isOlderThan(API_VERSION)) {
         setHubOnCarrier(registry, new Hub());
     }
 
-    // Prefer domains over global if they are there (applicable only to Node environment)
-    if (isNodeEnv()) {
-        return getHubFromActiveDomain(registry);
-    }
     // Return hub that lives on a global object
     return getHubFromCarrier(registry);
 }
 
 /**
- * Try to read the hub from an active domain, and fallback to the registry if one doesn't exist
- * @returns discovered hub
+ * @private Private API with no semver guarantees!
+ *
+ * If the carrier does not contain a hub, a new hub is created with the global hub client and scope.
  */
-function getHubFromActiveDomain(registry) {
-    try {
-        const sentry = getMainCarrier().__SENTRY__;
-        const activeDomain = sentry && sentry.extensions && sentry.extensions.domain && sentry.extensions.domain.active;
-
-        // If there's no active domain, just return global hub
-        if (!activeDomain) {
-            return getHubFromCarrier(registry);
-        }
-
-        // If there's no hub on current domain, or it's an old API, assign a new one
-        if (!hasHubOnCarrier(activeDomain) || getHubFromCarrier(activeDomain).isOlderThan(API_VERSION)) {
-            const registryHubTopStack = getHubFromCarrier(registry).getStackTop();
-            setHubOnCarrier(activeDomain, new Hub(registryHubTopStack.client, Scope.clone(registryHubTopStack.scope)));
-        }
-
-        // Return hub that lives on a domain
-        return getHubFromCarrier(activeDomain);
-    } catch (_Oo) {
-        // Return hub that lives on a global object
-        return getHubFromCarrier(registry);
+function ensureHubOnCarrier(carrier, parent = getGlobalHub()) {
+    // If there's no hub on current domain, or it's an old API, assign a new one
+    if (!hasHubOnCarrier(carrier) || getHubFromCarrier(carrier).isOlderThan(API_VERSION)) {
+        const globalHubTopStack = parent.getStackTop();
+        setHubOnCarrier(carrier, new Hub(globalHubTopStack.client, scope.Scope.clone(globalHubTopStack.scope)));
     }
 }
 
 /**
+ * @private Private API with no semver guarantees!
+ *
+ * Sets the global async context strategy
+ */
+function setAsyncContextStrategy(strategy) {
+    // Get main carrier (global for every environment)
+    const registry = getMainCarrier();
+    registry.__SENTRY__ = registry.__SENTRY__ || {};
+    registry.__SENTRY__.acs = strategy;
+}
+
+/**
+ * Runs the supplied callback in its own async context. Async Context strategies are defined per SDK.
+ *
+ * @param callback The callback to run in its own async context
+ * @param options Options to pass to the async context strategy
+ * @returns The result of the callback
+ */
+function runWithAsyncContext(callback, options = {}) {
+    const registry = getMainCarrier();
+
+    if (registry.__SENTRY__ && registry.__SENTRY__.acs) {
+        return registry.__SENTRY__.acs.runWithAsyncContext(callback, options);
+    }
+
+    // if there was no strategy, fallback to just calling the callback
+    return callback();
+}
+
+/**
  * This will tell whether a carrier has a hub on it or not
  * @param carrier object
  */
 function hasHubOnCarrier(carrier) {
     return !!(carrier && carrier.__SENTRY__ && carrier.__SENTRY__.hub);
 }
 
 /**
  * This will create a new {@link Hub} and add to the passed object on
  * __SENTRY__.hub.
  * @param carrier object
  * @hidden
  */
 function getHubFromCarrier(carrier) {
-    return getGlobalSingleton('hub', () => new Hub(), carrier);
+    return utils.getGlobalSingleton('hub', () => new Hub(), carrier);
 }
 
 /**
  * This will set passed {@link Hub} on the passed object's __SENTRY__.hub attribute
  * @param carrier object
  * @param hub Hub
  * @returns A boolean indicating success or failure
@@ -579,17 +593,18 @@
 function setHubOnCarrier(carrier, hub) {
     if (!carrier) return false;
     const __SENTRY__ = (carrier.__SENTRY__ = carrier.__SENTRY__ || {});
     __SENTRY__.hub = hub;
     return true;
 }
 
-export {
-    API_VERSION,
-    Hub,
-    getCurrentHub,
-    getHubFromCarrier,
-    getMainCarrier,
-    makeMain,
-    setHubOnCarrier
-};
+exports.API_VERSION = API_VERSION;
+exports.Hub = Hub;
+exports.ensureHubOnCarrier = ensureHubOnCarrier;
+exports.getCurrentHub = getCurrentHub;
+exports.getHubFromCarrier = getHubFromCarrier;
+exports.getMainCarrier = getMainCarrier;
+exports.makeMain = makeMain;
+exports.runWithAsyncContext = runWithAsyncContext;
+exports.setAsyncContextStrategy = setAsyncContextStrategy;
+exports.setHubOnCarrier = setHubOnCarrier;
 //# sourceMappingURL=hub.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/index.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,21 @@
     setUser,
     startTransaction,
     withScope
 }
 from './exports.js';
 export {
     Hub,
+    ensureHubOnCarrier,
     getCurrentHub,
     getHubFromCarrier,
     getMainCarrier,
     makeMain,
+    runWithAsyncContext,
+    setAsyncContextStrategy,
     setHubOnCarrier
 }
 from './hub.js';
 export {
     closeSession,
     makeSession,
     updateSession
@@ -87,14 +90,18 @@
 }
 from './transports/base.js';
 export {
     makeOfflineTransport
 }
 from './transports/offline.js';
 export {
+    makeMultiplexedTransport
+}
+from './transports/multiplexed.js';
+export {
     SDK_VERSION
 }
 from './version.js';
 export {
     getIntegrationsToSetup
 }
 from './integration.js';
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/integration.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/integration.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/integrations/inboundfilters.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/integrations/inboundfilters.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/scope.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/scope.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -489,20 +489,27 @@
         // a trace context on the event. There is a product feature in place where we link
         // errors with transaction and it relies on that.
         if (this._span) {
             event.contexts = {
                 trace: this._span.getTraceContext(),
                 ...event.contexts
             };
-            const transactionName = this._span.transaction && this._span.transaction.name;
-            if (transactionName) {
-                event.tags = {
-                    transaction: transactionName,
-                    ...event.tags
+            const transaction = this._span.transaction;
+            if (transaction) {
+                event.sdkProcessingMetadata = {
+                    dynamicSamplingContext: transaction.getDynamicSamplingContext(),
+                    ...event.sdkProcessingMetadata,
                 };
+                const transactionName = transaction.name;
+                if (transactionName) {
+                    event.tags = {
+                        transaction: transactionName,
+                        ...event.tags
+                    };
+                }
             }
         }
 
         this._applyFingerprint(event);
 
         event.breadcrumbs = [...(event.breadcrumbs || []), ...this._breadcrumbs];
         event.breadcrumbs = event.breadcrumbs.length > 0 ? event.breadcrumbs : undefined;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/sdk.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/sdk.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/session.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/session.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/sessionflusher.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/sessionflusher.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/errors.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/errors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/hubextensions.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/hubextensions.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/idletransaction.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/idletransaction.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     logger,
-    timestampWithMs
+    timestampInSeconds
 } from '@sentry/utils';
 import {
     SpanRecorder
 } from './span.js';
 import {
     Transaction
 } from './transaction.js';
@@ -47,15 +47,15 @@
      */
     add(span) {
         // We should make sure we do not push and pop activities for
         // the transaction that this span recorder belongs to.
         if (span.spanId !== this.transactionSpanId) {
             // We patch span.finish() to pop an activity after setting an endTimestamp.
             span.finish = (endTimestamp) => {
-                span.endTimestamp = typeof endTimestamp === 'number' ? endTimestamp : timestampWithMs();
+                span.endTimestamp = typeof endTimestamp === 'number' ? endTimestamp : timestampInSeconds();
                 this._popActivity(span.spanId);
             };
 
             // We should only push new activities if the span does not have an end timestamp.
             if (span.endTimestamp === undefined) {
                 this._pushActivity(span.spanId);
             }
@@ -130,17 +130,14 @@
         IdleTransaction.prototype.__init.call(this);
         IdleTransaction.prototype.__init2.call(this);
         IdleTransaction.prototype.__init3.call(this);
         IdleTransaction.prototype.__init4.call(this);
         IdleTransaction.prototype.__init5.call(this);
         IdleTransaction.prototype.__init6.call(this);
         if (_onScope) {
-            // There should only be one active transaction on the scope
-            clearActiveTransaction(_idleHub);
-
             // We set the transaction here on the scope so error events pick up the trace
             // context and attach it to the error.
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.log(`Setting idle transaction on scope. Span ID: ${this.spanId}`);
             _idleHub.configureScope(scope => scope.setSpan(this));
         }
 
         this._restartIdleTimeout();
@@ -150,15 +147,15 @@
                 this._finishReason = IDLE_TRANSACTION_FINISH_REASONS[3];
                 this.finish();
             }
         }, this._finalTimeout);
     }
 
     /** {@inheritDoc} */
-    finish(endTimestamp = timestampWithMs()) {
+    finish(endTimestamp = timestampInSeconds()) {
         this._finished = true;
         this.activities = {};
 
         if (this.op === 'ui.action.click') {
             this.setTag(FINISH_REASON_TAG, this._finishReason);
         }
 
@@ -198,15 +195,18 @@
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.log('[Tracing] flushing IdleTransaction');
         } else {
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.log('[Tracing] No active IdleTransaction');
         }
 
         // if `this._onScope` is `true`, the transaction put itself on the scope when it started
         if (this._onScope) {
-            clearActiveTransaction(this._idleHub);
+            const scope = this._idleHub.getScope();
+            if (scope.getTransaction() === this) {
+                scope.setSpan(undefined);
+            }
         }
 
         return super.finish(endTimestamp);
     }
 
     /**
      * Register a callback function that gets excecuted before the transaction finishes.
@@ -321,21 +321,21 @@
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.log(`[Tracing] popActivity ${spanId}`);
             // eslint-disable-next-line @typescript-eslint/no-dynamic-delete
             delete this.activities[spanId];
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.log('[Tracing] new activities count', Object.keys(this.activities).length);
         }
 
         if (Object.keys(this.activities).length === 0) {
-            const endTimestamp = timestampWithMs();
+            const endTimestamp = timestampInSeconds();
             if (this._idleTimeoutCanceledPermanently) {
                 this._finishReason = IDLE_TRANSACTION_FINISH_REASONS[5];
                 this.finish(endTimestamp);
             } else {
                 // We need to add the timeout here to have the real endtimestamp of the transaction
-                // Remember timestampWithMs is in seconds, timeout is in ms
+                // Remember timestampInSeconds is in seconds, timeout is in ms
                 this._restartIdleTimeout(endTimestamp + this._idleTimeout / 1000);
             }
         }
     }
 
     /**
      * Checks when entries of this.activities are not changing for 3 beats.
@@ -374,23 +374,13 @@
         (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.log(`pinging Heartbeat -> current counter: ${this._heartbeatCounter}`);
         setTimeout(() => {
             this._beat();
         }, this._heartbeatInterval);
     }
 }
 
-/**
- * Reset transaction on scope to `undefined`
- */
-function clearActiveTransaction(hub) {
-    const scope = hub.getScope();
-    if (scope.getTransaction()) {
-        scope.setSpan(undefined);
-    }
-}
-
 export {
     IdleTransaction,
     IdleTransactionSpanRecorder,
     TRACING_DEFAULTS
 };
 //# sourceMappingURL=idletransaction.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/span.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/span.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     uuid4,
-    timestampWithMs,
+    timestampInSeconds,
     logger,
     dropUndefinedKeys
 } from '@sentry/utils';
 
 /**
  * Keeps track of finished spans for a given transaction
  * @internal
@@ -66,15 +66,15 @@
      * @inheritDoc
      */
 
     /**
      * Timestamp in seconds when the span was created.
      */
     __init4() {
-        this.startTimestamp = timestampWithMs();
+        this.startTimestamp = timestampInSeconds();
     }
 
     /**
      * Timestamp in seconds when the span ended.
      */
 
     /**
@@ -270,15 +270,15 @@
                 logMessage
             } = this.transaction.metadata.spanMetadata[this.spanId];
             if (logMessage) {
                 logger.log((logMessage).replace('Starting', 'Finishing'));
             }
         }
 
-        this.endTimestamp = typeof endTimestamp === 'number' ? endTimestamp : timestampWithMs();
+        this.endTimestamp = typeof endTimestamp === 'number' ? endTimestamp : timestampInSeconds();
     }
 
     /**
      * @inheritDoc
      */
     toTraceparent() {
         let sampledString = '';
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/spanstatus.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/spanstatus.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/trace.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/trace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/tracing/transaction.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/tracing/transaction.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/transports/base.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/transports/base.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/transports/offline.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/transports/offline.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/utils/hasTracingEnabled.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/utils/hasTracingEnabled.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/esm/utils/prepareEvent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/core/esm/utils/prepareEvent.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -44,15 +44,19 @@
         event_id: event.event_id || hint.event_id || uuid4(),
         timestamp: event.timestamp || dateTimestampInSeconds(),
     };
     const integrations = hint.integrations || options.integrations.map(i => i.name);
 
     applyClientOptions(prepared, options);
     applyIntegrationsMetadata(prepared, integrations);
-    applyDebugMetadata(prepared, options.stackParser);
+
+    // Only apply debug metadata to error events.
+    if (event.type === undefined) {
+        applyDebugMetadata(prepared, options.stackParser);
+    }
 
     // If we have scope given to us, use it as the base for further modifications.
     // This allows us to prevent unnecessary copying of data if `captureContext` is not provided.
     let finalScope = scope;
     if (hint.captureContext) {
         finalScope = Scope.clone(finalScope).update(hint.captureContext);
     }
@@ -126,28 +130,48 @@
 
     const request = event.request;
     if (request && request.url) {
         request.url = truncate(request.url, maxValueLength);
     }
 }
 
+const debugIdStackParserCache = new WeakMap();
+
 /**
  * Applies debug metadata images to the event in order to apply source maps by looking up their debug ID.
  */
 function applyDebugMetadata(event, stackParser) {
     const debugIdMap = GLOBAL_OBJ._sentryDebugIds;
 
     if (!debugIdMap) {
         return;
     }
 
+    let debugIdStackFramesCache;
+    const cachedDebugIdStackFrameCache = debugIdStackParserCache.get(stackParser);
+    if (cachedDebugIdStackFrameCache) {
+        debugIdStackFramesCache = cachedDebugIdStackFrameCache;
+    } else {
+        debugIdStackFramesCache = new Map();
+        debugIdStackParserCache.set(stackParser, debugIdStackFramesCache);
+    }
+
     // Build a map of filename -> debug_id
     const filenameDebugIdMap = Object.keys(debugIdMap).reduce((acc, debugIdStackTrace) => {
-        const parsedStack = stackParser(debugIdStackTrace);
-        for (const stackFrame of parsedStack) {
+        let parsedStack;
+        const cachedParsedStack = debugIdStackFramesCache.get(debugIdStackTrace);
+        if (cachedParsedStack) {
+            parsedStack = cachedParsedStack;
+        } else {
+            parsedStack = stackParser(debugIdStackTrace);
+            debugIdStackFramesCache.set(debugIdStackTrace, parsedStack);
+        }
+
+        for (let i = parsedStack.length - 1; i >= 0; i--) {
+            const stackFrame = parsedStack[i];
             if (stackFrame.filename) {
                 acc[stackFrame.filename] = debugIdMap[debugIdStackTrace];
                 break;
             }
         }
         return acc;
     }, {});
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/modules/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/modules/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/tslib.es6.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/tslib.es6.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/node_modules/tslib/tslib.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/tslib/tslib.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/core/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7833333333333333%*

 * *Differences: {"'dependencies'": "{'@sentry/types': '7.50.0', delete: ['@sentry/utils']}",*

 * * "'description'": "'Utilities for all Sentry JavaScript SDKs'",*

 * * "'devDependencies'": "OrderedDict([('@types/array.prototype.flat', '^1.2.1'), "*

 * *                      "('array.prototype.flat', '^1.3.0'), ('chai', '^4.1.2')])",*

 * * "'homepage'": "'https://github.com/getsentry/sentry-javascript/tree/master/packages/utils'",*

 * * "'name'": "'@sentry/utils'",*

 * * "'version'": "'7.50.0'"}*

```diff
@@ -1,24 +1,28 @@
 {
     "author": "Sentry",
     "dependencies": {
-        "@sentry/types": "7.46.0",
-        "@sentry/utils": "7.46.0",
+        "@sentry/types": "7.50.0",
         "tslib": "^1.9.3"
     },
-    "description": "Base implementation for all Sentry JavaScript SDKs",
+    "description": "Utilities for all Sentry JavaScript SDKs",
+    "devDependencies": {
+        "@types/array.prototype.flat": "^1.2.1",
+        "array.prototype.flat": "^1.3.0",
+        "chai": "^4.1.2"
+    },
     "engines": {
         "node": ">=8"
     },
-    "homepage": "https://github.com/getsentry/sentry-javascript/tree/master/packages/core",
+    "homepage": "https://github.com/getsentry/sentry-javascript/tree/master/packages/utils",
     "license": "MIT",
     "main": "cjs/index.js",
     "module": "esm/index.js",
-    "name": "@sentry/core",
+    "name": "@sentry/utils",
     "publishConfig": {
         "access": "public"
     },
     "repository": "git://github.com/getsentry/sentry-javascript.git",
     "sideEffects": false,
     "types": "types/index.d.ts",
-    "version": "7.46.0"
+    "version": "7.50.0"
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/client.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/client.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/eventbuilder.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/eventbuilder.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/handlers.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/handlers.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,14 @@
 
 Object.defineProperty(exports, '__esModule', {
     value: true
 });
 
 const core = require('@sentry/core');
 const utils = require('@sentry/utils');
-const domain = require('domain');
 const requestdata = require('./requestdata.js');
 const sdk = require('./sdk.js');
 const requestDataDeprecated = require('./requestDataDeprecated.js');
 
 /* eslint-disable @typescript-eslint/no-explicit-any */
 
 /**
@@ -180,21 +179,16 @@
                     })
                     .then(null, e => {
                         (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.error(e);
                         _end.call(this, chunk, encoding, cb);
                     });
             };
         }
-        const local = domain.create();
-        local.add(req);
-        local.add(res);
-
-        local.run(() => {
+        core.runWithAsyncContext(() => {
             const currentHub = core.getCurrentHub();
-
             currentHub.configureScope(scope => {
                 scope.setSDKProcessingMetadata({
                     request: req,
                     // TODO (v8): Stop passing this
                     requestDataOptionsFromExpressHandler: requestDataOptions,
                 });
 
@@ -310,27 +304,27 @@
 
 /**
  * Sentry tRPC middleware that names the handling transaction after the called procedure.
  *
  * Use the Sentry tRPC middleware in combination with the Sentry server integration,
  * e.g. Express Request Handlers or Next.js SDK.
  */
-async function trpcMiddleware(options = {}) {
+function trpcMiddleware(options = {}) {
     return function({
         path,
         type,
         next,
         rawInput
     }) {
         const hub = core.getCurrentHub();
         const clientOptions = _optionalChain([hub, 'access', _13 => _13.getClient, 'call', _14 => _14(), 'optionalAccess', _15 => _15.getOptions, 'call', _16 => _16()]);
         const sentryTransaction = _optionalChain([hub, 'access', _17 => _17.getScope, 'call', _18 => _18(), 'optionalAccess', _19 => _19.getTransaction, 'call', _20 => _20()]);
 
         if (sentryTransaction) {
-            sentryTransaction.setName(`trcp/${path}`, 'route');
+            sentryTransaction.setName(`trpc/${path}`, 'route');
             sentryTransaction.op = 'rpc.server';
 
             const trpcContext = {
                 procedure_type: type,
             };
 
             if (options.attachRpcInput !== undefined ? options.attachRpcInput : _optionalChain([clientOptions, 'optionalAccess', _21 => _21.sendDefaultPii])) {
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/index.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -5,33 +5,24 @@
 const core = require('@sentry/core');
 const index = require('./tracing/index.js');
 const client = require('./client.js');
 const http = require('./transports/http.js');
 const sdk = require('./sdk.js');
 const requestdata = require('./requestdata.js');
 const utils = require('./utils.js');
-const domain = require('domain');
 const handlers = require('./handlers.js');
 const index$1 = require('./integrations/index.js');
 const integrations = require('./tracing/integrations.js');
 
 const INTEGRATIONS = {
     ...core.Integrations,
     ...index$1,
     ...integrations,
 };
 
-// We need to patch domain on the global __SENTRY__ object to make it work for node in cross-platform packages like
-// @sentry/core. If we don't do this, browser bundlers will have troubles resolving `require('domain')`.
-const carrier = core.getMainCarrier();
-if (carrier.__SENTRY__) {
-    carrier.__SENTRY__.extensions = carrier.__SENTRY__.extensions || {};
-    carrier.__SENTRY__.extensions.domain = carrier.__SENTRY__.extensions.domain || domain;
-}
-
 exports.Hub = core.Hub;
 exports.SDK_VERSION = core.SDK_VERSION;
 exports.Scope = core.Scope;
 exports.addBreadcrumb = core.addBreadcrumb;
 exports.addGlobalEventProcessor = core.addGlobalEventProcessor;
 exports.captureEvent = core.captureEvent;
 exports.captureException = core.captureException;
@@ -39,14 +30,15 @@
 exports.configureScope = core.configureScope;
 exports.createTransport = core.createTransport;
 exports.extractTraceparentData = core.extractTraceparentData;
 exports.getActiveTransaction = core.getActiveTransaction;
 exports.getCurrentHub = core.getCurrentHub;
 exports.getHubFromCarrier = core.getHubFromCarrier;
 exports.makeMain = core.makeMain;
+exports.runWithAsyncContext = core.runWithAsyncContext;
 exports.setContext = core.setContext;
 exports.setExtra = core.setExtra;
 exports.setExtras = core.setExtras;
 exports.setTag = core.setTag;
 exports.setTags = core.setTags;
 exports.setUser = core.setUser;
 exports.spanStatusfromHttpCode = core.spanStatusfromHttpCode;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/console.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/console.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/context.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/context.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/contextlines.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/contextlines.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/http.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/http.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,18 +5,17 @@
 Object.defineProperty(exports, '__esModule', {
     value: true
 });
 
 const core = require('@sentry/core');
 const utils = require('@sentry/utils');
 const lru_map = require('lru_map');
+const nodeVersion = require('../nodeVersion.js');
 const http = require('./utils/http.js');
 
-const NODE_VERSION = utils.parseSemver(process.versions.node);
-
 /**
  * The http module integration instruments Node's internal http module. It creates breadcrumbs, transactions for outgoing
  * http requests and attaches trace data when tracing is enabled via its `tracing` option.
  */
 class Http {
     /**
      * @inheritDoc
@@ -73,15 +72,15 @@
         const wrappedHttpHandlerMaker = _createWrappedRequestMethodFactory(this._breadcrumbs, tracingOptions, httpModule);
         utils.fill(httpModule, 'get', wrappedHttpHandlerMaker);
         utils.fill(httpModule, 'request', wrappedHttpHandlerMaker);
 
         // NOTE: Prior to Node 9, `https` used internals of `http` module, thus we don't patch it.
         // If we do, we'd get double breadcrumbs and double spans for `https` calls.
         // It has been changed in Node 9, so for all versions equal and above, we patch `https` separately.
-        if (NODE_VERSION.major && NODE_VERSION.major > 8) {
+        if (nodeVersion.NODE_VERSION.major && nodeVersion.NODE_VERSION.major > 8) {
             // eslint-disable-next-line @typescript-eslint/no-var-requires
             const httpsModule = require('https');
             const wrappedHttpsHandlerMaker = _createWrappedRequestMethodFactory(
                 this._breadcrumbs,
                 tracingOptions,
                 httpsModule,
             );
@@ -275,15 +274,14 @@
     if (!core.getCurrentHub().getIntegration(Http)) {
         return;
     }
 
     core.getCurrentHub().addBreadcrumb({
         category: 'http',
         data: {
-            method: req.method,
             status_code: res && res.statusCode,
             ...requestSpanData,
         },
         type: 'http',
     }, {
         event,
         request: req,
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/linkederrors.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/linkederrors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/localvariables.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/localvariables.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,17 @@
     _optionalChain
 } = require('@sentry/utils/cjs/buildPolyfills');
 
 Object.defineProperty(exports, '__esModule', {
     value: true
 });
 
+const utils = require('@sentry/utils');
 const lru_map = require('lru_map');
+const nodeVersion = require('../nodeVersion.js');
 
 /** Creates a container for callbacks to be called sequentially */
 function createCallbackList(complete) {
     // A collection of callbacks to be executed last to first
     let callbacks = [];
 
     let completedCalled = false;
@@ -267,14 +269,23 @@
 
     /** Setup in a way that's easier to call from tests */
     _setup(
         addGlobalEventProcessor,
         clientOptions,
     ) {
         if (this._session && _optionalChain([clientOptions, 'optionalAccess', _29 => _29.includeLocalVariables])) {
+            // Only setup this integration if the Node version is >= v18
+            // https://github.com/getsentry/sentry-javascript/issues/7697
+            const unsupportedNodeVersion = (nodeVersion.NODE_VERSION.major || 0) < 18;
+
+            if (unsupportedNodeVersion) {
+                utils.logger.log('The `LocalVariables` integration is only supported on Node >= v18.');
+                return;
+            }
+
             this._session.configureAndConnect(
                 (ev, complete) =>
                 this._handlePaused(clientOptions.stackParser, ev, complete),
                 !!this._options.captureAllExceptions,
             );
 
             addGlobalEventProcessor(async event => this._addLocalVariables(event));
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/modules.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/modules.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/onuncaughtexception.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/onuncaughtexception.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/onunhandledrejection.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/onunhandledrejection.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/requestdata.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/undici/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/undici/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,15 @@
 Object.defineProperty(exports, '__esModule', {
     value: true
 });
 
 const utils = require('@sentry/utils');
+const nodeVersion = require('../../nodeVersion.js');
 const http = require('../utils/http.js');
 
-const NODE_VERSION = utils.parseSemver(process.versions.node);
-
 exports.ChannelName = void 0;
 (function(ChannelName) {
     // https://github.com/nodejs/undici/blob/e6fc80f809d1217814c044f52ed40ef13f21e43c/docs/api/DiagnosticsChannel.md#undicirequestcreate
     const RequestCreate = 'undici:request:create';
     ChannelName["RequestCreate"] = RequestCreate;
     const RequestEnd = 'undici:request:headers';
     ChannelName["RequestEnd"] = RequestEnd;
@@ -54,15 +53,15 @@
     }
 
     /**
      * @inheritDoc
      */
     setupOnce(_addGlobalEventProcessor, getCurrentHub) {
         // Requires Node 16+ to use the diagnostics_channel API.
-        if (NODE_VERSION.major && NODE_VERSION.major < 16) {
+        if (nodeVersion.NODE_VERSION.major && nodeVersion.NODE_VERSION.major < 16) {
             return;
         }
 
         let ds;
         try {
             // eslint-disable-next-line @typescript-eslint/no-var-requires
             ds = utils.dynamicRequire(module, 'diagnostics_channel');
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/errorhandling.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/errorhandling.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/http.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/http.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -3,18 +3,16 @@
 } = require('@sentry/utils/cjs/buildPolyfills');
 
 Object.defineProperty(exports, '__esModule', {
     value: true
 });
 
 const core = require('@sentry/core');
-const utils = require('@sentry/utils');
 const url = require('url');
-
-const NODE_VERSION = utils.parseSemver(process.versions.node);
+const nodeVersion = require('../../nodeVersion.js');
 
 /**
  * Checks whether given url points to Sentry server
  * @param url url to verify
  */
 function isSentryRequest(url) {
     const dsn = _optionalChain([core.getCurrentHub, 'call', _ => _(), 'access', _2 => _2.getClient, 'call', _3 => _3(), 'optionalAccess', _4 => _4.getDsn, 'call', _5 => _5()]);
@@ -48,19 +46,25 @@
 function extractUrl(requestOptions) {
     const protocol = requestOptions.protocol || '';
     const hostname = requestOptions.hostname || requestOptions.host || '';
     // Don't log standard :80 (http) and :443 (https) ports to reduce the noise
     const port = !requestOptions.port || requestOptions.port === 80 || requestOptions.port === 443 ? '' : `:${requestOptions.port}`;
     // do not include search or hash in span descriptions, per https://develop.sentry.dev/sdk/data-handling/#structuring-data
     const path = requestOptions.pathname || '/';
-    const authority = requestOptions.auth ? `${requestOptions.auth}@` : '';
+    // always filter authority, see https://develop.sentry.dev/sdk/data-handling/#structuring-data
+    const authority = requestOptions.auth ? redactAuthority(requestOptions.auth) : '';
 
     return `${protocol}//${authority}${hostname}${port}${path}`;
 }
 
+function redactAuthority(auth) {
+    const [user, password] = auth.split(':');
+    return `${user ? '[Filtered]' : ''}:${password ? '[Filtered]' : ''}@`;
+}
+
 /**
  * Handle various edge cases in the span description (for spans representing http(s) requests).
  *
  * @param description current `description` property of the span representing the request
  * @param requestOptions Configuration data for the request
  * @param Request Request object
  *
@@ -116,16 +120,15 @@
         path: `${url.pathname || ''}${url.search || ''}`,
         href: url.href,
     };
     if (url.port !== '') {
         options.port = Number(url.port);
     }
     if (url.username || url.password) {
-        // always filter authority, see https://develop.sentry.dev/sdk/data-handling/#structuring-data
-        options.auth = '[Filtered]:[Filtered]';
+        options.auth = `${url.username}:${url.password}`;
     }
     return options;
 }
 
 /**
  * Normalize inputs to `http(s).request()` and `http(s).get()`.
  *
@@ -177,15 +180,15 @@
         /* eslint-disable @typescript-eslint/no-unsafe-member-access, @typescript-eslint/no-explicit-any */
 
         // NOTE: Prior to Node 9, `https` used internals of `http` module, thus we don't patch it.
         // Because of that, we cannot rely on `httpModule` to provide us with valid protocol,
         // as it will always return `http`, even when using `https` module.
         //
         // See test/integrations/http.test.ts for more details on Node <=v8 protocol issue.
-        if (NODE_VERSION.major && NODE_VERSION.major > 8) {
+        if (nodeVersion.NODE_VERSION.major && nodeVersion.NODE_VERSION.major > 8) {
             requestOptions.protocol =
                 _optionalChain([(_optionalChain([httpModule, 'optionalAccess', _10 => _10.globalAgent])), 'optionalAccess', _11 => _11.protocol]) ||
                 _optionalChain([(requestOptions.agent), 'optionalAccess', _12 => _12.protocol]) ||
                 _optionalChain([(requestOptions._defaultAgent), 'optionalAccess', _13 => _13.protocol]);
         } else {
             requestOptions.protocol =
                 _optionalChain([(requestOptions.agent), 'optionalAccess', _14 => _14.protocol]) ||
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/module.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/module.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/requestDataDeprecated.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/requestDataDeprecated.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/requestdata.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/sdk.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/sdk.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -4,39 +4,40 @@
 
 Object.defineProperty(exports, '__esModule', {
     value: true
 });
 
 const core = require('@sentry/core');
 const utils = require('@sentry/utils');
-const domain = require('domain');
+const index$1 = require('./async/index.js');
 const client = require('./client.js');
 const console = require('./integrations/console.js');
 const http = require('./integrations/http.js');
 const onuncaughtexception = require('./integrations/onuncaughtexception.js');
 const onunhandledrejection = require('./integrations/onunhandledrejection.js');
 const linkederrors = require('./integrations/linkederrors.js');
 const modules = require('./integrations/modules.js');
 const contextlines = require('./integrations/contextlines.js');
 const context = require('./integrations/context.js');
 const requestdata = require('./integrations/requestdata.js');
 const localvariables = require('./integrations/localvariables.js');
-require('./integrations/undici/index.js');
+const index = require('./integrations/undici/index.js');
 const module$1 = require('./module.js');
 const http$1 = require('./transports/http.js');
 
 /* eslint-disable max-lines */
 
 const defaultIntegrations = [
     // Common
     new core.Integrations.InboundFilters(),
     new core.Integrations.FunctionToString(),
     // Native Wrappers
     new console.Console(),
     new http.Http(),
+    new index.Undici(),
     // Global Handlers
     new onuncaughtexception.OnUncaughtException(),
     new onunhandledrejection.OnUnhandledRejection(),
     // Event Info
     new contextlines.ContextLines(),
     new localvariables.LocalVariables(),
     new context.Context(),
@@ -99,14 +100,17 @@
  * });
  * ```
  *
  * @see {@link NodeOptions} for documentation on configuration options.
  */
 function init(options = {}) {
     const carrier = core.getMainCarrier();
+
+    index$1.setNodeAsyncContextStrategy();
+
     const autoloadedIntegrations = _optionalChain([carrier, 'access', _ => _.__SENTRY__, 'optionalAccess', _2 => _2.integrations]) || [];
 
     options.defaultIntegrations =
         options.defaultIntegrations === false ?
         [] :
         [
             ...(Array.isArray(options.defaultIntegrations) ? options.defaultIntegrations : defaultIntegrations),
@@ -142,19 +146,14 @@
         options.autoSessionTracking = true;
     }
 
     if (options.instrumenter === undefined) {
         options.instrumenter = 'sentry';
     }
 
-    // eslint-disable-next-line @typescript-eslint/no-unsafe-member-access, @typescript-eslint/no-explicit-any
-    if ((domain).active) {
-        core.setHubOnCarrier(carrier, core.getCurrentHub());
-    }
-
     // TODO(v7): Refactor this to reduce the logic above
     const clientOptions = {
         ...options,
         stackParser: utils.stackParserFromStackParserOptions(options.stackParser || defaultStackParser),
         integrations: core.getIntegrationsToSetup(options),
         transport: options.transport || http$1.makeNodeTransport,
     };
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/tracing/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/tracing/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/transports/http.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/transports/http.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/cjs/utils.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/cjs/utils.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -27,18 +27,19 @@
     // deals in absolute paths rather than relative ones). We need this to be separate from the outer function to preserve
     // the difference between `targetDirAbsPath` and `currentDirAbsPath`.
     const deepReadCurrentDir = (currentDirAbsPath) => {
         return fs.readdirSync(currentDirAbsPath).reduce((absPaths, itemName) => {
             const itemAbsPath = path.join(currentDirAbsPath, itemName);
 
             if (fs.statSync(itemAbsPath).isDirectory()) {
-                return [...absPaths, ...deepReadCurrentDir(itemAbsPath)];
+                return absPaths.concat(deepReadCurrentDir(itemAbsPath));
             }
 
-            return [...absPaths, itemAbsPath];
+            absPaths.push(itemAbsPath);
+            return absPaths;
         }, []);
     };
 
     return deepReadCurrentDir(targetDirAbsPath).map(absPath => path.relative(targetDirAbsPath, absPath));
 }
 
 exports.deepReadDirSync = deepReadDirSync;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/client.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/client.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/eventbuilder.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/eventbuilder.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/handlers.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/handlers.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
 import {
     _optionalChain
 } from '@sentry/utils/esm/buildPolyfills';
 import {
     getCurrentHub,
     hasTracingEnabled,
     startTransaction,
+    runWithAsyncContext,
     withScope,
     captureException
 } from '@sentry/core';
 import {
     logger,
     isString,
     extractTraceparentData,
     baggageHeaderToDynamicSamplingContext,
     extractPathForTransaction,
     addRequestDataToTransaction,
     normalize,
     dropUndefinedKeys
 } from '@sentry/utils';
-import * as domain from 'domain';
 import {
     extractRequestData
 } from './requestdata.js';
 import {
     isAutoSessionTrackingEnabled,
     flush
 } from './sdk.js';
@@ -199,21 +199,16 @@
                     })
                     .then(null, e => {
                         (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.error(e);
                         _end.call(this, chunk, encoding, cb);
                     });
             };
         }
-        const local = domain.create();
-        local.add(req);
-        local.add(res);
-
-        local.run(() => {
+        runWithAsyncContext(() => {
             const currentHub = getCurrentHub();
-
             currentHub.configureScope(scope => {
                 scope.setSDKProcessingMetadata({
                     request: req,
                     // TODO (v8): Stop passing this
                     requestDataOptionsFromExpressHandler: requestDataOptions,
                 });
 
@@ -329,27 +324,27 @@
 
 /**
  * Sentry tRPC middleware that names the handling transaction after the called procedure.
  *
  * Use the Sentry tRPC middleware in combination with the Sentry server integration,
  * e.g. Express Request Handlers or Next.js SDK.
  */
-async function trpcMiddleware(options = {}) {
+function trpcMiddleware(options = {}) {
     return function({
         path,
         type,
         next,
         rawInput
     }) {
         const hub = getCurrentHub();
         const clientOptions = _optionalChain([hub, 'access', _13 => _13.getClient, 'call', _14 => _14(), 'optionalAccess', _15 => _15.getOptions, 'call', _16 => _16()]);
         const sentryTransaction = _optionalChain([hub, 'access', _17 => _17.getScope, 'call', _18 => _18(), 'optionalAccess', _19 => _19.getTransaction, 'call', _20 => _20()]);
 
         if (sentryTransaction) {
-            sentryTransaction.setName(`trcp/${path}`, 'route');
+            sentryTransaction.setName(`trpc/${path}`, 'route');
             sentryTransaction.op = 'rpc.server';
 
             const trpcContext = {
                 procedure_type: type,
             };
 
             if (options.attachRpcInput !== undefined ? options.attachRpcInput : _optionalChain([clientOptions, 'optionalAccess', _21 => _21.sendDefaultPii])) {
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/console.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/console.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/context.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/context.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/contextlines.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/contextlines.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/http.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/http.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,33 +1,33 @@
 import {
     _optionalChain
 } from '@sentry/utils/esm/buildPolyfills';
 import {
     getCurrentHub
 } from '@sentry/core';
 import {
-    parseSemver,
     logger,
     fill,
     dynamicSamplingContextToSentryBaggageHeader,
     stringMatchesSomePattern
 } from '@sentry/utils';
 import {
     LRUMap
 } from 'lru_map';
 import {
+    NODE_VERSION
+} from '../nodeVersion.js';
+import {
     normalizeRequestArgs,
     extractRawUrl,
     extractUrl,
     isSentryRequest,
     cleanSpanDescription
 } from './utils/http.js';
 
-const NODE_VERSION = parseSemver(process.versions.node);
-
 /**
  * The http module integration instruments Node's internal http module. It creates breadcrumbs, transactions for outgoing
  * http requests and attaches trace data when tracing is enabled via its `tracing` option.
  */
 class Http {
     /**
      * @inheritDoc
@@ -286,15 +286,14 @@
     if (!getCurrentHub().getIntegration(Http)) {
         return;
     }
 
     getCurrentHub().addBreadcrumb({
         category: 'http',
         data: {
-            method: req.method,
             status_code: res && res.statusCode,
             ...requestSpanData,
         },
         type: 'http',
     }, {
         event,
         request: req,
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/linkederrors.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/linkederrors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/localvariables.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/localvariables.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,19 @@
 import {
     _optionalChain
 } from '@sentry/utils/esm/buildPolyfills';
 import {
+    logger
+} from '@sentry/utils';
+import {
     LRUMap
 } from 'lru_map';
+import {
+    NODE_VERSION
+} from '../nodeVersion.js';
 
 /** Creates a container for callbacks to be called sequentially */
 function createCallbackList(complete) {
     // A collection of callbacks to be executed last to first
     let callbacks = [];
 
     let completedCalled = false;
@@ -264,14 +270,23 @@
 
     /** Setup in a way that's easier to call from tests */
     _setup(
         addGlobalEventProcessor,
         clientOptions,
     ) {
         if (this._session && _optionalChain([clientOptions, 'optionalAccess', _29 => _29.includeLocalVariables])) {
+            // Only setup this integration if the Node version is >= v18
+            // https://github.com/getsentry/sentry-javascript/issues/7697
+            const unsupportedNodeVersion = (NODE_VERSION.major || 0) < 18;
+
+            if (unsupportedNodeVersion) {
+                logger.log('The `LocalVariables` integration is only supported on Node >= v18.');
+                return;
+            }
+
             this._session.configureAndConnect(
                 (ev, complete) =>
                 this._handlePaused(clientOptions.stackParser, ev, complete),
                 !!this._options.captureAllExceptions,
             );
 
             addGlobalEventProcessor(async event => this._addLocalVariables(event));
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/modules.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/modules.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/onuncaughtexception.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/onuncaughtexception.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/onunhandledrejection.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/onunhandledrejection.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/requestdata.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/undici/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/undici/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 import {
-    parseSemver,
     dynamicRequire,
     stripUrlQueryAndFragment,
     stringMatchesSomePattern,
     dynamicSamplingContextToSentryBaggageHeader
 } from '@sentry/utils';
 import {
+    NODE_VERSION
+} from '../../nodeVersion.js';
+import {
     isSentryRequest
 } from '../utils/http.js';
 
-const NODE_VERSION = parseSemver(process.versions.node);
-
 var ChannelName;
 (function(ChannelName) {
     // https://github.com/nodejs/undici/blob/e6fc80f809d1217814c044f52ed40ef13f21e43c/docs/api/DiagnosticsChannel.md#undicirequestcreate
     const RequestCreate = 'undici:request:create';
     ChannelName["RequestCreate"] = RequestCreate;
     const RequestEnd = 'undici:request:headers';
     ChannelName["RequestEnd"] = RequestEnd;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/errorhandling.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/errorhandling.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/http.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/http.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,19 @@
 import {
     _optionalChain
 } from '@sentry/utils/esm/buildPolyfills';
 import {
     getCurrentHub
 } from '@sentry/core';
 import {
-    parseSemver
-} from '@sentry/utils';
-import {
     URL
 } from 'url';
-
-const NODE_VERSION = parseSemver(process.versions.node);
+import {
+    NODE_VERSION
+} from '../../nodeVersion.js';
 
 /**
  * Checks whether given url points to Sentry server
  * @param url url to verify
  */
 function isSentryRequest(url) {
     const dsn = _optionalChain([getCurrentHub, 'call', _ => _(), 'access', _2 => _2.getClient, 'call', _3 => _3(), 'optionalAccess', _4 => _4.getDsn, 'call', _5 => _5()]);
@@ -49,19 +47,25 @@
 function extractUrl(requestOptions) {
     const protocol = requestOptions.protocol || '';
     const hostname = requestOptions.hostname || requestOptions.host || '';
     // Don't log standard :80 (http) and :443 (https) ports to reduce the noise
     const port = !requestOptions.port || requestOptions.port === 80 || requestOptions.port === 443 ? '' : `:${requestOptions.port}`;
     // do not include search or hash in span descriptions, per https://develop.sentry.dev/sdk/data-handling/#structuring-data
     const path = requestOptions.pathname || '/';
-    const authority = requestOptions.auth ? `${requestOptions.auth}@` : '';
+    // always filter authority, see https://develop.sentry.dev/sdk/data-handling/#structuring-data
+    const authority = requestOptions.auth ? redactAuthority(requestOptions.auth) : '';
 
     return `${protocol}//${authority}${hostname}${port}${path}`;
 }
 
+function redactAuthority(auth) {
+    const [user, password] = auth.split(':');
+    return `${user ? '[Filtered]' : ''}:${password ? '[Filtered]' : ''}@`;
+}
+
 /**
  * Handle various edge cases in the span description (for spans representing http(s) requests).
  *
  * @param description current `description` property of the span representing the request
  * @param requestOptions Configuration data for the request
  * @param Request Request object
  *
@@ -117,16 +121,15 @@
         path: `${url.pathname || ''}${url.search || ''}`,
         href: url.href,
     };
     if (url.port !== '') {
         options.port = Number(url.port);
     }
     if (url.username || url.password) {
-        // always filter authority, see https://develop.sentry.dev/sdk/data-handling/#structuring-data
-        options.auth = '[Filtered]:[Filtered]';
+        options.auth = `${url.username}:${url.password}`;
     }
     return options;
 }
 
 /**
  * Normalize inputs to `http(s).request()` and `http(s).get()`.
  *
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/module.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/module.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/requestDataDeprecated.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/requestDataDeprecated.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/requestdata.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/sdk.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/sdk.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,27 @@
 import {
     _optionalChain
 } from '@sentry/utils/esm/buildPolyfills';
 import {
     Integrations,
     getMainCarrier,
-    setHubOnCarrier,
-    getCurrentHub,
     getIntegrationsToSetup,
-    initAndBind
+    initAndBind,
+    getCurrentHub
 } from '@sentry/core';
 import {
     createStackParser,
     nodeStackLineParser,
     stackParserFromStackParserOptions,
     logger,
     GLOBAL_OBJ
 } from '@sentry/utils';
-import * as domain from 'domain';
+import {
+    setNodeAsyncContextStrategy
+} from './async/index.js';
 import {
     NodeClient
 } from './client.js';
 import {
     Console
 } from './integrations/console.js';
 import {
@@ -46,15 +47,17 @@
 } from './integrations/context.js';
 import {
     RequestData
 } from './integrations/requestdata.js';
 import {
     LocalVariables
 } from './integrations/localvariables.js';
-import './integrations/undici/index.js';
+import {
+    Undici
+} from './integrations/undici/index.js';
 import {
     getModule
 } from './module.js';
 import {
     makeNodeTransport
 } from './transports/http.js';
 
@@ -63,14 +66,15 @@
 const defaultIntegrations = [
     // Common
     new Integrations.InboundFilters(),
     new Integrations.FunctionToString(),
     // Native Wrappers
     new Console(),
     new Http(),
+    new Undici(),
     // Global Handlers
     new OnUncaughtException(),
     new OnUnhandledRejection(),
     // Event Info
     new ContextLines(),
     new LocalVariables(),
     new Context(),
@@ -133,14 +137,17 @@
  * });
  * ```
  *
  * @see {@link NodeOptions} for documentation on configuration options.
  */
 function init(options = {}) {
     const carrier = getMainCarrier();
+
+    setNodeAsyncContextStrategy();
+
     const autoloadedIntegrations = _optionalChain([carrier, 'access', _ => _.__SENTRY__, 'optionalAccess', _2 => _2.integrations]) || [];
 
     options.defaultIntegrations =
         options.defaultIntegrations === false ?
         [] :
         [
             ...(Array.isArray(options.defaultIntegrations) ? options.defaultIntegrations : defaultIntegrations),
@@ -176,19 +183,14 @@
         options.autoSessionTracking = true;
     }
 
     if (options.instrumenter === undefined) {
         options.instrumenter = 'sentry';
     }
 
-    // eslint-disable-next-line @typescript-eslint/no-unsafe-member-access, @typescript-eslint/no-explicit-any
-    if ((domain).active) {
-        setHubOnCarrier(carrier, getCurrentHub());
-    }
-
     // TODO(v7): Refactor this to reduce the logic above
     const clientOptions = {
         ...options,
         stackParser: stackParserFromStackParserOptions(options.stackParser || defaultStackParser),
         integrations: getIntegrationsToSetup(options),
         transport: options.transport || makeNodeTransport,
     };
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/tracing/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/tracing/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/transports/http.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/transports/http.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/esm/utils.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/esm/utils.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -23,18 +23,19 @@
     // deals in absolute paths rather than relative ones). We need this to be separate from the outer function to preserve
     // the difference between `targetDirAbsPath` and `currentDirAbsPath`.
     const deepReadCurrentDir = (currentDirAbsPath) => {
         return fs.readdirSync(currentDirAbsPath).reduce((absPaths, itemName) => {
             const itemAbsPath = path.join(currentDirAbsPath, itemName);
 
             if (fs.statSync(itemAbsPath).isDirectory()) {
-                return [...absPaths, ...deepReadCurrentDir(itemAbsPath)];
+                return absPaths.concat(deepReadCurrentDir(itemAbsPath));
             }
 
-            return [...absPaths, itemAbsPath];
+            absPaths.push(itemAbsPath);
+            return absPaths;
         }, []);
     };
 
     return deepReadCurrentDir(targetDirAbsPath).map(absPath => path.relative(targetDirAbsPath, absPath));
 }
 
 export {
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/node/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/node/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8916666666666667%*

 * *Differences: {"'dependencies'": "{'@sentry-internal/tracing': '7.50.0', '@sentry/core': '7.50.0', "*

 * *                   "'@sentry/types': '7.50.0', '@sentry/utils': '7.50.0'}",*

 * * "'sideEffects'": 'False',*

 * * "'version'": "'7.50.0'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Sentry",
     "dependencies": {
-        "@sentry-internal/tracing": "7.46.0",
-        "@sentry/core": "7.46.0",
-        "@sentry/types": "7.46.0",
-        "@sentry/utils": "7.46.0",
+        "@sentry-internal/tracing": "7.50.0",
+        "@sentry/core": "7.50.0",
+        "@sentry/types": "7.50.0",
+        "@sentry/utils": "7.50.0",
         "cookie": "^0.4.1",
         "https-proxy-agent": "^5.0.0",
         "lru_map": "^0.3.3",
         "tslib": "^1.9.3"
     },
     "description": "Official Sentry SDK for Node.js",
     "devDependencies": {
@@ -28,10 +28,11 @@
     "main": "cjs/index.js",
     "module": "esm/index.js",
     "name": "@sentry/node",
     "publishConfig": {
         "access": "public"
     },
     "repository": "git://github.com/getsentry/sentry-javascript.git",
+    "sideEffects": false,
     "types": "types/index.d.ts",
-    "version": "7.46.0"
+    "version": "7.50.0"
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/baggage.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/baggage.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/browser.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/browser.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncNullishCoalesce.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncNullishCoalesce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChain.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChainDelete.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChainDelete.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createNamedExportFrom.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createNamedExportFrom.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createStarExport.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createStarExport.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopDefault.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopDefault.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespace.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespaceDefaultOnly.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespaceDefaultOnly.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireDefault.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireDefault.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireWildcard.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireWildcard.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_nullishCoalesce.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_nullishCoalesce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChain.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChainDelete.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChainDelete.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/clientreport.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/clientreport.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/dsn.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/dsn.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/env.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/env.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/envelope.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/envelope.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -187,14 +187,15 @@
     transaction: 'transaction',
     event: 'error',
     client_report: 'internal',
     user_report: 'default',
     profile: 'profile',
     replay_event: 'replay',
     replay_recording: 'replay',
+    check_in: 'monitor',
 };
 
 /**
  * Maps the type of an envelope item to a data category.
  */
 function envelopeItemTypeToDataCategory(type) {
     return ITEM_TYPE_TO_DATA_CATEGORY_MAP[type];
@@ -222,30 +223,28 @@
 function createEventEnvelopeHeaders(
     event,
     sdkInfo,
     tunnel,
     dsn$1,
 ) {
     const dynamicSamplingContext = event.sdkProcessingMetadata && event.sdkProcessingMetadata.dynamicSamplingContext;
-
     return {
         event_id: event.event_id,
         sent_at: new Date().toISOString(),
         ...(sdkInfo && {
             sdk: sdkInfo
         }),
         ...(!!tunnel && {
             dsn: dsn.dsnToString(dsn$1)
         }),
-        ...(event.type === 'transaction' &&
-            dynamicSamplingContext && {
-                trace: object.dropUndefinedKeys({
-                    ...dynamicSamplingContext
-                }),
+        ...(dynamicSamplingContext && {
+            trace: object.dropUndefinedKeys({
+                ...dynamicSamplingContext
             }),
+        }),
     };
 }
 
 exports.addItemToEnvelope = addItemToEnvelope;
 exports.createAttachmentEnvelopeItem = createAttachmentEnvelopeItem;
 exports.createEnvelope = createEnvelope;
 exports.createEventEnvelopeHeaders = createEventEnvelopeHeaders;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/error.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/error.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,17 @@
 exports.dsnFromString = dsn.dsnFromString;
 exports.dsnToString = dsn.dsnToString;
 exports.makeDsn = dsn.makeDsn;
 exports.SentryError = error.SentryError;
 exports.GLOBAL_OBJ = worldwide.GLOBAL_OBJ;
 exports.getGlobalObject = worldwide.getGlobalObject;
 exports.getGlobalSingleton = worldwide.getGlobalSingleton;
+exports.SENTRY_XHR_DATA_KEY = instrument.SENTRY_XHR_DATA_KEY;
 exports.addInstrumentationHandler = instrument.addInstrumentationHandler;
+exports.parseFetchArgs = instrument.parseFetchArgs;
 exports.isDOMError = is.isDOMError;
 exports.isDOMException = is.isDOMException;
 exports.isElement = is.isElement;
 exports.isError = is.isError;
 exports.isErrorEvent = is.isErrorEvent;
 exports.isEvent = is.isEvent;
 exports.isInstanceOf = is.isInstanceOf;
@@ -159,13 +161,14 @@
 exports.BAGGAGE_HEADER_NAME = baggage.BAGGAGE_HEADER_NAME;
 exports.MAX_BAGGAGE_STRING_LENGTH = baggage.MAX_BAGGAGE_STRING_LENGTH;
 exports.SENTRY_BAGGAGE_KEY_PREFIX = baggage.SENTRY_BAGGAGE_KEY_PREFIX;
 exports.SENTRY_BAGGAGE_KEY_PREFIX_REGEX = baggage.SENTRY_BAGGAGE_KEY_PREFIX_REGEX;
 exports.baggageHeaderToDynamicSamplingContext = baggage.baggageHeaderToDynamicSamplingContext;
 exports.dynamicSamplingContextToSentryBaggageHeader = baggage.dynamicSamplingContextToSentryBaggageHeader;
 exports.getNumberOfUrlSegments = url.getNumberOfUrlSegments;
+exports.getSanitizedUrlString = url.getSanitizedUrlString;
 exports.parseUrl = url.parseUrl;
 exports.stripUrlQueryAndFragment = url.stripUrlQueryAndFragment;
 exports.addOrUpdateIntegration = userIntegrations.addOrUpdateIntegration;
 exports.escapeStringForRegex = escapeStringForRegex.escapeStringForRegex;
 exports.supportsHistory = supportsHistory.supportsHistory;
 //# sourceMappingURL=index.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/instrument.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/instrument.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -9,14 +9,16 @@
 const supports = require('./supports.js');
 const worldwide = require('./worldwide.js');
 const supportsHistory = require('./vendor/supportsHistory.js');
 
 // eslint-disable-next-line deprecation/deprecation
 const WINDOW = worldwide.getGlobalObject();
 
+const SENTRY_XHR_DATA_KEY = '__sentry_xhr_v2__';
+
 /**
  * Instrument native APIs to call handlers that can be used to create breadcrumbs, APM spans etc.
  *  - Console API
  *  - Fetch API
  *  - XHR API
  *  - History API
  *  - DOM API (click/typing)
@@ -124,19 +126,24 @@
 function instrumentFetch() {
     if (!supports.supportsNativeFetch()) {
         return;
     }
 
     object.fill(WINDOW, 'fetch', function(originalFetch) {
         return function(...args) {
+            const {
+                method,
+                url
+            } = parseFetchArgs(args);
+
             const handlerData = {
                 args,
                 fetchData: {
-                    method: getFetchMethod(args),
-                    url: getFetchUrl(args),
+                    method,
+                    url,
                 },
                 startTimestamp: Date.now(),
             };
 
             triggerHandlers('fetch', {
                 ...handlerData,
             });
@@ -163,64 +170,92 @@
                     throw error;
                 },
             );
         };
     });
 }
 
-/* eslint-disable @typescript-eslint/no-unsafe-member-access */
-/** Extract `method` from fetch call arguments */
-function getFetchMethod(fetchArgs = []) {
-    if ('Request' in WINDOW && is.isInstanceOf(fetchArgs[0], Request) && fetchArgs[0].method) {
-        return String(fetchArgs[0].method).toUpperCase();
+function hasProp(obj, prop) {
+    return !!obj && typeof obj === 'object' && !!(obj)[prop];
+}
+
+function getUrlFromResource(resource) {
+    if (typeof resource === 'string') {
+        return resource;
+    }
+
+    if (!resource) {
+        return '';
+    }
+
+    if (hasProp(resource, 'url')) {
+        return resource.url;
     }
-    if (fetchArgs[1] && fetchArgs[1].method) {
-        return String(fetchArgs[1].method).toUpperCase();
+
+    if (resource.toString) {
+        return resource.toString();
     }
-    return 'GET';
+
+    return '';
 }
 
-/** Extract `url` from fetch call arguments */
-function getFetchUrl(fetchArgs = []) {
-    if (typeof fetchArgs[0] === 'string') {
-        return fetchArgs[0];
+/**
+ * Parses the fetch arguments to find the used Http method and the url of the request
+ */
+function parseFetchArgs(fetchArgs) {
+    if (fetchArgs.length === 0) {
+        return {
+            method: 'GET',
+            url: ''
+        };
     }
-    if ('Request' in WINDOW && is.isInstanceOf(fetchArgs[0], Request)) {
-        return fetchArgs[0].url;
+
+    if (fetchArgs.length === 2) {
+        const [url, options] = fetchArgs;
+
+        return {
+            url: getUrlFromResource(url),
+            method: hasProp(options, 'method') ? String(options.method).toUpperCase() : 'GET',
+        };
     }
-    return String(fetchArgs[0]);
+
+    const arg = fetchArgs[0];
+    return {
+        url: getUrlFromResource(arg),
+        method: hasProp(arg, 'method') ? String(arg.method).toUpperCase() : 'GET',
+    };
 }
-/* eslint-enable @typescript-eslint/no-unsafe-member-access */
 
 /** JSDoc */
 function instrumentXHR() {
     if (!('XMLHttpRequest' in WINDOW)) {
         return;
     }
 
     const xhrproto = XMLHttpRequest.prototype;
 
     object.fill(xhrproto, 'open', function(originalOpen) {
         return function(...args) {
             const url = args[1];
-            const xhrInfo = (this.__sentry_xhr__ = {
+            const xhrInfo = (this[SENTRY_XHR_DATA_KEY] = {
                 // eslint-disable-next-line @typescript-eslint/no-unsafe-member-access
                 method: is.isString(args[0]) ? args[0].toUpperCase() : args[0],
                 url: args[1],
+                request_headers: {},
             });
 
             // if Sentry key appears in URL, don't capture it as a request
             // eslint-disable-next-line @typescript-eslint/no-unsafe-member-access
             if (is.isString(url) && xhrInfo.method === 'POST' && url.match(/sentry_key/)) {
                 this.__sentry_own_request__ = true;
             }
 
             const onreadystatechangeHandler = () => {
                 // For whatever reason, this is not the same instance here as from the outer method
-                const xhrInfo = this.__sentry_xhr__;
+                const xhrInfo = this[SENTRY_XHR_DATA_KEY];
 
                 if (!xhrInfo) {
                     return;
                 }
 
                 if (this.readyState === 4) {
                     try {
@@ -247,22 +282,40 @@
                         return original.apply(this, readyStateArgs);
                     };
                 });
             } else {
                 this.addEventListener('readystatechange', onreadystatechangeHandler);
             }
 
+            // Intercepting `setRequestHeader` to access the request headers of XHR instance.
+            // This will only work for user/library defined headers, not for the default/browser-assigned headers.
+            // Request cookies are also unavailable for XHR, as `Cookie` header can't be defined by `setRequestHeader`.
+            object.fill(this, 'setRequestHeader', function(original) {
+                return function(...setRequestHeaderArgs) {
+                    const [header, value] = setRequestHeaderArgs;
+
+                    const xhrInfo = this[SENTRY_XHR_DATA_KEY];
+
+                    if (xhrInfo) {
+                        xhrInfo.request_headers[header.toLowerCase()] = value;
+                    }
+
+                    return original.apply(this, setRequestHeaderArgs);
+                };
+            });
+
             return originalOpen.apply(this, args);
         };
     });
 
     object.fill(xhrproto, 'send', function(originalSend) {
         return function(...args) {
-            if (this.__sentry_xhr__ && args[0] !== undefined) {
-                this.__sentry_xhr__.body = args[0];
+            const sentryXhrData = this[SENTRY_XHR_DATA_KEY];
+            if (sentryXhrData && args[0] !== undefined) {
+                sentryXhrData.body = args[0];
             }
 
             triggerHandlers('xhr', {
                 args,
                 startTimestamp: Date.now(),
                 xhr: this,
             });
@@ -555,35 +608,41 @@
             column,
             error,
             line,
             msg,
             url,
         });
 
-        if (_oldOnErrorHandler) {
+        if (_oldOnErrorHandler && !_oldOnErrorHandler.__SENTRY_LOADER__) {
             // eslint-disable-next-line prefer-rest-params
             return _oldOnErrorHandler.apply(this, arguments);
         }
 
         return false;
     };
+
+    WINDOW.onerror.__SENTRY_INSTRUMENTED__ = true;
 }
 
 let _oldOnUnhandledRejectionHandler = null;
 /** JSDoc */
 function instrumentUnhandledRejection() {
     _oldOnUnhandledRejectionHandler = WINDOW.onunhandledrejection;
 
     WINDOW.onunhandledrejection = function(e) {
         triggerHandlers('unhandledrejection', e);
 
-        if (_oldOnUnhandledRejectionHandler) {
+        if (_oldOnUnhandledRejectionHandler && !_oldOnUnhandledRejectionHandler.__SENTRY_LOADER__) {
             // eslint-disable-next-line prefer-rest-params
             return _oldOnUnhandledRejectionHandler.apply(this, arguments);
         }
 
         return true;
     };
+
+    WINDOW.onunhandledrejection.__SENTRY_INSTRUMENTED__ = true;
 }
 
+exports.SENTRY_XHR_DATA_KEY = SENTRY_XHR_DATA_KEY;
 exports.addInstrumentationHandler = addInstrumentationHandler;
+exports.parseFetchArgs = parseFetchArgs;
 //# sourceMappingURL=instrument.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/is.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/is.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/logger.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/logger.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/memo.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/memo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/misc.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/misc.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/node-stack-trace.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/node-stack-trace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/node.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/node.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/normalize.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/normalize.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -23,15 +23,15 @@
  * @param input The object to be normalized.
  * @param depth The max depth to which to normalize the object. (Anything deeper stringified whole.)
  * @param maxProperties The max number of elements or properties to be included in any single array or
  * object in the normallized output.
  * @returns A normalized version of the object, or `"**non-serializable**"` if any errors are thrown during normalization.
  */
 // eslint-disable-next-line @typescript-eslint/no-explicit-any
-function normalize(input, depth = +Infinity, maxProperties = +Infinity) {
+function normalize(input, depth = 100, maxProperties = +Infinity) {
     try {
         // since we're at the outermost level, we don't provide a key
         return visit('', input, depth, maxProperties);
     } catch (err) {
         return {
             ERROR: `**non-serializable** (${err})`
         };
@@ -92,25 +92,24 @@
     // Do not normalize objects that we know have already been normalized. As a general rule, the
     // "__sentry_skip_normalization__" property should only be used sparingly and only should only be set on objects that
     // have already been normalized.
     if ((value)['__sentry_skip_normalization__']) {
         return value;
     }
 
-    // Do not normalize objects that we know have already been normalized. As a general rule, the
-    // "__sentry_skip_normalization__" property should only be used sparingly and only should only be set on objects that
-    // have already been normalized.
-    let overriddenDepth = depth;
-
-    if (typeof(value)['__sentry_override_normalization_depth__'] === 'number') {
-        overriddenDepth = (value)['__sentry_override_normalization_depth__'];
-    }
+    // We can set `__sentry_override_normalization_depth__` on an object to ensure that from there
+    // We keep a certain amount of depth.
+    // This should be used sparingly, e.g. we use it for the redux integration to ensure we get a certain amount of state.
+    const remainingDepth =
+        typeof(value)['__sentry_override_normalization_depth__'] === 'number' ?
+        ((value)['__sentry_override_normalization_depth__']) :
+        depth;
 
     // We're also done if we've reached the max depth
-    if (overriddenDepth === 0) {
+    if (remainingDepth === 0) {
         // At this point we know `serialized` is a string of the form `"[object XXXX]"`. Clean it up so it's just `"[XXXX]"`.
         return stringified.replace('object ', '');
     }
 
     // If we've already visited this branch, bail out, as it's circular reference. If not, note that we're seeing it now.
     if (memoize(value)) {
         return '[Circular ~]';
@@ -118,15 +117,15 @@
 
     // If the value has a `toJSON` method, we call it to extract more information
     const valueWithToJSON = value;
     if (valueWithToJSON && typeof valueWithToJSON.toJSON === 'function') {
         try {
             const jsonValue = valueWithToJSON.toJSON();
             // We need to normalize the return value of `.toJSON()` in case it has circular references
-            return visit('', jsonValue, overriddenDepth - 1, maxProperties, memo$1);
+            return visit('', jsonValue, remainingDepth - 1, maxProperties, memo$1);
         } catch (err) {
             // pass (The built-in `toJSON` failed, but we can still try to do it ourselves)
         }
     }
 
     // At this point we know we either have an object or an array, we haven't seen it before, and we're going to recurse
     // because we haven't yet reached the max depth. Create an accumulator to hold the results of visiting each
@@ -147,26 +146,27 @@
         if (numAdded >= maxProperties) {
             normalized[visitKey] = '[MaxProperties ~]';
             break;
         }
 
         // Recursively visit all the child nodes
         const visitValue = visitable[visitKey];
-        normalized[visitKey] = visit(visitKey, visitValue, overriddenDepth - 1, maxProperties, memo$1);
+        normalized[visitKey] = visit(visitKey, visitValue, remainingDepth - 1, maxProperties, memo$1);
 
         numAdded++;
     }
 
     // Once we've visited all the branches, remove the parent from memo storage
     unmemoize(value);
 
     // Return accumulated values
     return normalized;
 }
 
+/* eslint-disable complexity */
 /**
  * Stringify the given value. Handles various known special values and types.
  *
  * Not meant to be used on simple primitives which already have a string representation, as it will, for example, turn
  * the number 1231 into "[Object Number]", nor on `null`, as it will throw.
  *
  * @param value The value to stringify
@@ -231,19 +231,27 @@
             return `[BigInt: ${String(value)}]`;
         }
 
         // Now that we've knocked out all the special cases and the primitives, all we have left are objects. Simply casting
         // them to strings means that instances of classes which haven't defined their `toStringTag` will just come out as
         // `"[object Object]"`. If we instead look at the constructor's name (which is the same as the name of the class),
         // we can make sure that only plain objects come out that way.
-        return `[object ${getConstructorName(value)}]`;
+        const objName = getConstructorName(value);
+
+        // Handle HTML Elements
+        if (/^HTML(\w*)Element$/.test(objName)) {
+            return `[HTMLElement: ${objName}]`;
+        }
+
+        return `[object ${objName}]`;
     } catch (err) {
         return `**non-serializable** (${err})`;
     }
 }
+/* eslint-enable complexity */
 
 function getConstructorName(value) {
     const prototype = Object.getPrototypeOf(value);
 
     return prototype ? prototype.constructor.name : 'null prototype';
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/object.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/object.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/path.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/path.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/promisebuffer.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/promisebuffer.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/ratelimit.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/ratelimit.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/requestdata.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/severity.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/severity.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/stacktrace.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/stacktrace.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -32,14 +32,20 @@
                 continue;
             }
 
             // https://github.com/getsentry/sentry-javascript/issues/5459
             // Remove webpack (error: *) wrappers
             const cleanedLine = WEBPACK_ERROR_REGEXP.test(line) ? line.replace(WEBPACK_ERROR_REGEXP, '$1') : line;
 
+            // https://github.com/getsentry/sentry-javascript/issues/7813
+            // Skip Error: lines
+            if (cleanedLine.match(/\S*Error: /)) {
+                continue;
+            }
+
             for (const parser of sortedParsers) {
                 const frame = parser(cleanedLine);
 
                 if (frame) {
                     frames.push(frame);
                     break;
                 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/string.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/string.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/supports.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/supports.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/syncpromise.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/syncpromise.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/time.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/time.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -110,15 +110,20 @@
  * BUG: Note that because of how browsers implement the Performance API, the clock might stop when the computer is
  * asleep. This creates a skew between `dateTimestampInSeconds` and `timestampInSeconds`. The
  * skew can grow to arbitrary amounts like days, weeks or months.
  * See https://github.com/getsentry/sentry-javascript/issues/2590.
  */
 const timestampInSeconds = timestampSource.nowSeconds.bind(timestampSource);
 
-// Re-exported with an old name for backwards-compatibility.
+/**
+ * Re-exported with an old name for backwards-compatibility.
+ * TODO (v8): Remove this
+ *
+ * @deprecated Use `timestampInSeconds` instead.
+ */
 const timestampWithMs = timestampInSeconds;
 
 /**
  * A boolean that is true when timestampInSeconds uses the Performance API to produce monotonic timestamps.
  */
 const usingPerformanceAPI = platformPerformance !== undefined;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/tracing.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/tracing.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/url.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/url.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,15 @@
-Object.defineProperty(exports, '__esModule', {
-    value: true
-});
-
 /**
  * Parses string form of URL into an object
  * // borrowed from https://tools.ietf.org/html/rfc3986#appendix-B
  * // intentionally using regex and not <a/> href parsing trick because React Native and other
  * // environments where DOM might not be available
  * @returns parsed URL object
  */
-function parseUrl(url)
-
-{
+function parseUrl(url) {
     if (!url) {
         return {};
     }
 
     const match = url.match(/^(([^:/?#]+):)?(\/\/([^/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?$/);
 
     if (!match) {
@@ -25,14 +19,16 @@
     // coerce to undefined values to empty string so we don't get 'undefined'
     const query = match[6] || '';
     const fragment = match[8] || '';
     return {
         host: match[4],
         path: match[5],
         protocol: match[2],
+        search: query,
+        hash: fragment,
         relative: match[5] + query + fragment, // everything minus origin
     };
 }
 
 /**
  * Strip the query string and fragment off of a given URL or path (if present)
  *
@@ -48,11 +44,38 @@
  * Returns number of URL segments of a passed string URL.
  */
 function getNumberOfUrlSegments(url) {
     // split at '/' or at '\/' to split regex urls correctly
     return url.split(/\\?\//).filter(s => s.length > 0 && s !== ',').length;
 }
 
-exports.getNumberOfUrlSegments = getNumberOfUrlSegments;
-exports.parseUrl = parseUrl;
-exports.stripUrlQueryAndFragment = stripUrlQueryAndFragment;
+/**
+ * Takes a URL object and returns a sanitized string which is safe to use as span description
+ * see: https://develop.sentry.dev/sdk/data-handling/#structuring-data
+ */
+function getSanitizedUrlString(url) {
+    const {
+        protocol,
+        host,
+        path
+    } = url;
+
+    const filteredHost =
+        (host &&
+            host
+            // Always filter out authority
+            .replace(/^.*@/, '[filtered]:[filtered]@')
+            // Don't show standard :80 (http) and :443 (https) ports to reduce the noise
+            .replace(':80', '')
+            .replace(':443', '')) ||
+        '';
+
+    return `${protocol ? `${protocol}://` : ''}${filteredHost}${path}`;
+}
+
+export {
+    getNumberOfUrlSegments,
+    getSanitizedUrlString,
+    parseUrl,
+    stripUrlQueryAndFragment
+};
 //# sourceMappingURL=url.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/userIntegrations.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/userIntegrations.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/vendor/escapeStringForRegex.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/vendor/escapeStringForRegex.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/vendor/supportsHistory.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/vendor/supportsHistory.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/cjs/worldwide.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/cjs/worldwide.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/baggage.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/baggage.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/browser.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/browser.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncNullishCoalesce.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncNullishCoalesce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChain.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChainDelete.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChainDelete.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createNamedExportFrom.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createNamedExportFrom.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createStarExport.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createStarExport.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopDefault.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopDefault.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespace.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespaceDefaultOnly.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespaceDefaultOnly.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireDefault.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireDefault.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireWildcard.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireWildcard.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_nullishCoalesce.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_nullishCoalesce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChain.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChainDelete.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChainDelete.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/clientreport.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/clientreport.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/dsn.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/dsn.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/env.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/env.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/envelope.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/envelope.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -189,14 +189,15 @@
     transaction: 'transaction',
     event: 'error',
     client_report: 'internal',
     user_report: 'default',
     profile: 'profile',
     replay_event: 'replay',
     replay_recording: 'replay',
+    check_in: 'monitor',
 };
 
 /**
  * Maps the type of an envelope item to a data category.
  */
 function envelopeItemTypeToDataCategory(type) {
     return ITEM_TYPE_TO_DATA_CATEGORY_MAP[type];
@@ -224,30 +225,28 @@
 function createEventEnvelopeHeaders(
     event,
     sdkInfo,
     tunnel,
     dsn,
 ) {
     const dynamicSamplingContext = event.sdkProcessingMetadata && event.sdkProcessingMetadata.dynamicSamplingContext;
-
     return {
         event_id: event.event_id,
         sent_at: new Date().toISOString(),
         ...(sdkInfo && {
             sdk: sdkInfo
         }),
         ...(!!tunnel && {
             dsn: dsnToString(dsn)
         }),
-        ...(event.type === 'transaction' &&
-            dynamicSamplingContext && {
-                trace: dropUndefinedKeys({
-                    ...dynamicSamplingContext
-                }),
+        ...(dynamicSamplingContext && {
+            trace: dropUndefinedKeys({
+                ...dynamicSamplingContext
             }),
+        }),
     };
 }
 
 export {
     addItemToEnvelope,
     createAttachmentEnvelopeItem,
     createEnvelope,
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/error.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/error.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,17 @@
 export {
     GLOBAL_OBJ,
     getGlobalObject,
     getGlobalSingleton
 }
 from './worldwide.js';
 export {
-    addInstrumentationHandler
+    SENTRY_XHR_DATA_KEY,
+    addInstrumentationHandler,
+    parseFetchArgs
 }
 from './instrument.js';
 export {
     isDOMError,
     isDOMException,
     isElement,
     isError,
@@ -197,14 +199,15 @@
     SENTRY_BAGGAGE_KEY_PREFIX_REGEX,
     baggageHeaderToDynamicSamplingContext,
     dynamicSamplingContextToSentryBaggageHeader
 }
 from './baggage.js';
 export {
     getNumberOfUrlSegments,
+    getSanitizedUrlString,
     parseUrl,
     stripUrlQueryAndFragment
 }
 from './url.js';
 export {
     addOrUpdateIntegration
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/instrument.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/instrument.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,8 @@
 import {
-    isInstanceOf,
     isString
 } from './is.js';
 import {
     logger,
     CONSOLE_LEVELS
 } from './logger.js';
 import {
@@ -21,14 +20,16 @@
 import {
     supportsHistory
 } from './vendor/supportsHistory.js';
 
 // eslint-disable-next-line deprecation/deprecation
 const WINDOW = getGlobalObject();
 
+const SENTRY_XHR_DATA_KEY = '__sentry_xhr_v2__';
+
 /**
  * Instrument native APIs to call handlers that can be used to create breadcrumbs, APM spans etc.
  *  - Console API
  *  - Fetch API
  *  - XHR API
  *  - History API
  *  - DOM API (click/typing)
@@ -136,19 +137,24 @@
 function instrumentFetch() {
     if (!supportsNativeFetch()) {
         return;
     }
 
     fill(WINDOW, 'fetch', function(originalFetch) {
         return function(...args) {
+            const {
+                method,
+                url
+            } = parseFetchArgs(args);
+
             const handlerData = {
                 args,
                 fetchData: {
-                    method: getFetchMethod(args),
-                    url: getFetchUrl(args),
+                    method,
+                    url,
                 },
                 startTimestamp: Date.now(),
             };
 
             triggerHandlers('fetch', {
                 ...handlerData,
             });
@@ -175,64 +181,92 @@
                     throw error;
                 },
             );
         };
     });
 }
 
-/* eslint-disable @typescript-eslint/no-unsafe-member-access */
-/** Extract `method` from fetch call arguments */
-function getFetchMethod(fetchArgs = []) {
-    if ('Request' in WINDOW && isInstanceOf(fetchArgs[0], Request) && fetchArgs[0].method) {
-        return String(fetchArgs[0].method).toUpperCase();
+function hasProp(obj, prop) {
+    return !!obj && typeof obj === 'object' && !!(obj)[prop];
+}
+
+function getUrlFromResource(resource) {
+    if (typeof resource === 'string') {
+        return resource;
+    }
+
+    if (!resource) {
+        return '';
+    }
+
+    if (hasProp(resource, 'url')) {
+        return resource.url;
     }
-    if (fetchArgs[1] && fetchArgs[1].method) {
-        return String(fetchArgs[1].method).toUpperCase();
+
+    if (resource.toString) {
+        return resource.toString();
     }
-    return 'GET';
+
+    return '';
 }
 
-/** Extract `url` from fetch call arguments */
-function getFetchUrl(fetchArgs = []) {
-    if (typeof fetchArgs[0] === 'string') {
-        return fetchArgs[0];
+/**
+ * Parses the fetch arguments to find the used Http method and the url of the request
+ */
+function parseFetchArgs(fetchArgs) {
+    if (fetchArgs.length === 0) {
+        return {
+            method: 'GET',
+            url: ''
+        };
     }
-    if ('Request' in WINDOW && isInstanceOf(fetchArgs[0], Request)) {
-        return fetchArgs[0].url;
+
+    if (fetchArgs.length === 2) {
+        const [url, options] = fetchArgs;
+
+        return {
+            url: getUrlFromResource(url),
+            method: hasProp(options, 'method') ? String(options.method).toUpperCase() : 'GET',
+        };
     }
-    return String(fetchArgs[0]);
+
+    const arg = fetchArgs[0];
+    return {
+        url: getUrlFromResource(arg),
+        method: hasProp(arg, 'method') ? String(arg.method).toUpperCase() : 'GET',
+    };
 }
-/* eslint-enable @typescript-eslint/no-unsafe-member-access */
 
 /** JSDoc */
 function instrumentXHR() {
     if (!('XMLHttpRequest' in WINDOW)) {
         return;
     }
 
     const xhrproto = XMLHttpRequest.prototype;
 
     fill(xhrproto, 'open', function(originalOpen) {
         return function(...args) {
             const url = args[1];
-            const xhrInfo = (this.__sentry_xhr__ = {
+            const xhrInfo = (this[SENTRY_XHR_DATA_KEY] = {
                 // eslint-disable-next-line @typescript-eslint/no-unsafe-member-access
                 method: isString(args[0]) ? args[0].toUpperCase() : args[0],
                 url: args[1],
+                request_headers: {},
             });
 
             // if Sentry key appears in URL, don't capture it as a request
             // eslint-disable-next-line @typescript-eslint/no-unsafe-member-access
             if (isString(url) && xhrInfo.method === 'POST' && url.match(/sentry_key/)) {
                 this.__sentry_own_request__ = true;
             }
 
             const onreadystatechangeHandler = () => {
                 // For whatever reason, this is not the same instance here as from the outer method
-                const xhrInfo = this.__sentry_xhr__;
+                const xhrInfo = this[SENTRY_XHR_DATA_KEY];
 
                 if (!xhrInfo) {
                     return;
                 }
 
                 if (this.readyState === 4) {
                     try {
@@ -259,22 +293,40 @@
                         return original.apply(this, readyStateArgs);
                     };
                 });
             } else {
                 this.addEventListener('readystatechange', onreadystatechangeHandler);
             }
 
+            // Intercepting `setRequestHeader` to access the request headers of XHR instance.
+            // This will only work for user/library defined headers, not for the default/browser-assigned headers.
+            // Request cookies are also unavailable for XHR, as `Cookie` header can't be defined by `setRequestHeader`.
+            fill(this, 'setRequestHeader', function(original) {
+                return function(...setRequestHeaderArgs) {
+                    const [header, value] = setRequestHeaderArgs;
+
+                    const xhrInfo = this[SENTRY_XHR_DATA_KEY];
+
+                    if (xhrInfo) {
+                        xhrInfo.request_headers[header.toLowerCase()] = value;
+                    }
+
+                    return original.apply(this, setRequestHeaderArgs);
+                };
+            });
+
             return originalOpen.apply(this, args);
         };
     });
 
     fill(xhrproto, 'send', function(originalSend) {
         return function(...args) {
-            if (this.__sentry_xhr__ && args[0] !== undefined) {
-                this.__sentry_xhr__.body = args[0];
+            const sentryXhrData = this[SENTRY_XHR_DATA_KEY];
+            if (sentryXhrData && args[0] !== undefined) {
+                sentryXhrData.body = args[0];
             }
 
             triggerHandlers('xhr', {
                 args,
                 startTimestamp: Date.now(),
                 xhr: this,
             });
@@ -567,37 +619,43 @@
             column,
             error,
             line,
             msg,
             url,
         });
 
-        if (_oldOnErrorHandler) {
+        if (_oldOnErrorHandler && !_oldOnErrorHandler.__SENTRY_LOADER__) {
             // eslint-disable-next-line prefer-rest-params
             return _oldOnErrorHandler.apply(this, arguments);
         }
 
         return false;
     };
+
+    WINDOW.onerror.__SENTRY_INSTRUMENTED__ = true;
 }
 
 let _oldOnUnhandledRejectionHandler = null;
 /** JSDoc */
 function instrumentUnhandledRejection() {
     _oldOnUnhandledRejectionHandler = WINDOW.onunhandledrejection;
 
     WINDOW.onunhandledrejection = function(e) {
         triggerHandlers('unhandledrejection', e);
 
-        if (_oldOnUnhandledRejectionHandler) {
+        if (_oldOnUnhandledRejectionHandler && !_oldOnUnhandledRejectionHandler.__SENTRY_LOADER__) {
             // eslint-disable-next-line prefer-rest-params
             return _oldOnUnhandledRejectionHandler.apply(this, arguments);
         }
 
         return true;
     };
+
+    WINDOW.onunhandledrejection.__SENTRY_INSTRUMENTED__ = true;
 }
 
 export {
-    addInstrumentationHandler
+    SENTRY_XHR_DATA_KEY,
+    addInstrumentationHandler,
+    parseFetchArgs
 };
 //# sourceMappingURL=instrument.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/is.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/is.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/logger.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/logger.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/memo.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/memo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/misc.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/misc.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/node-stack-trace.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/node-stack-trace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/node.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/node.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/normalize.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/normalize.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -28,15 +28,15 @@
  * @param input The object to be normalized.
  * @param depth The max depth to which to normalize the object. (Anything deeper stringified whole.)
  * @param maxProperties The max number of elements or properties to be included in any single array or
  * object in the normallized output.
  * @returns A normalized version of the object, or `"**non-serializable**"` if any errors are thrown during normalization.
  */
 // eslint-disable-next-line @typescript-eslint/no-explicit-any
-function normalize(input, depth = +Infinity, maxProperties = +Infinity) {
+function normalize(input, depth = 100, maxProperties = +Infinity) {
     try {
         // since we're at the outermost level, we don't provide a key
         return visit('', input, depth, maxProperties);
     } catch (err) {
         return {
             ERROR: `**non-serializable** (${err})`
         };
@@ -97,25 +97,24 @@
     // Do not normalize objects that we know have already been normalized. As a general rule, the
     // "__sentry_skip_normalization__" property should only be used sparingly and only should only be set on objects that
     // have already been normalized.
     if ((value)['__sentry_skip_normalization__']) {
         return value;
     }
 
-    // Do not normalize objects that we know have already been normalized. As a general rule, the
-    // "__sentry_skip_normalization__" property should only be used sparingly and only should only be set on objects that
-    // have already been normalized.
-    let overriddenDepth = depth;
-
-    if (typeof(value)['__sentry_override_normalization_depth__'] === 'number') {
-        overriddenDepth = (value)['__sentry_override_normalization_depth__'];
-    }
+    // We can set `__sentry_override_normalization_depth__` on an object to ensure that from there
+    // We keep a certain amount of depth.
+    // This should be used sparingly, e.g. we use it for the redux integration to ensure we get a certain amount of state.
+    const remainingDepth =
+        typeof(value)['__sentry_override_normalization_depth__'] === 'number' ?
+        ((value)['__sentry_override_normalization_depth__']) :
+        depth;
 
     // We're also done if we've reached the max depth
-    if (overriddenDepth === 0) {
+    if (remainingDepth === 0) {
         // At this point we know `serialized` is a string of the form `"[object XXXX]"`. Clean it up so it's just `"[XXXX]"`.
         return stringified.replace('object ', '');
     }
 
     // If we've already visited this branch, bail out, as it's circular reference. If not, note that we're seeing it now.
     if (memoize(value)) {
         return '[Circular ~]';
@@ -123,15 +122,15 @@
 
     // If the value has a `toJSON` method, we call it to extract more information
     const valueWithToJSON = value;
     if (valueWithToJSON && typeof valueWithToJSON.toJSON === 'function') {
         try {
             const jsonValue = valueWithToJSON.toJSON();
             // We need to normalize the return value of `.toJSON()` in case it has circular references
-            return visit('', jsonValue, overriddenDepth - 1, maxProperties, memo);
+            return visit('', jsonValue, remainingDepth - 1, maxProperties, memo);
         } catch (err) {
             // pass (The built-in `toJSON` failed, but we can still try to do it ourselves)
         }
     }
 
     // At this point we know we either have an object or an array, we haven't seen it before, and we're going to recurse
     // because we haven't yet reached the max depth. Create an accumulator to hold the results of visiting each
@@ -152,26 +151,27 @@
         if (numAdded >= maxProperties) {
             normalized[visitKey] = '[MaxProperties ~]';
             break;
         }
 
         // Recursively visit all the child nodes
         const visitValue = visitable[visitKey];
-        normalized[visitKey] = visit(visitKey, visitValue, overriddenDepth - 1, maxProperties, memo);
+        normalized[visitKey] = visit(visitKey, visitValue, remainingDepth - 1, maxProperties, memo);
 
         numAdded++;
     }
 
     // Once we've visited all the branches, remove the parent from memo storage
     unmemoize(value);
 
     // Return accumulated values
     return normalized;
 }
 
+/* eslint-disable complexity */
 /**
  * Stringify the given value. Handles various known special values and types.
  *
  * Not meant to be used on simple primitives which already have a string representation, as it will, for example, turn
  * the number 1231 into "[Object Number]", nor on `null`, as it will throw.
  *
  * @param value The value to stringify
@@ -236,19 +236,27 @@
             return `[BigInt: ${String(value)}]`;
         }
 
         // Now that we've knocked out all the special cases and the primitives, all we have left are objects. Simply casting
         // them to strings means that instances of classes which haven't defined their `toStringTag` will just come out as
         // `"[object Object]"`. If we instead look at the constructor's name (which is the same as the name of the class),
         // we can make sure that only plain objects come out that way.
-        return `[object ${getConstructorName(value)}]`;
+        const objName = getConstructorName(value);
+
+        // Handle HTML Elements
+        if (/^HTML(\w*)Element$/.test(objName)) {
+            return `[HTMLElement: ${objName}]`;
+        }
+
+        return `[object ${objName}]`;
     } catch (err) {
         return `**non-serializable** (${err})`;
     }
 }
+/* eslint-enable complexity */
 
 function getConstructorName(value) {
     const prototype = Object.getPrototypeOf(value);
 
     return prototype ? prototype.constructor.name : 'null prototype';
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/object.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/object.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/path.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/path.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/promisebuffer.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/promisebuffer.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/ratelimit.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/ratelimit.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/requestdata.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/severity.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/severity.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/stacktrace.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/stacktrace.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -30,14 +30,20 @@
                 continue;
             }
 
             // https://github.com/getsentry/sentry-javascript/issues/5459
             // Remove webpack (error: *) wrappers
             const cleanedLine = WEBPACK_ERROR_REGEXP.test(line) ? line.replace(WEBPACK_ERROR_REGEXP, '$1') : line;
 
+            // https://github.com/getsentry/sentry-javascript/issues/7813
+            // Skip Error: lines
+            if (cleanedLine.match(/\S*Error: /)) {
+                continue;
+            }
+
             for (const parser of sortedParsers) {
                 const frame = parser(cleanedLine);
 
                 if (frame) {
                     frames.push(frame);
                     break;
                 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/string.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/string.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/supports.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/supports.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/syncpromise.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/syncpromise.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/time.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/time.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -111,15 +111,20 @@
  * BUG: Note that because of how browsers implement the Performance API, the clock might stop when the computer is
  * asleep. This creates a skew between `dateTimestampInSeconds` and `timestampInSeconds`. The
  * skew can grow to arbitrary amounts like days, weeks or months.
  * See https://github.com/getsentry/sentry-javascript/issues/2590.
  */
 const timestampInSeconds = timestampSource.nowSeconds.bind(timestampSource);
 
-// Re-exported with an old name for backwards-compatibility.
+/**
+ * Re-exported with an old name for backwards-compatibility.
+ * TODO (v8): Remove this
+ *
+ * @deprecated Use `timestampInSeconds` instead.
+ */
 const timestampWithMs = timestampInSeconds;
 
 /**
  * A boolean that is true when timestampInSeconds uses the Performance API to produce monotonic timestamps.
  */
 const usingPerformanceAPI = platformPerformance !== undefined;
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/tracing.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/tracing.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/userIntegrations.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/userIntegrations.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/vendor/escapeStringForRegex.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/vendor/escapeStringForRegex.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/vendor/supportsHistory.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/vendor/supportsHistory.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/esm/worldwide.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry/utils/esm/worldwide.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry/utils/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8125%*

 * *Differences: {"'dependencies'": "{'@sentry/types': '7.50.0', '@sentry/core': '7.50.0', '@sentry/utils': "*

 * *                   "'7.50.0'}",*

 * * "'description'": "'Sentry Internal Tracing Package'",*

 * * "'devDependencies'": "{replace: OrderedDict([('@types/express', '^4.17.14')])}",*

 * * "'homepage'": "'https://github.com/getsentry/sentry-javascript/tree/master/packages/tracing-internal'",*

 * * "'name'": "'@sentry-internal/tracing'",*

 * * "'version'": "'7.50.0'"}*

```diff
@@ -1,28 +1,28 @@
 {
     "author": "Sentry",
     "dependencies": {
-        "@sentry/types": "7.46.0",
+        "@sentry/core": "7.50.0",
+        "@sentry/types": "7.50.0",
+        "@sentry/utils": "7.50.0",
         "tslib": "^1.9.3"
     },
-    "description": "Utilities for all Sentry JavaScript SDKs",
+    "description": "Sentry Internal Tracing Package",
     "devDependencies": {
-        "@types/array.prototype.flat": "^1.2.1",
-        "array.prototype.flat": "^1.3.0",
-        "chai": "^4.1.2"
+        "@types/express": "^4.17.14"
     },
     "engines": {
         "node": ">=8"
     },
-    "homepage": "https://github.com/getsentry/sentry-javascript/tree/master/packages/utils",
+    "homepage": "https://github.com/getsentry/sentry-javascript/tree/master/packages/tracing-internal",
     "license": "MIT",
     "main": "cjs/index.js",
     "module": "esm/index.js",
-    "name": "@sentry/utils",
+    "name": "@sentry-internal/tracing",
     "publishConfig": {
         "access": "public"
     },
     "repository": "git://github.com/getsentry/sentry-javascript.git",
     "sideEffects": false,
     "types": "types/index.d.ts",
-    "version": "7.46.0"
+    "version": "7.50.0"
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/backgroundtab.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/backgroundtab.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/browsertracing.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/browsertracing.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/utils.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/request.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/request.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -133,16 +133,19 @@
                 span,
                 options,
             );
         }
     }
 }
 
+/**
+ * Adds sentry-trace and baggage headers to the various forms of fetch headers
+ */
 function addTracingHeadersToFetchRequest(
-    request,
+    request, // unknown is actually type Request but we can't export DOM types from this package,
     dynamicSamplingContext,
     span,
     options
 
     ,
 ) {
     const sentryBaggageHeader = utils.dynamicSamplingContextToSentryBaggageHeader(dynamicSamplingContext);
@@ -158,15 +161,15 @@
         };
     } else if (typeof Headers !== 'undefined' && utils.isInstanceOf(headers, Headers)) {
         const newHeaders = new Headers(headers);
 
         newHeaders.append('sentry-trace', sentryTraceHeader);
 
         if (sentryBaggageHeader) {
-            // If the same header is appended miultiple times the browser will merge the values into a single request header.
+            // If the same header is appended multiple times the browser will merge the values into a single request header.
             // Its therefore safe to simply push a "baggage" entry, even though there might already be another baggage header.
             newHeaders.append(utils.BAGGAGE_HEADER_NAME, sentryBaggageHeader);
         }
 
         return newHeaders;
     } else if (Array.isArray(headers)) {
         const newHeaders = [...headers, ['sentry-trace', sentryTraceHeader]];
@@ -205,32 +208,33 @@
  */
 function xhrCallback(
     handlerData,
     shouldCreateSpan,
     shouldAttachHeaders,
     spans,
 ) {
+    const xhr = handlerData.xhr;
+    const sentryXhrData = xhr && xhr[utils.SENTRY_XHR_DATA_KEY];
+
     if (
         !core.hasTracingEnabled() ||
-        (handlerData.xhr && handlerData.xhr.__sentry_own_request__) ||
-        !(handlerData.xhr && handlerData.xhr.__sentry_xhr__ && shouldCreateSpan(handlerData.xhr.__sentry_xhr__.url))
+        (xhr && xhr.__sentry_own_request__) ||
+        !(xhr && sentryXhrData && shouldCreateSpan(sentryXhrData.url))
     ) {
         return;
     }
 
-    const xhr = handlerData.xhr.__sentry_xhr__;
-
     // check first if the request has finished and is tracked by an existing span which should now end
     if (handlerData.endTimestamp) {
-        const spanId = handlerData.xhr.__sentry_xhr_span_id__;
+        const spanId = xhr.__sentry_xhr_span_id__;
         if (!spanId) return;
 
         const span = spans[spanId];
         if (span) {
-            span.setHttpStatus(xhr.status_code);
+            span.setHttpStatus(sentryXhrData.status_code);
             span.finish();
 
             // eslint-disable-next-line @typescript-eslint/no-dynamic-delete
             delete spans[spanId];
         }
         return;
     }
@@ -238,46 +242,47 @@
     const currentScope = core.getCurrentHub().getScope();
     const currentSpan = currentScope && currentScope.getSpan();
     const activeTransaction = currentSpan && currentSpan.transaction;
 
     if (currentSpan && activeTransaction) {
         const span = currentSpan.startChild({
             data: {
-                ...xhr.data,
+                ...sentryXhrData.data,
                 type: 'xhr',
-                method: xhr.method,
-                url: xhr.url,
+                method: sentryXhrData.method,
+                url: sentryXhrData.url,
             },
-            description: `${xhr.method} ${xhr.url}`,
+            description: `${sentryXhrData.method} ${sentryXhrData.url}`,
             op: 'http.client',
         });
 
-        handlerData.xhr.__sentry_xhr_span_id__ = span.spanId;
-        spans[handlerData.xhr.__sentry_xhr_span_id__] = span;
+        xhr.__sentry_xhr_span_id__ = span.spanId;
+        spans[xhr.__sentry_xhr_span_id__] = span;
 
-        if (handlerData.xhr.setRequestHeader && shouldAttachHeaders(handlerData.xhr.__sentry_xhr__.url)) {
+        if (xhr.setRequestHeader && shouldAttachHeaders(sentryXhrData.url)) {
             try {
-                handlerData.xhr.setRequestHeader('sentry-trace', span.toTraceparent());
+                xhr.setRequestHeader('sentry-trace', span.toTraceparent());
 
                 const dynamicSamplingContext = activeTransaction.getDynamicSamplingContext();
                 const sentryBaggageHeader = utils.dynamicSamplingContextToSentryBaggageHeader(dynamicSamplingContext);
 
                 if (sentryBaggageHeader) {
                     // From MDN: "If this method is called several times with the same header, the values are merged into one single request header."
                     // We can therefore simply set a baggage header without checking what was there before
                     // https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/setRequestHeader
-                    handlerData.xhr.setRequestHeader(utils.BAGGAGE_HEADER_NAME, sentryBaggageHeader);
+                    xhr.setRequestHeader(utils.BAGGAGE_HEADER_NAME, sentryBaggageHeader);
                 }
             } catch (_) {
                 // Error: InvalidStateError: Failed to execute 'setRequestHeader' on 'XMLHttpRequest': The object's state must be OPENED.
             }
         }
     }
 }
 
 exports.DEFAULT_TRACE_PROPAGATION_TARGETS = DEFAULT_TRACE_PROPAGATION_TARGETS;
+exports.addTracingHeadersToFetchRequest = addTracingHeadersToFetchRequest;
 exports.defaultRequestInstrumentationOptions = defaultRequestInstrumentationOptions;
 exports.fetchCallback = fetchCallback;
 exports.instrumentOutgoingRequests = instrumentOutgoingRequests;
 exports.shouldAttachHeaders = shouldAttachHeaders;
 exports.xhrCallback = xhrCallback;
 //# sourceMappingURL=request.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/router.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/router.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -20,16 +20,16 @@
 
     let startingUrl = types.WINDOW.location.href;
 
     let activeTransaction;
     if (startTransactionOnPageLoad) {
         activeTransaction = customStartTransaction({
             name: types.WINDOW.location.pathname,
-            // pageload should always start at timeOrigin
-            startTimestamp: utils.browserPerformanceTimeOrigin,
+            // pageload should always start at timeOrigin (and needs to be in s, not ms)
+            startTimestamp: utils.browserPerformanceTimeOrigin ? utils.browserPerformanceTimeOrigin / 1000 : undefined,
             op: 'pageload',
             metadata: {
                 source: 'url'
             },
         });
     }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getCLS.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getCLS.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getFID.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getFID.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getLCP.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getLCP.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/bindReporter.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/bindReporter.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/generateUniqueID.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/generateUniqueID.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getActivationStart.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getActivationStart.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getNavigationEntry.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getNavigationEntry.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getVisibilityWatcher.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getVisibilityWatcher.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/initMetric.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/initMetric.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/observe.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/observe.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/onHidden.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/onHidden.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/extensions.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/extensions.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -21,17 +21,15 @@
             ;
             return new integration.Mongo();
         },
         mongoose() {
             const integration = utils.dynamicRequire(module, './node/integrations/mongo')
 
             ;
-            return new integration.Mongo({
-                mongoose: true
-            });
+            return new integration.Mongo();
         },
         mysql() {
             const integration = utils.dynamicRequire(module, './node/integrations/mysql')
 
             ;
             return new integration.Mysql();
         },
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/index.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -35,11 +35,12 @@
 exports.Mongo = mongo.Mongo;
 exports.Prisma = prisma.Prisma;
 exports.GraphQL = graphql.GraphQL;
 exports.Apollo = apollo.Apollo;
 exports.lazyLoadedNodePerformanceMonitoringIntegrations = lazy.lazyLoadedNodePerformanceMonitoringIntegrations;
 exports.BROWSER_TRACING_INTEGRATION_ID = browsertracing.BROWSER_TRACING_INTEGRATION_ID;
 exports.BrowserTracing = browsertracing.BrowserTracing;
+exports.addTracingHeadersToFetchRequest = request.addTracingHeadersToFetchRequest;
 exports.defaultRequestInstrumentationOptions = request.defaultRequestInstrumentationOptions;
 exports.instrumentOutgoingRequests = request.instrumentOutgoingRequests;
 exports.addExtensionMethods = extensions.addExtensionMethods;
 //# sourceMappingURL=index.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/apollo.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/apollo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/express.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/express.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/graphql.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/graphql.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/lazy.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/lazy.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mongo.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mongo.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -209,14 +209,15 @@
         operation,
         args,
     ) {
         const data = {
             collectionName: collection.collectionName,
             dbName: collection.dbName,
             namespace: collection.namespace,
+            'db.system': 'mongodb',
         };
         const spanContext = {
             op: 'db',
             description: operation,
             data,
         };
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mysql.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mysql.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -56,14 +56,17 @@
         utils.fill(pkg, 'createQuery', function(orig) {
             return function(options, values, callback) {
                 const scope = getCurrentHub().getScope();
                 const parentSpan = _optionalChain([scope, 'optionalAccess', _2 => _2.getSpan, 'call', _3 => _3()]);
                 const span = _optionalChain([parentSpan, 'optionalAccess', _4 => _4.startChild, 'call', _5 => _5({
                     description: typeof options === 'string' ? options : (options).sql,
                     op: 'db',
+                    data: {
+                        'db.system': 'mysql',
+                    },
                 })]);
 
                 if (typeof callback === 'function') {
                     return orig.call(this, options, values, function(err, result, fields) {
                         _optionalChain([span, 'optionalAccess', _6 => _6.finish, 'call', _7 => _7()]);
                         callback(err, result, fields);
                     });
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/postgres.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/postgres.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -70,14 +70,17 @@
         utils.fill(Client.prototype, 'query', function(orig) {
             return function(config, values, callback) {
                 const scope = getCurrentHub().getScope();
                 const parentSpan = _optionalChain([scope, 'optionalAccess', _4 => _4.getSpan, 'call', _5 => _5()]);
                 const span = _optionalChain([parentSpan, 'optionalAccess', _6 => _6.startChild, 'call', _7 => _7({
                     description: typeof config === 'string' ? config : (config).text,
                     op: 'db',
+                    data: {
+                        'db.system': 'postgresql',
+                    },
                 })]);
 
                 if (typeof callback === 'function') {
                     return orig.call(this, config, values, function(err, result) {
                         _optionalChain([span, 'optionalAccess', _8 => _8.finish, 'call', _9 => _9()]);
                         callback(err, result);
                     });
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/prisma.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/prisma.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,12 @@
-var {
-    _optionalChain
-} = require('@sentry/utils/cjs/buildPolyfills');
-
 Object.defineProperty(exports, '__esModule', {
     value: true
 });
 
+const core = require('@sentry/core');
 const utils = require('@sentry/utils');
 const nodeUtils = require('./utils/node-utils.js');
 
 function isValidPrismaClient(possibleClient) {
     return possibleClient && !!(possibleClient)['$use'];
 }
 
@@ -59,36 +56,25 @@
 
         if (nodeUtils.shouldDisableAutoInstrumentation(getCurrentHub)) {
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && utils.logger.log('Prisma Integration is skipped because of instrumenter configuration.');
             return;
         }
 
         this._client.$use((params, next) => {
-            const scope = getCurrentHub().getScope();
-            const parentSpan = _optionalChain([scope, 'optionalAccess', _2 => _2.getSpan, 'call', _3 => _3()]);
-
             const action = params.action;
             const model = params.model;
-
-            const span = _optionalChain([parentSpan, 'optionalAccess', _4 => _4.startChild, 'call', _5 => _5({
-                description: model ? `${model} ${action}` : action,
-                op: 'db.sql.prisma',
-            })]);
-
-            const rv = next(params);
-
-            if (utils.isThenable(rv)) {
-                return rv.then((res) => {
-                    _optionalChain([span, 'optionalAccess', _6 => _6.finish, 'call', _7 => _7()]);
-                    return res;
-                });
-            }
-
-            _optionalChain([span, 'optionalAccess', _8 => _8.finish, 'call', _9 => _9()]);
-            return rv;
+            return core.trace({
+                    name: model ? `${model} ${action}` : action,
+                    op: 'db.sql.prisma',
+                    data: {
+                        'db.system': 'prisma'
+                    }
+                },
+                () => next(params),
+            );
         });
     }
 }
 Prisma.__initStatic();
 
 exports.Prisma = Prisma;
 //# sourceMappingURL=prisma.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/utils/node-utils.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/utils/node-utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/backgroundtab.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/backgroundtab.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/browsertracing.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/browsertracing.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/utils.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/request.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/request.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -3,14 +3,15 @@
     getCurrentHub
 } from '@sentry/core';
 import {
     addInstrumentationHandler,
     dynamicSamplingContextToSentryBaggageHeader,
     isInstanceOf,
     BAGGAGE_HEADER_NAME,
+    SENTRY_XHR_DATA_KEY,
     stringMatchesSomePattern
 } from '@sentry/utils';
 
 /* eslint-disable max-lines */
 
 const DEFAULT_TRACE_PROPAGATION_TARGETS = ['localhost', /^\//];
 
@@ -138,16 +139,19 @@
                 span,
                 options,
             );
         }
     }
 }
 
+/**
+ * Adds sentry-trace and baggage headers to the various forms of fetch headers
+ */
 function addTracingHeadersToFetchRequest(
-    request,
+    request, // unknown is actually type Request but we can't export DOM types from this package,
     dynamicSamplingContext,
     span,
     options
 
     ,
 ) {
     const sentryBaggageHeader = dynamicSamplingContextToSentryBaggageHeader(dynamicSamplingContext);
@@ -163,15 +167,15 @@
         };
     } else if (typeof Headers !== 'undefined' && isInstanceOf(headers, Headers)) {
         const newHeaders = new Headers(headers);
 
         newHeaders.append('sentry-trace', sentryTraceHeader);
 
         if (sentryBaggageHeader) {
-            // If the same header is appended miultiple times the browser will merge the values into a single request header.
+            // If the same header is appended multiple times the browser will merge the values into a single request header.
             // Its therefore safe to simply push a "baggage" entry, even though there might already be another baggage header.
             newHeaders.append(BAGGAGE_HEADER_NAME, sentryBaggageHeader);
         }
 
         return newHeaders;
     } else if (Array.isArray(headers)) {
         const newHeaders = [...headers, ['sentry-trace', sentryTraceHeader]];
@@ -210,32 +214,33 @@
  */
 function xhrCallback(
     handlerData,
     shouldCreateSpan,
     shouldAttachHeaders,
     spans,
 ) {
+    const xhr = handlerData.xhr;
+    const sentryXhrData = xhr && xhr[SENTRY_XHR_DATA_KEY];
+
     if (
         !hasTracingEnabled() ||
-        (handlerData.xhr && handlerData.xhr.__sentry_own_request__) ||
-        !(handlerData.xhr && handlerData.xhr.__sentry_xhr__ && shouldCreateSpan(handlerData.xhr.__sentry_xhr__.url))
+        (xhr && xhr.__sentry_own_request__) ||
+        !(xhr && sentryXhrData && shouldCreateSpan(sentryXhrData.url))
     ) {
         return;
     }
 
-    const xhr = handlerData.xhr.__sentry_xhr__;
-
     // check first if the request has finished and is tracked by an existing span which should now end
     if (handlerData.endTimestamp) {
-        const spanId = handlerData.xhr.__sentry_xhr_span_id__;
+        const spanId = xhr.__sentry_xhr_span_id__;
         if (!spanId) return;
 
         const span = spans[spanId];
         if (span) {
-            span.setHttpStatus(xhr.status_code);
+            span.setHttpStatus(sentryXhrData.status_code);
             span.finish();
 
             // eslint-disable-next-line @typescript-eslint/no-dynamic-delete
             delete spans[spanId];
         }
         return;
     }
@@ -243,48 +248,49 @@
     const currentScope = getCurrentHub().getScope();
     const currentSpan = currentScope && currentScope.getSpan();
     const activeTransaction = currentSpan && currentSpan.transaction;
 
     if (currentSpan && activeTransaction) {
         const span = currentSpan.startChild({
             data: {
-                ...xhr.data,
+                ...sentryXhrData.data,
                 type: 'xhr',
-                method: xhr.method,
-                url: xhr.url,
+                method: sentryXhrData.method,
+                url: sentryXhrData.url,
             },
-            description: `${xhr.method} ${xhr.url}`,
+            description: `${sentryXhrData.method} ${sentryXhrData.url}`,
             op: 'http.client',
         });
 
-        handlerData.xhr.__sentry_xhr_span_id__ = span.spanId;
-        spans[handlerData.xhr.__sentry_xhr_span_id__] = span;
+        xhr.__sentry_xhr_span_id__ = span.spanId;
+        spans[xhr.__sentry_xhr_span_id__] = span;
 
-        if (handlerData.xhr.setRequestHeader && shouldAttachHeaders(handlerData.xhr.__sentry_xhr__.url)) {
+        if (xhr.setRequestHeader && shouldAttachHeaders(sentryXhrData.url)) {
             try {
-                handlerData.xhr.setRequestHeader('sentry-trace', span.toTraceparent());
+                xhr.setRequestHeader('sentry-trace', span.toTraceparent());
 
                 const dynamicSamplingContext = activeTransaction.getDynamicSamplingContext();
                 const sentryBaggageHeader = dynamicSamplingContextToSentryBaggageHeader(dynamicSamplingContext);
 
                 if (sentryBaggageHeader) {
                     // From MDN: "If this method is called several times with the same header, the values are merged into one single request header."
                     // We can therefore simply set a baggage header without checking what was there before
                     // https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/setRequestHeader
-                    handlerData.xhr.setRequestHeader(BAGGAGE_HEADER_NAME, sentryBaggageHeader);
+                    xhr.setRequestHeader(BAGGAGE_HEADER_NAME, sentryBaggageHeader);
                 }
             } catch (_) {
                 // Error: InvalidStateError: Failed to execute 'setRequestHeader' on 'XMLHttpRequest': The object's state must be OPENED.
             }
         }
     }
 }
 
 export {
     DEFAULT_TRACE_PROPAGATION_TARGETS,
+    addTracingHeadersToFetchRequest,
     defaultRequestInstrumentationOptions,
     fetchCallback,
     instrumentOutgoingRequests,
     shouldAttachHeaders,
     xhrCallback
 };
 //# sourceMappingURL=request.js.map
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/router.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/router.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -22,16 +22,16 @@
 
     let startingUrl = WINDOW.location.href;
 
     let activeTransaction;
     if (startTransactionOnPageLoad) {
         activeTransaction = customStartTransaction({
             name: WINDOW.location.pathname,
-            // pageload should always start at timeOrigin
-            startTimestamp: browserPerformanceTimeOrigin,
+            // pageload should always start at timeOrigin (and needs to be in s, not ms)
+            startTimestamp: browserPerformanceTimeOrigin ? browserPerformanceTimeOrigin / 1000 : undefined,
             op: 'pageload',
             metadata: {
                 source: 'url'
             },
         });
     }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getCLS.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getCLS.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getFID.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getFID.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getLCP.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getLCP.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/bindReporter.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/bindReporter.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/generateUniqueID.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/generateUniqueID.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getActivationStart.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getActivationStart.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getNavigationEntry.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getNavigationEntry.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getVisibilityWatcher.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getVisibilityWatcher.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/initMetric.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/initMetric.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/observe.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/observe.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/onHidden.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/onHidden.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/extensions.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/extensions.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -24,17 +24,15 @@
             ;
             return new integration.Mongo();
         },
         mongoose() {
             const integration = dynamicRequire(module, './node/integrations/mongo')
 
             ;
-            return new integration.Mongo({
-                mongoose: true
-            });
+            return new integration.Mongo();
         },
         mysql() {
             const integration = dynamicRequire(module, './node/integrations/mysql')
 
             ;
             return new integration.Mysql();
         },
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/index.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -49,14 +49,15 @@
 from './node/integrations/lazy.js';
 export {
     BROWSER_TRACING_INTEGRATION_ID,
     BrowserTracing
 }
 from './browser/browsertracing.js';
 export {
+    addTracingHeadersToFetchRequest,
     defaultRequestInstrumentationOptions,
     instrumentOutgoingRequests
 }
 from './browser/request.js';
 export {
     addExtensionMethods
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/apollo.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/apollo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/express.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/express.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/graphql.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/graphql.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/lazy.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/lazy.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mongo.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mongo.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -211,14 +211,15 @@
         operation,
         args,
     ) {
         const data = {
             collectionName: collection.collectionName,
             dbName: collection.dbName,
             namespace: collection.namespace,
+            'db.system': 'mongodb',
         };
         const spanContext = {
             op: 'db',
             description: operation,
             data,
         };
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mysql.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mysql.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -57,14 +57,17 @@
         fill(pkg, 'createQuery', function(orig) {
             return function(options, values, callback) {
                 const scope = getCurrentHub().getScope();
                 const parentSpan = _optionalChain([scope, 'optionalAccess', _2 => _2.getSpan, 'call', _3 => _3()]);
                 const span = _optionalChain([parentSpan, 'optionalAccess', _4 => _4.startChild, 'call', _5 => _5({
                     description: typeof options === 'string' ? options : (options).sql,
                     op: 'db',
+                    data: {
+                        'db.system': 'mysql',
+                    },
                 })]);
 
                 if (typeof callback === 'function') {
                     return orig.call(this, options, values, function(err, result, fields) {
                         _optionalChain([span, 'optionalAccess', _6 => _6.finish, 'call', _7 => _7()]);
                         callback(err, result, fields);
                     });
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/postgres.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/postgres.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -72,14 +72,17 @@
         fill(Client.prototype, 'query', function(orig) {
             return function(config, values, callback) {
                 const scope = getCurrentHub().getScope();
                 const parentSpan = _optionalChain([scope, 'optionalAccess', _4 => _4.getSpan, 'call', _5 => _5()]);
                 const span = _optionalChain([parentSpan, 'optionalAccess', _6 => _6.startChild, 'call', _7 => _7({
                     description: typeof config === 'string' ? config : (config).text,
                     op: 'db',
+                    data: {
+                        'db.system': 'postgresql',
+                    },
                 })]);
 
                 if (typeof callback === 'function') {
                     return orig.call(this, config, values, function(err, result) {
                         _optionalChain([span, 'optionalAccess', _8 => _8.finish, 'call', _9 => _9()]);
                         callback(err, result);
                     });
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,12 @@
 import {
-    _optionalChain
-} from '@sentry/utils/esm/buildPolyfills';
+    trace
+} from '@sentry/core';
 import {
-    logger,
-    isThenable
+    logger
 } from '@sentry/utils';
 import {
     shouldDisableAutoInstrumentation
 } from './utils/node-utils.js';
 
 function isValidPrismaClient(possibleClient) {
     return possibleClient && !!(possibleClient)['$use'];
@@ -59,36 +58,25 @@
 
         if (shouldDisableAutoInstrumentation(getCurrentHub)) {
             (typeof __SENTRY_DEBUG__ === 'undefined' || __SENTRY_DEBUG__) && logger.log('Prisma Integration is skipped because of instrumenter configuration.');
             return;
         }
 
         this._client.$use((params, next) => {
-            const scope = getCurrentHub().getScope();
-            const parentSpan = _optionalChain([scope, 'optionalAccess', _2 => _2.getSpan, 'call', _3 => _3()]);
-
             const action = params.action;
             const model = params.model;
-
-            const span = _optionalChain([parentSpan, 'optionalAccess', _4 => _4.startChild, 'call', _5 => _5({
-                description: model ? `${model} ${action}` : action,
-                op: 'db.sql.prisma',
-            })]);
-
-            const rv = next(params);
-
-            if (isThenable(rv)) {
-                return rv.then((res) => {
-                    _optionalChain([span, 'optionalAccess', _6 => _6.finish, 'call', _7 => _7()]);
-                    return res;
-                });
-            }
-
-            _optionalChain([span, 'optionalAccess', _8 => _8.finish, 'call', _9 => _9()]);
-            return rv;
+            return trace({
+                    name: model ? `${model} ${action}` : action,
+                    op: 'db.sql.prisma',
+                    data: {
+                        'db.system': 'prisma'
+                    }
+                },
+                () => next(params),
+            );
         });
     }
 }
 Prisma.__initStatic();
 
 export {
     Prisma
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/agent-base/dist/src/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/agent-base/dist/src/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/agent-base/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/agent-base/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/build/lib/boolean.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/build/lib/boolean.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/build/lib/isBooleanable.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/build/lib/isBooleanable.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/boolean/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/boolean/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/cookie/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/cookie/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/cookie/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/cookie/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/src/browser.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/src/browser.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/src/common.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/src/common.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/debug/src/node.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/debug/src/node.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/define-properties/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/define-properties/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/define-properties/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/define-properties/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/detect-node/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/detect-node/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/es6-error/es6/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/es6-error/es6/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/es6-error/lib/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/es6-error/lib/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/es6-error/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/es6-error/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/escape-string-regexp/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/.jscs.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/.jscs.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/implementation.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/implementation.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/function-bind/test/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/function-bind/test/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/get-intrinsic/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/get-intrinsic/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/get-intrinsic/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/get-intrinsic/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/get-intrinsic/test/GetIntrinsic.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/get-intrinsic/test/GetIntrinsic.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/classes/Agent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/classes/Agent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/classes/HttpProxyAgent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/classes/HttpProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/classes/HttpsProxyAgent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/classes/HttpsProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/classes/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/classes/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/errors.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/errors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/factories/createGlobalProxyAgent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/factories/createGlobalProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/factories/createProxyController.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/factories/createProxyController.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/factories/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/factories/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/routines/bootstrap.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/routines/bootstrap.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/utilities/bindHttpMethod.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/utilities/bindHttpMethod.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/utilities/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/utilities/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/utilities/isUrlMatchingNoProxy.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/utilities/isUrlMatchingNoProxy.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/dist/utilities/parseProxyUrl.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/dist/utilities/parseProxyUrl.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/classes/Agent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/classes/Agent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/classes/HttpProxyAgent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/classes/HttpProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/classes/HttpsProxyAgent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/classes/HttpsProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/factories/createGlobalProxyAgent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/factories/createGlobalProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/factories/createProxyController.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/factories/createProxyController.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/routines/bootstrap.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/routines/bootstrap.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/types.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/types.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/utilities/bindHttpMethod.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/utilities/bindHttpMethod.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/utilities/isUrlMatchingNoProxy.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/utilities/isUrlMatchingNoProxy.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/global-agent/src/utilities/parseProxyUrl.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/global-agent/src/utilities/parseProxyUrl.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/shim.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/shim.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/test/native.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/test/native.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/test/shimmed.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/test/shimmed.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/globalthis/test/tests.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/globalthis/test/tests.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-property-descriptors/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-property-descriptors/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-property-descriptors/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-property-descriptors/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-property-descriptors/test/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-property-descriptors/test/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/shams.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/shams.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/test/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/test/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/test/shams/core-js.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/test/shams/core-js.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/test/shams/get-own-property-symbols.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/test/shams/get-own-property-symbols.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/has-symbols/test/tests.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/has-symbols/test/tests.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/https-proxy-agent/dist/agent.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/https-proxy-agent/dist/agent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/https-proxy-agent/dist/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/https-proxy-agent/dist/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/https-proxy-agent/dist/parse-proxy-response.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/https-proxy-agent/dist/parse-proxy-response.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/https-proxy-agent/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/https-proxy-agent/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/json-stringify-safe/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/json-stringify-safe/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/json-stringify-safe/stringify.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/json-stringify-safe/stringify.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/json-stringify-safe/test/stringify_test.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/json-stringify-safe/test/stringify_test.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru-cache/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru-cache/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru-cache/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru-cache/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/benchmark.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/benchmark.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/lru.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/lru.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/lru_map/test.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/lru_map/test.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/matcher/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/matcher/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/matcher/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/matcher/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/ms/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/ms/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/ms/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/ms/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/object-keys/implementation.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/object-keys/implementation.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/object-keys/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/object-keys/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/object-keys/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/object-keys/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/createLogger.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/createLogger.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/createMockLogger.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/createMockLogger.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/createNodeWriter.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/createNodeWriter.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/createRoarrInititialGlobalState.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/createRoarrInititialGlobalState.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/factories/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/factories/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/dist/log.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/dist/log.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/roarr/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/roarr/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/bin/semver.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/bin/semver.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -19,15 +19,18 @@
 
 let coerce = false
 
 let rtl = false
 
 let identifier
 
+let identifierBase
+
 const semver = require('../')
+const parseOptions = require('../internal/parse-options')
 
 let reverse = false
 
 let options = {}
 
 const main = () => {
     if (!argv.length) {
@@ -81,14 +84,20 @@
             case '--preid':
                 identifier = argv.shift()
                 break
             case '-r':
             case '--range':
                 range.push(argv.shift())
                 break
+            case '-n':
+                identifierBase = argv.shift()
+                if (identifierBase === 'false') {
+                    identifierBase = false
+                }
+                break
             case '-c':
             case '--coerce':
                 coerce = true
                 break
             case '--rtl':
                 rtl = true
                 break
@@ -101,19 +110,19 @@
                 return help()
             default:
                 versions.push(a)
                 break
         }
     }
 
-    options = {
-        loose: loose,
-        includePrerelease: includePrerelease,
-        rtl: rtl
-    }
+    options = parseOptions({
+        loose,
+        includePrerelease,
+        rtl
+    })
 
     versions = versions.map((v) => {
         return coerce ? (semver.coerce(v, options) || {
             version: v
         }).version : v
     }).filter((v) => {
         return semver.valid(v)
@@ -146,15 +155,15 @@
 const success = () => {
     const compare = reverse ? 'rcompare' : 'compare'
     versions.sort((a, b) => {
         return semver[compare](a, b, options)
     }).map((v) => {
         return semver.clean(v, options)
     }).map((v) => {
-        return inc ? semver.inc(v, inc, options, identifier) : v
+        return inc ? semver.inc(v, inc, options, identifier, identifierBase) : v
     }).forEach((v, i, _) => {
         console.log(v)
     })
 }
 
 const help = () => console.log(
     `SemVer ${version}
@@ -191,14 +200,19 @@
 
 --rtl
         Coerce version strings right to left
 
 --ltr
         Coerce version strings left to right (default)
 
+-n <base>
+        Base number to be used for the prerelease identifier.
+        Can be either 0 or 1, or false to omit the number altogether.
+        Defaults to 0.
+
 Program exits successfully if any valid version satisfies
 all supplied ranges, and prints all satisfying versions.
 
 If no satisfying versions are found, then exits failure.
 
 Versions are printed in ascending order, so supplying
 multiple versions to the utility will just sort them.`)
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/classes/comparator.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/classes/comparator.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -74,59 +74,63 @@
     }
 
     intersects(comp, options) {
         if (!(comp instanceof Comparator)) {
             throw new TypeError('a Comparator is required')
         }
 
-        if (!options || typeof options !== 'object') {
-            options = {
-                loose: !!options,
-                includePrerelease: false,
-            }
-        }
-
         if (this.operator === '') {
             if (this.value === '') {
                 return true
             }
             return new Range(comp.value, options).test(this.value)
         } else if (comp.operator === '') {
             if (comp.value === '') {
                 return true
             }
             return new Range(this.value, options).test(comp.semver)
         }
 
-        const sameDirectionIncreasing =
-            (this.operator === '>=' || this.operator === '>') &&
-            (comp.operator === '>=' || comp.operator === '>')
-        const sameDirectionDecreasing =
-            (this.operator === '<=' || this.operator === '<') &&
-            (comp.operator === '<=' || comp.operator === '<')
-        const sameSemVer = this.semver.version === comp.semver.version
-        const differentDirectionsInclusive =
-            (this.operator === '>=' || this.operator === '<=') &&
-            (comp.operator === '>=' || comp.operator === '<=')
-        const oppositeDirectionsLessThan =
-            cmp(this.semver, '<', comp.semver, options) &&
-            (this.operator === '>=' || this.operator === '>') &&
-            (comp.operator === '<=' || comp.operator === '<')
-        const oppositeDirectionsGreaterThan =
-            cmp(this.semver, '>', comp.semver, options) &&
-            (this.operator === '<=' || this.operator === '<') &&
-            (comp.operator === '>=' || comp.operator === '>')
-
-        return (
-            sameDirectionIncreasing ||
-            sameDirectionDecreasing ||
-            (sameSemVer && differentDirectionsInclusive) ||
-            oppositeDirectionsLessThan ||
-            oppositeDirectionsGreaterThan
-        )
+        options = parseOptions(options)
+
+        // Special cases where nothing can possibly be lower
+        if (options.includePrerelease &&
+            (this.value === '<0.0.0-0' || comp.value === '<0.0.0-0')) {
+            return false
+        }
+        if (!options.includePrerelease &&
+            (this.value.startsWith('<0.0.0') || comp.value.startsWith('<0.0.0'))) {
+            return false
+        }
+
+        // Same direction increasing (> or >=)
+        if (this.operator.startsWith('>') && comp.operator.startsWith('>')) {
+            return true
+        }
+        // Same direction decreasing (< or <=)
+        if (this.operator.startsWith('<') && comp.operator.startsWith('<')) {
+            return true
+        }
+        // same SemVer and both sides are inclusive (<= or >=)
+        if (
+            (this.semver.version === comp.semver.version) &&
+            this.operator.includes('=') && comp.operator.includes('=')) {
+            return true
+        }
+        // opposite directions less than
+        if (cmp(this.semver, '<', comp.semver, options) &&
+            this.operator.startsWith('>') && comp.operator.startsWith('<')) {
+            return true
+        }
+        // opposite directions greater than
+        if (cmp(this.semver, '>', comp.semver, options) &&
+            this.operator.startsWith('<') && comp.operator.startsWith('>')) {
+            return true
+        }
+        return false
     }
 }
 
 module.exports = Comparator
 
 const parseOptions = require('../internal/parse-options')
 const {
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/classes/range.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/classes/range.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -79,16 +79,18 @@
     }
 
     parseRange(range) {
         range = range.trim()
 
         // memoize range parsing for performance.
         // this is a very hot path, and fully deterministic.
-        const memoOpts = Object.keys(this.options).join(',')
-        const memoKey = `parseRange:${memoOpts}:${range}`
+        const memoOpts =
+            (this.options.includePrerelease && FLAG_INCLUDE_PRERELEASE) |
+            (this.options.loose && FLAG_LOOSE)
+        const memoKey = memoOpts + ':' + range
         const cached = cache.get(memoKey)
         if (cached) {
             return cached
         }
 
         const loose = this.options.loose
         // `1.2.3 - 1.2.4` => `>=1.2.3 <=1.2.4`
@@ -188,14 +190,15 @@
             if (testSet(this.set[i], version, this.options)) {
                 return true
             }
         }
         return false
     }
 }
+
 module.exports = Range
 
 const LRU = require('lru-cache')
 const cache = new LRU({
     max: 1000
 })
 
@@ -206,14 +209,18 @@
 const {
     re,
     t,
     comparatorTrimReplace,
     tildeTrimReplace,
     caretTrimReplace,
 } = require('../internal/re')
+const {
+    FLAG_INCLUDE_PRERELEASE,
+    FLAG_LOOSE
+} = require('../internal/constants')
 
 const isNullSet = c => c.value === '<0.0.0-0'
 const isAny = c => c.value === ''
 
 // take a set of comparators and determine whether there
 // exists a version which can satisfy it
 const isSatisfiable = (comparators, options) => {
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/classes/semver.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/classes/semver.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
             if (version.loose === !!options.loose &&
                 version.includePrerelease === !!options.includePrerelease) {
                 return version
             } else {
                 version = version.version
             }
         } else if (typeof version !== 'string') {
-            throw new TypeError(`Invalid Version: ${version}`)
+            throw new TypeError(`Invalid Version: ${require('util').inspect(version)}`)
         }
 
         if (version.length > MAX_LENGTH) {
             throw new TypeError(
                 `version is longer than ${MAX_LENGTH} characters`
             )
         }
@@ -179,44 +179,44 @@
                 return compareIdentifiers(a, b)
             }
         } while (++i)
     }
 
     // preminor will bump the version up to the next minor release, and immediately
     // down to pre-release. premajor and prepatch work the same way.
-    inc(release, identifier) {
+    inc(release, identifier, identifierBase) {
         switch (release) {
             case 'premajor':
                 this.prerelease.length = 0
                 this.patch = 0
                 this.minor = 0
                 this.major++
-                this.inc('pre', identifier)
+                this.inc('pre', identifier, identifierBase)
                 break
             case 'preminor':
                 this.prerelease.length = 0
                 this.patch = 0
                 this.minor++
-                this.inc('pre', identifier)
+                this.inc('pre', identifier, identifierBase)
                 break
             case 'prepatch':
                 // If this is already a prerelease, it will bump to the next version
                 // drop any prereleases that might already exist, since they are not
                 // relevant at this point.
                 this.prerelease.length = 0
-                this.inc('patch', identifier)
-                this.inc('pre', identifier)
+                this.inc('patch', identifier, identifierBase)
+                this.inc('pre', identifier, identifierBase)
                 break
                 // If the input is a non-prerelease version, this acts the same as
                 // prepatch.
             case 'prerelease':
                 if (this.prerelease.length === 0) {
-                    this.inc('patch', identifier)
+                    this.inc('patch', identifier, identifierBase)
                 }
-                this.inc('pre', identifier)
+                this.inc('pre', identifier, identifierBase)
                 break
 
             case 'major':
                 // If this is a pre-major version, bump up to the same major version.
                 // Otherwise increment major.
                 // 1.0.0-5 bumps to 1.0.0
                 // 1.1.0 bumps to 2.0.0
@@ -250,43 +250,56 @@
                 if (this.prerelease.length === 0) {
                     this.patch++
                 }
                 this.prerelease = []
                 break
                 // This probably shouldn't be used publicly.
                 // 1.0.0 'pre' would become 1.0.0-0 which is the wrong direction.
-            case 'pre':
+            case 'pre': {
+                const base = Number(identifierBase) ? 1 : 0
+
+                if (!identifier && identifierBase === false) {
+                    throw new Error('invalid increment argument: identifier is empty')
+                }
+
                 if (this.prerelease.length === 0) {
-                    this.prerelease = [0]
+                    this.prerelease = [base]
                 } else {
                     let i = this.prerelease.length
                     while (--i >= 0) {
                         if (typeof this.prerelease[i] === 'number') {
                             this.prerelease[i]++
                             i = -2
                         }
                     }
                     if (i === -1) {
                         // didn't increment anything
-                        this.prerelease.push(0)
+                        if (identifier === this.prerelease.join('.') && identifierBase === false) {
+                            throw new Error('invalid increment argument: identifier already exists')
+                        }
+                        this.prerelease.push(base)
                     }
                 }
                 if (identifier) {
                     // 1.2.0-beta.1 bumps to 1.2.0-beta.2,
                     // 1.2.0-beta.fooblz or 1.2.0-beta bumps to 1.2.0-beta.0
+                    let prerelease = [identifier, base]
+                    if (identifierBase === false) {
+                        prerelease = [identifier]
+                    }
                     if (compareIdentifiers(this.prerelease[0], identifier) === 0) {
                         if (isNaN(this.prerelease[1])) {
-                            this.prerelease = [identifier, 0]
+                            this.prerelease = prerelease
                         }
                     } else {
-                        this.prerelease = [identifier, 0]
+                        this.prerelease = prerelease
                     }
                 }
                 break
-
+            }
             default:
                 throw new Error(`invalid increment argument: ${release}`)
         }
         this.format()
         this.raw = this.version
         return this
     }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/cmp.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/cmp.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/functions/coerce.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/functions/coerce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/index.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -79,10 +79,11 @@
     simplifyRange,
     subset,
     SemVer,
     re: internalRe.re,
     src: internalRe.src,
     tokens: internalRe.t,
     SEMVER_SPEC_VERSION: constants.SEMVER_SPEC_VERSION,
+    RELEASE_TYPES: constants.RELEASE_TYPES,
     compareIdentifiers: identifiers.compareIdentifiers,
     rcompareIdentifiers: identifiers.rcompareIdentifiers,
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/internal/re.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/internal/re.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9425925925925925%*

 * *Differences: {"'devDependencies'": "{'@npmcli/eslint-config': '^4.0.0', '@npmcli/template-oss': '4.13.0'}",*

 * * "'templateOSS'": "{'version': '4.13.0', 'npmSpec': '8', 'publish': 'true', delete: ['content']}",*

 * * "'version'": "'7.5.0'"}*

```diff
@@ -4,16 +4,16 @@
         "semver": "bin/semver.js"
     },
     "dependencies": {
         "lru-cache": "^6.0.0"
     },
     "description": "The semantic version parser used by npm.",
     "devDependencies": {
-        "@npmcli/eslint-config": "^3.0.1",
-        "@npmcli/template-oss": "4.4.4",
+        "@npmcli/eslint-config": "^4.0.0",
+        "@npmcli/template-oss": "4.13.0",
         "tap": "^16.0.0"
     },
     "engines": {
         "node": ">=10"
     },
     "files": [
         "bin/",
@@ -65,22 +65,23 @@
             "10.0.0",
             "10.x",
             "12.x",
             "14.x",
             "16.x",
             "18.x"
         ],
-        "content": "./scripts",
         "distPaths": [
             "classes/",
             "functions/",
             "internal/",
             "ranges/",
             "index.js",
             "preload.js",
             "range.bnf"
         ],
         "engines": ">=10",
-        "version": "4.4.4"
+        "npmSpec": "8",
+        "publish": "true",
+        "version": "4.13.0"
     },
-    "version": "7.3.8"
+    "version": "7.5.0"
 }
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/max-satisfying.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/max-satisfying.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/min-satisfying.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/min-satisfying.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/min-version.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/min-version.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/outside.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/outside.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/simplify.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/simplify.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver/ranges/subset.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver/ranges/subset.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -66,34 +66,37 @@
         if (sawNonNull) {
             return false
         }
     }
     return true
 }
 
+const minimumVersionWithPreRelease = [new Comparator('>=0.0.0-0')]
+const minimumVersion = [new Comparator('>=0.0.0')]
+
 const simpleSubset = (sub, dom, options) => {
     if (sub === dom) {
         return true
     }
 
     if (sub.length === 1 && sub[0].semver === ANY) {
         if (dom.length === 1 && dom[0].semver === ANY) {
             return true
         } else if (options.includePrerelease) {
-            sub = [new Comparator('>=0.0.0-0')]
+            sub = minimumVersionWithPreRelease
         } else {
-            sub = [new Comparator('>=0.0.0')]
+            sub = minimumVersion
         }
     }
 
     if (dom.length === 1 && dom[0].semver === ANY) {
         if (options.includePrerelease) {
             return true
         } else {
-            dom = [new Comparator('>=0.0.0')]
+            dom = minimumVersion
         }
     }
 
     const eqSet = new Set()
     let gt, lt
     for (const c of sub) {
         if (c.operator === '>' || c.operator === '>=') {
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/semver-compare/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/semver-compare/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/serialize-error/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/serialize-error/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/serialize-error/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/serialize-error/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/110.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/110.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/213.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/213.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/31.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/31.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/38.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/38.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/384.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/384.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/395.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/395.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/477.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/477.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/503.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/503.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/519.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/519.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/522.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/522.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/535.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/535.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/542.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/542.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/575.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/575.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/663.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/663.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/726.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/726.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/741.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/741.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/784.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/784.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/790.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/790.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/831.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/831.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/85.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/85.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/855.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/855.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/875.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/875.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/895.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/895.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/905.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/905.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/917.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/917.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/95.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/95.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/959.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/959.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/970.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/970.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/974.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/974.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/989.index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/989.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/sql-wasm.wasm` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/sql-wasm.wasm`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/dist/cli/thirdPartyNotice.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/dist/cli/thirdPartyNotice.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/distPackage.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/distPackage.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/package.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/package.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/__about__.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/__init__.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/_compat.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/_structures.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/_typing.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/markers.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/requirements.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/specifiers.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/tags.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/utils.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/packaging/version.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/packaging/version.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pip_resolve.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pip_resolve.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pipfile.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pipfile.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pyparsing.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pyparsing.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pytoml/parser.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pytoml/parser.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/pytoml/writer.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/pytoml/writer.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/reqPackage.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/reqPackage.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/requirements/fragment.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/requirements/fragment.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/requirements/parser.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/requirements/parser.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/requirements/requirement.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/requirements/requirement.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/setup_file.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/setup_file.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/test_pip_resolve.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/test_pip_resolve.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/pysrc/utils.py` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/pysrc/utils.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/wrapper_dist/bootstrap.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/wrapper_dist/bootstrap.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/wrapper_dist/common.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/wrapper_dist/common.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/snyk/wrapper_dist/index.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/snyk/wrapper_dist/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/dist/sprintf.min.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/dist/sprintf.min.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/src/angular-sprintf.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/src/angular-sprintf.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/sprintf-js/src/sprintf.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/sprintf-js/src/sprintf.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/type-fest/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/type-fest/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/yallist/package.json` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/yallist/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/node_modules/yallist/yallist.js` & `c2cciutils-1.6.0.dev93/c2cciutils/node_modules/yallist/yallist.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/package-lock.json` & `c2cciutils-1.6.0.dev93/c2cciutils/package-lock.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.982077710968082%*

 * *Differences: {"'dependencies'": "{'@sentry-internal/tracing': {'version': '7.50.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@sentry-internal/tracing/-/tracing-7.50.0.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-4TQ4vN0aMBWsUXfJWk2xbe4x7fKfwCXgXKTtHC/ocwwKM+0EefV5Iw9YFG8IrIQN4vMtuRzktqcs9q0/Sbv7tg==', "*

 * *                   "'requires': {'@sentry/core': '7.50.0', '@sentry/types': '7.50.0', "*

 * *                   "'@sentry/utils': '7.50.0'}, delete: ['dependencies']}, '@sentry/c […]*

```diff
@@ -1,86 +1,58 @@
 {
     "dependencies": {
         "@sentry-internal/tracing": {
-            "dependencies": {
-                "tslib": {
-                    "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-                    "version": "1.14.1"
-                }
-            },
-            "integrity": "sha512-KYoppa7PPL8Er7bdPoxTNUfIY804JL7hhOEomQHYD22rLynwQ4AaLm3YEY75QWwcGb0B7ZDMV+tSumW7Rxuwuw==",
+            "integrity": "sha512-4TQ4vN0aMBWsUXfJWk2xbe4x7fKfwCXgXKTtHC/ocwwKM+0EefV5Iw9YFG8IrIQN4vMtuRzktqcs9q0/Sbv7tg==",
             "requires": {
-                "@sentry/core": "7.46.0",
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry/core": "7.50.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "tslib": "^1.9.3"
             },
-            "resolved": "https://registry.npmjs.org/@sentry-internal/tracing/-/tracing-7.46.0.tgz",
-            "version": "7.46.0"
+            "resolved": "https://registry.npmjs.org/@sentry-internal/tracing/-/tracing-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "@sentry/core": {
-            "dependencies": {
-                "tslib": {
-                    "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-                    "version": "1.14.1"
-                }
-            },
-            "integrity": "sha512-BnNHGh/ZTztqQedFko7vb2u6yLs/kWesOQNivav32ZbsEpVCjcmG1gOJXh2YmGIvj3jXOC9a4xfIuh+lYFcA6A==",
+            "integrity": "sha512-6oD1a3fYs4aiNK7tuJSd88LHjYJAetd7ZK/AfJniU7zWKj4jxIYfO8nhm0qdnhEDs81RcweVDmPhWm3Kwrzzsg==",
             "requires": {
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "tslib": "^1.9.3"
             },
-            "resolved": "https://registry.npmjs.org/@sentry/core/-/core-7.46.0.tgz",
-            "version": "7.46.0"
+            "resolved": "https://registry.npmjs.org/@sentry/core/-/core-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "@sentry/node": {
-            "dependencies": {
-                "tslib": {
-                    "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-                    "version": "1.14.1"
-                }
-            },
-            "integrity": "sha512-+GrgJMCye2WXGarRiU5IJHCK27xg7xbPc2XjGojBKbBoZfqxVAWbXEK4bnBQgRGP1pCmrU/M6ZhVgR3dP580xA==",
+            "integrity": "sha512-11UJBKoQFMp7f8sbzeO2gENsKIUkVCNBTzuPRib7l2K1HMjSfacXmwwma7ZEs0mc3ofIZ1UYuyONAXmI1lK9cQ==",
             "requires": {
-                "@sentry-internal/tracing": "7.46.0",
-                "@sentry/core": "7.46.0",
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry-internal/tracing": "7.50.0",
+                "@sentry/core": "7.50.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "cookie": "^0.4.1",
                 "https-proxy-agent": "^5.0.0",
                 "lru_map": "^0.3.3",
                 "tslib": "^1.9.3"
             },
-            "resolved": "https://registry.npmjs.org/@sentry/node/-/node-7.46.0.tgz",
-            "version": "7.46.0"
+            "resolved": "https://registry.npmjs.org/@sentry/node/-/node-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "@sentry/types": {
-            "integrity": "sha512-2FMEMgt2h6u7AoELhNhu9L54GAh67KKfK2pJ1kEXJHmWxM9FSCkizjLs/t+49xtY7jEXr8qYq8bV967VfDPQ9g==",
-            "resolved": "https://registry.npmjs.org/@sentry/types/-/types-7.46.0.tgz",
-            "version": "7.46.0"
+            "integrity": "sha512-Zo9vyI98QNeYT0K0y57Rb4JRWDaPEgmp+QkQ4CRQZFUTWetO5fvPZ4Gb/R7TW16LajuHZlbJBHmvmNj2pkL2kw==",
+            "resolved": "https://registry.npmjs.org/@sentry/types/-/types-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "@sentry/utils": {
-            "dependencies": {
-                "tslib": {
-                    "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-                    "version": "1.14.1"
-                }
-            },
-            "integrity": "sha512-elRezDAF84guMG0OVIIZEWm6wUpgbda4HGks98CFnPsrnMm3N1bdBI9XdlxYLtf+ir5KsGR5YlEIf/a0kRUwAQ==",
+            "integrity": "sha512-iyPwwC6fwJsiPhH27ZbIiSsY5RaccHBqADS2zEjgKYhmP4P9WGgHRDrvLEnkOjqQyKNb6c0yfmv83n0uxYnolw==",
             "requires": {
-                "@sentry/types": "7.46.0",
+                "@sentry/types": "7.50.0",
                 "tslib": "^1.9.3"
             },
-            "resolved": "https://registry.npmjs.org/@sentry/utils/-/utils-7.46.0.tgz",
-            "version": "7.46.0"
+            "resolved": "https://registry.npmjs.org/@sentry/utils/-/utils-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "agent-base": {
             "integrity": "sha512-RZNwNclF7+MS/8bDg70amg32dyeZGZxiDuQmZxKLAlQjr3jGyLx+4Kkk58UO7D2QdgFIQCovuSuZESne6RG6XQ==",
             "requires": {
                 "debug": "4"
             },
             "resolved": "https://registry.npmjs.org/agent-base/-/agent-base-6.0.2.tgz",
@@ -240,20 +212,20 @@
                 "semver-compare": "^1.0.0",
                 "sprintf-js": "^1.1.2"
             },
             "resolved": "https://registry.npmjs.org/roarr/-/roarr-2.15.4.tgz",
             "version": "2.15.4"
         },
         "semver": {
-            "integrity": "sha512-NB1ctGL5rlHrPJtFDVIVzTyQylMLu9N9VICA6HSFJo8MCGVTMW6gfpicwKmmK/dAjTOrqu5l63JJOpDSrAis3A==",
+            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
             "requires": {
                 "lru-cache": "^6.0.0"
             },
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.3.8.tgz",
-            "version": "7.3.8"
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+            "version": "7.5.0"
         },
         "semver-compare": {
             "integrity": "sha512-YM3/ITh2MJ5MtzaM429anh+x2jiLVjqILF4m4oyQB18W7Ggea7BfqdH/wGMK7dDiMghv/6WG7znWMwUDzJiXow==",
             "resolved": "https://registry.npmjs.org/semver-compare/-/semver-compare-1.0.0.tgz",
             "version": "1.0.0"
         },
         "serialize-error": {
@@ -274,14 +246,19 @@
             "version": "1.1150.0"
         },
         "sprintf-js": {
             "integrity": "sha512-VE0SOVEHCk7Qc8ulkWw3ntAzXuqf7S2lvwQaDLRnUeIEaKNQJzV6BwmLKhOqT61aGhfUMrXeaBk+oDGCzvhcug==",
             "resolved": "https://registry.npmjs.org/sprintf-js/-/sprintf-js-1.1.2.tgz",
             "version": "1.1.2"
         },
+        "tslib": {
+            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
+            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
+            "version": "1.14.1"
+        },
         "type-fest": {
             "integrity": "sha512-34R7HTnG0XIJcBSn5XhDd7nNFPRcXYRZrBB2O2jdKqYODldSzBAqzsWoZYYvduky73toYS/ESqxPvkDf/F0XMg==",
             "resolved": "https://registry.npmjs.org/type-fest/-/type-fest-0.13.1.tgz",
             "version": "0.13.1"
         },
         "yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
@@ -297,96 +274,76 @@
                 "snyk": "1.1150.0"
             },
             "name": "c2ccicheck",
             "version": "1.0.0"
         },
         "node_modules/@sentry-internal/tracing": {
             "dependencies": {
-                "@sentry/core": "7.46.0",
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry/core": "7.50.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "tslib": "^1.9.3"
             },
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-KYoppa7PPL8Er7bdPoxTNUfIY804JL7hhOEomQHYD22rLynwQ4AaLm3YEY75QWwcGb0B7ZDMV+tSumW7Rxuwuw==",
-            "resolved": "https://registry.npmjs.org/@sentry-internal/tracing/-/tracing-7.46.0.tgz",
-            "version": "7.46.0"
-        },
-        "node_modules/@sentry-internal/tracing/node_modules/tslib": {
-            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-4TQ4vN0aMBWsUXfJWk2xbe4x7fKfwCXgXKTtHC/ocwwKM+0EefV5Iw9YFG8IrIQN4vMtuRzktqcs9q0/Sbv7tg==",
+            "resolved": "https://registry.npmjs.org/@sentry-internal/tracing/-/tracing-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/@sentry/core": {
             "dependencies": {
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "tslib": "^1.9.3"
             },
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-BnNHGh/ZTztqQedFko7vb2u6yLs/kWesOQNivav32ZbsEpVCjcmG1gOJXh2YmGIvj3jXOC9a4xfIuh+lYFcA6A==",
-            "resolved": "https://registry.npmjs.org/@sentry/core/-/core-7.46.0.tgz",
-            "version": "7.46.0"
-        },
-        "node_modules/@sentry/core/node_modules/tslib": {
-            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-6oD1a3fYs4aiNK7tuJSd88LHjYJAetd7ZK/AfJniU7zWKj4jxIYfO8nhm0qdnhEDs81RcweVDmPhWm3Kwrzzsg==",
+            "resolved": "https://registry.npmjs.org/@sentry/core/-/core-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/@sentry/node": {
             "dependencies": {
-                "@sentry-internal/tracing": "7.46.0",
-                "@sentry/core": "7.46.0",
-                "@sentry/types": "7.46.0",
-                "@sentry/utils": "7.46.0",
+                "@sentry-internal/tracing": "7.50.0",
+                "@sentry/core": "7.50.0",
+                "@sentry/types": "7.50.0",
+                "@sentry/utils": "7.50.0",
                 "cookie": "^0.4.1",
                 "https-proxy-agent": "^5.0.0",
                 "lru_map": "^0.3.3",
                 "tslib": "^1.9.3"
             },
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-+GrgJMCye2WXGarRiU5IJHCK27xg7xbPc2XjGojBKbBoZfqxVAWbXEK4bnBQgRGP1pCmrU/M6ZhVgR3dP580xA==",
-            "resolved": "https://registry.npmjs.org/@sentry/node/-/node-7.46.0.tgz",
-            "version": "7.46.0"
-        },
-        "node_modules/@sentry/node/node_modules/tslib": {
-            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-11UJBKoQFMp7f8sbzeO2gENsKIUkVCNBTzuPRib7l2K1HMjSfacXmwwma7ZEs0mc3ofIZ1UYuyONAXmI1lK9cQ==",
+            "resolved": "https://registry.npmjs.org/@sentry/node/-/node-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/@sentry/types": {
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-2FMEMgt2h6u7AoELhNhu9L54GAh67KKfK2pJ1kEXJHmWxM9FSCkizjLs/t+49xtY7jEXr8qYq8bV967VfDPQ9g==",
-            "resolved": "https://registry.npmjs.org/@sentry/types/-/types-7.46.0.tgz",
-            "version": "7.46.0"
+            "integrity": "sha512-Zo9vyI98QNeYT0K0y57Rb4JRWDaPEgmp+QkQ4CRQZFUTWetO5fvPZ4Gb/R7TW16LajuHZlbJBHmvmNj2pkL2kw==",
+            "resolved": "https://registry.npmjs.org/@sentry/types/-/types-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/@sentry/utils": {
             "dependencies": {
-                "@sentry/types": "7.46.0",
+                "@sentry/types": "7.50.0",
                 "tslib": "^1.9.3"
             },
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-elRezDAF84guMG0OVIIZEWm6wUpgbda4HGks98CFnPsrnMm3N1bdBI9XdlxYLtf+ir5KsGR5YlEIf/a0kRUwAQ==",
-            "resolved": "https://registry.npmjs.org/@sentry/utils/-/utils-7.46.0.tgz",
-            "version": "7.46.0"
-        },
-        "node_modules/@sentry/utils/node_modules/tslib": {
-            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
-            "version": "1.14.1"
+            "integrity": "sha512-iyPwwC6fwJsiPhH27ZbIiSsY5RaccHBqADS2zEjgKYhmP4P9WGgHRDrvLEnkOjqQyKNb6c0yfmv83n0uxYnolw==",
+            "resolved": "https://registry.npmjs.org/@sentry/utils/-/utils-7.50.0.tgz",
+            "version": "7.50.0"
         },
         "node_modules/agent-base": {
             "dependencies": {
                 "debug": "4"
             },
             "engines": {
                 "node": ">= 6.0.0"
@@ -620,17 +577,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-NB1ctGL5rlHrPJtFDVIVzTyQylMLu9N9VICA6HSFJo8MCGVTMW6gfpicwKmmK/dAjTOrqu5l63JJOpDSrAis3A==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.3.8.tgz",
-            "version": "7.3.8"
+            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
+            "version": "7.5.0"
         },
         "node_modules/semver-compare": {
             "integrity": "sha512-YM3/ITh2MJ5MtzaM429anh+x2jiLVjqILF4m4oyQB18W7Ggea7BfqdH/wGMK7dDiMghv/6WG7znWMwUDzJiXow==",
             "resolved": "https://registry.npmjs.org/semver-compare/-/semver-compare-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/serialize-error": {
@@ -664,14 +621,19 @@
             "version": "1.1150.0"
         },
         "node_modules/sprintf-js": {
             "integrity": "sha512-VE0SOVEHCk7Qc8ulkWw3ntAzXuqf7S2lvwQaDLRnUeIEaKNQJzV6BwmLKhOqT61aGhfUMrXeaBk+oDGCzvhcug==",
             "resolved": "https://registry.npmjs.org/sprintf-js/-/sprintf-js-1.1.2.tgz",
             "version": "1.1.2"
         },
+        "node_modules/tslib": {
+            "integrity": "sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==",
+            "resolved": "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz",
+            "version": "1.14.1"
+        },
         "node_modules/type-fest": {
             "engines": {
                 "node": ">=10"
             },
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/pr_checks.py` & `c2cciutils-1.6.0.dev93/c2cciutils/pr_checks.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/publish.py` & `c2cciutils-1.6.0.dev93/c2cciutils/publish.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/schema-applications.json` & `c2cciutils-1.6.0.dev93/c2cciutils/schema-applications.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/schema.json` & `c2cciutils-1.6.0.dev93/c2cciutils/schema.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/audit.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/audit.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/clean.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/docker_logs.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/docker_logs.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/docker_versions_gen.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/docker_versions_gen.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/download_applications.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/download_applications.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/db.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/db.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/install.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/install.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/logs.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/logs.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/k8s/wait.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/k8s/wait.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/main.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/main.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/pin_pipenv.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/pin_pipenv.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/pr_checks.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/pr_checks.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/publish.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,15 +367,17 @@
         c2cciutils.configuration.PublishHelmConfig,
         config.get("publish", {}).get("helm", {}) if config.get("publish", {}).get("helm", False) else {},
     )
     if helm_config and helm_config["folders"] and version_type in helm_config.get("versions", []):
         url = "https://github.com/helm/chart-releaser/releases/download/v1.2.1/chart-releaser_1.2.1_linux_amd64.tar.gz"
         response = requests.get(url, stream=True, timeout=int(os.environ.get("C2CCIUTILS_TIMEOUT", "30")))
         with tarfile.open(fileobj=response.raw, mode="r:gz") as file:
-            file.extractall(path=os.path.expanduser("~/.local/bin"))
+            filename_re = re.compile(r"^[a-zA-Z0-9][a-zA-Z0-9._/-]*$")
+            members = [member for member in file.getmembers() if filename_re.match(member.name) is not None]
+            file.extractall(path=os.path.expanduser("~/.local/bin"), members=members)  # nosec
 
         owner, repo = full_repo_split
         commit_sha = (
             subprocess.run(["git", "rev-parse", "HEAD"], check=True, stdout=subprocess.PIPE)
             .stdout.strip()
             .decode()
         )
```

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/scripts/trigger_image_update.py` & `c2cciutils-1.6.0.dev93/c2cciutils/scripts/trigger_image_update.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/c2cciutils/security.py` & `c2cciutils-1.6.0.dev93/c2cciutils/security.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev89/pyproject.toml` & `c2cciutils-1.6.0.dev93/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "c2cciutils"
-version = "1.6.0.dev89"
+version = "1.6.0.dev93"
 description = "Common utilities for Camptocamp CI"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 keywords = ["ci"]
 repository = "https://github.com/camptocamp/c2cciutils"
 license = "FreeBSD"
 packages = [{ include = "c2cciutils" }]
```

### Comparing `c2cciutils-1.6.0.dev89/setup.py` & `c2cciutils-1.6.0.dev93/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,24 +352,14 @@
                 'node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js',
                 'node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js',
                 'node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js',
                 'node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js',
                 'node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js',
                 'node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js',
                 'node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/modules/*',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/package.json',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/package.json',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/package.json',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/tslib.js',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/tslib.js',
-                'node_modules/@sentry-internal/tracing/node_modules/tslib/tslib.js',
                 'node_modules/@sentry-internal/tracing/package.json',
                 'node_modules/@sentry/core/cjs/api.js',
                 'node_modules/@sentry/core/cjs/api.js',
                 'node_modules/@sentry/core/cjs/api.js',
                 'node_modules/@sentry/core/cjs/api.js',
                 'node_modules/@sentry/core/cjs/api.js',
                 'node_modules/@sentry/core/cjs/api.js',
@@ -594,14 +584,19 @@
                 'node_modules/@sentry/core/cjs/tracing/utils.js',
                 'node_modules/@sentry/core/cjs/tracing/utils.js',
                 'node_modules/@sentry/core/cjs/tracing/utils.js',
                 'node_modules/@sentry/core/cjs/tracing/utils.js',
                 'node_modules/@sentry/core/cjs/tracing/utils.js',
                 'node_modules/@sentry/core/cjs/transports/base.js',
                 'node_modules/@sentry/core/cjs/transports/base.js',
+                'node_modules/@sentry/core/cjs/transports/base.js',
+                'node_modules/@sentry/core/cjs/transports/multiplexed.js',
+                'node_modules/@sentry/core/cjs/transports/multiplexed.js',
+                'node_modules/@sentry/core/cjs/transports/multiplexed.js',
+                'node_modules/@sentry/core/cjs/transports/offline.js',
                 'node_modules/@sentry/core/cjs/transports/offline.js',
                 'node_modules/@sentry/core/cjs/transports/offline.js',
                 'node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js',
                 'node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js',
                 'node_modules/@sentry/core/cjs/utils/prepareEvent.js',
                 'node_modules/@sentry/core/cjs/utils/prepareEvent.js',
                 'node_modules/@sentry/core/cjs/version.js',
@@ -844,14 +839,19 @@
                 'node_modules/@sentry/core/esm/tracing/utils.js',
                 'node_modules/@sentry/core/esm/tracing/utils.js',
                 'node_modules/@sentry/core/esm/tracing/utils.js',
                 'node_modules/@sentry/core/esm/tracing/utils.js',
                 'node_modules/@sentry/core/esm/tracing/utils.js',
                 'node_modules/@sentry/core/esm/transports/base.js',
                 'node_modules/@sentry/core/esm/transports/base.js',
+                'node_modules/@sentry/core/esm/transports/base.js',
+                'node_modules/@sentry/core/esm/transports/multiplexed.js',
+                'node_modules/@sentry/core/esm/transports/multiplexed.js',
+                'node_modules/@sentry/core/esm/transports/multiplexed.js',
+                'node_modules/@sentry/core/esm/transports/offline.js',
                 'node_modules/@sentry/core/esm/transports/offline.js',
                 'node_modules/@sentry/core/esm/transports/offline.js',
                 'node_modules/@sentry/core/esm/utils/hasTracingEnabled.js',
                 'node_modules/@sentry/core/esm/utils/hasTracingEnabled.js',
                 'node_modules/@sentry/core/esm/utils/prepareEvent.js',
                 'node_modules/@sentry/core/esm/utils/prepareEvent.js',
                 'node_modules/@sentry/core/esm/version.js',
@@ -863,25 +863,25 @@
                 'node_modules/@sentry/core/esm/version.js',
                 'node_modules/@sentry/core/esm/version.js',
                 'node_modules/@sentry/core/esm/version.js',
                 'node_modules/@sentry/core/esm/version.js',
                 'node_modules/@sentry/core/esm/version.js',
                 'node_modules/@sentry/core/esm/version.js',
                 'node_modules/@sentry/core/esm/version.js',
-                'node_modules/@sentry/core/node_modules/tslib/modules/*',
-                'node_modules/@sentry/core/node_modules/tslib/package.json',
-                'node_modules/@sentry/core/node_modules/tslib/package.json',
-                'node_modules/@sentry/core/node_modules/tslib/package.json',
-                'node_modules/@sentry/core/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/core/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/core/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/core/node_modules/tslib/tslib.js',
-                'node_modules/@sentry/core/node_modules/tslib/tslib.js',
-                'node_modules/@sentry/core/node_modules/tslib/tslib.js',
                 'node_modules/@sentry/core/package.json',
+                'node_modules/@sentry/node/cjs/async/domain.js',
+                'node_modules/@sentry/node/cjs/async/domain.js',
+                'node_modules/@sentry/node/cjs/async/domain.js',
+                'node_modules/@sentry/node/cjs/async/hooks.js',
+                'node_modules/@sentry/node/cjs/async/hooks.js',
+                'node_modules/@sentry/node/cjs/async/hooks.js',
+                'node_modules/@sentry/node/cjs/async/index.js',
+                'node_modules/@sentry/node/cjs/async/index.js',
+                'node_modules/@sentry/node/cjs/async/index.js',
+                'node_modules/@sentry/node/cjs/client.js',
                 'node_modules/@sentry/node/cjs/client.js',
                 'node_modules/@sentry/node/cjs/client.js',
                 'node_modules/@sentry/node/cjs/client.js',
                 'node_modules/@sentry/node/cjs/client.js',
                 'node_modules/@sentry/node/cjs/client.js',
                 'node_modules/@sentry/node/cjs/client.js',
                 'node_modules/@sentry/node/cjs/client.js',
@@ -892,23 +892,26 @@
                 'node_modules/@sentry/node/cjs/eventbuilder.js',
                 'node_modules/@sentry/node/cjs/eventbuilder.js',
                 'node_modules/@sentry/node/cjs/eventbuilder.js',
                 'node_modules/@sentry/node/cjs/eventbuilder.js',
                 'node_modules/@sentry/node/cjs/eventbuilder.js',
                 'node_modules/@sentry/node/cjs/eventbuilder.js',
                 'node_modules/@sentry/node/cjs/eventbuilder.js',
+                'node_modules/@sentry/node/cjs/eventbuilder.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
                 'node_modules/@sentry/node/cjs/handlers.js',
+                'node_modules/@sentry/node/cjs/handlers.js',
+                'node_modules/@sentry/node/cjs/index.js',
                 'node_modules/@sentry/node/cjs/index.js',
                 'node_modules/@sentry/node/cjs/index.js',
                 'node_modules/@sentry/node/cjs/index.js',
                 'node_modules/@sentry/node/cjs/index.js',
                 'node_modules/@sentry/node/cjs/index.js',
                 'node_modules/@sentry/node/cjs/index.js',
                 'node_modules/@sentry/node/cjs/index.js',
@@ -1045,23 +1048,36 @@
                 'node_modules/@sentry/node/cjs/module.js',
                 'node_modules/@sentry/node/cjs/module.js',
                 'node_modules/@sentry/node/cjs/module.js',
                 'node_modules/@sentry/node/cjs/module.js',
                 'node_modules/@sentry/node/cjs/module.js',
                 'node_modules/@sentry/node/cjs/module.js',
                 'node_modules/@sentry/node/cjs/module.js',
+                'node_modules/@sentry/node/cjs/module.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
+                'node_modules/@sentry/node/cjs/nodeVersion.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
                 'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
+                'node_modules/@sentry/node/cjs/requestDataDeprecated.js',
+                'node_modules/@sentry/node/cjs/requestdata.js',
                 'node_modules/@sentry/node/cjs/requestdata.js',
                 'node_modules/@sentry/node/cjs/requestdata.js',
                 'node_modules/@sentry/node/cjs/requestdata.js',
                 'node_modules/@sentry/node/cjs/requestdata.js',
                 'node_modules/@sentry/node/cjs/requestdata.js',
                 'node_modules/@sentry/node/cjs/requestdata.js',
                 'node_modules/@sentry/node/cjs/requestdata.js',
@@ -1072,28 +1088,40 @@
                 'node_modules/@sentry/node/cjs/sdk.js',
                 'node_modules/@sentry/node/cjs/sdk.js',
                 'node_modules/@sentry/node/cjs/sdk.js',
                 'node_modules/@sentry/node/cjs/sdk.js',
                 'node_modules/@sentry/node/cjs/sdk.js',
                 'node_modules/@sentry/node/cjs/sdk.js',
                 'node_modules/@sentry/node/cjs/sdk.js',
+                'node_modules/@sentry/node/cjs/sdk.js',
                 'node_modules/@sentry/node/cjs/tracing/index.js',
                 'node_modules/@sentry/node/cjs/tracing/index.js',
                 'node_modules/@sentry/node/cjs/tracing/integrations.js',
                 'node_modules/@sentry/node/cjs/tracing/integrations.js',
                 'node_modules/@sentry/node/cjs/transports/http.js',
                 'node_modules/@sentry/node/cjs/utils.js',
                 'node_modules/@sentry/node/cjs/utils.js',
                 'node_modules/@sentry/node/cjs/utils.js',
                 'node_modules/@sentry/node/cjs/utils.js',
                 'node_modules/@sentry/node/cjs/utils.js',
                 'node_modules/@sentry/node/cjs/utils.js',
                 'node_modules/@sentry/node/cjs/utils.js',
                 'node_modules/@sentry/node/cjs/utils.js',
                 'node_modules/@sentry/node/cjs/utils.js',
+                'node_modules/@sentry/node/cjs/utils.js',
+                'node_modules/@sentry/node/esm/async/domain.js',
+                'node_modules/@sentry/node/esm/async/domain.js',
+                'node_modules/@sentry/node/esm/async/domain.js',
+                'node_modules/@sentry/node/esm/async/hooks.js',
+                'node_modules/@sentry/node/esm/async/hooks.js',
+                'node_modules/@sentry/node/esm/async/hooks.js',
+                'node_modules/@sentry/node/esm/async/index.js',
+                'node_modules/@sentry/node/esm/async/index.js',
+                'node_modules/@sentry/node/esm/async/index.js',
+                'node_modules/@sentry/node/esm/client.js',
                 'node_modules/@sentry/node/esm/client.js',
                 'node_modules/@sentry/node/esm/client.js',
                 'node_modules/@sentry/node/esm/client.js',
                 'node_modules/@sentry/node/esm/client.js',
                 'node_modules/@sentry/node/esm/client.js',
                 'node_modules/@sentry/node/esm/client.js',
                 'node_modules/@sentry/node/esm/client.js',
@@ -1104,14 +1132,16 @@
                 'node_modules/@sentry/node/esm/eventbuilder.js',
                 'node_modules/@sentry/node/esm/eventbuilder.js',
                 'node_modules/@sentry/node/esm/eventbuilder.js',
                 'node_modules/@sentry/node/esm/eventbuilder.js',
                 'node_modules/@sentry/node/esm/eventbuilder.js',
                 'node_modules/@sentry/node/esm/eventbuilder.js',
                 'node_modules/@sentry/node/esm/eventbuilder.js',
+                'node_modules/@sentry/node/esm/eventbuilder.js',
+                'node_modules/@sentry/node/esm/handlers.js',
                 'node_modules/@sentry/node/esm/handlers.js',
                 'node_modules/@sentry/node/esm/handlers.js',
                 'node_modules/@sentry/node/esm/handlers.js',
                 'node_modules/@sentry/node/esm/handlers.js',
                 'node_modules/@sentry/node/esm/handlers.js',
                 'node_modules/@sentry/node/esm/handlers.js',
                 'node_modules/@sentry/node/esm/handlers.js',
@@ -1122,14 +1152,15 @@
                 'node_modules/@sentry/node/esm/index.js',
                 'node_modules/@sentry/node/esm/index.js',
                 'node_modules/@sentry/node/esm/index.js',
                 'node_modules/@sentry/node/esm/index.js',
                 'node_modules/@sentry/node/esm/index.js',
                 'node_modules/@sentry/node/esm/index.js',
                 'node_modules/@sentry/node/esm/index.js',
+                'node_modules/@sentry/node/esm/index.js',
                 'node_modules/@sentry/node/esm/integrations/console.js',
                 'node_modules/@sentry/node/esm/integrations/console.js',
                 'node_modules/@sentry/node/esm/integrations/console.js',
                 'node_modules/@sentry/node/esm/integrations/console.js',
                 'node_modules/@sentry/node/esm/integrations/console.js',
                 'node_modules/@sentry/node/esm/integrations/console.js',
                 'node_modules/@sentry/node/esm/integrations/console.js',
@@ -1257,14 +1288,26 @@
                 'node_modules/@sentry/node/esm/module.js',
                 'node_modules/@sentry/node/esm/module.js',
                 'node_modules/@sentry/node/esm/module.js',
                 'node_modules/@sentry/node/esm/module.js',
                 'node_modules/@sentry/node/esm/module.js',
                 'node_modules/@sentry/node/esm/module.js',
                 'node_modules/@sentry/node/esm/module.js',
+                'node_modules/@sentry/node/esm/module.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/nodeVersion.js',
+                'node_modules/@sentry/node/esm/requestDataDeprecated.js',
                 'node_modules/@sentry/node/esm/requestDataDeprecated.js',
                 'node_modules/@sentry/node/esm/requestDataDeprecated.js',
                 'node_modules/@sentry/node/esm/requestDataDeprecated.js',
                 'node_modules/@sentry/node/esm/requestDataDeprecated.js',
                 'node_modules/@sentry/node/esm/requestDataDeprecated.js',
                 'node_modules/@sentry/node/esm/requestDataDeprecated.js',
                 'node_modules/@sentry/node/esm/requestDataDeprecated.js',
@@ -1275,14 +1318,16 @@
                 'node_modules/@sentry/node/esm/requestdata.js',
                 'node_modules/@sentry/node/esm/requestdata.js',
                 'node_modules/@sentry/node/esm/requestdata.js',
                 'node_modules/@sentry/node/esm/requestdata.js',
                 'node_modules/@sentry/node/esm/requestdata.js',
                 'node_modules/@sentry/node/esm/requestdata.js',
                 'node_modules/@sentry/node/esm/requestdata.js',
+                'node_modules/@sentry/node/esm/requestdata.js',
+                'node_modules/@sentry/node/esm/sdk.js',
                 'node_modules/@sentry/node/esm/sdk.js',
                 'node_modules/@sentry/node/esm/sdk.js',
                 'node_modules/@sentry/node/esm/sdk.js',
                 'node_modules/@sentry/node/esm/sdk.js',
                 'node_modules/@sentry/node/esm/sdk.js',
                 'node_modules/@sentry/node/esm/sdk.js',
                 'node_modules/@sentry/node/esm/sdk.js',
@@ -1298,24 +1343,15 @@
                 'node_modules/@sentry/node/esm/utils.js',
                 'node_modules/@sentry/node/esm/utils.js',
                 'node_modules/@sentry/node/esm/utils.js',
                 'node_modules/@sentry/node/esm/utils.js',
                 'node_modules/@sentry/node/esm/utils.js',
                 'node_modules/@sentry/node/esm/utils.js',
                 'node_modules/@sentry/node/esm/utils.js',
-                'node_modules/@sentry/node/node_modules/tslib/modules/*',
-                'node_modules/@sentry/node/node_modules/tslib/package.json',
-                'node_modules/@sentry/node/node_modules/tslib/package.json',
-                'node_modules/@sentry/node/node_modules/tslib/package.json',
-                'node_modules/@sentry/node/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/node/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/node/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/node/node_modules/tslib/tslib.js',
-                'node_modules/@sentry/node/node_modules/tslib/tslib.js',
-                'node_modules/@sentry/node/node_modules/tslib/tslib.js',
+                'node_modules/@sentry/node/esm/utils.js',
                 'node_modules/@sentry/node/package.json',
                 'node_modules/@sentry/types/cjs/index.js',
                 'node_modules/@sentry/types/esm/index.js',
                 'node_modules/@sentry/types/package.json',
                 'node_modules/@sentry/utils/cjs/baggage.js',
                 'node_modules/@sentry/utils/cjs/baggage.js',
                 'node_modules/@sentry/utils/cjs/baggage.js',
@@ -3634,24 +3670,14 @@
                 'node_modules/@sentry/utils/esm/worldwide.js',
                 'node_modules/@sentry/utils/esm/worldwide.js',
                 'node_modules/@sentry/utils/esm/worldwide.js',
                 'node_modules/@sentry/utils/esm/worldwide.js',
                 'node_modules/@sentry/utils/esm/worldwide.js',
                 'node_modules/@sentry/utils/esm/worldwide.js',
                 'node_modules/@sentry/utils/esm/worldwide.js',
-                'node_modules/@sentry/utils/node_modules/tslib/modules/*',
-                'node_modules/@sentry/utils/node_modules/tslib/package.json',
-                'node_modules/@sentry/utils/node_modules/tslib/package.json',
-                'node_modules/@sentry/utils/node_modules/tslib/package.json',
-                'node_modules/@sentry/utils/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/utils/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/utils/node_modules/tslib/tslib.es6.js',
-                'node_modules/@sentry/utils/node_modules/tslib/tslib.js',
-                'node_modules/@sentry/utils/node_modules/tslib/tslib.js',
-                'node_modules/@sentry/utils/node_modules/tslib/tslib.js',
                 'node_modules/@sentry/utils/package.json',
                 'node_modules/agent-base/dist/src/index.js',
                 'node_modules/agent-base/dist/src/index.js',
                 'node_modules/agent-base/dist/src/promisify.js',
                 'node_modules/agent-base/dist/src/promisify.js',
                 'node_modules/agent-base/package.json',
                 'node_modules/boolean/.eslintrc.json',
@@ -5130,14 +5156,24 @@
                 'node_modules/snyk/wrapper_dist/index.js',
                 'node_modules/sprintf-js/dist/angular-sprintf.min.js',
                 'node_modules/sprintf-js/dist/angular-sprintf.min.js',
                 'node_modules/sprintf-js/dist/sprintf.min.js',
                 'node_modules/sprintf-js/dist/sprintf.min.js',
                 'node_modules/sprintf-js/package.json',
                 'node_modules/sprintf-js/src/*',
+                'node_modules/tslib/modules/*',
+                'node_modules/tslib/package.json',
+                'node_modules/tslib/package.json',
+                'node_modules/tslib/package.json',
+                'node_modules/tslib/tslib.es6.js',
+                'node_modules/tslib/tslib.es6.js',
+                'node_modules/tslib/tslib.es6.js',
+                'node_modules/tslib/tslib.js',
+                'node_modules/tslib/tslib.js',
+                'node_modules/tslib/tslib.js',
                 'node_modules/type-fest/package.json',
                 'node_modules/yallist/iterator.js',
                 'node_modules/yallist/iterator.js',
                 'node_modules/yallist/iterator.js',
                 'node_modules/yallist/package.json',
                 'node_modules/yallist/package.json',
                 'node_modules/yallist/package.json',
@@ -5189,15 +5225,15 @@
                      'c2cciutils-pull-request-checks = '
                      'c2cciutils.scripts.pr_checks:main',
                      'c2cciutils-trigger-image-update = '
                      'c2cciutils.scripts.trigger_image_update:main']}
 
 setup_kwargs = {
     'name': 'c2cciutils',
-    'version': '1.6.0.dev89',
+    'version': '1.6.0.dev93',
     'description': 'Common utilities for Camptocamp CI',
     'long_description': '# C2C CI utils\n\nThe goals of C2C CI utils are:\n\n- Have some global checks that\'s didn\'t request any dependency related to the application:\n  this commands return 3 types of results:\n  - Print some useful information:\n    - The version of some packages\n    - The used configuration (with default and autodetect)\n    - The environment variables\n    - The GitHub event file\n  - Check that some configuration where correct:\n    - Git attributes\n    - That the timeout is present in the GitHub workflow files\n    - That the stabilization version (get from the Security.md) are used everywhere it\'s needed\n  - Snyk tests\n    - Test (never failed)\n    - Code test (never failed, disabled by default)\n    - Iac Test (never failed, disabled by default)\n    - Fix (For information only, disabled by default)\n\nEvery check can be disabled with the following config (the configuration is `ci/config.yaml`):\n\n```yaml\nchecks:\n  <check name>: false\n```\n\nIt make easier to place the following workflows:\n\n- `audit.yaml`: Audit the stabilization branches of the application against vulnerabilities in the python and node dependency\n- `auto-review.yaml`: Auto review the Renovate pull requests\n- `backport.yaml`: Trigger the backports (work with labels)\n- `clean.yaml`: Clean the Docker images related on a deleted feature branch\n- `codeql.yaml`: Run a GitHub CodeQL check\n- `main.yaml`: Main workflow especially with the c2cciutils-checks command\n- `rebuild.yaml`: Daily rebuild of the Docker images on the stabilization branches.\n\nAll the provided commands:\n\n- `c2cciutils`: some generic tools.\n- `c2cciutils-checks`: Run the checks on the code (those checks don\'t need any project dependencies).\n- `c2cciutils-audit`: Do the audit, the main difference with checks is that it can change between runs on the same code.\n- `c2cciutils-publish`: Publish the project.\n- `c2cciutils-clean`: Delete Docker images on Docker Hub after corresponding branch have been deleted.\n- `c2cciutils-google-calendar`: Tool to test the Google credentials for calendar API and refresh them if needed. See `c2cciutils-google-calendar -h` for more information.\n- `c2cciutils-k8s-install`: Install a k3d / k3s cluster, see below.\n- `c2cciutils-k8s-db`: Create a database in the k8s cluster, see below.\n- `c2cciutils-k8s-wait`: Wait that the application started correctly in the cluster, see below.\n- `c2cciutils-k8s-logs`: Display the logs of the application in the k8s cluster, see below.\n- `c2cciutils-pin-pipenv`: Display all the dependencies that\'s in the `Pipenv.lock` but not in the `Pipenv` to be able to pin them.\n- `c2cciutils-docker-logs`: Display the logs of the application in Docker (compose).\n- `c2cciutils-trigger-image-update`: Trigger the ArgoCD repository about image update on the CI (automatically done in the publishing).\n- `c2cciutils-download-applications`: Download the applications with version managed by Renovate, see below.\n- `c2cciutils-docker-versions-gen`: Generate the Docker package versions file (`ci/dpkg-versions.yaml`), see below.\n\n## New project\n\nThe content of `example-project` can be a good base for a new project.\n\n## Secrets\n\nIn the CI we need to have the following secrets::\n\n- `HAS_SECRETS` to be set to \'HAS_SECRETS\', to avoid error errors from external\n  pull requests, already set globally on Camptocamp organization.\n- `GOPASS_CI_GITHUB_TOKEN` and `CI_GPG_PRIVATE_KEY` required to initialize the gopass password store,\n  the secrets exists in the Camptocamp organization but not shared on all project, then you should add\n  your project to the shared list.\n\n## Use locally, in the projects that use c2cciutils\n\nInstall it: `python3 -m pip install --user --requirement ci/requirements.txt`\nRun the checkers: `c2cciutils-checks [--fix] [--stop] [--check CHECK]`\nDry run publish: `GITHUB_REF=... c2cciutils-publish --dry-run ...`\n\n## Configuration\n\nYou can get the current configuration with `c2cciutils --get-config`, the default configuration depends on your project.\nNote that it didn\'t contain the default defined the schema and visible in the [generated documentation](./config.md).\n\nYou can override the configuration with the file `ci/config.yaml`.\n\nAt the base of the configuration you have:\n\n- `version`: Contains some regular expressions to find the versions branches and tags, and to convert them into application versions.\n- `checks`: The checker\'s configuration, see `c2cciutils/checks.py` for more information.\n- `audit`: The audit configuration, see `c2cciutils/audit.py` for more information.\n- `publish`: The publishing configuration, see `c2cciutils/publish.py` for more information.\n\nMany actions can be disabled by setting the corresponding configuration part to `False`.\n\n## SECURITY.md\n\nThe `SECURITY.md` file should contain the security policy of the repository, especially the end of\nsupport dates.\n\nFor compatibility with `c2cciutils` it should contain an array with at least the columns\n`Version` and `Supported Until`. The `Version` column will contain the concerned version.\nThe `Supported Until` will contain the date of end of support `dd/mm/yyyy`.\nIt can also contain the following sentences:\n\n- `Unsupported`: no longer supported => no audit, no rebuild.\n- `Best effort`: the support is ended, it is still rebuilt and audited, but this can be stopped without any notice.\n- `To be defined`: not yet released or the date will be set related of another project release date (like for GeoMapFish).\n\nSee also [GitHub Documentation](https://docs.github.com/en/github/managing-security-vulnerabilities/adding-a-security-policy-to-your-repository)\n\n## IDE\n\nThe IDE should be configured as:\n\n- using `black` and `isort` without any arguments,\n- using the `editorconfig` configuration.\n\n### VScode\n\n- Recommend extensions to work well with c2cciutils:\n  - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) And use EditorConfig\n  - [shell-format](https://marketplace.visualstudio.com/items?itemName=foxundermoon.shell-format) With the configuration\n    `"shellformat.flag": "-bn"`.\n  - [Better TOML](https://marketplace.visualstudio.com/items?itemName=bodil.prettier-toml)\n- Other recommend extensions:\n  - [hadolint](https://marketplace.visualstudio.com/items?itemName=exiasr.hadolint)\n  - [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)\n\nSelect a formatter:\n\n- `CTRL+MAJ+P`\n- Format document With...\n- Configure Default Formatter...\n- Select the formatter\n\n## Publishing\n\n### To pypi\n\nThe config is like this:\n\n```yaml\nversions:\n  # List of kinds of versions you want to publish, that can be:\n  # rebuild (specified with --type),\n  # version_tag, version_branch, feature_branch, feature_tag (for pull request)\n```\n\nIt we have a `setup.py` file, we will be in legacy mode:\nWhen publishing, the version computed from arguments or `GITHUB_REF` is put in environment variable `VERSION`, thus you should use it in `setup.py`, example:\n\n```python\nVERSION = os.environ.get("VERSION", "1.0.0")\n```\n\nAlso we consider that we use `poetry` with [poetry-dynamic-versioning](https://pypi.org/project/poetry-dynamic-versioning/) to manage the version, and [poetry-plugin-tweak-dependencies-version](https://pypi.org/project/poetry-plugin-tweak-dependencies-version/) to manage the dependencies versions.\n\nExample of configuration:\n\n```toml\n[tool.poetry-dynamic-versioning]\nenable = true\nvcs = "git"\npattern = "^(?P<base>\\\\d+(\\\\.\\\\d+)*)"\nformat-jinja = """\n{%- if env.get("VERSION_TYPE") == "version_branch" -%}\n{{serialize_pep440(bump_version(base, 1 if env.get("IS_MASTER") == "TRUE" else 2), dev=distance)}}\n{%- elif distance == 0 -%}\n{{serialize_pep440(base)}}\n{%- else -%}\n{{serialize_pep440(bump_version(base), dev=distance)}}\n{%- endif -%}\n"""\n\n```\n\nNote that we can access to the environment variables `VERSION`,`VERSION_TYPE` and `IS_MASTER`.\n\nThen by default:\n\n- Tag with `1.2.3` => release `1.2.3`\n- Commit on feature branch just do a validation\n- Commit on `master` branch after the tag 1.3.0 => release `1.4.0.dev1`\n- Commit on `1.3` branch after the tag 1.3.0 => release `1.3.1.dev1`\n\nTo make it working in the `Dockerfile` you should have in the `poetry` stage:\n\n```Dockerfile\nENV POETRY_DYNAMIC_VERSIONING_BYPASS=dev\nRUN poetry export --extras=checks --extras=publish --extras=audit --output=requirements.txt \\\n    && poetry export --with=dev --output=requirements-dev.txt\n```\n\nAnd in the `run` stage\n\n```Dockerfile\nARG VERSION=dev\nRUN --mount=type=cache,target=/root/.cache \\\n    POETRY_DYNAMIC_VERSIONING_BYPASS=${VERSION} python3 -m pip install --disable-pip-version-check --no-deps --editable=.\n```\n\nAnd in the `Makefile`:\n\n```Makefile\nVERSION = $(strip $(shell poetry version --short))\n\n.PHONY: build\nbuild: ## Build the Docker images\n    docker build --build-arg=VERSION=$(VERSION) --tag=$(GITHUB_REPOSITORY) .\n```\n\n### To Docker registry\n\nThe config is like this:\n\n```yaml\nlatest: True\nimages:\n  - name: # The base name of the image we want to publish\nrepository:\n  <internal_name>:\n    \'server\': # The fqdn name of the server if not Docker hub\n    \'version\':# List of kinds of versions you want to publish, that can be: rebuild (specified using --type),\n      # version_tag, version_branch, feature_branch, feature_tag (for pull request)\n    \'tags\':# List of tags we want to publish interpreted with `template(version=version)`\n      # e.g. if you use `{version}-lite` when you publish the version `1.2.3` the source tag\n      # (that should be built by the application build) is `latest-lite`, and it will be published\n      # with the tag `1.2.3-lite`.\n    \'group\':# If your images are published by different jobs you can separate them in different groups\n      # and publish them with `c2cciutils-publish --group=<group>`\n```\n\nBy default, the last line of the `SECURITY.md` file will be published (`docker`) with the tag\n`latest`. Set `latest` to `False` to disable it.\n\nWith the `c2cciutils-clean` the images on Docker hub for `feature_branch` will be removed on branch removing.\n\n## Download applications\n\nIn case some executables or applications from GitHub releases or any other URLs are required on the CI host\nand are not handled by any dependency manager, we provide a set of tools to install them and manage upgrades\nthrough Renovate.\n\nCreate an application file (e.-g. `applications.yaml`) with:\n\n```yaml\n# yaml-language-server: $schema=https://raw.githubusercontent.com/camptocamp/c2cciutils/master/c2cciutils/schema-applications.json\n\n# Application from GitHub release\n<organization>/<project>:\n  get-file-name: <file name present in the release>\n  to-file-name: <The file name you want to create in ~/.local/bin>\n  finish-command: # The command you want to run after the file is downloaded\n    - - chmod # To be executable (usually required)\n      - +x\n      - <to-file-name>\n    - - <to-file-name> # Print the version of the application\n      - --version\n# Application from GitHub release in a tar file (or tar.gz)\n<organization>/<project>:\n  get-file-name: <file name present in the release>\n  type: tar\n  tar-file-name: <The file name available in the tar file>\n  to-file-name: <The file name you want to create in ~/.local/bin>\n  finish-command: [...] # The command you want to run after the file is downloaded\n# Application from an URL\n<application reference name>:\n  url-pattern: <The URL used to download the application>\n  to-file-name: <The file name you want to create in ~/.local/bin>\n  finish-command: [...] # The command you want to run after the file is downloaded\n```\n\nIn the attributes `url-pattern`, `get-file-name` you can use the following variables:\n\n- `{version}`: The version of the application present in the version file.\n- `{version_quote}`: The URL encoded version.\n- `{short_version}`: The version without the `v` prefix.\n\nThe `applications-versions.yaml` file is a map of applications and their versions.\n\nAdd in your Renovate configuration:\n\n```json5\n\n  regexManagers: [\n    {\n      fileMatch: [\'^applications-versions.yaml$\'],\n      matchStrings: [\n        \'(?<depName>[^\\\\s]+): (?<currentValue>[^\\\\s]+) # (?<datasource>[^\\\\s]+)\',\n      ],\n    },\n  ],\n```\n\nNow you need to call `c2cciutils-download-applications --applications-file=applications.yaml --versions-file=applications-version.yaml`\nto install required applications on CI host before using them (an already installed application is installed only if needed).\n\n## Use Renovate to trigger a new build instead of the legacy rebuild\n\nRun the command `c2cciutils-docker-versions-gen camptocamp/image[:tag]` to generate a file that is a kind of package lock of the Debian packages in the file `ci/dpkg-versions.yaml`.\n\nAdd in your renovate configuration:\n\n```javascript\n  regexManagers: [\n    {\n      fileMatch: [\'^ci/dpkg-versions.yaml$\'],\n      matchStrings: [" *(?<depName>[^\'\\\\s]+): \'?(?<currentValue>[^\'\\\\s/]*[0-9][^\'\\\\s/]*)\'?"],\n      datasourceTemplate: \'repology\',\n      versioningTemplate: \'loose\',\n    },\n  ],\n```\n\nWhen a new version of a Debian package will be available:\n\n- Renovate will automatically open a pull request to update the file `ci/dpkg-versions.yaml`.\n- And the continuous integration will build a new fresh Docker image with latest versions of all Debian packages.\n\n## Kubernetes\n\nC2cciutils provide some commands for Kubernetes.\n\nYou can define a workflow like that:\n\n```yaml\n- name: Install k3s/k3d (Kubernetes cluster)\n  run: c2cciutils-k8s-install\n\n- name: Create a database to do the tests\n  run: c2cciutils-k8s-db --script=<my_script>.sql\n\n- name: Install the application in the Kubernetes cluster\n  run: kubectl apply -f <my_application>.yaml\n\n- name: Wait that the application is ready\n  run: c2cciutils-k8s-wait\n- name: Print the application status and logs\n  run: c2cciutils-k8s-logs\n  if: always()\n\n- name: Uninstall the application\n  run: kubectl delete -f <my_application>.yaml || true\n\n- name: Cleanup the database\n  run: c2cciutils-k8s-db --cleanup\n```\n\n`c2cciutils-k8s-install` can be configured in the `ci/config.yaml` file, in section `k8s/k3d/install-commands`, default is:\n\n```yaml\n- - k3d\n    cluster\n    create\n    test-cluster\n    --no-lb\n    --no-rollback\n```\n\nSee also: [K3d cluster create documentation](https://k3d.io/v4.4.8/usage/commands/k3d_cluster_create/).\n\n`c2cciutils-k8s-db` can be configured in the `ci/config.yaml` file, in section `k8s/db/chart-options`, default is:\n\n```yaml\npersistence.enabled: \'false\'\ntls.enabled: \'true\'\ntls.autoGenerated: \'true\'\npostgresqlPassword: mySuperTestingPassword\nvolumePermissions.enabled: \'true\'\n```\n\nSee also: [Parameters documentations](https://github.com/bitnami/charts/tree/master/bitnami/postgresql#parameters).\n\n## Contributing\n\nInstall the pre-commit hooks:\n\n```bash\npip install pre-commit\npre-commit install --allow-missing-config\n```\n',
     'author': 'Camptocamp',
     'author_email': 'info@camptocamp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/camptocamp/c2cciutils',
```

### Comparing `c2cciutils-1.6.0.dev89/PKG-INFO` & `c2cciutils-1.6.0.dev93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2cciutils
-Version: 1.6.0.dev89
+Version: 1.6.0.dev93
 Summary: Common utilities for Camptocamp CI
 Home-page: https://github.com/camptocamp/c2cciutils
 License: FreeBSD
 Keywords: ci
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4.0
```

