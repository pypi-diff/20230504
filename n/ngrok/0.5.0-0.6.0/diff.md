# Comparing `tmp/ngrok-0.5.0-cp37-abi3-win_amd64.whl.zip` & `tmp/ngrok-0.6.0-cp37-abi3-musllinux_1_2_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 2286101 bytes, number of entries: 10
--rw-r--r--  4.6 unx     8497 b- defN 23-Apr-13 17:16 ngrok-0.5.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-13 17:16 ngrok-0.5.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       53 b- defN 23-Apr-13 17:16 ngrok-0.5.0.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11558 b- defN 23-Apr-13 17:16 ngrok-0.5.0.dist-info/license_files/LICENSE-APACHE
--rw-r--r--  4.6 unx     1056 b- defN 23-Apr-13 17:16 ngrok-0.5.0.dist-info/license_files/LICENSE-MIT
--rw-r--r--  4.6 unx     5139 b- defN 23-Apr-13 17:16 ngrok/ngrok_parser.py
--rw-r--r--  4.6 unx      109 b- defN 23-Apr-13 17:16 ngrok/__init__.py
--rw-r--r--  4.6 unx     6527 b- defN 23-Apr-13 17:16 ngrok/__main__.py
--rwxr-xr-x  4.6 unx  6341632 b- defN 23-Apr-13 17:16 ngrok/ngrok.pyd
--rw-r--r--  4.6 unx      805 b- defN 23-Apr-13 17:16 ngrok-0.5.0.dist-info/RECORD
-10 files, 6375472 bytes uncompressed, 2284739 bytes compressed:  64.2%
+Zip file size: 2248646 bytes, number of entries: 11
+-rw-r--r--  4.6 unx     8613 b- defN 23-May-04 17:38 ngrok-0.6.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      108 b- defN 23-May-04 17:38 ngrok-0.6.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx       53 b- defN 23-May-04 17:38 ngrok-0.6.0.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11357 b- defN 23-May-04 17:38 ngrok-0.6.0.dist-info/license_files/LICENSE-APACHE
+-rw-r--r--  4.6 unx     1050 b- defN 23-May-04 17:38 ngrok-0.6.0.dist-info/license_files/LICENSE-MIT
+-rwxr-xr-x  4.6 unx   724137 b- defN 23-May-04 17:38 ngrok.libs/libgcc_s-d7088d38.so.1
+-rw-r--r--  4.6 unx     6303 b- defN 23-May-04 17:38 ngrok/__main__.py
+-rw-r--r--  4.6 unx     5001 b- defN 23-May-04 17:38 ngrok/ngrok_parser.py
+-rw-r--r--  4.6 unx      104 b- defN 23-May-04 17:38 ngrok/__init__.py
+-rwxr-xr-x  4.6 unx  4787561 b- defN 23-May-04 17:38 ngrok/ngrok.abi3.so
+-rw-r--r--  4.6 unx      902 b- defN 23-May-04 17:38 ngrok-0.6.0.dist-info/RECORD
+11 files, 5545189 bytes uncompressed, 2247134 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
-Filename: ngrok-0.5.0.dist-info/METADATA
+Filename: ngrok-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: ngrok-0.5.0.dist-info/WHEEL
+Filename: ngrok-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: ngrok-0.5.0.dist-info/entry_points.txt
+Filename: ngrok-0.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ngrok-0.5.0.dist-info/license_files/LICENSE-APACHE
+Filename: ngrok-0.6.0.dist-info/license_files/LICENSE-APACHE
 Comment: 
 
-Filename: ngrok-0.5.0.dist-info/license_files/LICENSE-MIT
+Filename: ngrok-0.6.0.dist-info/license_files/LICENSE-MIT
 Comment: 
 
-Filename: ngrok/ngrok_parser.py
+Filename: ngrok.libs/libgcc_s-d7088d38.so.1
 Comment: 
 
-Filename: ngrok/__init__.py
+Filename: ngrok/__main__.py
 Comment: 
 
-Filename: ngrok/__main__.py
+Filename: ngrok/ngrok_parser.py
+Comment: 
+
+Filename: ngrok/__init__.py
 Comment: 
 
-Filename: ngrok/ngrok.pyd
+Filename: ngrok/ngrok.abi3.so
 Comment: 
 
-Filename: ngrok-0.5.0.dist-info/RECORD
+Filename: ngrok-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ngrok/ngrok_parser.py

 * *Ordering differences only*

