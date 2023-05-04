# Comparing `tmp/nornir_srl-0.1.2.tar.gz` & `tmp/nornir_srl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_srl-0.1.2.tar", max compression
+gzip compressed data, was "nornir_srl-0.1.4.tar", max compression
```

## Comparing `nornir_srl-0.1.2.tar` & `nornir_srl-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    12132 2023-05-02 12:36:36.599945 nornir_srl-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-05-02 12:36:36.599945 nornir_srl-0.1.2/nornir_srl/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 12:36:36.599945 nornir_srl-0.1.2/nornir_srl/connections/__init__.py
--rw-r--r--   0        0        0     3854 2023-05-02 12:36:36.599945 nornir_srl-0.1.2/nornir_srl/connections/helpers.py
--rw-r--r--   0        0        0    22594 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/connections/srlinux.py
--rw-r--r--   0        0        0     9593 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/fsc.py
--rw-r--r--   0        0        0        0 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/tasks/__init__.py
--rw-r--r--   0        0        0      373 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/tasks/helpers.py
--rw-r--r--   0        0        0     8844 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/tasks/srl_config.py
--rw-r--r--   0        0        0      846 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    13193 1970-01-01 00:00:00.000000 nornir_srl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    13035 2023-05-04 15:20:18.677329 nornir_srl-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-04 15:20:18.677329 nornir_srl-0.1.4/nornir_srl/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:20:18.677329 nornir_srl-0.1.4/nornir_srl/connections/__init__.py
+-rw-r--r--   0        0        0     3904 2023-05-04 15:20:18.677329 nornir_srl-0.1.4/nornir_srl/connections/helpers.py
+-rw-r--r--   0        0        0    25090 2023-05-04 15:20:18.677329 nornir_srl-0.1.4/nornir_srl/connections/srlinux.py
+-rw-r--r--   0        0        0    10756 2023-05-04 15:20:18.677329 nornir_srl-0.1.4/nornir_srl/fsc.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:20:18.677329 nornir_srl-0.1.4/nornir_srl/tasks/__init__.py
+-rw-r--r--   0        0        0      374 2023-05-04 15:20:18.677329 nornir_srl-0.1.4/nornir_srl/tasks/helpers.py
+-rw-r--r--   0        0        0     8905 2023-05-04 15:20:18.681329 nornir_srl-0.1.4/nornir_srl/tasks/srl_config.py
+-rw-r--r--   0        0        0      860 2023-05-04 15:20:18.681329 nornir_srl-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    14096 1970-01-01 00:00:00.000000 nornir_srl-0.1.4/PKG-INFO
```

### Comparing `nornir_srl-0.1.2/nornir_srl/connections/helpers.py` & `nornir_srl-0.1.4/nornir_srl/connections/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 from typing import Any, Dict, List, Tuple, Optional
 import json
 import difflib
 import re
 
+
 def normalize_gnmi_resp(resp: Dict) -> List[Dict[str, Any]]:
     """
     remove gnmi notification and update envelopes from payload
     to make it comparable to intent struct
 
     Args:
         resp: dictionary as returned by gnmi client (get)
-    
+
     Returns:
         dict: with notif and update envelopes removed
     """
     r = []
-    for notif in resp.get("notification"):
+    for notif in resp.get("notification", {}):
         if "update" in notif:
-            updates = [ upd for upd in notif.get("update")]
+            updates = [upd for upd in notif.get("update")]
             for u in updates:
                 if u.get("path"):
-                    r.append( { u.get("path") : u.get("val") } )
+                    r.append({u.get("path"): u.get("val")})
                 else:
-                    if isinstance(u.get("val"), dict) and len(u["val"])>1: # no path with multiple dicts in val: path='/', as per gnmi-spec
-                        r.append( { "/": u["val"] })
+                    if (
+                        isinstance(u.get("val"), dict) and len(u["val"]) > 1
+                    ):  # no path with multiple dicts in val: path='/', as per gnmi-spec
+                        r.append({"/": u["val"]})
                     else:
-                        r.append(u["val"]) # a yang-list that gets a None path in SRL, e.g. /interface
+                        r.append(
+                            u["val"]
+                        )  # a yang-list that gets a None path in SRL, e.g. /interface
         else:
             r.append({})
     return r
 
-def diff_obj(
-        a:Dict, 
-        a_name: str,
-        b:Dict,
-        b_name: str) -> Tuple[bool, str]:
+
+def diff_obj(a: Dict, a_name: str, b: Dict, b_name: str) -> Tuple[bool, str]:
     """
     compares to dicts and show diff
-    
+
     Args:
         a: dict to compare against b
         a_name: name of source of 'a' to show in diff output
         b: dict to compare against a
         b_name: name of source of 'b' to show in diff output
 
     Returns:
@@ -62,60 +64,65 @@
     ):
         diff += line
     if not diff == "":
         return (True, diff)
     else:
         return (False, "")
 
+
 def filter_fields(d: Dict, *fields: str) -> Dict:
-    return  { 
-            k:v for k,v in d.items()
-                if k in [ f.replace('_', '-') for f in fields ]
-        }
-    
-def strip_modules(d: Dict) -> Dict:
+    return {k: v for k, v in d.items() if k in [f.replace("_", "-") for f in fields]}
+
+
+def strip_modules(d: Dict) -> Any:
     p = re.compile(r"srl_nokia-[^:]+:")
 
     if isinstance(d, list):
         return [strip_modules(x) for x in d]
     elif isinstance(d, dict):
         return {strip_modules(k): strip_modules(v) for k, v in d.items()}
     elif isinstance(d, str):
         if d.startswith("srl_nokia-") and ":" in d:
-#            return d[(d.index(":") + 1):]
-            return re.sub(p, '', d)
+            #            return d[(d.index(":") + 1):]
+            return re.sub(p, "", d)
         return d
     else:
         return d
 
 
-#def strip_modules(d: Dict) -> Dict:
+# def strip_modules(d: Dict) -> Dict:
 #    stripped = {}
 #    for k,v in d.items():
 #        k = '/'.join([e.split(':')[-1] for e in k.split('/')])
 #        stripped[k] = copy.deepcopy(v)
 #    for k, v in stripped.items():
 #        if isinstance(v, dict):
 #            stripped[k] = strip_modules(v)
 #        elif isinstance(v, list):
 #            stripped[k] = [strip_modules(d) for d in v if isinstance(d, dict)]
 #        elif isinstance(v, str):
 #            stripped[k] = v.split(':')[-1] if v.startswith('srl_nokia') else v
 #    return stripped
 
-def get_fields_at_depth(d:Dict, depth:int) -> Dict:
+
+def get_fields_at_depth(d: Dict, depth: int) -> Dict:
     if depth == 1:
-        return {k: v for k,v in d.items() if isinstance(v, (str, int, float, list))}
-    return {k: get_fields_at_depth(v, depth-1) for k,v in d.items() if isinstance(v, dict)}
+        return {k: v for k, v in d.items() if isinstance(v, (str, int, float, list))}
+    return {
+        k: get_fields_at_depth(v, depth - 1)
+        for k, v in d.items()
+        if isinstance(v, dict)
+    }
+
 
-def flatten_dict(d: Dict, depth:Optional[int]) -> Dict:
+def flatten_dict(d: Dict) -> Dict:
     r = {}
-    for k,v in d.items():
+    for k, v in d.items():
         if isinstance(v, dict):
             v = [v]
         if isinstance(v, list):
             for e in v:
                 tmp = flatten_dict(e)
-                r.update({ k + '_' + k2:v2 for k2,v2 in tmp.items() } )
+                r.update({k + "_" + k2: v2 for k2, v2 in tmp.items()})
         else:
             r[k] = v
     return r
```

### Comparing `nornir_srl-0.1.2/nornir_srl/connections/srlinux.py` & `nornir_srl-0.1.4/nornir_srl/connections/srlinux.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,79 +8,84 @@
 from natsort import natsorted
 import jmespath
 
 from pygnmi.client import gNMIclient
 
 from nornir.core.plugins.connections import ConnectionPlugin
 from nornir.core.configuration import Config
+from nornir.core.exceptions import ConnectionException
+
 
 from .helpers import strip_modules, normalize_gnmi_resp, filter_fields, flatten_dict
 
 CONNECTION_NAME = "srlinux"
 
+
 class GnmiPath:
-    RE_PATH_COMPONENT = re.compile(r'''
+    RE_PATH_COMPONENT = re.compile(
+        r"""
     (?P<pname>[^/[]+)  # gNMI path name
     (\[(?P<key>\w\D+)   # gNMI path key
     =
     (?P<value>[^\]]+)    # gNMI path value
     \])?
