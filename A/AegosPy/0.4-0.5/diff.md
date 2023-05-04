# Comparing `tmp/AegosPy-0.4.tar.gz` & `tmp/AegosPy-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AegosPy-0.4.tar", last modified: Thu May  4 07:46:41 2023, max compression
+gzip compressed data, was "AegosPy-0.5.tar", last modified: Thu May  4 08:49:15 2023, max compression
```

## Comparing `AegosPy-0.4.tar` & `AegosPy-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:46:41.469097 AegosPy-0.4/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:46:41.403411 AegosPy-0.4/AegosPy/
--rw-rw-rw-   0        0        0    29934 2023-05-04 07:38:54.000000 AegosPy-0.4/AegosPy/AegosPy.py
--rw-rw-rw-   0        0        0      393 2023-05-04 07:46:04.000000 AegosPy-0.4/AegosPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:46:41.460120 AegosPy-0.4/AegosPy.egg-info/
--rw-rw-rw-   0        0        0      277 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2023-05-04 07:46:41.465107 AegosPy-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-04 07:46:41.470095 AegosPy-0.4/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-05-04 07:46:25.000000 AegosPy-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:49:15.919464 AegosPy-0.5/
+drwxrwxrwx   0        0        0        0 2023-05-04 08:49:15.867007 AegosPy-0.5/AegosPy/
+-rw-rw-rw-   0        0        0    36083 2023-05-04 08:48:05.000000 AegosPy-0.5/AegosPy/AegosPy.py
+-rw-rw-rw-   0        0        0      353 2023-05-04 08:48:24.000000 AegosPy-0.5/AegosPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:49:15.911535 AegosPy-0.5/AegosPy.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-05-04 08:49:15.000000 AegosPy-0.5/AegosPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-04 08:49:15.000000 AegosPy-0.5/AegosPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 08:49:15.000000 AegosPy-0.5/AegosPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 08:49:15.000000 AegosPy-0.5/AegosPy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-05-04 08:49:15.000000 AegosPy-0.5/AegosPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      277 2023-05-04 08:49:15.914484 AegosPy-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-04 08:49:15.919464 AegosPy-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-05-04 08:48:45.000000 AegosPy-0.5/setup.py
```

### Comparing `AegosPy-0.4/AegosPy/AegosPy.py` & `AegosPy-0.5/AegosPy/AegosPy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-import json , requests , time , os , re , json
-from rich import print_json
+import json , requests , os , re , json , random
 from OneClick import Hunter
 hd = str(Hunter.Services())
 from uuid import uuid4
 ud = str(uuid4())
 from user_agent import generate_user_agent
 gd = str(generate_user_agent())
-addlist=[]
-addlist2=[]
-addlist3=[]
 def A_Gmail(email):
     url = 'https://android.clients.google.com/setup/checkavail'
     headers = {
         'Content-Length':'98',
 		'Content-Type':'text/plain; charset=UTF-8',
 		'Host':'android.clients.google.com',
 		'Connection':'Keep-Alive',
@@ -258,15 +254,15 @@
 	    }
         u5 = 'https://i.instagram.com/api/v1/accounts/send_password_reset/'
         r6 = requests.post(u5,headers=hd5,data=d5).json()
         f7 = r6['obfuscated_email']
         return {'result':'true','user':'true','name':f1,'id':f2,'followers':f3,'following':f4,'posts':f5,'date':f6,'reset':f7,'Tele':'@G_4_2'}
     except KeyError:
         return {'result':'true','user':'true','name':f1,'id':f2,'followers':f3,'following':f4,'posts':f5,'date':f6,'reset':'false','Tele':'@G_4_2'}