```diff
@@ -1,138 +1,138 @@
-import argparse
-
-
-def get_pass_through_args():
-    return {"host", "port", "uds", "fd", "config", "bind"}
-
-
-def get_parser():
-    # argument parsing
-    parser = argparse.ArgumentParser(
-        prog="ngrok-asgi",
-        description="ASGI wrapper for ngrok",
-        epilog="Online in One Line",
-    )
-    parser.add_argument(
-        "command", choices=["gunicorn", "uvicorn"], help="gunicorn or uvicorn"
-    )
-    # ngrok session options
-    parser.add_argument(
-        "--authtoken",
-        help="Ngrok authtoken, otherwise uses NGROK_AUTH_TOKEN environment variable",
-    )
-    parser.add_argument(
-        "--session-metadata",
-        help="Configures the opaque, machine-readable metadata string for this session.",
-    )
-
-    # ngrok tunnel options
-    parser.add_argument(
-        "--allow-cidr",
-        action="append",
-        help="Restriction placed on the origin of incoming connections to the edge to only allow these CIDR ranges. Call multiple times to add additional CIDR ranges.",
-    )
-    parser.add_argument(
-        "--basic-auth",
-        nargs=2,
-        metavar=("username", "password"),
-        help="Credentials for basic authentication.",
-    )
-    parser.add_argument(
-        "--circuit-breaker",
-        help="Reject requests when 5XX responses exceed this ratio. Disabled when 0.",
-    )
-    parser.add_argument(
-        "--compression",
-        action="store_true",
-        help="Enable gzip compression for HTTP responses.",
-    )
-    parser.add_argument(
-        "--deny-cidr",
-        action="append",
-        help="Restriction placed on the origin of incoming connections to the edge to deny these CIDR ranges. Call multiple times to add additional CIDR ranges.",
-    )
-    parser.add_argument("--domain", help="The domain to request for this edge.")
-    parser.add_argument(
-        "--forwards-to",
-        help="Tunnel backend metadata. Viewable via the dashboard and API, but has no bearing on tunnel behavior.",
-    )
-    parser.add_argument(
-        "--metadata", help="Tunnel-specific opaque metadata. Viewable via the API."
-    )
-    parser.add_argument(
-        "--mutual-tlsca",
-        help="Filename of certificates to use for client authentication at the ngrok edge.",
-    )
-    parser.add_argument("--oauth-provider", help="OAuth provider configuration.")
-    parser.add_argument(
-        "--oidc",
-        nargs=3,
-        metavar=("issuer-url", "client-id", "client-secret"),
-        help="OIDC configuration.",
-    )
-    parser.add_argument(
-        "--allow-emails", action="append", help="OAuth/OIDC configuration."
-    )
-    parser.add_argument(
-        "--allow-domains", action="append", help="OAuth/OIDC configuration."
-    )
-    parser.add_argument("--scopes", action="append", help="OAuth/OIDC configuration.")
-    parser.add_argument(
-        "--proxy-proto",
-        choices=["", "1", "2"],
-        help="The version of PROXY protocol to use with this tunnel “1”, “2”, or “” if not using.",
-    )
-    parser.add_argument(
-        "--remove-request-header",
-        action="append",
-        help="Removes a header from requests to this edge. Call multiple times to add additional values.",
-    )
-    parser.add_argument(
-        "--remove-response-header",
-        action="append",
-        help="Removes a header from responses from this edge Call multiple times to add additional values..",
-    )
-    parser.add_argument(
-        "--request-header",
-        action="append",
-        nargs=2,
-        metavar=("header", "value"),
-        help="Adds a header to all requests to this edge. Call multiple times to add additional values.",
-    )
-    parser.add_argument(
-        "--response-header",
-        action="append",
-        nargs=2,
-        metavar=("header", "value"),
-        help="Adds a header to all responses coming from this edge. Call multiple times to add additional values.",
-    )
-    parser.add_argument(
-        "--scheme",
-        choices=["HTTPS", "HTTP"],
-        help="The scheme that this edge should use. Defaults to HTTPS.",
-    )
-    parser.add_argument(
-        "--webhook-verification",
-        nargs=2,
-        metavar=("provider", "secret"),
-        help="WebhookVerification configuration.",
-    )
-    parser.add_argument(
-        "--websocket-tcp-conversion",
-        action="store_true",
-        help="Convert incoming websocket connections to TCP-like streams.",
-    )
-    # uvicorn options
-    parser.add_argument("--host", help="Hostname or IP address")
-    parser.add_argument("--port", help="Port number", type=int)
-    parser.add_argument("--uds", help="Unix domain socket")
-    parser.add_argument("--fd", help="File descriptor")
-    # gunicorn options
-    parser.add_argument("--config", "-c", help="Config file not supported")
-    parser.add_argument(
-        "--bind",
-        "-b",
-        help="Specify a server socket to bind. Server sockets can be any of $(HOST), $(HOST):$(PORT), "
-        + "fd://$(FD), or unix:$(PATH). An IP is a valid $(HOST).",
-    )
-    return parser
+import argparse
+
+
+def get_pass_through_args():
+    return {"host", "port", "uds", "fd", "config", "bind"}
+
+
+def get_parser():
+    # argument parsing
+    parser = argparse.ArgumentParser(
+        prog="ngrok-asgi",
+        description="ASGI wrapper for ngrok",
+        epilog="Online in One Line",
+    )
+    parser.add_argument(
+        "command", choices=["gunicorn", "uvicorn"], help="gunicorn or uvicorn"
+    )
+    # ngrok session options
+    parser.add_argument(
+        "--authtoken",
+        help="Ngrok authtoken, otherwise uses NGROK_AUTH_TOKEN environment variable",
+    )
+    parser.add_argument(
+        "--session-metadata",
+        help="Configures the opaque, machine-readable metadata string for this session.",
+    )
+
+    # ngrok tunnel options
+    parser.add_argument(
+        "--allow-cidr",
+        action="append",
+        help="Restriction placed on the origin of incoming connections to the edge to only allow these CIDR ranges. Call multiple times to add additional CIDR ranges.",
+    )
+    parser.add_argument(
+        "--basic-auth",
+        nargs=2,
+        metavar=("username", "password"),
+        help="Credentials for basic authentication.",
+    )
+    parser.add_argument(
+        "--circuit-breaker",
+        help="Reject requests when 5XX responses exceed this ratio. Disabled when 0.",
+    )
+    parser.add_argument(
+        "--compression",
+        action="store_true",
+        help="Enable gzip compression for HTTP responses.",
+    )
+    parser.add_argument(
+        "--deny-cidr",
+        action="append",
+        help="Restriction placed on the origin of incoming connections to the edge to deny these CIDR ranges. Call multiple times to add additional CIDR ranges.",
+    )
+    parser.add_argument("--domain", help="The domain to request for this edge.")
+    parser.add_argument(
+        "--forwards-to",
+        help="Tunnel backend metadata. Viewable via the dashboard and API, but has no bearing on tunnel behavior.",
+    )
+    parser.add_argument(
+        "--metadata", help="Tunnel-specific opaque metadata. Viewable via the API."
+    )
+    parser.add_argument(
+        "--mutual-tlsca",
+        help="Filename of certificates to use for client authentication at the ngrok edge.",
+    )
+    parser.add_argument("--oauth-provider", help="OAuth provider configuration.")
+    parser.add_argument(
+        "--oidc",
+        nargs=3,
+        metavar=("issuer-url", "client-id", "client-secret"),
+        help="OIDC configuration.",
+    )
+    parser.add_argument(
+        "--allow-emails", action="append", help="OAuth/OIDC configuration."
+    )
+    parser.add_argument(
+        "--allow-domains", action="append", help="OAuth/OIDC configuration."
+    )
+    parser.add_argument("--scopes", action="append", help="OAuth/OIDC configuration.")
+    parser.add_argument(
+        "--proxy-proto",
+        choices=["", "1", "2"],
+        help="The version of PROXY protocol to use with this tunnel “1”, “2”, or “” if not using.",
+    )
+    parser.add_argument(
+        "--remove-request-header",
+        action="append",
+        help="Removes a header from requests to this edge. Call multiple times to add additional values.",
+    )
+    parser.add_argument(
+        "--remove-response-header",
+        action="append",
+        help="Removes a header from responses from this edge Call multiple times to add additional values..",
+    )
+    parser.add_argument(
+        "--request-header",
+        action="append",
+        nargs=2,
+        metavar=("header", "value"),
+        help="Adds a header to all requests to this edge. Call multiple times to add additional values.",
+    )
+    parser.add_argument(
+        "--response-header",
+        action="append",
+        nargs=2,
+        metavar=("header", "value"),
+        help="Adds a header to all responses coming from this edge. Call multiple times to add additional values.",
+    )
+    parser.add_argument(
+        "--scheme",
+        choices=["HTTPS", "HTTP"],
+        help="The scheme that this edge should use. Defaults to HTTPS.",
+    )
+    parser.add_argument(
+        "--webhook-verification",
+        nargs=2,
+        metavar=("provider", "secret"),
+        help="WebhookVerification configuration.",
+    )
+    parser.add_argument(
+        "--websocket-tcp-conversion",
+        action="store_true",
+        help="Convert incoming websocket connections to TCP-like streams.",
+    )
+    # uvicorn options
+    parser.add_argument("--host", help="Hostname or IP address")
+    parser.add_argument("--port", help="Port number", type=int)
+    parser.add_argument("--uds", help="Unix domain socket")
+    parser.add_argument("--fd", help="File descriptor")
+    # gunicorn options
+    parser.add_argument("--config", "-c", help="Config file not supported")
+    parser.add_argument(
+        "--bind",
+        "-b",
+        help="Specify a server socket to bind. Server sockets can be any of $(HOST), $(HOST):$(PORT), "
+        + "fd://$(FD), or unix:$(PATH). An IP is a valid $(HOST).",
+    )
+    return parser
```