-    ''', re.VERBOSE)
-
-    def __init__(self, path:str):
-        self.path = path.strip('/')
-        self.comp = GnmiPath.RE_PATH_COMPONENT.findall(self.path) # list (1 item per path-el) of tuples (pname, [k=v], k, v)
-        self.elems = [''.join(e[:2]) for e in self.comp]
+    """,
+        re.VERBOSE,
+    )
+
+    def __init__(self, path: str):
+        self.path = path.strip("/")
+        self.comp = GnmiPath.RE_PATH_COMPONENT.findall(
+            self.path
+        )  # list (1 item per path-el) of tuples (pname, [k=v], k, v)
+        self.elems = ["".join(e[:2]) for e in self.comp]
 
     def __str__(self):
         return self.path
-    
+
     def __repr__(self):
         return f"{self.__class__.__name__}('{self.path}')"
-    
+
     @property
-    def resource(self) -> Dict[str,str]:
+    def resource(self) -> Dict[str, str]:
         return {
-            "resource": self.comp[-1][0], 
-            "key": self.comp[-1][2], 
+            "resource": self.comp[-1][0],
+            "key": self.comp[-1][2],
             "val": self.comp[-1][3],
         }
 
     @property
     def with_no_prefix(self):
-        return GnmiPath('/'.join([e.split(':')[-1] for e in self.elems ]))
+        return GnmiPath("/".join([e.split(":")[-1] for e in self.elems]))
 
     @property
     def parent(self):
         if len(self.elems) > 0:
-            return GnmiPath('/'.join(self.elems[:-1]))
+            return GnmiPath("/".join(self.elems[:-1]))
         return None
-    
+
 
 class SrLinux:
     def open(
-            self,
-            hostname: Optional[str],
-            username: Optional[str],
-            password: Optional[str],
-            port: Optional[int],
-            platform: Optional[str],
-            extras: Optional[Dict[str, Any]] = None,
-            configuration: Optional[Config] = None,
+        self,
+        hostname: Optional[str],
+        username: Optional[str],
+        password: Optional[str],
+        port: Optional[int],
+        platform: Optional[str],
+        extras: Optional[Dict[str, Any]] = None,
+        configuration: Optional[Config] = None,
     ) -> None:
         """
         Open a gNMI connection to a device
         """
         target = (hostname, port)
         _connection = gNMIclient(
-                target=target,
-                username=username,
-                password=password,
-                **extras
-                )
+            target=target, username=username, password=password, **extras  # type: ignore
+        )
         _connection.connect()
         self._connection = _connection
         self.connection = self
         self.hostname = hostname
         self.capabilities = self._connection.capabilities()
 
     def gnmi_get(self, **kw):
@@ -92,52 +97,79 @@
     def close(self) -> None:
         self._connection.close()
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} on {self.hostname}"
 
     def get_info(self) -> Dict[str, Any]:
-        path_specs = [
-                { 
-                    "path": "/platform/chassis",
-                    "datatype": "state",
-                    "fields": ['type', 'serial-number', 'part-number', 'hw-mac-address', 'last-booted'],
-                },
-                {
-                    "path": "/platform/control[slot=A]",
-                    "datatype": "state",
-                    "fields": ['software-version', ],
-                }
-        ]                
+        path_specs: List[Dict[str, Any]] = [
+            {
+                "path": "/platform/chassis",
+                "datatype": "state",
+                "fields": [
+                    "type",
+                    "serial-number",
+                    "part-number",
+                    "hw-mac-address",
+                    "last-booted",
+                ],
+            },
+            {
+                "path": "/platform/control[slot=A]",
+                "datatype": "state",
+                "fields": [
+                    "software-version",
+                ],
+            },
+        ]
         result = {}
         for spec in path_specs:
-            resp = self.get(paths = [spec.get("path") ], datatype=spec["datatype"])
+            resp = self.get(paths=[spec.get("path", "")], datatype=spec["datatype"])
             for path in resp[0]:
-                result.update({k:v for k,v in resp[0][path].items() if k in spec["fields"] } )
-        if result.get('software-version'):
-                result['software-version'] = result['software-version'].split('-')[0].lstrip('v')
+                result.update(
+                    {k: v for k, v in resp[0][path].items() if k in spec["fields"]}
+                )
+        if result.get("software-version"):
+            result["software-version"] = (
+                result["software-version"].split("-")[0].lstrip("v")
+            )
 
-        return {'sys_info': [result] }
+        return {"sys_info": [result]}
 
-    def get_sum_subitf(self, interface:Optional[str] = '*' ) -> Dict[str, Any]:
+    def get_sum_subitf(self, interface: str = "*") -> Dict[str, Any]:
         path_spec = {
-                "path": f"/interface[name={interface}]/subinterface",
-                "jmespath": 'interface[].{Itf:name, subitfs: subinterface[].{Subitf:name,\
+            "path": f"/interface[name={interface}]/subinterface",
+            "jmespath": 'interface[].{Itf:name, subitfs: subinterface[].{Subitf:name,\
                       type:type, admin:"admin-state",oper:"oper-state", \
                         ipv4: ipv4.address[]."ip-prefix", vlan: vlan.encap."single-tagged"."vlan-id"}}',
-                "datatype": "state",
-                "key": "index",
-            }
-        resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
+            "datatype": "state",
+            "key": "index",
+        }
+        resp = self.get(
+            paths=[path_spec.get("path", "")], datatype=path_spec["datatype"]
+        )
         res = jmespath.search(path_spec["jmespath"], resp[0])
-        return {'subinterface': res }
-    
-    def get_bgp_rib(self, route_fam:str, route_type:Optional[str] = '2', network_instance:Optional[str] = '*') -> Dict[str, Any]:
-        BGP_RIB_MOD = 'bgp-rib'
-        mod_version = [ m for m in self.capabilities.get("supported_models", []) if BGP_RIB_MOD in m.get("name")][0].get("version") 
+        return {"subinterface": res}
+
+    def get_bgp_rib(
+        self,
+        route_fam: str,
+        route_type: Optional[str] = "2",
+        network_instance: str = "*",
+    ) -> Dict[str, Any]:
+        BGP_RIB_MOD = "bgp-rib"
+        if self.capabilities is not None:
+            mod_version = [
+                m
+                for m in self.capabilities.get("supported_models", [])
+                if BGP_RIB_MOD in m.get("name")
+            ][0].get("version")
+        else:
+            raise Exception("Cannot get gNMI capabilities")
+
         BGP_EVPN_VERSION_MAP = {
             1: ("20"),
         }
         BGP_IP_VERSION_MAP = {
             1: ("2021-", "2022-"),
             2: ("2023-", "20"),
         }
@@ -149,338 +181,429 @@
         ROUTE_TYPE = {
             "1": "ethernet-ad-routes",
             "2": "mac-ip-routes",
             "3": "imet-routes",
             "4": "ethernet-segment-routes",
             "5": "ip-prefix-routes",
         }
-        def augment_routes(d, attribs): # augment routes with attributes
+
+        def augment_routes(d, attribs):  # augment routes with attributes
             if isinstance(d, list):
                 return [augment_routes(x, attribs) for x in d]
             elif isinstance(d, dict):
                 if "attr-id" in d:
                     d.update(attribs.get(d["attr-id"], {}))
-                    d['_r_state'] = ('u' if d['used-route'] else '') + ('*' if d['valid-route'] else '') + ('>' if d['best-route'] else '')
-                    if d.get('vni', 0) == 0:
-                        d['vni'] = '-'
+                    d["_r_state"] = (
+                        ("u" if d["used-route"] else "")
+                        + ("*" if d["valid-route"] else "")
+                        + (">" if d["best-route"] else "")
+                    )
+                    if d.get("vni", 0) == 0:
+                        d["vni"] = "-"
                     return d
                 else:
-                    return {k: augment_routes(v,attribs) for k, v in d.items()}
+                    return {k: augment_routes(v, attribs) for k, v in d.items()}
             else:
                 return d
 
-        evpn_path_version = [ k for k,v  in sorted(BGP_EVPN_VERSION_MAP.items(), key=lambda item: item[0]) if len ( [ ver for ver in v if mod_version.startswith(ver)]) > 0 ] [0]
-        ip_path_version = [ k for k,v  in sorted(BGP_IP_VERSION_MAP.items(), key=lambda item: item[0]) if len ( [ ver for ver in v if mod_version.startswith(ver)]) > 0 ] [0]
+        evpn_path_version = [
+            k
+            for k, v in sorted(BGP_EVPN_VERSION_MAP.items(), key=lambda item: item[0])
+            if len([ver for ver in v if mod_version.startswith(ver)]) > 0
+        ][0]
+        ip_path_version = [
+            k
+            for k, v in sorted(BGP_IP_VERSION_MAP.items(), key=lambda item: item[0])
+            if len([ver for ver in v if mod_version.startswith(ver)]) > 0
+        ][0]
 
         if route_fam not in ROUTE_FAMILY:
             raise ValueError(f"Invalid route family {route_fam}")
         if route_type and route_type not in ROUTE_TYPE:
             raise ValueError(f"Invalid route type {route_type}")
-        
-        PATH_BGP_PATH_ATTRIBS = f"/network-instance[name={network_instance}]/bgp-rib/attr-sets/attr-set"
+
+        PATH_BGP_PATH_ATTRIBS = (
+            f"/network-instance[name={network_instance}]/bgp-rib/attr-sets/attr-set"
+        )
         RIB_EVPN_PATH_VERSIONS = {
-            1: { 
-                'RIB_EVPN_PATH':
-                    (
-                        f"/network-instance[name={network_instance}]/bgp-rib/"
-                        f"{ROUTE_FAMILY[route_fam]}/rib-in-out/rib-in-post/"
-                        f"{ROUTE_TYPE[route_type]}"
-                    ),
-                'RIB_EVPN_JMESPATH_COMMON': '"network-instance"[].{ni:name, Rib:"bgp-rib"."' + ROUTE_FAMILY[route_fam] + \
-                            '"."rib-in-out"."rib-in-post"."' + ROUTE_TYPE[route_type] + '"[]',
-                'RIB_EVPN_JMESPATH_ATTRS': {
+            1: {
+                "RIB_EVPN_PATH": (
+                    f"/network-instance[name={network_instance}]/bgp-rib/"
+                    f"{ROUTE_FAMILY[route_fam]}/rib-in-out/rib-in-post/"
+                    f"{ROUTE_TYPE[route_type]}"  # type: ignore
+                ),
+                "RIB_EVPN_JMESPATH_COMMON": '"network-instance"[].{ni:name, Rib:"bgp-rib"."'
+                + ROUTE_FAMILY[route_fam]
+                + '"."rib-in-out"."rib-in-post"."'
+                + ROUTE_TYPE[route_type]  # type: ignore
+                + '"[]',
+                "RIB_EVPN_JMESPATH_ATTRS": {
                     "1": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, Tag:"ethernet-tag-id",vni:vni, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
                     "2": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, "MAC":"mac-address", "IP":"ip-address",vni:vni,"next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
                     "3": '.{RD:"route-distinguisher", peer:neighbor, Tag:"ethernet-tag-id", "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
                     "4": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
                     "5": '.{RD:"route-distinguisher", peer:neighbor, lpref:"local-pref", "IP-Pfx":"ip-prefix",vni:vni, med:med, "next-hop":"next-hop", GW:"gateway-ip",origin:origin, "0_st":"_r_state"}}',
-                },       
+                },
             },
         }
         RIB_IP_PATH_VERSIONS = {
             1: {
-                'RIB_IP_PATH': 
-                    (
-                        f"/network-instance[name={network_instance}]/bgp-rib/"
-                        f"{ROUTE_FAMILY[route_fam]}/local-rib/routes"
-                    ),
-                'RIB_IP_JMESPATH': '"network-instance"[].{ni:name, Rib:"bgp-rib"."' + ROUTE_FAMILY[route_fam] +
-                        '"."local-rib"."routes"[]' +
-                        '.{neighbor:neighbor, "0_st":"_r_state", "Pfx":prefix, "lpref":"local-pref", med:med, "next-hop":"next-hop","as-path":"as-path".segment[0].member}}',
-
+                "RIB_IP_PATH": (
+                    f"/network-instance[name={network_instance}]/bgp-rib/"
+                    f"{ROUTE_FAMILY[route_fam]}/local-rib/routes"
+                ),
+                "RIB_IP_JMESPATH": '"network-instance"[].{ni:name, Rib:"bgp-rib"."'
+                + ROUTE_FAMILY[route_fam]
+                + '"."local-rib"."routes"[]'
+                + '.{neighbor:neighbor, "0_st":"_r_state", "Pfx":prefix, "lpref":"local-pref", med:med, "next-hop":"next-hop","as-path":"as-path".segment[0].member}}',
             },
             2: {
-                'RIB_IP_PATH':    
-                    (
-                        f"/network-instance[name={network_instance}]/bgp-rib/afi-safi[afi-safi-name={ROUTE_FAMILY[route_fam]}]/"
-                        f"{ROUTE_FAMILY[route_fam]}/local-rib/routes"
-                    ),  
-                'RIB_IP_JMESPATH': '"network-instance"[].{ni:name, Rib:"bgp-rib"."afi-safi"[]."' + ROUTE_FAMILY[route_fam] +
-                        '"."local-rib"."routes"[]' +
-                        '.{neighbor:neighbor, "0_st":"_r_state", "Pfx":prefix, "lpref":"local-pref", med:med, "next-hop":"next-hop","as-path":"as-path".segment[0].member}}',
+                "RIB_IP_PATH": (
+                    f"/network-instance[name={network_instance}]/bgp-rib/afi-safi[afi-safi-name={ROUTE_FAMILY[route_fam]}]/"
+                    f"{ROUTE_FAMILY[route_fam]}/local-rib/routes"
+                ),
+                "RIB_IP_JMESPATH": '"network-instance"[].{ni:name, Rib:"bgp-rib"."afi-safi"[]."'
+                + ROUTE_FAMILY[route_fam]
+                + '"."local-rib"."routes"[]'
+                + '.{neighbor:neighbor, "0_st":"_r_state", "Pfx":prefix, "lpref":"local-pref", med:med, "next-hop":"next-hop","as-path":"as-path".segment[0].member}}',
             },
         }
 
         PATH_SPECS = {
             "evpn": {
                 "path": RIB_EVPN_PATH_VERSIONS[evpn_path_version]["RIB_EVPN_PATH"],
-                "jmespath": RIB_EVPN_PATH_VERSIONS[evpn_path_version]["RIB_EVPN_JMESPATH_COMMON"] + RIB_EVPN_PATH_VERSIONS[evpn_path_version]['RIB_EVPN_JMESPATH_ATTRS'][route_type],
+                "jmespath": RIB_EVPN_PATH_VERSIONS[evpn_path_version][
+                    "RIB_EVPN_JMESPATH_COMMON"
+                ]
+                + RIB_EVPN_PATH_VERSIONS[evpn_path_version]["RIB_EVPN_JMESPATH_ATTRS"][
+                    route_type
+                ],
                 "datatype": "state",
             },
             "ipv4": {
-                "path": RIB_IP_PATH_VERSIONS[ip_path_version]['RIB_IP_PATH'],
-                "jmespath": RIB_IP_PATH_VERSIONS[ip_path_version]['RIB_IP_JMESPATH'],
+                "path": RIB_IP_PATH_VERSIONS[ip_path_version]["RIB_IP_PATH"],
+                "jmespath": RIB_IP_PATH_VERSIONS[ip_path_version]["RIB_IP_JMESPATH"],
                 "datatype": "state",
             },
-            
         }
         attribs = dict()
-        resp = self.get(paths = [ PATH_BGP_PATH_ATTRIBS ], datatype="state")
+        resp = self.get(paths=[PATH_BGP_PATH_ATTRIBS], datatype="state")
         for ni in resp[0].get("network-instance", []):
             if ni["name"] not in attribs:
                 attribs[ni["name"]] = dict()
             for path in ni.get("bgp-rib", {}).get("attr-sets", {}).get("attr-set", []):
                 path_copy = copy.deepcopy(path)
-                attribs[ni["name"]].update( { path_copy.pop("index"): path_copy } )
+                attribs[ni["name"]].update({path_copy.pop("index"): path_copy})
 
         path_spec = PATH_SPECS[route_fam]
-        resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
+        resp = self.get(paths=[path_spec.get("path")], datatype=path_spec["datatype"])
         for ni in resp[0].get("network-instance", []):
             ni = augment_routes(ni, attribs[ni["name"]])
 
         res = jmespath.search(path_spec["jmespath"], resp[0])
         if res:
             for ni in res:
-                for route in ni.get('Rib', []):
-                    route['as-path'] = str(route['as-path']) + ' i' if route.get('as-path') else 'i'
+                for route in ni.get("Rib", []):
+                    route["as-path"] = (
+                        str(route["as-path"]) + " i" if route.get("as-path") else "i"
+                    )
         else:
             res = []
-        return {'bgp_rib': res }
+        return {"bgp_rib": res}
+
+    def get_sum_bgp(self, network_instance: Optional[str] = "*") -> Dict[str, Any]:
+        BGP_MOD = "urn:srl_nokia/bgp:srl_nokia-bgp"
+
+        if self.capabilities is not None:
+            mod_version = [
+                m
+                for m in self.capabilities.get("supported_models", [])
+                if BGP_MOD == m.get("name")
+            ][0].get("version")
+        else:
+            raise Exception("Capabilities not set")
+        BGP_VERSION_MAP = {1: ("2021-", "2022-"), 2: ("2023-3", "20")}
+        our_version = [
+            k
+            for k, v in sorted(BGP_VERSION_MAP.items(), key=lambda item: item[0])
+            if len([ver for ver in v if mod_version.startswith(ver)]) > 0
+        ][0]
 
-    def get_sum_bgp(self, network_instance:Optional[str] = '*' ) -> Dict[str, Any]:
-        BGP_MOD = 'urn:srl_nokia/bgp:srl_nokia-bgp'
-        mod_version = [ m for m in self.capabilities.get("supported_models", []) if BGP_MOD == m.get("name")][0].get("version") 
-        BGP_VERSION_MAP = {
-            1: ("2021-", "2022-"),
-            2: ("2023-3", "20")
-        }
-        our_version = [ k for k,v  in sorted(BGP_VERSION_MAP.items(), key=lambda item: item[0]) if len ( [ ver for ver in v if mod_version.startswith(ver)]) > 0 ] [0]
         def augment_resp(resp):
             for ni in resp[0]["network-instance"]:
-                if ni.get('protocols') and ni['protocols'].get('bgp'):
-                    for peer in ni['protocols']['bgp']['neighbor']:
+                if ni.get("protocols") and ni["protocols"].get("bgp"):
+                    for peer in ni["protocols"]["bgp"]["neighbor"]:
                         peer_data = dict()
                         if our_version == 1:
-                            peer_data['evpn'] = peer.get('evpn')
-                            peer_data['ipv4-unicast'] = peer.get('ipv4-unicast')
-                            peer_data['local-as'] = peer.get('local-as', [{}])[0].get('as-number', '-')
+                            peer_data["evpn"] = peer.get("evpn")
+                            peer_data["ipv4-unicast"] = peer.get("ipv4-unicast")
+                            peer_data["local-as"] = peer.get("local-as", [{}])[0].get(
+                                "as-number", "-"
+                            )
                         elif our_version == 2:
-                            peer_data['local-as'] = peer.get('local-as', {}).get('as-number', '-')
-                            for afi in peer.get('afi-safi', []):
-                                if afi['afi-safi-name'] == 'evpn':
-                                    peer_data['evpn'] = afi
-                                elif afi['afi-safi-name'] == 'ipv4-unicast':
-                                    peer_data['ipv4-unicast'] = afi
-                        peer["_local-asn"] = peer_data['local-as']
-                        if peer_data.get('evpn'):
-                            peer["_evpn"] = str(peer_data["evpn"]["received-routes"]) + "/" + \
-                            str(peer_data["evpn"]["active-routes"]) + "/" + \
-                            str(peer_data["evpn"]["sent-routes"]) if peer_data["evpn"]["admin-state"] == "enable" else "disabled"
+                            peer_data["local-as"] = peer.get("local-as", {}).get(
+                                "as-number", "-"
+                            )
+                            for afi in peer.get("afi-safi", []):
+                                if afi["afi-safi-name"] == "evpn":
+                                    peer_data["evpn"] = afi
+                                elif afi["afi-safi-name"] == "ipv4-unicast":
+                                    peer_data["ipv4-unicast"] = afi
+                        peer["_local-asn"] = peer_data["local-as"]
+                        if peer_data.get("evpn"):
+                            peer["_evpn"] = (
+                                str(peer_data["evpn"]["received-routes"])
+                                + "/"
+                                + str(peer_data["evpn"]["active-routes"])
+                                + "/"
+                                + str(peer_data["evpn"]["sent-routes"])
+                                if peer_data["evpn"]["admin-state"] == "enable"
+                                else "disabled"
+                            )
                         else:
                             peer["_evpn"] = "-"
-                        if peer_data.get('ipv4-unicast'):
+                        if peer_data.get("ipv4-unicast"):
                             if peer_data["ipv4-unicast"]["admin-state"] == "enable":
-                                peer["_ipv4"] = str(peer_data["ipv4-unicast"]["received-routes"]) + "/" + \
-                                    str(peer_data["ipv4-unicast"]["active-routes"]) + "/" + \
-                                    str(peer_data["ipv4-unicast"]["sent-routes"])
-                                if peer_data["ipv4-unicast"].get("oper-state")== "down":
+                                peer["_ipv4"] = (
+                                    str(peer_data["ipv4-unicast"]["received-routes"])
+                                    + "/"
+                                    + str(peer_data["ipv4-unicast"]["active-routes"])
+                                    + "/"
+                                    + str(peer_data["ipv4-unicast"]["sent-routes"])
+                                )
+                                if (
+                                    peer_data["ipv4-unicast"].get("oper-state")
+                                    == "down"
+                                ):
                                     peer["_ipv4"] = "down"
                             else:
                                 peer["_ipv4"] = "disabled"
                         else:
                             peer["_ipv4"] = "-"
 
         path_spec = {
-                "path": f"/network-instance[name={network_instance}]/protocols/bgp/neighbor",
-                "jmespath": '"network-instance"[].{NetwInst:name, Neighbors: protocols.bgp.neighbor[].{"1_peer":"peer-address",\
+            "path": f"/network-instance[name={network_instance}]/protocols/bgp/neighbor",
+            "jmespath": '"network-instance"[].{NetwInst:name, Neighbors: protocols.bgp.neighbor[].{"1_peer":"peer-address",\
                     peer_as:"peer-as", state:"session-state",local_as:"_local-asn",\
                     "group":"peer-group", "export_policy":"export-policy", "import_policy":"import-policy",\
                     "AFI/SAFI\\nIPv4-UC\\nRx/Act/Tx":"_ipv4", "AFI/SAFI\\nEVPN\\nRx/Act/Tx":"_evpn"}}',
-                "datatype": "state",
-                "key": "index",
-            }
-        resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
+            "datatype": "state",
+            "key": "index",
+        }
+        resp = self.get(
+            paths=[path_spec.get("path", "")], datatype=path_spec["datatype"]
+        )
         augment_resp(resp)
         res = jmespath.search(path_spec["jmespath"], resp[0])
-        return {'bgp_peers': res }
+        return {"bgp_peers": res}
 
-    def get_lldp_sum(self, interface:Optional[str] = '*' ) -> Dict[str, Any]:
+    def get_lldp_sum(self, interface: Optional[str] = "*") -> Dict[str, Any]:
         path_spec = {
-                "path": f"/system/lldp/interface[name={interface}]/neighbor",
-                "jmespath": '"system/lldp".interface[].{interface:name, Neighbors:neighbor[].{"Nbr-port":"port-id",\
+            "path": f"/system/lldp/interface[name={interface}]/neighbor",
+            "jmespath": '"system/lldp".interface[].{interface:name, Neighbors:neighbor[].{"Nbr-port":"port-id",\
                     "Nbr-System":"system-name", "Nbr-port-desc":"port-description"}}',
-                "datatype": "state",
-            }
-        resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
+            "datatype": "state",
+        }
+        resp = self.get(
+            paths=[path_spec.get("path", "")], datatype=path_spec["datatype"]
+        )
         res = jmespath.search(path_spec["jmespath"], resp[0])
-        return {'lldp_nbrs': res }    
+        return {"lldp_nbrs": res}
 
-    def get_mac_table(self, network_instance:Optional[str] = '*') -> Dict[str, Any]:
+    def get_mac_table(self, network_instance: Optional[str] = "*") -> Dict[str, Any]:
         path_spec = {
             "path": f"/network-instance[name={network_instance}]/bridge-table/mac-table/mac",
             "jmespath": '"network-instance"[].{"Netw-Inst":name, Fib:"bridge-table"."mac-table".mac[].{Address:address,\
                         Dest:destination, Type:type}}',
             "datatype": "state",
         }
-        resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
+        resp = self.get(
+            paths=[path_spec.get("path", "")], datatype=path_spec["datatype"]
+        )
         res = jmespath.search(path_spec["jmespath"], resp[0])
-        return {'mac_table': res}
-    
-    def get_rib_ipv4(self, network_instance:Optional[str] = '*' ) -> Dict[str, Any]:   
+        return {"mac_table": res}
 
+    def get_rib_ipv4(self, network_instance: Optional[str] = "*") -> Dict[str, Any]:
         path_spec = {
-                "path": f"/network-instance[name={network_instance}]/route-table/ipv4-unicast",
-                "jmespath": '"network-instance"[].{"Netw-Inst":name, Rib:"route-table"."ipv4-unicast".route[].{"Prefix":"ipv4-prefix",\
+            "path": f"/network-instance[name={network_instance}]/route-table/ipv4-unicast",
+            "jmespath": '"network-instance"[].{"Netw-Inst":name, Rib:"route-table"."ipv4-unicast".route[].{"Prefix":"ipv4-prefix",\
                     "next-hop":"_next-hop",type:"route-type", metric:metric, pref:preference, itf:"_nh_itf"}}',
-                "datatype": "state",
-            }
+            "datatype": "state",
+        }
 
-        nhgroups = self.get(paths = [ f"/network-instance[name={network_instance}]/route-table/next-hop-group[index=*]" ],
-                        datatype="state")
-        nhs = self.get(paths = [ f"/network-instance[name={network_instance}]/route-table/next-hop[index=*]" ],
-                        datatype="state")
+        nhgroups = self.get(
+            paths=[
+                f"/network-instance[name={network_instance}]/route-table/next-hop-group[index=*]"
+            ],
+            datatype="state",
+        )
+        nhs = self.get(
+            paths=[
+                f"/network-instance[name={network_instance}]/route-table/next-hop[index=*]"
+            ],
+            datatype="state",
+        )
 
         nh_mapping = {}
-        for ni in nhs[0].get("network-instance"):
+        for ni in nhs[0].get("network-instance", {}):
             tmp_map = {}
             for nh in ni["route-table"]["next-hop"]:
-                tmp_map[nh["index"]] = { "ip-address":      nh.get("ip-address"),
-                                        "type":             nh.get("type"),
-                                        "subinterface":    nh.get("subinterface"),
+                tmp_map[nh["index"]] = {
+                    "ip-address": nh.get("ip-address"),
+                    "type": nh.get("type"),
+                    "subinterface": nh.get("subinterface"),
                 }
                 if "resolving-tunnel" in nh:
-                    tmp_map[nh["index"]].update( 
-                        { 
-                            "tunnel": (nh.get("resolving-tunnel")).get("tunnel-type") + ":" +  (nh.get("resolving-tunnel")).get("ip-prefix")        
-                        })
+                    tmp_map[nh["index"]].update(
+                        {
+                            "tunnel": (nh.get("resolving-tunnel")).get("tunnel-type")
+                            + ":"
+                            + (nh.get("resolving-tunnel")).get("ip-prefix")
+                        }
+                    )
                 if "resolving-route" in nh:
-                    tmp_map[nh["index"]].update( 
-                        { 
-                            "resolving-route": (nh.get("resolving-route")).get("ip-prefix")        
-                        })
-                    
-            nh_mapping.update( { ni["name"]: tmp_map})
+                    tmp_map[nh["index"]].update(
+                        {
+                            "resolving-route": (nh.get("resolving-route")).get(
+                                "ip-prefix"
+                            )
+                        }
+                    )
+
+            nh_mapping.update({ni["name"]: tmp_map})
         nhgroup_mapping = {}
-        for ni in nhgroups[0].get("network-instance"):
+        for ni in nhgroups[0].get("network-instance", {}):
             network_instance = ni["name"]
             tmp_map = {}
             for nhgroup in ni["route-table"]["next-hop-group"]:
-#                    tmp_map[nhgroup["index"]] = [ nh["next-hop"] for nh in nhgroup["next-hop"] ]
-                tmp_map[nhgroup["index"]] = [ 
-                        nh_mapping[network_instance][nh.get("next-hop")] 
-                                for nh in nhgroup["next-hop"] 
-                        ]
-            nhgroup_mapping.update( { ni["name"]: tmp_map})
-        
-        resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
-        for ni in resp[0].get("network-instance"):
-            if len(ni["route-table"]["ipv4-unicast"])>0:
+                #                    tmp_map[nhgroup["index"]] = [ nh["next-hop"] for nh in nhgroup["next-hop"] ]
+                tmp_map[nhgroup["index"]] = [
+                    nh_mapping[network_instance][nh.get("next-hop")]
+                    for nh in nhgroup["next-hop"]
+                ]
+            nhgroup_mapping.update({ni["name"]: tmp_map})
+
+        resp = self.get(
+            paths=[path_spec.get("path", "")], datatype=path_spec["datatype"]
+        )
+        for ni in resp[0].get("network-instance", {}):
+            if len(ni["route-table"]["ipv4-unicast"]) > 0:
                 for route in ni["route-table"]["ipv4-unicast"]["route"]:
                     if "next-hop-group" in route:
-                        route["_next-hop"] = [ nh.get("ip-address") for nh in nhgroup_mapping[ni["name"]][route["next-hop-group"]] ]
-                        route["_nh_itf"] = [ nh.get("subinterface") for nh in nhgroup_mapping[ni["name"]][route["next-hop-group"]] ]
-                        
+                        route["_next-hop"] = [
+                            nh.get("ip-address")
+                            for nh in nhgroup_mapping[ni["name"]][
+                                route["next-hop-group"]
+                            ]
+                        ]
+                        route["_nh_itf"] = [
+                            nh.get("subinterface")
+                            for nh in nhgroup_mapping[ni["name"]][
+                                route["next-hop-group"]
+                            ]
+                        ]
+
         res = jmespath.search(path_spec["jmespath"], resp[0])
-        return {'ipv4_rib': res }    
-    
-    def get_nwi_itf(self, nw_instance:Optional[str] = '*') -> Dict[str, Any]:
+        return {"ipv4_rib": res}
+
+    def get_nwi_itf(self, nw_instance: str = "*") -> Dict[str, Any]:
+        SUBITF_PATH = "/interface[name=*]/subinterface"
         path_spec = {
-                "path": f"/network-instance[name={nw_instance}]",
-                "jmespath": '"network-instance"[].{name:name,oper:"oper-state",type:type,itfs: interface[].{Subitf:name,\
-                      "if-oper":"oper-state", "if-dwn-reason":"oper-down-reason"}}',
-                "datatype": "state",
-            }
-        resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
+            "path": f"/network-instance[name={nw_instance}]",
+            "jmespath": '"network-instance"[].{ni:name,oper:"oper-state",type:type,"router-id":protocols.bgp."router-id",\
+                    itfs: interface[].{Subitf:name,"if-oper":"oper-state", ipv4:ipv4.address[]."ip-prefix",\
+                        vlan:vlan.encap."single-tagged"."vlan-id"}}',
+            "datatype": "state",
+        }
+        subitf: Dict[str, Dict[str, Any]] = {}
+        resp = self.get(paths=[SUBITF_PATH], datatype="config")
+        for itf in resp[0].get("interface", []):
+            for si in itf.get("subinterface", []):
+                subif_name = itf["name"] + "." + str(si.pop("index"))
+                subitf[subif_name] = si
+
+        resp = self.get(
+            paths=[path_spec.get("path", "")], datatype=path_spec["datatype"]
+        )
+        for ni in resp[0].get("network-instance", {}):
+            for ni_itf in ni.get("interface", []):
+                ni_itf.update(subitf.get(ni_itf["name"], {}))
+
         res = jmespath.search(path_spec["jmespath"], resp[0])
-        return {'nwi_itfs': res }
+        return {"nwi_itfs": res}
 
     def get(
-            self, 
-            paths:List[str], 
-            datatype: Optional[str] = "config", 
-            strip_mod:Optional[bool] = True
-        ) -> List[Dict[str, Any]]:
-
+        self,
+        paths: List[str],
+        datatype: Optional[str] = "config",
+        strip_mod: Optional[bool] = True,
+    ) -> List[Dict[str, Any]]:
         if self._connection:
             resp = normalize_gnmi_resp(
-                    self._connection.get(path=paths, datatype=datatype, encoding="json_ietf")
-                    )
+                self._connection.get(
+                    path=paths, datatype=datatype, encoding="json_ietf"  # type: ignore
+                )
+            )
         else:
             raise Exception("no active connection")
         if strip_mod:
-            return [ strip_modules(d) for d in resp ]
+            return [strip_modules(d) for d in resp]
         else:
             return resp
 
     def set_config(
-            self, 
-            input: List[Dict[str, Any]], 
-            op: Optional[str] = 'update',
-            dry_run: Optional[bool] = False,
-            strip_mod: Optional[bool] = True,
-            ) -> str:
-
+        self,
+        input: List[Dict[str, Any]],
+        op: Optional[str] = "update",
+        dry_run: Optional[bool] = False,
+        strip_mod: Optional[bool] = True,
+    ) -> str:
         device_cfg_after = []
         r_list = []
         for r in input:
             r_list += r.keys()
-#        r_list = [ list(r.keys())[0] for r in input ]
+        #        r_list = [ list(r.keys())[0] for r in input ]
         device_cfg_before = self.get(paths=r_list, datatype="config")
 
         if not dry_run:
             paths = []
             for d in input:
                 for p, v in d.items():
                     ### to check - hack
                     ### to address intents that are lists, e.g. /interface
-#                    if isinstance(v, list): 
-#                        v = { p: v }
-#                        p = '/'.join(p.split('/')[:-1])
-#                        if len(p) == 0:
-#                            p = "/"
+                    #                    if isinstance(v, list):
+                    #                        v = { p: v }
+                    #                        p = '/'.join(p.split('/')[:-1])
+                    #                        if len(p) == 0:
+                    #                            p = "/"
                     ###
                     paths.append((p, v))
-            if op == 'update':
-                r = self._connection.set(update=paths, encoding='json_ietf')
-            elif op == 'replace':
-                r = self._connection.set(replace=paths, encoding='json_ietf')
-            elif op == 'delete':
-                delete_paths = [ list(p.keys())[0] for p in input ]
+            if op == "update":
+                r = self._connection.set(update=paths, encoding="json_ietf")
+            elif op == "replace":
+                r = self._connection.set(replace=paths, encoding="json_ietf")
+            elif op == "delete":
+                delete_paths = [list(p.keys())[0] for p in input]
                 r = self._connection.set(delete=delete_paths, encoding="json_ietf")
             else:
                 raise ValueError(f"invalid value for parameter 'op': {op}")
             device_cfg_after = self.get(paths=r_list, datatype="config")
         else:
             device_cfg_after = input
 
-        dd = DeepDiff(device_cfg_before, device_cfg_after)        
+        dd = DeepDiff(device_cfg_before, device_cfg_after)
         diff = ""
         for i in range(len(r_list)):
             before_json = json.dumps(device_cfg_before[i], indent=2, sort_keys=True)
             after_json = json.dumps(device_cfg_after[i], indent=2, sort_keys=True)
             for line in difflib.unified_diff(
-                        before_json.splitlines(keepends=True),
-                        after_json.splitlines(keepends=True),
-                        fromfile="before",
-                        tofile="after", 
-                        n=5,
+                before_json.splitlines(keepends=True),
+                after_json.splitlines(keepends=True),
+                fromfile="before",
+                tofile="after",
+                n=5,
             ):
                 diff += line
             if len(diff) > 0:
                 diff += "\n"
 
         return diff
-
-                
-    
-
-
```

### Comparing `nornir_srl-0.1.2/nornir_srl/fsc.py` & `nornir_srl-0.1.4/nornir_srl/fsc.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,215 +4,301 @@
 from nornir import InitNornir
 
 from nornir.core.task import Result, Task, AggregatedResult
 
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
-from rich.box import    MINIMAL_DOUBLE_HEAD
+from rich.box import MINIMAL_DOUBLE_HEAD
 from rich.style import Style
 from rich.theme import Theme
 
 from nornir_utils.plugins.functions import print_result
 from nornir_srl.tasks.srl_config import configure_device, restore_config
 
 from nornir_srl.connections.srlinux import CONNECTION_NAME
 
 import click
 
+
 def sys_info(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
     return Result(host=task.host, result=device.get_info())
 
+
 def get_itfs(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
     return Result(host=task.host, result=device.get_itf())
 
+
 def subinterface(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
     return Result(host=task.host, result=device.get_sum_subitf())
 
+
 def bgp_peers(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    return Result(host=task.host, result = device.get_sum_bgp())
+    return Result(host=task.host, result=device.get_sum_bgp())
+
 
 def ipv4_rib(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    return Result(host=task.host, result = device.get_rib_ipv4())
+    return Result(host=task.host, result=device.get_rib_ipv4())
+
 
 def bgp_rib(task: Task, **kwargs) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
     route_fam = kwargs.get("route_fam")
     route_type = kwargs.get("route_type", "2")
     if not route_fam:
         raise Exception("bgp_rib task requires route_fam report option")
-    return Result(host=task.host, result = device.get_bgp_rib(route_fam=route_fam, route_type=route_type))
+    return Result(
+        host=task.host,
+        result=device.get_bgp_rib(route_fam=route_fam, route_type=route_type),
+    )
+
 
 def mac_table(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    return Result(host=task.host, result = device.get_mac_table())
+    return Result(host=task.host, result=device.get_mac_table())
+
 
 def nwi_itfs(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    return Result(host=task.host, result = device.get_nwi_itf())
+    return Result(host=task.host, result=device.get_nwi_itf())
+
 
 def lldp_nbrs(task: Task) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    return Result(host=task.host, result = device.get_lldp_sum())
+    return Result(host=task.host, result=device.get_lldp_sum())
 
-def print_table ( title: str, resource: str, results: AggregatedResult, filter: Optional[Dict], **kwargs) -> None:
 
-    table_theme = Theme({
-        "ok": "green",
-        "warn": "orange3",
-        "info": "blue",
-        "err": "bold red",
-    })
+def print_table(
+    title: str,
+    resource: str,
+    results: AggregatedResult,
+    filter: Optional[Dict],
+    **kwargs,
+) -> None:
+    table_theme = Theme(
+        {
+            "ok": "green",
+            "warn": "orange3",
+            "info": "blue",
+            "err": "bold red",
+        }
+    )
     STYLE_MAP = {
-        'up': '[ok]',
-        'down': '[err]',
-        'enable': '[ok]',
-        'disable': '[info]',
-        'routed': '[cyan]',
-        'bridged': '[blue]',
-        'established': '[ok]',
-        'active': '[cyan]',
+        "up": "[ok]",
+        "down": "[err]",
+        "enable": "[ok]",
+        "disable": "[info]",
+        "routed": "[cyan]",
+        "bridged": "[blue]",
+        "established": "[ok]",
+        "active": "[cyan]",
     }
 
     console = Console(theme=table_theme)
     if kwargs.get("box_type") and kwargs["box_type"] != None:
         box_type = str(kwargs["box_type"]).upper()
         try:
             box_type = getattr(importlib.import_module("rich.box"), box_type)
         except AttributeError:
-            print(f"Unknown box type {box_type}. Check 'python -m rich.box' for valid box types.")
+            print(
+                f"Unknown box type {box_type}. Check 'python -m rich.box' for valid box types."
+            )
             box_type = MINIMAL_DOUBLE_HEAD
     else:
         box_type = MINIMAL_DOUBLE_HEAD
-#    table = Table(title=title, highlight=True, box=MINIMAL_DOUBLE_HEAD)
+    #    table = Table(title=title, highlight=True, box=MINIMAL_DOUBLE_HEAD)
     table = Table(title=title, highlight=True, box=box_type)
-    table.add_column('Node', no_wrap=True)
+    table.add_column("Node", no_wrap=True)
 
     # get fields across a nested dict with dicts and lists of dicts
     def get_fields(b, depth=0):
         fields = []
         if isinstance(b, list) and len(b) > 0:
-            fields.extend(get_fields(b[0], depth=depth+1))
+            fields.extend(get_fields(b[0], depth=depth + 1))
         elif isinstance(b, dict):
-            for k,v in b.items():
-                if isinstance(v, list) and len(v)>0  and isinstance(v[0], dict):
-                    fields.extend(get_fields(v[0], depth=depth+1))
+            for k, v in b.items():
+                if isinstance(v, list) and len(v) > 0 and isinstance(v[0], dict):
+                    fields.extend(get_fields(v[0], depth=depth + 1))
                 elif isinstance(v, dict):
-                    fields.extend(get_fields(v, depth=depth+1))
+                    fields.extend(get_fields(v, depth=depth + 1))
                 else:
                     fields.append(k)
-            if depth>0:
+            if depth > 0:
                 fields = sorted(fields)
         return fields
 
     def pass_filter(row, filter):
         if filter == None:
             return True
         if len(
             {
-                k:v for k,v in row.items() 
-                    if filter.get(k) and str(filter[k]) in str(row[k])
+                k: v
+                for k, v in row.items()
+                if filter.get(k) and str(filter[k]) in str(row[k])
             }
         ) < len(filter):
             return False
         else:
             return True
-    
-    col_names = []   
+
+    col_names = []
     for host, host_result in results.items():
         rows = []
         r = host_result[0]  # only look at result of first task, 1 task per table
         if r.failed:
             print(f"Failed to get {resource} for {host}. Exception: {r.exception}")
             continue
         if r.result.get(resource) == None:
             continue
         for n, l in enumerate(r.result.get(resource)):
             if len(col_names) == 0:
                 col_names = get_fields(l)
                 for col in col_names:
                     table.add_column(col, no_wrap=True)
-            common = {x:y for x,y in l.items() if  isinstance(y, (str, int, float)) or 
-                      (isinstance(y, list) and len(y) > 0 and not isinstance(y[0], dict)) }
-            if len ( [v for v in l.values() if isinstance(v, list)] ) == 0: # single row per host
+            common = {
+                x: y
+                for x, y in l.items()
+                if isinstance(y, (str, int, float))
+                or (isinstance(y, list) and len(y) > 0 and not isinstance(y[0], dict))
+            }
+            if (
+                len([v for v in l.values() if isinstance(v, list)]) == 0
+            ):  # single row per host
                 if pass_filter(common, filter):
                     rows.append(common)
-#                if pass_filter(row, filter):
-#                    rows.append({k:v for k,v in l.items()})
+            #                if pass_filter(row, filter):
+            #                    rows.append({k:v for k,v in l.items()})
             else:
-                for key,v in l.items():
+                for key, v in l.items():
                     if isinstance(v, list):
-                        first_row=True
+                        first_row = True
                         for item in v:
                             row = {}
-                            row.update({k:y for k,y in item.items() if isinstance(y, (str, int, float)) or
-                                        ( isinstance(y, list) and len(y)>0 and not isinstance(y[0], dict))})
-                            if pass_filter({k:v for k,v in list(common.items()) + list(row.items()) }, filter):
+                            row.update(
+                                {
+                                    k: y
+                                    for k, y in item.items()
+                                    if isinstance(y, (str, int, float))
+                                    or (
+                                        isinstance(y, list)
+                                        and len(y) > 0
+                                        and not isinstance(y[0], dict)
+                                    )
+                                }
+                            )
+                            if pass_filter(
+                                {
+                                    k: v
+                                    for k, v in list(common.items()) + list(row.items())
+                                },
+                                filter,
+                            ):
                                 if first_row:
-                                    rows.append( {k:v for k,v in list(common.items()) + list(row.items()) } )
+                                    rows.append(
+                                        {
+                                            k: v
+                                            for k, v in list(common.items())
+                                            + list(row.items())
+                                        }
+                                    )
                                 else:
                                     rows.append(row)
                                 first_row = False
-                                    
+
         first_row = True
         for row in rows:
             for k, v in row.items():
-                row[k] = str(STYLE_MAP.get(str(v),'')) + str(v)
-            values = [ row.get(k,'') for k in col_names ]
+                row[k] = str(STYLE_MAP.get(str(v), "")) + str(v)
+            values = [row.get(k, "") for k in col_names]
             if first_row:
-                table.add_row(host, *values) 
+                table.add_row(host, *values)
                 first_row = False
             else:
-                table.add_row( "", *values)
+                table.add_row("", *values)
 
         table.add_section()
     console.print(table)
 
 
 @click.command
-@click.argument('report')
-@click.option('--cfg', '-c', default='nornir_config.yaml', show_default=True, help='Nornir config file')
-@click.option('--inv-filter', '-i', multiple=True, help='filter inventory, e.g. -i site=lab -i role=leaf')
-@click.option('--field-filter', '-f', multiple=True, help='filter fields, e.g. -f state=up -f admin_state=enable')
-@click.option('--box-type', '-b', multiple=False, help="box type of printed table, e.g. -b minimal_double_head. 'python -m rich.box' for options")
-@click.option('--report-options', '-r', multiple=True, help="report-specific options, e.g. -o route_fam=evpn -o route_type=2 for 'bgp-rib report")
+@click.argument("report")
+@click.option(
+    "--cfg",
+    "-c",
+    default="nornir_config.yaml",
+    show_default=True,
+    help="Nornir config file",
+)
+@click.option(
+    "--inv-filter",
+    "-i",
+    multiple=True,
+    help="filter inventory, e.g. -i site=lab -i role=leaf",
+)
+@click.option(
+    "--field-filter",
+    "-f",
+    multiple=True,
+    help="filter fields, e.g. -f state=up -f admin_state=enable",
+)
+@click.option(
+    "--box-type",
+    "-b",
+    multiple=False,
+    help="box type of printed table, e.g. -b minimal_double_head. 'python -m rich.box' for options",
+)
+@click.option(
+    "--report-options",
+    "-r",
+    multiple=True,
+    help="report-specific options, e.g. -o route_fam=evpn -o route_type=2 for 'bgp-rib report",
+)
 def cli(
-    report: str, 
-    cfg: str = 'config.yaml',
-    inv_filter:Optional[List] = None,
-    field_filter:Optional[List] = None,
-    report_options:Optional[List] = None,
-    box_type:Optional[str] = None,
-    ) -> None: 
-
-    i_filter = {k:v for k,v in [ f.split('=') for f in inv_filter]} if inv_filter else {}
-    f_filter = {k:v for k,v in [ f.split('=') for f in field_filter]} if field_filter else {}
-    report_options = {k:v for k,v in [ f.split('=') for f in report_options]} if report_options else {}
+    report: str,
+    cfg: str = "config.yaml",
+    inv_filter: Optional[List] = None,
+    field_filter: Optional[List] = None,
+    report_options: Optional[List] = None,
+    box_type: Optional[str] = None,
+) -> None:
+    i_filter = (
+        {k: v for k, v in [f.split("=") for f in inv_filter]} if inv_filter else {}
+    )
+    f_filter = (
+        {k: v for k, v in [f.split("=") for f in field_filter]} if field_filter else {}
+    )
+    report_options = (
+        {k: v for k, v in [f.split("=") for f in report_options]}
+        if report_options
+        else {}
+    )
 
     if box_type:
         box_type = box_type.upper()
 
     reports = {
-        'bgp-peers': (bgp_peers, "BGP Peers"),
-        'subinterface': (subinterface, "Sub-Interfaces"),
-        'ipv4-rib': (ipv4_rib, "IPv4 RIB"),
-        'mac-table': (mac_table, "MAC Table"),
-        'sys-info': (sys_info, "System Info"),
-        'nwi-itfs': (nwi_itfs, "Network-Instance Interfaces"),
-        'lldp-nbrs': (lldp_nbrs, "LLDP Neighbors"),
-        'bgp-rib': (bgp_rib, "BGP RIB"),
+        "bgp-peers": (bgp_peers, "BGP Peers"),
+        "subinterface": (subinterface, "Sub-Interfaces"),
+        "ipv4-rib": (ipv4_rib, "IPv4 RIB"),
+        "mac-table": (mac_table, "MAC Table"),
+        "sys-info": (sys_info, "System Info"),
+        "nwi-itfs": (nwi_itfs, "Network-Instance Interfaces"),
+        "lldp-nbrs": (lldp_nbrs, "LLDP Neighbors"),
+        "bgp-rib": (bgp_rib, "BGP RIB"),
     }
 
     if report not in reports:
-        click.echo(f"Report {report} not found. Available reports: {list(reports.keys())}")
+        click.echo(
+            f"Report {report} not found. Available reports: {list(reports.keys())}"
+        )
         return
     if not field_filter:
         field_filter = {}
     fabric = InitNornir(config_file=cfg)
     if i_filter:
         target = fabric.filter(**i_filter)
     else:
@@ -221,22 +307,20 @@
     title = "[bold]" + reports[report][1] + "[/bold]"
     if f_filter:
         title += "\nFields:" + str(f_filter)
     if i_filter:
         title += "\nInventory:" + str(i_filter)
     if report_options:
         title += "\nReport options:" + str(report_options)
-    if len(target.data.failed_hosts)>0:
+    if len(target.data.failed_hosts) > 0:
         title += "\n[red]Failed hosts:" + str(target.data.failed_hosts)
     print_table(
-            title=title, 
-            resource=result.name, 
-            results=result, 
-            filter=f_filter,
-            box_type=box_type,
-            )
+        title=title,
+        resource=result.name,
+        results=result,
+        filter=f_filter,
+        box_type=box_type,
+    )
 
 
 if __name__ == "__main__":
-     cli()
-
-
+    cli()
```

### Comparing `nornir_srl-0.1.2/nornir_srl/tasks/srl_config.py` & `nornir_srl-0.1.4/nornir_srl/tasks/srl_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,258 +11,269 @@
 from nornir.core.task import Result, Task
 from ruamel.yaml import YAML
 
 from nornir_srl.connections.srlinux import CONNECTION_NAME
 
 from .helpers import _merge
 
+
 def configure_device(
-    task: Task, 
-    intent_path: str, 
+    task: Task,
+    intent_path: str,
     state_path: str,
     backup_path: str,
     dry_run: Optional[bool] = None,
-    **kwargs: Any
-    ) -> Result:
-    '''
+    **kwargs: Any,
+) -> Result:
+    """
     A Nornir task that configures a device from an intent. It is meant to be called via the Nornir.run() method.
-    It runs various sub-tasks to load vars from files, render templates, apply configuration and potentially delete 
+    It runs various sub-tasks to load vars from files, render templates, apply configuration and potentially delete
     configuration in case of purged resources from a previous version of intent.
 
     Args:
     task: A Nornir Task object that holds device details (e.g. connection)
     intent_path: path to the directory that holds the variables (intent)
     state_path: path to the directory to store state (i.e. to prune resourcesvthat are no longer part of the intent)
     backup_path: path to directory to hold config backups
     dry_run: boolean to indicate if this is a dry-run (dry-run == True) (no config changes applied to device)
     kwargs: optional key, value pairs to pass intent vars directly to the task
 
     Returns a Nornir Result object that holds the result of the outcome)
-    '''
+    """
     config_changed = False
 
     r = task.run(
-        name=f"Load vars from {intent_path}", 
+        name=f"Load vars from {intent_path}",
         severity_level=logging.DEBUG,
-        task=load_vars, 
-        path=intent_path 
+        task=load_vars,
+        path=intent_path,
     )
     vars = r.result
 
     r = task.run(
         name="Render templates",
         severity_level=logging.DEBUG,
         task=render_template,
-        base_path = intent_path,
-        **vars
+        base_path=intent_path,
+        **vars,
     )
 
     r = task.run(
         name="Load YAML from template",
         severity_level=logging.DEBUG,
         task=load_yaml,
-        doc=r.result
+        doc=r.result,
     )
     device_intent = r.result
 
     for data in device_intent:
         for set_mode, resources in data.items():