-def GetListInsta_FG(n5,sessionid):
+#def GetListInsta_FG(n5,sessionid):
     try:
         u6 = f'https://i.instagram.com/api/v1/users/web_profile_info/?username={n5}'
         hd6 = {
             'accept': '*/*',
             'accept-encoding': 'gzip, deflate, br',
             'accept-language': 'en-US,en;q=0.9',
             'cookie': f'mid=Y3bGYwALAAHNwaKANMB8QCsRu7VA; ig_did=092BD3C7-0BB2-414B-9F43-3170EAED8778; ig_nrcb=1; shbid=1685054; shbts=1675191368.6684434090; rur=CLN; ig_direct_region_hint=ATN; csrftoken=gLlFX76z8qqwDgmh8ZIp3uFhAeX4zKdO; ds_user_id=921803283; sessionid={sessionid}',
@@ -313,43 +309,40 @@
         if str('"has_next_page":false,') in r8.text:
             try:
                 nu = json.loads(r8.text)['data']['user']['edge_follow']['edges']
                 if nu == '[]':
                     return {'Status':'False','Sessionid':'False'}
                 for ns in nu:
                     n6 = str(ns["node"]["username"])
-                    addlist.append(n6)
                 pass
             except KeyboardInterrupt:
                 pass
         else:
             if aegos22 != 0:
                 try:
                     end = re.findall(',"end_cursor":"(.*)"},"edges":', r8.text)
                     r8 = requests.get('https://www.instagram.com/graphql/query/?query_hash=d04b0a864b4b54837c0d870b0e77e076&variables={"id":"'+str(id)+'","include_reel":true,"fetch_mutual":false,"first":50,"after":"'+end[0]+'"}',headers=hd7,cookies=s1)
                     try:
                         nu = json.loads(r8.text)['data']['user']['edge_follow']['edges']
                     except KeyboardInterrupt:
                         pass
                     for ns in nu:
                         n6 = str(ns["node"]["username"])
-                        addlist.append(n6)
                 except KeyboardInterrupt:
                     pass
             else:
                 try:
                     nu = json.loads(r8.text)['data']['user']['edge_follow']['edges']
                     for ns in nu:
                         n6 = str(ns["node"]["username"])
-                        addlist.append(n6)
                     return {'Status':'Ok','Users':nu}
                 except KeyboardInterrupt:
                     pass
                 aegos22 += 1
-def GetListInsta_FS(n5,sessionid):
+#def GetListInsta_FS(n5,sessionid):
     try:
         u6 = f'https://i.instagram.com/api/v1/users/web_profile_info/?username={n5}'
         hd6 = {
             'accept': '*/*',
             'accept-encoding': 'gzip, deflate, br',
             'accept-language': 'en-US,en;q=0.9',
             'cookie': f'mid=Y3bGYwALAAHNwaKANMB8QCsRu7VA; ig_did=092BD3C7-0BB2-414B-9F43-3170EAED8778; ig_nrcb=1; shbid=1685054; shbts=1675191368.6684434090; rur=CLN; ig_direct_region_hint=ATN; csrftoken=gLlFX76z8qqwDgmh8ZIp3uFhAeX4zKdO; ds_user_id=921803283; sessionid={sessionid}',
@@ -396,42 +389,40 @@
         if str('"has_next_page":false,') in r8.text:
             try:
                 nu = json.loads(r8.text)["data"]["user"]["edge_followed_by"]["edges"]
                 if nu == '[]':
                     return {'Status':'False','Sessionid':'False'}
                 for ns in nu:
                     n6 = str(ns["node"]["username"])
-                    addlist.append(n6)
                 pass
             except KeyboardInterrupt:
                 pass
         else:
             if aegos22 != 0:
                 try:
                     end = re.findall(',"end_cursor":"(.*)"},"edges":', r8.text)
                     r8 = requests.get('https://www.instagram.com/graphql/query/?query_hash=c76146de99bb02f6415203be841dd25a&variables={"id":"'+str(id)+'","include_reel":true,"fetch_mutual":true,"first":50,"after":"'+end[0]+'"}|',headers=hd7,cookies=s1)
                     try:
                         nu = json.loads(r8.text)["data"]["user"]["edge_followed_by"]["edges"]
                     except KeyboardInterrupt:
                         pass
                     for ns in nu:
                         n6 = str(ns["node"]["username"])
-                        addlist.append(n6)
                 except KeyboardInterrupt:
                     pass
             else:
                 try:
                     nu = json.loads(r8.text)["data"]["user"]["edge_followed_by"]["edges"]
                     for ns in nu:
                         n6 = str(ns["node"]["username"])
-                        addlist.append(n6)
-                    return {'Status':'Ok','Users':nu}
+                    
                 except KeyboardInterrupt:
                     pass
                 aegos22 += 1
+                return {'Status':'Ok','Users':nu}
 lii = 0
 pp = 0
 def GetListTik_FG(user):
     global lii,pp
     r = requests.get(f'https://www.tiktok.com/@{user}').text
     k = str(r.split('"UserModule":')[1]).split('"RecommendUserList"')[0]
     s = str(k.split('secUid":"')[1]).split('"')[0]
@@ -458,8 +449,35 @@
     rt = requests.get(f'https://www.tiktok.com/api/user/list/?aid=1988&app_language=ar&app_name=tiktok_web&battery_info=0.88&browser_language=ar-EG&browser_name=Mozilla&browser_online=true&browser_platform=Linux%20aarch64&browser_version=5.0%20%28Linux%3B%20Android%2010%3B%20Infinix%20X690B%29%20AppleWebKit%2F537.36%20%28KHTML%2C%20like%20Gecko%29%20Chrome%2F112.0.0.0%20Mobile%20Safari%2F537.36&channel=tiktok_web&cookie_enabled=true&count=200&device_id=7227896390197003781&device_platform=web_mobile&focus_state=true&from_page=user&history_len=6&is_fullscreen=false&is_page_visible=true&maxCursor=0&minCursor=0&os=android&priority_region=&referer=https%3A%2F%2Fwww.tiktok.com%2Flogin%3Fenter_from%3Dhomepage_hot%26lang%3Dar%26redirect_url%3Dhttps%253A%252F%252Fwww.tiktok.com%252Fforyou%253Fitem_id%253D7216022215656262917&region=IQ&root_referer=https%3A%2F%2Fwww.google.com%2F&scene=21&screen_height=820&screen_width=360&secUid={s}&tz_name=Asia%2FBaghdad&verifyFp=verify_lh3ospm9_Reu7fKhn_mc4D_4qqD_BFQ3_dphns44cCPKG&webcast_language=ar',headers=h).json()['userList']
     g = 0
     for gt in rt:
         try:
             g+=1
         except IndexError:
             exit()
-    return{'status':'ok','users':rt}
+    return{'status':'ok','users':rt}
+def GetListTik_RM():
+    url = 'https://www.tiktok.com/'
+    headers = {'user-agent':str(generate_user_agent())}
+    resp = requests.get(url,headers=headers).cookies.get_dict()
+    tw = resp['ttwid']
+    resp = requests.get(f'https://www.tiktok.com/api/search/user/full/?aid=1988&app_language=en&app_name=tiktok_web&battery_info=0.95&browser_language=en-US&browser_name=Mozilla&browser_online=true&browser_platform=Win32&browser_version=5.0%20%28Windows%20NT%2010.0%3B%20Win64%3B%20x64%29%20AppleWebKit%2F537.36%20%28KHTML%2C%20like%20Gecko%29%20Chrome%2F112.0.0.0%20Safari%2F537.36%20Edg%2F112.0.1722.58&channel=tiktok_web&cookie_enabled=true&cursor=0&device_id=7167133500737406469&device_platform=web_pc&focus_state=true&from_page=search&history_len=12&is_fullscreen=false&is_page_visible=true&keyword=Ahmed&os=windows&priority_region=&referer=&region=IQ&screen_height=864&screen_width=1536&tz_name=Asia%2FBaghdad&webcast_language=en&msToken=Jh2Un0eoRktVfI93pGX8cCnjRORmfpHcdVk3CX3iFej0oFwd4KkZbjtj4gVtMIcKhXsdNszAv59W5Hv4B1uqr4MEN1QLpDdyPbK0H_5XQxUIeebrnEz3m3lWx7RqYD-vYc_r2dD4dSnBoCz07w==&X-Bogus=DFSzswVLKvhANe8ktehWvBesEu3F&_signature=_02B4Z6wo00001nxbdaQAAIDD9Q7cROrxgA58W3EAAPti03',headers=headers)
+    ms = resp.cookies.get_dict()['msToken']
+    chars = 'qwertyuiopasdfghjklzxcvbnm'
+    numbers = '12345'
+    ch_nu = int(''.join(random.choice(numbers) for i in range(1)))
+    ch_ch = str(''.join(random.choice(chars) for i in range(ch_nu)))
+    url2 = f'https://www.tiktok.com/api/search/user/full/?aid=1988&app_language=en&app_name=tiktok_web&battery_info=0.97&browser_language=en-US&browser_name=Mozilla&browser_online=true&browser_platform=Win32&browser_version=5.0%20%28Windows%20NT%2010.0%3B%20Win64%3B%20x64%29%20AppleWebKit%2F537.36%20%28KHTML%2C%20like%20Gecko%29%20Chrome%2F112.0.0.0%20Safari%2F537.36%20Edg%2F112.0.1722.58&channel=tiktok_web&cookie_enabled=true&cursor=0&device_id=7167133500737406469&device_platform=web_pc&focus_state=true&from_page=search&history_len=7&is_fullscreen=false&is_page_visible=true&keyword={ch_ch}&os=windows&priority_region=&referer=&region=IQ&screen_height=864&screen_width=1536&tz_name=Asia%2FBaghdad&verifyFp=verify_lgwmfhzk_e7prK74z_FrTN_4Bjb_9Qcm_PfCyiV29qUyq&webcast_language=en&msToken=GSw6qQneGxQwgJwO_ohDdJtIP-zDkOo_Z8c7RBM8klCYf5kd0iMyt5XK1c7qGJyB_Upb5HOHG3ZV7QNTpeO65HSAiTexDNGrD9NOKrbJTBGaRMG-EnLCp7bVAeTRUjbq_uruufqqDbUVOH7bxg==&X-Bogus=DFSzswVL9VvANe8kterLuPesEu3p&_signature=_02B4Z6wo00001ycn0EQAAIDCrnJ5pIWNJdcnJ9TAAK2M63'
+    headers2 = {
+        'accept': '*/*',
+        'accept-language':'ar-AE,ar-IQ;q=0.9,ar;q=0.8,en-US;q=0.7,en;q=0.6',
+        'cookie':'passport_csrf_token=446c23e1b656077bd01b1f379ff01c64; passport_csrf_token_default=446c23e1b656077bd01b1f379ff01c64; tiktok_webapp_theme=dark; cookie-consent={"ga":true,"af":true,"fbp":true,"lip":true,"bing":true,"ttads":true,"reddit":true,"version":"v8"}; _ttp=2HZr0KnJ2pqKwJRyQ8myJ28Lpa8; __tea_cache_tokens_1988={"user_unique_id":"7160599742786815489","timestamp":1667850947815,"_type_":"default"}; passport_auth_status=c8fe9febc06f8f7a271309fa9e4f80e9,; passport_auth_status_ss=c8fe9febc06f8f7a271309fa9e4f80e9,; tt_csrf_token=CSVYu9wW-NbmqJ_cgNMHwEIItUNZGwDPM-hU; tt_chain_token=K01fXiH8q/IKwxFnx8jzcA==; _abck=951F354EE38142028A7429E8C92DB598~0~YAAQVvvOF6YBsxSFAQAAMc+wPgl24s0qz4P3iMup3WLL4PWyu/iF6+jb4qL2RfvMEKOGTv6dPfAH9AA2Hm+t/Z/Qn1TlkKHzKXk+KmuWj5d1dmCzqXD0BWgAUcMFCLRinQHou0lzh0ImXOw3B98dRIVnofWMwN8L8JxOErAxrQfi2JIEgTjNECxiZFYaqhpfLqyAUXBESaQxfCYfbNwLNwAAZvjpAfc1viGc/I9vlRIeVc2jYPA5/YUVwAytWPIOb2RuvdrXc2bfybwD3ffG0godURyE+r0QSJapjZK7kfVwbPGnVLal0dzAQM6MK2iDC5YhXugMYw9ZXB2CIaYRg4Cqy/t6BabKM9i+ZJgdvwWQQ6ljnk0pa1bKBsAYL79BxNMrQWccpQxQhUm9n09604O82PBKq8E=~-1~-1~-1; bm_sz=304AE404FA2929B0E90042E8314D20CA~YAAQVvvOF6kBsxSFAQAAMc+wPhIfC1eYkaU2YudlghSK8pNrkVcLYapeM/xrzvQbQkT9quFNwKNHsG4xkv6anwuDXn+BSd+gzoBWSdRZJscGEzPghGpbTStjyG61DtaJIqpkgjW7q6BEP37XgXgrWfHRdmoN5zraADDH7wpkIQ3UlBq5rj88cFl1IY4CUg2DSRugvtjKk+vcNV5AUjQ++v859Tv3vYF3Ga6m5lifIf0u50u/dC1xeVz0p4ew+7U21dwrDdNrai63bM7T9ArdMNk1q+2YK55FJU7tdQwtKtdLtnI=~4407620~4277556; ak_bmsc=EE17F7D340A941EB628DF68B5981EA8D~000000000000000000000000000000~YAAQVvvOF/8BsxSFAQAAS/SwPhJbeUd2XpuVnfaiGo9WDUNsMw3AUn4T4r4BtvFH6pwejSxQJ/K4aoQUK/hGU8InWjW8iSyWgKZxkNIl6lgAAvUdX8CiKcyfyQKJYfQcPDyxW6dnF6+VF2/BABsRcYTw9LUX6MjuhvgtLs1uh3AbWeHxdZFDhp/YYwjrPxoOEXgItQjGUSsxRhgRubItrsXwhW20gW9y+I7Eq22TORlAZOn+jyrl2bYH6C4yxD8yld+5OcSAQ3zKJfQLUjNj03BMgtlIyYT74OIh6GwUzgtjpGLUCzpqdeiOFZdfZApTnRoTK9J01CpUY+YxrThJKz4dScjK1V78LSd2CkfUakgFa7TXfZ1fgfPX/RW2nkWTe9SZtvDH3f62qd9b5oNojffOAM0fpnNeX06hNWSNDRRuiHOmv3m49PN2cJhknh753LdNdt81kj8LJ3SEe1y3sfHb0nPwafPExOaSSrXviHwj4+yLWrZw+dXy3Q==; sid_guard=5d52768f6a4a876314ea37244edfd0d0|1671794088|21600|Fri,+23-Dec-2022+17:14:48+GMT; uid_tt=9392403db19bcfc1eb8eb48532fd8d5e; uid_tt_ss=9392403db19bcfc1eb8eb48532fd8d5e; sid_tt=5d52768f6a4a876314ea37244edfd0d0; sessionid=5d52768f6a4a876314ea37244edfd0d0; sessionid_ss=5d52768f6a4a876314ea37244edfd0d0; sid_ucp_v1=1.0.0-KDM1ZGU2ODk4YzcyNDJkMzUxNWRiMTVlMzc3OTMyZTNlY2JlYWYwYWMKCRCom5adBhizCxADGgZtYWxpdmEiIDVkNTI3NjhmNmE0YTg3NjMxNGVhMzcyNDRlZGZkMGQw; ssid_ucp_v1=1.0.0-KDM1ZGU2ODk4YzcyNDJkMzUxNWRiMTVlMzc3OTMyZTNlY2JlYWYwYWMKCRCom5adBhizCxADGgZtYWxpdmEiIDVkNTI3NjhmNmE0YTg3NjMxNGVhMzcyNDRlZGZkMGQw; bm_sv=F556D2E15739C190D1B417337724D81E~YAAQVvvOF8ACsxSFAQAAaICxPhJ1QOpVK0jJSh0nuEay3Iz+L/0up1OoP09MVnndgBSzTjunJoYxBBQH4BTuDkQIQY+zt9kedbGoP5/7AUt2jVEq7DfEwQYdr31ZvZiHlhdU2Q5jwNvbZvNzQSokkwHoGbPqes9c4kV0ZGJuEuWc3pLurp0dkRkEBTY0UrcljYpQayw5/w7+4BlpmrMR5UAHElAGf2njGNpz3vRls+WGkTy9l8jRTCEseWkwnA9X~1; ttwid='+tw+'; odin_tt=70015f10b12827e4d2b9cce32ead78da9bd1f5af11487a83ba408d86d9a4fb55ec780a14ad91b601d9fe256fcb8160786311c12ef294e6bf285fbbf7eed8dff8080f26ed1bcedbdfca7244743dcbc60e; msToken='+ms+'; msToken='+ms+'; s_v_web_id=verify_lc0f2h1w_v9MWasYr_Uw4b_4j2o_8gdZ_QkWrSxI57MTt',
+        'referer': 'https://www.tiktok.com/search/user?q=its.veba&t=1671705430400',
+        'sec-ch-ua': '"Chromium";v="107", "Not=A?Brand";v="24"',
+        'sec-ch-ua-mobile': '?0',
+        'sec-ch-ua-platform': '"Linux"',
+        'sec-fetch-dest': 'empty',
+        'sec-fetch-mode': 'cors',
+        'sec-fetch-site': 'same-origin',
+        'user-agent': 'Mozilla/5.0 (Linux; Android 12; SM-A025F) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Mobile Safari/537.36'
+    }
+    resp2 = requests.get(url2,headers=headers2).json()['user_list']
+    return {'status':'ok','users':resp2}
```