## ngrok/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-from .ngrok import *
-
-__doc__ = ngrok.__doc__
-if hasattr(ngrok, "__all__"):
-    __all__ = ngrok.__all__
+from .ngrok import *
+
+__doc__ = ngrok.__doc__
+if hasattr(ngrok, "__all__"):
+    __all__ = ngrok.__all__
```

## ngrok/__main__.py

 * *Ordering differences only*

```diff
@@ -1,224 +1,224 @@
-import asyncio
-import logging
-import ngrok
-from ngrok import ngrok_parser
-import os
-import re
-import shlex
-import sys
-
-DEFAULT_HOST = "localhost"
-DEFAULT_PORT = "8000"
-
-
-def configure_session(args):
-    builder = ngrok.NgrokSessionBuilder()
-    if args.authtoken:
-        builder.authtoken(args.authtoken)
-    else:
-        builder.authtoken_from_env()
-
-    if args.session_metadata:
-        builder.metadata(args.session_metadata)
-    return builder
-
-
-def configure_tunnel(session, args):
-    builder = session.http_endpoint()
-    if args.allow_cidr:
-        for cidr in args.allow_cidr:
-            builder.allow_cidr(cidr)
-    if args.basic_auth:
-        builder.basic_auth(args.basic_auth[0], args.basic_auth[1])
-    if args.circuit_breaker:
-        builder.circuit_breaker(float(args.circuit_breaker))
-    if args.compression:
-        builder.compression()
-    if args.deny_cidr:
-        for cidr in args.deny_cidr:
-            builder.deny_cidr(cidr)
-    if args.domain:
-        builder.domain(args.domain)
-    if args.forwards_to:
-        builder.forwards_to(args.forwards_to)
-    if args.metadata:
-        builder.metadata(args.metadata)
-    if args.mutual_tlsca:
-        with open(args.mutual_tlsca, "r") as crt:
-            builder.mutual_tlsca(bytearray(crt.read().encode()))
-    if args.oauth_provider:
-        builder.oauth(
-            args.oauth_provider, args.allow_emails, args.allow_domains, args.scopes
-        )
-    if args.oidc:
-        builder.oidc(
-            args.oidc[0],
-            args.oidc[1],
-            args.oidc[2],
-            args.allow_emails,
-            args.allow_domains,
-            args.scopes,
-        )
-    if args.proxy_proto:
-        builder.proxy_proto(args.proxy_proto)
-    if args.remove_request_header:
-        for header in args.remove_request_header:
-            builder.remove_request_header(header)
-    if args.remove_response_header:
-        for header in args.remove_response_header:
-            builder.remove_response_header(header)
-    if args.request_header:
-        for header in args.request_header:
-            builder.request_header(header[0], header[1])
-    if args.response_header:
-        for header in args.response_header:
-            builder.response_header(header[0], header[1])
-    if args.scheme:
-        builder.scheme(args.scheme)
-    if args.webhook_verification:
-        builder.webhook_verification(
-            args.webhook_verification[0], args.webhook_verification[1]
-        )
-    if args.websocket_tcp_conversion:
-        builder.websocket_tcp_conversion(args.websocket_tcp_conversion)
-    return builder
-
-
-def gunicorn():
-    from gunicorn.app.wsgiapp import run
-
-    run()
-
-
-def uvicorn():
-    import uvicorn
-
-    uvicorn.main()
-
-
-def get_pipe_string(args):
-    pipe_string = None
-    if args.uds:
-        pipe_string = args.uds
-    if args.bind and args.bind.startswith("unix:"):
-        pipe_string = args.bind[5:]
-    return pipe_string
-
-
-def fallback_port(args):
-    fallback_port = DEFAULT_PORT
-    if args.command == "gunicorn" and "PORT" in os.environ:
-        fallback_port = os.getenv("PORT")
-    return fallback_port
-
-
-def get_tcp_string(args):
-    tcp_string = None
-    if args.host and args.port:
-        tcp_string = args.host + ":" + str(args.port)
-    elif args.host:
-        tcp_string = args.host + ":" + fallback_port(args)
-    elif args.port:
-        tcp_string = DEFAULT_HOST + ":" + str(args.port)
-    elif (
-        args.bind
-        and not args.bind.startswith("fd://")
-        and not args.bind.startswith("unix:")
-    ):
-        tcp_string = args.bind
-        # check if missing host
-        if re.search("^:\d+$", tcp_string):
-            tcp_string = DEFAULT_HOST + tcp_string
-        # check if missing port
-        if not re.search(":\d+$", tcp_string):
-            tcp_string += ":" + fallback_port(args)
-    return tcp_string
-
-
-def setup_forwarding(tunnel, args, tcp_string=None):
-    if tcp_string:
-        tunnel.forward_tcp(tcp_string)
-        return True
-
-    # prefer pipe over tcp
-    pipe_string = get_pipe_string(args)
-    if pipe_string:
-        tunnel.forward_pipe(pipe_string)
-    else:
-        tcp_string = get_tcp_string(args)
-        if not tcp_string:
-            return False
-        tunnel.forward_tcp(tcp_string)
-
-    return True
-
-
-async def bind(parser, args):
-    session = await configure_session(args).connect()
-    tunnel = await configure_tunnel(session, args).listen()
-    tunnel_success = setup_forwarding(tunnel, args)
-
-    # if we don't have what we need, check gunicorn environment variable
-    if (
-        not tunnel_success
-        and args.command == "gunicorn"
-        and "GUNICORN_CMD_ARGS" in os.environ
-    ):
-        env_cmd_args = shlex.split(os.getenv("GUNICORN_CMD_ARGS"))
-        env_args, unknown = parser.parse_known_args(env_cmd_args)
-        tunnel_success = setup_forwarding(tunnel, env_args)
-
-    # fallback to the default host and port for these runners
-    if not tunnel_success:
-        tunnel_success = setup_forwarding(
-            tunnel, args, tcp_string=f"{DEFAULT_HOST}:{fallback_port(args)}"
-        )
-
-    # give up
-    if not tunnel_success:
-        logging.fatal("No tunnel created. Exiting.")
-        sys.exit(1)
-
-    return tunnel
-
-
-def main(args):
-    logging.basicConfig(level=logging.INFO)
-
-    # argument parsing
-    parser = ngrok_parser.get_parser()
-    args, unknown = parser.parse_known_args()
-
-    # validation
-    if args.config:
-        logging.fatal("Config file not supported. Exiting.")
-        sys.exit(2)
-    if args.fd or (args.bind and args.bind.startswith("fd://")):
-        logging.fatal("File Descriptor not supported. Exiting.")
-        sys.exit(3)
-
-    # bind to ngrok
-    tunnel = asyncio.run(bind(parser, args))
-
-    # now pretend we don't exist
-    pass_args = [args.command]
-    # pass through some args
-    pass_through_args = ngrok_parser.get_pass_through_args()
-    for key, val in vars(args).items():
-        if key in pass_through_args and val:
-            pass_args.append(f"--{key}")
-            pass_args.append(str(val))
-    # pass through all unknown args
-    sys.argv = pass_args + unknown
-    if args.command == "gunicorn":
-        gunicorn()
-    elif args.command == "uvicorn":
-        uvicorn()
-
-
-def asgi_cli():
-    main(sys.argv)
-
-
-if __name__ == "__main__":
-    main(sys.argv)
+import asyncio
+import logging
+import ngrok
+from ngrok import ngrok_parser
+import os
+import re
+import shlex
+import sys
+
+DEFAULT_HOST = "localhost"
+DEFAULT_PORT = "8000"
+
+
+def configure_session(args):
+    builder = ngrok.NgrokSessionBuilder()
+    if args.authtoken:
+        builder.authtoken(args.authtoken)
+    else:
+        builder.authtoken_from_env()
+
+    if args.session_metadata:
+        builder.metadata(args.session_metadata)
+    return builder
+
+
+def configure_tunnel(session, args):
+    builder = session.http_endpoint()
+    if args.allow_cidr:
+        for cidr in args.allow_cidr:
+            builder.allow_cidr(cidr)
+    if args.basic_auth:
+        builder.basic_auth(args.basic_auth[0], args.basic_auth[1])
+    if args.circuit_breaker:
+        builder.circuit_breaker(float(args.circuit_breaker))
+    if args.compression:
+        builder.compression()
+    if args.deny_cidr:
+        for cidr in args.deny_cidr:
+            builder.deny_cidr(cidr)
+    if args.domain:
+        builder.domain(args.domain)
+    if args.forwards_to:
+        builder.forwards_to(args.forwards_to)
+    if args.metadata:
+        builder.metadata(args.metadata)
+    if args.mutual_tlsca:
+        with open(args.mutual_tlsca, "r") as crt:
+            builder.mutual_tlsca(bytearray(crt.read().encode()))
+    if args.oauth_provider:
+        builder.oauth(
+            args.oauth_provider, args.allow_emails, args.allow_domains, args.scopes
+        )
+    if args.oidc:
+        builder.oidc(
+            args.oidc[0],
+            args.oidc[1],
+            args.oidc[2],
+            args.allow_emails,
+            args.allow_domains,
+            args.scopes,
+        )
+    if args.proxy_proto:
+        builder.proxy_proto(args.proxy_proto)
+    if args.remove_request_header:
+        for header in args.remove_request_header:
+            builder.remove_request_header(header)
+    if args.remove_response_header:
+        for header in args.remove_response_header:
+            builder.remove_response_header(header)
+    if args.request_header:
+        for header in args.request_header:
+            builder.request_header(header[0], header[1])
+    if args.response_header:
+        for header in args.response_header:
+            builder.response_header(header[0], header[1])
+    if args.scheme:
+        builder.scheme(args.scheme)
+    if args.webhook_verification:
+        builder.webhook_verification(
+            args.webhook_verification[0], args.webhook_verification[1]
+        )
+    if args.websocket_tcp_conversion:
+        builder.websocket_tcp_conversion(args.websocket_tcp_conversion)
+    return builder
+
+
+def gunicorn():
+    from gunicorn.app.wsgiapp import run
+
+    run()
+
+
+def uvicorn():
+    import uvicorn
+
+    uvicorn.main()
+
+
+def get_pipe_string(args):
+    pipe_string = None
+    if args.uds:
+        pipe_string = args.uds
+    if args.bind and args.bind.startswith("unix:"):
+        pipe_string = args.bind[5:]
+    return pipe_string
+
+
+def fallback_port(args):
+    fallback_port = DEFAULT_PORT
+    if args.command == "gunicorn" and "PORT" in os.environ:
+        fallback_port = os.getenv("PORT")
+    return fallback_port
+
+
+def get_tcp_string(args):
+    tcp_string = None
+    if args.host and args.port:
+        tcp_string = args.host + ":" + str(args.port)
+    elif args.host:
+        tcp_string = args.host + ":" + fallback_port(args)
+    elif args.port:
+        tcp_string = DEFAULT_HOST + ":" + str(args.port)
+    elif (
+        args.bind
+        and not args.bind.startswith("fd://")
+        and not args.bind.startswith("unix:")
+    ):
+        tcp_string = args.bind
+        # check if missing host
+        if re.search("^:\d+$", tcp_string):
+            tcp_string = DEFAULT_HOST + tcp_string
+        # check if missing port
+        if not re.search(":\d+$", tcp_string):
+            tcp_string += ":" + fallback_port(args)
+    return tcp_string
+
+
+def setup_forwarding(tunnel, args, tcp_string=None):
+    if tcp_string:
+        tunnel.forward_tcp(tcp_string)
+        return True
+
+    # prefer pipe over tcp
+    pipe_string = get_pipe_string(args)
+    if pipe_string:
+        tunnel.forward_pipe(pipe_string)
+    else:
+        tcp_string = get_tcp_string(args)
+        if not tcp_string:
+            return False
+        tunnel.forward_tcp(tcp_string)
+
+    return True
+
+
+async def bind(parser, args):
+    session = await configure_session(args).connect()
+    tunnel = await configure_tunnel(session, args).listen()
+    tunnel_success = setup_forwarding(tunnel, args)
+
+    # if we don't have what we need, check gunicorn environment variable
+    if (
+        not tunnel_success
+        and args.command == "gunicorn"
+        and "GUNICORN_CMD_ARGS" in os.environ
+    ):
+        env_cmd_args = shlex.split(os.getenv("GUNICORN_CMD_ARGS"))
+        env_args, unknown = parser.parse_known_args(env_cmd_args)
+        tunnel_success = setup_forwarding(tunnel, env_args)
+
+    # fallback to the default host and port for these runners
+    if not tunnel_success:
+        tunnel_success = setup_forwarding(
+            tunnel, args, tcp_string=f"{DEFAULT_HOST}:{fallback_port(args)}"
+        )
+
+    # give up
+    if not tunnel_success:
+        logging.fatal("No tunnel created. Exiting.")
+        sys.exit(1)
+
+    return tunnel
+
+
+def main(args):
+    logging.basicConfig(level=logging.INFO)
+
+    # argument parsing
+    parser = ngrok_parser.get_parser()
+    args, unknown = parser.parse_known_args()
+
+    # validation
+    if args.config:
+        logging.fatal("Config file not supported. Exiting.")
+        sys.exit(2)
+    if args.fd or (args.bind and args.bind.startswith("fd://")):
+        logging.fatal("File Descriptor not supported. Exiting.")
+        sys.exit(3)
+
+    # bind to ngrok
+    tunnel = asyncio.run(bind(parser, args))
+
+    # now pretend we don't exist
+    pass_args = [args.command]
+    # pass through some args
+    pass_through_args = ngrok_parser.get_pass_through_args()
+    for key, val in vars(args).items():
+        if key in pass_through_args and val:
+            pass_args.append(f"--{key}")
+            pass_args.append(str(val))
+    # pass through all unknown args
+    sys.argv = pass_args + unknown
+    if args.command == "gunicorn":
+        gunicorn()
+    elif args.command == "uvicorn":
+        uvicorn()
+
+
+def asgi_cli():
+    main(sys.argv)
+
+
+if __name__ == "__main__":
+    main(sys.argv)
```

## Comparing `ngrok-0.5.0.dist-info/METADATA` & `ngrok-0.6.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngrok
-Version: 0.5.0
+Version: 0.6.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Utilities
@@ -21,156 +21,157 @@
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: The ngrok Agent SDK for Python
 Keywords: ngrok,python,pypi,pyo3,ingress,networking
 License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: repository, https://github.com/ngrok/ngrok-py
 Project-URL: changelog, https://github.com/ngrok/ngrok-py/blob/main/CHANGELOG.md
 Project-URL: homepage, https://ngrok.com