-            if set_mode not in ('update', 'replace'):
+            if set_mode not in ("update", "replace"):
                 raise ValueError(f"Unexpected set_mode: {set_mode}")
             if isinstance(resources, list):
                 r = task.run(
                     name=f"DRY-RUN:{dry_run} {set_mode}:{[list(rsc.keys())[0] for rsc in resources]} to device",
                     severity_level=logging.INFO,
                     task=set_config,
                     device_config=resources,
                     op=set_mode,
                     dry_run=dry_run or task.is_dry_run(override=False),
                 )
                 config_changed |= r.changed
-    
+
     r = task.run(
-        name = "Check for purged resources",
-        severity_level = logging.WARN,
+        name="Check for purged resources",
+        severity_level=logging.WARN,
         task=purge_resources,
-        device_intent = device_intent,
-        state_base_path = state_path,
-        dry_run = dry_run,
+        device_intent=device_intent,
+        state_base_path=state_path,
+        dry_run=dry_run,
     )
     config_changed |= r.changed
 
     if config_changed:
         r = task.run(
             name=f"Backup configs to {backup_path}",
             severity_level=logging.INFO,
-            task = backup_config,
-            backup_base_path = backup_path,
+            task=backup_config,
+            backup_base_path=backup_path,
         )
 
 
 def backup_config(
     task: Task,
     backup_base_path: str,
     history_len: Optional[int] = 10,
 ) -> None:
-
-    p = Path(backup_base_path) 
+    p = Path(backup_base_path)
     suffix = datetime.now().strftime("%Y%m%d%H%M%S")
     p = p / task.host.hostname / f"{task.host.hostname}.{suffix}.json"
     p.parent.mkdir(parents=True, exist_ok=True)
-    
+
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-    cfg = device.get(paths=['/'], datatype="config", strip_mod=True)
+    cfg = device.get(paths=["/"], datatype="config", strip_mod=True)
     p.write_text(json.dumps(cfg, indent=4))
 
     backup_files = sorted(p.parent.glob("*.json"))
     if len(backup_files) > history_len:
         for f in backup_files[history_len:]:
             f.unlink()
 
+
 def restore_config(
     task: Task,
-    backup_base_path: str, 
+    backup_base_path: str,
     version: int,
     dry_run: Optional[bool] = True,
 ) -> Result:
-
     p = Path(backup_base_path)
     p = p / task.host.hostname
-    backup_files = sorted(p.glob("*.json"), reverse = True)
+    backup_files = sorted(p.glob("*.json"), reverse=True)
     if len(backup_files) < version:
-        raise ValueError(f"Version {version} asked but only {len(backup_files)} versions available")
-    p = backup_files[version-1]
+        raise ValueError(
+            f"Version {version} asked but only {len(backup_files)} versions available"
+        )
+    p = backup_files[version - 1]
 
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
     if dry_run:
         diff = ""