-Project-URL: repository, https://github.com/ngrok/ngrok-py
 
-# The ngrok Agent SDK for Python
-
-[![PyPI][pypi-badge]][pypi-url]
-[![Supported Versions][ver-badge]][ver-url]
-[![MIT licensed][mit-badge]][mit-url]
-[![Apache-2.0 licensed][apache-badge]][apache-url]
-[![Continuous integration][ci-badge]][ci-url]
-
-[pypi-badge]: https://img.shields.io/pypi/v/ngrok
-[pypi-url]: https://pypi.org/project/ngrok
-[ver-badge]: https://img.shields.io/pypi/pyversions/ngrok.svg
-[ver-url]: https://pypi.org/project/ngrok
-[mit-badge]: https://img.shields.io/badge/license-MIT-blue.svg
-[mit-url]: https://github.com/ngrok/ngrok-rs/blob/main/LICENSE-MIT
-[apache-badge]: https://img.shields.io/badge/license-Apache_2.0-blue.svg
-[apache-url]: https://github.com/ngrok/ngrok-rs/blob/main/LICENSE-APACHE
-[ci-badge]: https://github.com/ngrok/ngrok-py/actions/workflows/ci.yml/badge.svg
-[ci-url]: https://github.com/ngrok/ngrok-py/actions/workflows/ci.yml
-
-**Note: This is beta-quality software. Interfaces may change without warning.**
-
-[ngrok](https://ngrok.com) is a globally distributed reverse proxy commonly used for quickly getting a public URL to a
-service running inside a private network, such as on your local laptop. The ngrok agent is usually
-deployed inside a private network and is used to communicate with the ngrok cloud service.
-
-This is the ngrok agent in library form, suitable for integrating directly into Python
-applications. This allows you to quickly build ngrok into your application with no separate process
-to manage.
-
-If you're looking for the previous agent downloader project, it's over [here](https://github.com/OpenIoTHub/ngrok).
-
-# Installation
-
-The published library is available on
-[PyPI](https://pypi.org/project/ngrok).
-
-```shell
-python -m pip install ngrok
-```
-
-ngrok-py officially supports Python 3.7+.
-
-# Documentation
-
-A quickstart guide and a full API reference are included in the [ngrok-py Python API documentation](https://ngrok.github.io/ngrok-py/).
-
-# Quickstart
-
-After you've installed the package, you'll need an Auth Token. Retrieve one on the
-[Auth Token page of your ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken)
-
-There are multiple examples in [the /examples directory](https://github.com/ngrok/ngrok-py/tree/main/examples).
-A minimal use-case looks like the following:
-
-```python
-async def create_tunnel():
-    session = await ngrok.NgrokSessionBuilder().authtoken_from_env().connect()
-    tunnel = await session.http_endpoint().listen()
-    print (f"Ingress established at {tunnel.url()}")
-    tunnel.forward_tcp("localhost:9000")
-```
-
-# ASGI Runner - Tunnels to Uvicorn, Gunicorn, Django and More, With No Code
-
-Prefix the command line which starts up a Uvicorn or Gunicorn web server with either `ngrok-asgi` or `python -m ngrok`. Any TCP or Unix Domain Socket arguments will be used to establish connectivity automatically. There are many command line arguments to configure the Tunnel used, for instance adding `--basic-auth ngrok online1line` will introduce basic authentication to the ingress tunnel.
-
-## Uvicorn
-Examples:
-```shell
-ngrok-asgi uvicorn mysite.asgi:application
-ngrok-asgi uvicorn mysite.asgi:application --host localhost --port 1234
-ngrok-asgi uvicorn mysite.asgi:application --host localhost --port 1234 --basic-auth ngrok online1line
-ngrok-asgi uvicorn mysite.asgi:application --uds /tmp/uvicorn.sock
-
-# Can use the module name as well, such as:
-python -m ngrok uvicorn mysite.asgi:application --oauth-provider google --allow-emails bob@example.com
-```
-
-## Gunicorn
-Examples:
-```shell
-ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker
-ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --webhook-verification twilio s3cr3t
-ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --bind localhost:1234
-ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --bind unix:/tmp/gunicorn.sock
-
-# Can use the module name as well, such as:
-python -m ngrok gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --response-header X-Awesome True
-```
-
-# Examples
-
-## Frameworks
-* [Aiohttp](https://docs.aiohttp.org) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/aiohttp-ngrok.py)
-* [Django](https://www.djangoproject.com/) - [Single File Example](https://github.com/ngrok/ngrok-py/tree/main/examples/django-single-file.py), [Modify manage.py Example](https://github.com/ngrok/ngrok-py/tree/main/examples/djangosite/manage.py), [Modify asgi.py Example](https://github.com/ngrok/ngrok-py/tree/main/examples/djangosite/djangosite/ngrok-asgi.py), or use the `ngrok-asgi` ASGI Runner discussed above
-* [Flask](https://flask.palletsprojects.com) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/flask-ngrok.py)
-* [Gunicorn](https://gunicorn.org/) - Use the `ngrok-asgi` ASGI Runner discussed above
-* [Uvicorn](https://www.uvicorn.org/) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/uvicorn-ngrok.py), or use the `ngrok-asgi` ASGI Runner discussed above
-
-## Tunnel Types
-* HTTP - [Minimal Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-http-minimal.py), [Full Configuration Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-http-full.py)
-* Labeled - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-labeled.py)
-* TCP - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-tcp.py)
-* TLS - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-tls.py)
-
-# Platform Support
-
-Pre-built binaries are provided on PyPI for the following platforms:
-
-| OS         | i686 | x64 | aarch64 | arm |
-| ---------- | -----|-----|---------|-----|
-| Windows    |   ✓  |  ✓  |    *    |     |
-| MacOS      |      |  ✓  |    ✓    |     |
-| Linux      |      |  ✓  |    ✓    |  ✓  |
-| Linux musl |      |  ✓  |    ✓    |     |
-| FreeBSD    |      |  *  |         |     |
-
-ngrok-py, and [ngrok-rs](https://github.com/ngrok/ngrok-rs/) which it depends on, are open source, so it may be possible to build them for other platforms.
-
-* Windows-aarch64 will be supported after the next release of [Ring](https://github.com/briansmith/ring/issues/1167).
-* FreeBSD-x64 is built by the release process, but PyPI won't accept BSD flavors.
-
-# Dependencies
-
-This project relies on [PyO3](https://pyo3.rs/), an excellent system to ease development and building of Rust plugins for Python.
-
-Thank you to [OpenIoTHub](https://github.com/OpenIoTHub/ngrok) for handing over the ngrok name on PyPI.
-
-# License
-
-This project is licensed under either of
-
- * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or
-   http://www.apache.org/licenses/LICENSE-2.0)
- * MIT license ([LICENSE-MIT](LICENSE-MIT) or
-   http://opensource.org/licenses/MIT)
-
-at your option.
-
-### Contribution
-
-Unless you explicitly state otherwise, any contribution intentionally submitted
-for inclusion in tokio-core by you, as defined in the Apache-2.0 license, shall be
-dual licensed as above, without any additional terms or conditions.
+# The ngrok Agent SDK for Python
+
+[![PyPI][pypi-badge]][pypi-url]
+[![Supported Versions][ver-badge]][ver-url]
+[![MIT licensed][mit-badge]][mit-url]
+[![Apache-2.0 licensed][apache-badge]][apache-url]
+[![Continuous integration][ci-badge]][ci-url]
+
+[pypi-badge]: https://img.shields.io/pypi/v/ngrok
+[pypi-url]: https://pypi.org/project/ngrok
+[ver-badge]: https://img.shields.io/pypi/pyversions/ngrok.svg
+[ver-url]: https://pypi.org/project/ngrok
+[mit-badge]: https://img.shields.io/badge/license-MIT-blue.svg
+[mit-url]: https://github.com/ngrok/ngrok-rs/blob/main/LICENSE-MIT
+[apache-badge]: https://img.shields.io/badge/license-Apache_2.0-blue.svg
+[apache-url]: https://github.com/ngrok/ngrok-rs/blob/main/LICENSE-APACHE
+[ci-badge]: https://github.com/ngrok/ngrok-py/actions/workflows/ci.yml/badge.svg
+[ci-url]: https://github.com/ngrok/ngrok-py/actions/workflows/ci.yml
+
+**Note: This is beta-quality software. Interfaces may change without warning.**
+
+[ngrok](https://ngrok.com) is a globally distributed reverse proxy commonly used for quickly getting a public URL to a
+service running inside a private network, such as on your local laptop. The ngrok agent is usually
+deployed inside a private network and is used to communicate with the ngrok cloud service.
+
+This is the ngrok agent in library form, suitable for integrating directly into Python
+applications. This allows you to quickly build ngrok into your application with no separate process
+to manage.
+
+If you're looking for the previous agent downloader project, it's over [here](https://github.com/OpenIoTHub/ngrok).
+
+# Installation
+
+The published library is available on
+[PyPI](https://pypi.org/project/ngrok).
+
+```shell
+python -m pip install ngrok
+```
+
+ngrok-py officially supports Python 3.7+.
+
+# Documentation
+
+A quickstart guide and a full API reference are included in the [ngrok-py Python API documentation](https://ngrok.github.io/ngrok-py/).
+
+# Quickstart
+
+After you've installed the package, you'll need an Auth Token. Retrieve one on the
+[Auth Token page of your ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken)
+
+There are multiple examples in [the /examples directory](https://github.com/ngrok/ngrok-py/tree/main/examples).
+A minimal use-case looks like the following:
+
+```python
+async def create_tunnel():
+    session = await ngrok.NgrokSessionBuilder().authtoken_from_env().connect()
+    tunnel = await session.http_endpoint().listen()
+    print (f"Ingress established at {tunnel.url()}")
+    tunnel.forward_tcp("localhost:9000")
+```
+
+# ASGI Runner - Tunnels to Uvicorn, Gunicorn, Django and More, With No Code
+
+Prefix the command line which starts up a Uvicorn or Gunicorn web server with either `ngrok-asgi` or `python -m ngrok`. Any TCP or Unix Domain Socket arguments will be used to establish connectivity automatically. There are many command line arguments to configure the Tunnel used, for instance adding `--basic-auth ngrok online1line` will introduce basic authentication to the ingress tunnel.
+
+## Uvicorn
+Examples:
+```shell
+ngrok-asgi uvicorn mysite.asgi:application
+ngrok-asgi uvicorn mysite.asgi:application --host localhost --port 1234
+ngrok-asgi uvicorn mysite.asgi:application --host localhost --port 1234 --basic-auth ngrok online1line
+ngrok-asgi uvicorn mysite.asgi:application --uds /tmp/uvicorn.sock
+
+# Can use the module name as well, such as:
+python -m ngrok uvicorn mysite.asgi:application --oauth-provider google --allow-emails bob@example.com
+```
+
+## Gunicorn
+Examples:
+```shell
+ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker
+ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --webhook-verification twilio s3cr3t
+ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --bind localhost:1234
+ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --bind unix:/tmp/gunicorn.sock
+
+# Can use the module name as well, such as:
+python -m ngrok gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --response-header X-Awesome True
+```
+
+# Examples
+
+## Frameworks
+* [Aiohttp](https://docs.aiohttp.org) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/aiohttp-ngrok.py)
+* [Django](https://www.djangoproject.com/) - [Single File Example](https://github.com/ngrok/ngrok-py/tree/main/examples/django-single-file.py), [Modify manage.py Example](https://github.com/ngrok/ngrok-py/tree/main/examples/djangosite/manage.py), [Modify asgi.py Example](https://github.com/ngrok/ngrok-py/tree/main/examples/djangosite/djangosite/ngrok-asgi.py), or use the `ngrok-asgi` ASGI Runner discussed above
+* [Flask](https://flask.palletsprojects.com) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/flask-ngrok.py)
+* [Gradio](https://gradio.app/) - [ngrok-asgi Example](https://github.com/ngrok/ngrok-py/tree/main/examples/gradio/gradio-asgi.py), [gradio CLI Example](https://github.com/ngrok/ngrok-py/tree/main/examples/gradio/gradio-ngrok.py) sharing machine learning apps
+* [Gunicorn](https://gunicorn.org/) - Use the `ngrok-asgi` ASGI Runner discussed above
+* [Uvicorn](https://www.uvicorn.org/) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/uvicorn-ngrok.py), or use the `ngrok-asgi` ASGI Runner discussed above
+
+## Tunnel Types
+* HTTP - [Minimal Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-http-minimal.py), [Full Configuration Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-http-full.py)
+* Labeled - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-labeled.py)
+* TCP - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-tcp.py)
+* TLS - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-tls.py)
+
+# Platform Support
+
+Pre-built binaries are provided on PyPI for the following platforms:
+
+| OS         | i686 | x64 | aarch64 | arm |
+| ---------- | -----|-----|---------|-----|
+| Windows    |   ✓  |  ✓  |    *    |     |
+| MacOS      |      |  ✓  |    ✓    |     |
+| Linux      |      |  ✓  |    ✓    |  ✓  |
+| Linux musl |      |  ✓  |    ✓    |     |
+| FreeBSD    |      |  *  |         |     |
+
+ngrok-py, and [ngrok-rs](https://github.com/ngrok/ngrok-rs/) which it depends on, are open source, so it may be possible to build them for other platforms.
+
+* Windows-aarch64 will be supported after the next release of [Ring](https://github.com/briansmith/ring/issues/1167).
+* FreeBSD-x64 is built by the release process, but PyPI won't accept BSD flavors.
+
+# Dependencies
+
+This project relies on [PyO3](https://pyo3.rs/), an excellent system to ease development and building of Rust plugins for Python.
+
+Thank you to [OpenIoTHub](https://github.com/OpenIoTHub/ngrok) for handing over the ngrok name on PyPI.
+
+# License
+
+This project is licensed under either of
+
+ * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or
+   http://www.apache.org/licenses/LICENSE-2.0)
+ * MIT license ([LICENSE-MIT](LICENSE-MIT) or
+   http://opensource.org/licenses/MIT)
+
+at your option.
+
+### Contribution
+
+Unless you explicitly state otherwise, any contribution intentionally submitted
+for inclusion in tokio-core by you, as defined in the Apache-2.0 license, shall be
+dual licensed as above, without any additional terms or conditions.
```

## Comparing `ngrok-0.5.0.dist-info/license_files/LICENSE-APACHE` & `ngrok-0.6.0.dist-info/license_files/LICENSE-APACHE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `ngrok-0.5.0.dist-info/license_files/LICENSE-MIT` & `ngrok-0.6.0.dist-info/license_files/LICENSE-MIT`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 ngrok, Inc.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2022 ngrok, Inc.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