-        before_json = json.dumps(device.get(paths=['/'], datatype="config", strip_mod=True), indent=4)
+        before_json = json.dumps(
+            device.get(paths=["/"], datatype="config", strip_mod=True), indent=4
+        )
         after_json = p.read_text()
         for line in difflib.unified_diff(
             before_json.splitlines(keepends=True),
             after_json.splitlines(keepends=True),
             fromfile="before",
-            tofile="after"
+            tofile="after",
         ):
             diff += line
         return Result(host=task.host, result=diff, changed=False)
     else:
-        r = device.set_config(input=json.loads(p.read_text()), op='replace', dry_run=False)
-        return Result(host=task.host, result=r, changed=len(r)>0)
+        r = device.set_config(
+            input=json.loads(p.read_text()), op="replace", dry_run=False
+        )
+        return Result(host=task.host, result=r, changed=len(r) > 0)
 
 
 def purge_resources(
-    task: Task, 
-    device_intent: List[Dict[str, Any]], 
+    task: Task,
+    device_intent: List[Dict[str, Any]],
     state_base_path: str,
     dry_run: Optional[bool] = None,
-    ) -> Result:
-    
+) -> Result:
     new_rsc = dict()
     for l1 in device_intent:
-        if l1.get('update', []):
-            l2 = l1['update']
+        if l1.get("update", []):
+            l2 = l1["update"]
         else:
             l2 = []
-        if l1.get('replace', []):  # might be a dict entry with value None
-            l2 += l1['replace']
+        if l1.get("replace", []):  # might be a dict entry with value None
+            l2 += l1["replace"]
         for d in l2:
-                new_rsc.update(d)
-    
+            new_rsc.update(d)
+
     state_file = Path(state_base_path) / f"{task.host.hostname}.json"
     if state_file.exists():
-        with state_file.open(mode='r') as f:
+        with state_file.open(mode="r") as f:
             state = json.load(f)
-        purged = { k:v for k,v in state.items() if k not in new_rsc }
+        purged = {k: v for k, v in state.items() if k not in new_rsc}
     else:
         purged = {}
     if dry_run:
         changed = False
     else:
         if len(purged) > 0:
             device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
-            purge_config = [ {r: purged[r]} for r in purged.keys()]
-            r = device.set_config(input=purge_config, op='delete', dry_run=dry_run)
+            purge_config = [{r: purged[r]} for r in purged.keys()]
+            r = device.set_config(input=purge_config, op="delete", dry_run=dry_run)
             purged = r
             changed = True
         else:
             changed = False
         state_file.write_text(json.dumps(new_rsc, indent=4))
 
     return Result(host=task.host, result=purged, changed=changed)
 
-def render_template(task: Task, base_path: str, **kwargs: Any) -> Result:
 
+def render_template(task: Task, base_path: str, **kwargs: Any) -> Result:
     p = Path(base_path) / "templates"
-    env = Environment(loader=FileSystemLoader(str(p)), 
-            undefined=StrictUndefined, trim_blocks=True,
-            lstrip_blocks=True,
+    env = Environment(
+        loader=FileSystemLoader(str(p)),
+        undefined=StrictUndefined,
+        trim_blocks=True,
+        lstrip_blocks=True,
     )
     rendered = ""
-    for file in natsorted( t for t in p.glob("*.j2")):
+    for file in natsorted(t for t in p.glob("*.j2")):
         tpl = env.get_template(str(file.parts[-1]))
         txt = tpl.render(host=task.host, **kwargs)
         if len(txt) > 0:
             rendered += f"---\n{txt}"
 
     return Result(host=task.host, result=rendered)
 
+
 def load_yaml(task: Task, doc: str) -> Any:
-    
     yml = YAML(typ="safe")
     result = yml.load_all(doc)
 
     return Result(host=task.host, result=list(result))
-        
-def load_vars(task: Task, path: str, **kwargs: Any) -> Result:
 
+
+def load_vars(task: Task, path: str, **kwargs: Any) -> Result:
     intent = dict()
     intent.update(kwargs)
 
     def _render(matchobj):
         var = matchobj.group(2)
 
         return str(task.host.get(matchobj.group(2)))
 
     p = Path(path)
-    for file in natsorted( [ f for f in p.glob("**/*.y?ml") ] ):
+    for file in natsorted([f for f in p.glob("**/*.y?ml")]):
         yml = YAML(typ="safe")
-        with open(file, 'r') as f:
+        with open(file, "r") as f:
             y_str = f.read()
-        y_str = re.sub(r'(__(\S+))', _render, y_str)
+        y_str = re.sub(r"(__(\S+))", _render, y_str)
         for data in yml.load_all(y_str):
-            if not 'metadata' in data:
+            if not "metadata" in data:
                 continue
-            metadata = data.pop('metadata', {})
+            metadata = data.pop("metadata", {})
             if "hostname" in metadata and task.host.hostname != metadata["hostname"]:
                 continue
-            if "groups" in metadata and len(
-                    [ g for g in task.host.groups 
-                        if str(g) in metadata["groups"] ]
-            ) == 0:
+            if (
+                "groups" in metadata
+                and len([g for g in task.host.groups if str(g) in metadata["groups"]])
+                == 0
+            ):
                 continue
             if "labels" in metadata and len(
-                { k:v for k,v in task.host.extended_data().items()
-                    if metadata["labels"].get(k) == v }
+                {
+                    k: v
+                    for k, v in task.host.extended_data().items()
+                    if metadata["labels"].get(k) == v
+                }
             ) < len(metadata["labels"]):
                 continue
             _merge(intent, data)
-    
+
     return Result(host=task.host, result=intent)
 
+
 def set_config(
-    task: Task, 
-    device_config: List[Dict[str, Any]], 
+    task: Task,
+    device_config: List[Dict[str, Any]],
     dry_run: Optional[bool] = True,
     op: Optional[str] = None,
-    ) -> Result:
-    
+) -> Result:
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
     r = device.set_config(input=device_config, op=op, dry_run=dry_run)
     if dry_run:
-        changed=False
+        changed = False
     else:
         if len(r) > 0:
-            changed=True
+            changed = True
         else:
-            changed=False
+            changed = False
     return Result(host=task.host, result=r, changed=changed)
```

### Comparing `nornir_srl-0.1.2/pyproject.toml` & `nornir_srl-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_srl"
-version = "0.1.2"
+version = "0.1.4"
 description = "Nornir connection plugin for SRLinux"
 authors = ["Walter De Smedt <walter.de.smedt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/wdesmedt/nornir_srl"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -22,15 +22,16 @@
 
 [tool.poetry.plugins."nornir.plugins.connections"]
 "srlinux" = "nornir_srl.connections.srlinux:SrLinux"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 blessings = "^1.7"
-ipython = "^8.12.0"
+black = "^23.3.0"
+mypy = "^0.942"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fcli = 'nornir_srl.fsc:cli'
```

### Comparing `nornir_srl-0.1.2/PKG-INFO` & `nornir_srl-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,16 @@
-Metadata-Version: 2.1
-Name: nornir-srl
-Version: 0.1.2
-Summary: Nornir connection plugin for SRLinux
-Home-page: https://github.com/wdesmedt/nornir_srl
-Author: Walter De Smedt
-Author-email: walter.de.smedt@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: deepdiff (>=6.2.1,<7.0.0)
-Requires-Dist: jmespath (>=1.0.1,<2.0.0)
-Requires-Dist: jsondiff (>=2.0.0,<3.0.0)
-Requires-Dist: natsort (>=8.2.0,<9.0.0)
-Requires-Dist: nornir (>=3.3.0,<4.0.0)
-Requires-Dist: nornir-jinja2 (>=0.2.0,<0.3.0)
-Requires-Dist: nornir-scrapli (>=2022.1.30,<2023.0.0)
-Requires-Dist: nornir-utils (>=0.2.0,<0.3.0)
-Requires-Dist: pygnmi (>=0.8.9,<0.9.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
-Project-URL: Repository, https://github.com/wdesmedt/nornir_srl
-Description-Content-Type: text/markdown
-
 # nornir_srl
-This module provides a [Nornir](https://nornir.readthedocs.io/en/latest/) connection [plugin](https://nornir.tech/nornir/plugins/) for Nokia SRLinux devices. It uses the gNMI management interface of SRLinux to fetch state and push configurations.
+This module provides a [Nornir](https://nornir.readthedocs.io/en/latest/) connection [plugin](https://nornir.tech/nornir/plugins/) for Nokia SRLinux devices. It uses the gNMI management interface of SRLinux to fetch state and push configurations and the [PyGNMI](https://github.com/akarneliuk/pygnmi) Python module to interact with gNMI. 
+
+Rather than limiting the connection plugin to primitives like `open_connection`, `close_connection`, `get`, `set`, etc, this module provides also methods to get information from the device for common resources. Since the device model tends to change between releases, it was considered a better approach to provide this functionality as part of the connection plugin and hide complexity of model changes to the user or Nornir tasks. 
+
+In addition to the connection plugin, there is a set of Nornir tasks that use the connection plugin to perform common operations on the device, like get BGP peers, get MAC table, get subinterfaces, etc. These Nornir tasks are called by a command-line interface `fcli` that provides a network-wide CLI to perform show commands across an entire set or subset for SRLinux nodes.
 
 The current functionality is focused on a read-only _network-wide CLI_ to perform show commands across an entire set or subset for SRLinux nodes, as defined in the Nornir inventory and through command-line filter options. It shows output in a tabular format for easy reading.
-Following versions will focus on configuration management and command execution on the nodes.
+Following versions may focus on configuration management and command execution on the nodes.
 
 # Prerequisites
 
 This module requires [Nornir Core](https://github.com/nornir-automation/nornir) that includes the Nornir core components for which this module is an add-on.
 Nornir needs a [configuration file](https://nornir.readthedocs.io/en/latest/configuration/index.html) to tell it at a minimum where to find the inventory and what inventory plugin is used. Also runner configuration parameters, like #threads/workers for parallel execution are defined here but sane defaults are used.
 
 Since this module is using gNMI as the management inteface, at a minimum, a CA certificate is required that was used to create per-device certs and keys. If you use [Containerlab](https://containerlab.dev/) this root cert is auto-generated for SRLinux nodes and available in the lab subfolder created by the containerlab cli. This file needs to be referenced via the inventory (per-device or per-group). See below for details.
@@ -191,8 +168,7 @@
   clab-4l2s-l2 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  
                │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  
                │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.1   │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  
 ```
 
 
   
-
```

