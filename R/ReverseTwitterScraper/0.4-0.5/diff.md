# Comparing `tmp/ReverseTwitterScraper-0.4.tar.gz` & `tmp/ReverseTwitterScraper-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseTwitterScraper-0.4.tar", last modified: Mon Mar 27 18:54:23 2023, max compression
+gzip compressed data, was "ReverseTwitterScraper-0.5.tar", last modified: Thu May  4 15:27:20 2023, max compression
```

## Comparing `ReverseTwitterScraper-0.4.tar` & `ReverseTwitterScraper-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 18:54:23.825350 ReverseTwitterScraper-0.4/
--rw-rw-rw-   0        0        0     1090 2023-03-08 21:13:40.000000 ReverseTwitterScraper-0.4/LICENSE
--rw-rw-rw-   0        0        0     6754 2023-03-27 18:54:23.824850 ReverseTwitterScraper-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6259 2023-03-14 21:16:57.000000 ReverseTwitterScraper-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 18:54:23.804846 ReverseTwitterScraper-0.4/ReverseTwitterScraper/
--rw-rw-rw-   0        0        0    17561 2023-03-27 18:52:49.000000 ReverseTwitterScraper-0.4/ReverseTwitterScraper/Scraper.py
--rw-rw-rw-   0        0        0       37 2023-03-09 02:04:31.000000 ReverseTwitterScraper-0.4/ReverseTwitterScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 18:54:23.823850 ReverseTwitterScraper-0.4/ReverseTwitterScraper.egg-info/
--rw-rw-rw-   0        0        0     6754 2023-03-27 18:54:23.000000 ReverseTwitterScraper-0.4/ReverseTwitterScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-03-27 18:54:23.000000 ReverseTwitterScraper-0.4/ReverseTwitterScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 18:54:23.000000 ReverseTwitterScraper-0.4/ReverseTwitterScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-27 18:54:23.000000 ReverseTwitterScraper-0.4/ReverseTwitterScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-27 18:54:23.000000 ReverseTwitterScraper-0.4/ReverseTwitterScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 18:54:23.825850 ReverseTwitterScraper-0.4/setup.cfg
--rw-rw-rw-   0        0        0      840 2023-03-27 18:53:56.000000 ReverseTwitterScraper-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:27:20.936016 ReverseTwitterScraper-0.5/
+-rw-rw-rw-   0        0        0     1090 2023-03-08 21:13:40.000000 ReverseTwitterScraper-0.5/LICENSE
+-rw-rw-rw-   0        0        0     7671 2023-05-04 15:27:20.935516 ReverseTwitterScraper-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7176 2023-05-04 15:26:42.000000 ReverseTwitterScraper-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 15:27:20.910510 ReverseTwitterScraper-0.5/ReverseTwitterScraper/
+-rw-rw-rw-   0        0        0    20330 2023-05-04 15:21:46.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper/Scraper.py
+-rw-rw-rw-   0        0        0       37 2023-03-09 02:04:31.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:27:20.934014 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/
+-rw-rw-rw-   0        0        0     7671 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 15:27:20.936016 ReverseTwitterScraper-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-05-04 15:26:31.000000 ReverseTwitterScraper-0.5/setup.py
```

### Comparing `ReverseTwitterScraper-0.4/LICENSE` & `ReverseTwitterScraper-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseTwitterScraper-0.4/PKG-INFO` & `ReverseTwitterScraper-0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-Metadata-Version: 2.1
-Name: ReverseTwitterScraper
-Version: 0.4
-Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
-Home-page: https://github.com/1220moritz/reverse-twitter-scraper
-Author: 1220moritz
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ReverseTwitterScraper
-ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and Requests module to scrape tweets.
+ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and httpx to scrape tweets and other account data.
 
 ## Links
 GitHub: https://github.com/1220moritz/reverse-twitter-scraper  
 PyPI: https://pypi.org/project/ReverseTwitterScraper/
 
 ## Installation
 To install the package, simply run the following command:
@@ -37,40 +24,38 @@
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
 cookies = ""
 timeout = 5
 proxy_list = []
 
 # single account
-twitter_handle = "elonmusk"
-scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, timeout, proxy_list)
-tweets = scraper.getAllTweetsText()
+twitter_handle = ["elonmusk"]
+scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
+tweets = scraper.getTweetsText()
 
 # multiple accounts
 twitter_handles = ["elonmusk", "POTUS", "latestinspace"]
-scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, timeout, proxy_list)
-tweets = scraper.getTweetsTextMultiple()
+scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, proxy_list)
+tweets = scraper.getTweetsText()
 
 print(tweets)
 ```
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
-Finally, we call the getAllTweetsText() method to get the tweets of the specified Twitter account.
+Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
 
 ## Parameters
 The TwitterScraper class takes the following parameters:
 
-- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to elonmusk.
+- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
 
 - chromedriverPath: The path of the Chrome driver executable file. This file is required to use the Selenium module.
 
 - cookies: (Optional) The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
 
-- timeout: (Optional) The time (in seconds) to wait for the page to load. The default value is 5 seconds.
-
 - proxyList: (Optional) A list of proxies to use for scraping. The list should contain proxy addresses in the format ip:port:user:pw.
 
 
 ## How to get account cookies:
 Following a private "target" account is necessary to access its data. Then, account cookies can be used to scrape the account.
 1. Open the Chrome browser and go to the Twitter website.
 2. If you're not already logged in, log in to your Twitter account.
@@ -81,74 +66,76 @@
 7. In your Python code, create a new instance of the TwitterScraper class and paste the cookie value as the value of the "cookies" parameter.
 8. That's it! You can now use the TwitterScraper class to scrape data from your Twitter account.  
 
 By following these steps, you should be able to retrieve the necessary cookies from your Twitter account and use them in your Python code to scrape data.
 
 ## Methodes:
 
-### getTweetsPlainMultiple()
-      this is only if you want to scrape multiple twitter acccounts
+## get twitter data
+### getUserPlain()
+      get all (unfiltered) data from every account in your handle list ("unnecessary" data and ads included)
+      returns [{"handle": handle1, "id": id1, "resp": data1}, {"handle": handle2, "id": id2, "resp": data2},]
+
+### getTweetsPlain()
       get all (unfiltered) tweets from every account in your handle list (unnecessary data and ads included)
+      returns [{"handle": handle1, "id": id1, "resp": {1}}, {"handle": handle2, "id": id2, "resp": {2}}]
      
-### getTweetsTextMultiple()
-      this is only if you want to scrape multiple twitter acccounts
+### getTweetsText()
       get text from all tweets from every account in your handle list
+      returns [{'entryId': entryId1, 'retweet': retweet1, 'text': text1}, {'entryId': entryId2, 'retweet': retweet2, 'text': text2}]
 
-### getAllAccData()
-      returns all (unfiltered) data for the account
-
-### getRetweetInfo(singlePlainTweet, getRetweetInfo=False):
-        checks if the tweet is a retweet (returns True/False/TweetInfo)
 
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+## filter Tweet data
+### filterRetweetInfo(singlePlainTweet, getRetweetInfo=False):
+        checks if the tweet is a retweet (returns True, False or the TweetInfo (if you use getRetweetInfo=True))
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         :param getRetweetInfo: default=False -> get all info about the retweetet tweet
-        
-### getAllTweetsPlain()
-      get all tweets from an account (unnecessary data included)
-
-
-### getAllTweetsText()
-      get a dict with text, tweetID and retweetInfo from all tweets from an account
       
-### getCreatedAt(singlePlainTweet)
+### filterTweetCreatedAt(singlePlainTweet)
     returns createTimeDate of a tweet
-    :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+    :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getID(singlePlainTweet)
+### filterTweetID(singlePlainTweet)
         returns the ID of a tweet
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getRetweetCount(singlePlainTweet)
+### filterRetweetCount(singlePlainTweet)
         returns how many times the tweet has been retweeted
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getReplyCount( singlePlainTweet)
+### filterReplyCount( singlePlainTweet)
         returns how many replies the tweet has
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getViews(singlePlainTweet)
+### filterViews(singlePlainTweet)
         returns how many views the tweet has
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getPinnedTweetInfo()
+
+## filter Account data
+### filterPinnedTweetInfo(singleUserPlain)
         returns all (unfiltered) information about the pinned tweet
+		:param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### isBusinessAccount()
+### filterIsBusinessAccount(singleUserPlain)
         returns if the account is a business account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### hasNftAvatar()
-        returns if the account has an NFT avatar
-
-### userID()
-        returns the userID of the account
+### filterUserID(singleUserPlain)
+        returns the id of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### isBlueVerified()
+### filterIsBlueVerified(singleUserPlain)
         returns if the account is verified with a twitter blue check
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### createdAt()
+### filterAccountCreationDate(singleUserPlain)
         returns the creation time of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### description()
+### filterDescription(singleUserPlain)
         returns the description of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### getAllUserData()
+### getUserSpecificData(singleUserPlain)
         returns all (unfiltered) data about an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
```

### Comparing `ReverseTwitterScraper-0.4/README.md` & `ReverseTwitterScraper-0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+Metadata-Version: 2.1
+Name: ReverseTwitterScraper
+Version: 0.5
+Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
+Home-page: https://github.com/1220moritz/reverse-twitter-scraper
+Author: 1220moritz
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ReverseTwitterScraper
-ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and Requests module to scrape tweets.
+ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and httpx to scrape tweets and other account data.
 
 ## Links
 GitHub: https://github.com/1220moritz/reverse-twitter-scraper  
 PyPI: https://pypi.org/project/ReverseTwitterScraper/
 
 ## Installation
 To install the package, simply run the following command:
@@ -24,40 +37,38 @@
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
 cookies = ""
 timeout = 5
 proxy_list = []
 
 # single account
-twitter_handle = "elonmusk"
-scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, timeout, proxy_list)
-tweets = scraper.getAllTweetsText()
+twitter_handle = ["elonmusk"]
+scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
+tweets = scraper.getTweetsText()
 
 # multiple accounts
 twitter_handles = ["elonmusk", "POTUS", "latestinspace"]
-scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, timeout, proxy_list)
-tweets = scraper.getTweetsTextMultiple()
+scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, proxy_list)
+tweets = scraper.getTweetsText()
 
 print(tweets)
 ```
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
-Finally, we call the getAllTweetsText() method to get the tweets of the specified Twitter account.
+Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
 
 ## Parameters
 The TwitterScraper class takes the following parameters:
 
-- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to elonmusk.
+- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
 
 - chromedriverPath: The path of the Chrome driver executable file. This file is required to use the Selenium module.
 
 - cookies: (Optional) The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
 
-- timeout: (Optional) The time (in seconds) to wait for the page to load. The default value is 5 seconds.
-
 - proxyList: (Optional) A list of proxies to use for scraping. The list should contain proxy addresses in the format ip:port:user:pw.
 
 
 ## How to get account cookies:
 Following a private "target" account is necessary to access its data. Then, account cookies can be used to scrape the account.
 1. Open the Chrome browser and go to the Twitter website.
 2. If you're not already logged in, log in to your Twitter account.
@@ -68,74 +79,76 @@
 7. In your Python code, create a new instance of the TwitterScraper class and paste the cookie value as the value of the "cookies" parameter.
 8. That's it! You can now use the TwitterScraper class to scrape data from your Twitter account.  
 
 By following these steps, you should be able to retrieve the necessary cookies from your Twitter account and use them in your Python code to scrape data.
 
 ## Methodes:
 
-### getTweetsPlainMultiple()
-      this is only if you want to scrape multiple twitter acccounts
+## get twitter data
+### getUserPlain()
+      get all (unfiltered) data from every account in your handle list ("unnecessary" data and ads included)
+      returns [{"handle": handle1, "id": id1, "resp": data1}, {"handle": handle2, "id": id2, "resp": data2},]
+
+### getTweetsPlain()
       get all (unfiltered) tweets from every account in your handle list (unnecessary data and ads included)
+      returns [{"handle": handle1, "id": id1, "resp": {1}}, {"handle": handle2, "id": id2, "resp": {2}}]
      
-### getTweetsTextMultiple()
-      this is only if you want to scrape multiple twitter acccounts
+### getTweetsText()
       get text from all tweets from every account in your handle list
+      returns [{'entryId': entryId1, 'retweet': retweet1, 'text': text1}, {'entryId': entryId2, 'retweet': retweet2, 'text': text2}]
 
-### getAllAccData()
-      returns all (unfiltered) data for the account
-
-### getRetweetInfo(singlePlainTweet, getRetweetInfo=False):
-        checks if the tweet is a retweet (returns True/False/TweetInfo)
 
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+## filter Tweet data
+### filterRetweetInfo(singlePlainTweet, getRetweetInfo=False):
+        checks if the tweet is a retweet (returns True, False or the TweetInfo (if you use getRetweetInfo=True))
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         :param getRetweetInfo: default=False -> get all info about the retweetet tweet
-        
-### getAllTweetsPlain()
-      get all tweets from an account (unnecessary data included)
-
-
-### getAllTweetsText()
-      get a dict with text, tweetID and retweetInfo from all tweets from an account
       
-### getCreatedAt(singlePlainTweet)
+### filterTweetCreatedAt(singlePlainTweet)
     returns createTimeDate of a tweet
-    :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+    :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getID(singlePlainTweet)
+### filterTweetID(singlePlainTweet)
         returns the ID of a tweet
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getRetweetCount(singlePlainTweet)
+### filterRetweetCount(singlePlainTweet)
         returns how many times the tweet has been retweeted
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getReplyCount( singlePlainTweet)
+### filterReplyCount( singlePlainTweet)
         returns how many replies the tweet has
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getViews(singlePlainTweet)
+### filterViews(singlePlainTweet)
         returns how many views the tweet has
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getPinnedTweetInfo()
+
+## filter Account data
+### filterPinnedTweetInfo(singleUserPlain)
         returns all (unfiltered) information about the pinned tweet
+		:param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### isBusinessAccount()
+### filterIsBusinessAccount(singleUserPlain)
         returns if the account is a business account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### hasNftAvatar()
-        returns if the account has an NFT avatar
-
-### userID()
-        returns the userID of the account
+### filterUserID(singleUserPlain)
+        returns the id of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### isBlueVerified()
+### filterIsBlueVerified(singleUserPlain)
         returns if the account is verified with a twitter blue check
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### createdAt()
+### filterAccountCreationDate(singleUserPlain)
         returns the creation time of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### description()
+### filterDescription(singleUserPlain)
         returns the description of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### getAllUserData()
+### getUserSpecificData(singleUserPlain)
         returns all (unfiltered) data about an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
```

### Comparing `ReverseTwitterScraper-0.4/ReverseTwitterScraper/Scraper.py` & `ReverseTwitterScraper-0.5/ReverseTwitterScraper/Scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 import traceback
 
 import asyncio
-import aiohttp
+import httpx
 from seleniumwire import webdriver
 from selenium.webdriver.chrome.options import Options
-import requests
 
 
 class TwitterScraper:
 
     def cookieDict(self, cookies):
         if type(cookies) == dict:
             pass
@@ -25,389 +24,405 @@
         else:
             exit(
                 f"Twitter | Type: {type(cookies)} is currently unsupported for cookies, if you'd like to see it added please open an issue on Github")
 
         return cookies
 
     def changeProxy(self):
-        if self.proxies:
+        if type(self.proxies) is list and self.__proxyCounter < len(self.proxies) - 1:    #change to next proxy in list
+            return self.proxies[self.__proxyCounter]
+        elif type(self.proxies) is list and self.__proxyCounter >= len(self.proxies) - 1: # restart with first proxy in list
+            self.__proxyCounter = 0
             return self.proxies[self.__proxyCounter]
         else:
             return None
-
-
-    def __init__(self, twitterHandle, chromedriverPath, cookies="", timeout=5, proxyList=""):
+        
+    def __init__(self, twitterHandle: list, chromedriverPath: str, cookies="", proxyList=""):
         """
         makes everything ready to scrape twitter.
 
-        :param str twitterHandle: e.g. https://twitter.com/elonmusk -> handle = elonmusk or array with multiple handles ["elonmusk", "POTUS", "BitcoinMagazine"]
+        :param list twitterHandle: e.g. https://twitter.com/elonmusk -> handle = [elonmusk] or multiple handles ["elonmusk", "POTUS", "BitcoinMagazine"]
         :param str chromedriverPath: e.g. C:/Program Files (x86)/chromedriver.exe
         :param str cookies: your twitter account cookies
-        :param int timeout: default=5, if the page doesn't load in time, upper this value
         :param arr proxyList: your array of proxies. ip:port:user:pw
         """
         self.__twitterHandle = twitterHandle
         self.__chromedriverPath = chromedriverPath
         self.__accCookies = cookies
-        self.__timeout = timeout
 
         # format proxy
         self.__proxyCounter = 0
         if proxyList != "" and proxyList != None:
             self.proxies = []
             for proxy in proxyList:
                 __split = str(proxy).replace("\n", "").split(":")
                 fProxy = {'https': f'http://{__split[2]}:{__split[3]}@{__split[0]}:{__split[1]}'}
                 self.proxies.append(fProxy)
         else:
             self.proxies = None
             
             
         # convert handle to id [{"handle": handle, "id": id]}]
-        self.__multipleHandles = False
-        if isinstance(twitterHandle, list) and len(twitterHandle) > 1:
-            self.__multipleHandles = True
+        if isinstance(twitterHandle, list):
             print("converting twitter-ids", end=" ")
             retries = 0
             while retries < 5:
                 try:
                     self._IDList = asyncio.run(self.__getTwitterIDs())
                     break
                 except Exception as e:
-                    #print(traceback.format_exc())
+                    print(traceback.format_exc())
                     retries = retries + 1
             print("- done")
+        else:
+            raise Exception("twitterHandle must be a list of handles")
                 
 
         # get all the important data to send a request
-        __twitterData = self.getTwitterGuestData(cookies=cookies)
-        self.__headers = __twitterData[0]
-        self.__headersDict = __twitterData[1]
-        self.__cookies = __twitterData[2]
-        self.__reqUrl = __twitterData[3]
-        self.__userID = __twitterData[4]
-
-        self.__session = requests.session()
-        e2 = 0
-        while e2 < 5:
+        retries = 0
+        while retries < 5:
             try:
-                self.__openingResp = self.__session.get(url=self.__reqUrl, headers=self.__headers, cookies=self.__cookies, proxies=self.changeProxy())
+                self.getTwitterGuestData(cookies=cookies)
+                break
+            except:
+                #print(traceback.format_exc())
+                retries += 1
+                self.__proxyCounter += 1
+            
+        retries = 0
+        while retries < 5:
+            try:
+                self.__openingResp = httpx.get(url=self.__reqUrl, headers=self.__headers, cookies=self.__cookies).json()
+                self.__userResp = self.__openingResp['data']['user']['result']['timeline_v2']['timeline']['instructions'][1]['entries'][0]['content']['itemContent']['tweet_results']['result']['core']['user_results']['result']
                 break
             except:
                 #print(traceback.format_exc())
                 print("failed openingResp. Trying again with new proxy")
-                e2 = e2 + 1
-                self.__proxyCounter = self.__proxyCounter + 1
-                __twitterData = self.getTwitterGuestData(cookies=self.__accCookies)
-                self.__headers = __twitterData[0]
-                self.__headersDict = __twitterData[1]
-                self.__cookies = __twitterData[2]
-
-        self.__openingResp = self.__openingResp.json()  # may raise a JsonDecodeError when you get ratelimited
-        self.__userResp = \
-        self.__openingResp['data']['user']['result']['timeline_v2']['timeline']['instructions'][1]['entries'][0]['content']['itemContent']['tweet_results']['result']['core']['user_results']['result']
+                retries += 1
+                self.__proxyCounter += 1
+                self.getTwitterGuestData(cookies=self.__accCookies)
 
-
-    async def __getID(self, handle):
+    async def __getID(self, client: httpx.Client, handle):
         headers = {'content-type': 'application/x-www-form-urlencoded; charset=UTF-8'}
-        async with aiohttp.ClientSession() as s:
-            text = "error-co"
-            data = None
-            while text == "error-co":
-                async with s.post(url="https://tweeterid.com/ajax.php", headers=headers, data=f"input={handle}") as resp:
-                    text = await resp.text()
-                    if text != "error-co":
-                        data = {"handle": handle, "id": text}
-                    else:
-                        time.sleep(0.05)
-            return data
+        text = "error-co"
+        data = None
+        while text == "error-co":
+            resp = await client.post(url="https://tweeterid.com/ajax.php", headers=headers, data=f"input={handle}")
+            text = resp.text
+            if text != "error-co":
+                data = {"handle": handle, "id": text}
+            else:
+                await asyncio.sleep(0.05)
+        return data
 
     async def __getTwitterIDs(self):
+        async with httpx.AsyncClient() as client:
             coroutines = []
             for handle in self.__twitterHandle:
-                coroutines.append(self.__getID(handle))
+                coroutines.append(self.__getID(client, handle))
             info = await asyncio.gather(*coroutines)
+            await client.aclose()
             return info
-                    
-      
-    def getTwitterGuestData(self, cookies, proxySupport=False):
-        if proxySupport:
-            wireOptions = {
-                'proxy': self.proxies
-            }
-        else:
-            wireOptions = None
-
+ 
+    def getTwitterGuestData(self, cookies):
         print("gathering meta-information")
+        self.__resetData() #clear old data
+            
         # get driver
         options = Options()
         options.add_argument("--headless")
         driver = webdriver.Chrome(self.__chromedriverPath, options=options) #headless
-        #driver = webdriver.Chrome(self.__chromedriverPath, seleniumwire_options=wireOptions, options=options) #headless, proxy
         #driver = webdriver.Chrome(self.__chromedriverPath) #window
-
-
-        if self.__multipleHandles:
-            driver.get(f"https://twitter.com/{self.__twitterHandle[0]}")
-        else:
-            driver.get(f"https://twitter.com/{self.__twitterHandle}")
+    
+    
+        driver.get(f"https://twitter.com/{self.__twitterHandle[0]}")
         #time.sleep(self.__timeout)  # sleep to let the twitter page load
-
+        
+        
         headersDict = {}
         for headerReq in driver.requests:
             url = headerReq.url
             if "UserTweets" in url and "cursor" not in url:
-                reqUrl = url
-                userID = url.split("userId%22%3A%22")[1].split("%22%2C%22count%22")[0]
+                self.__reqUrl = url
                 headersDict = dict(headerReq.headers)
         time.sleep(1)
+        
         driver.close()
         
-        headers = {
+        self.__headers = {
             'authorization': headersDict['authorization'],
             'cookie': headersDict['cookie'],
             'user-agent': headersDict['user-agent'],
             'x-csrf-token': headersDict['x-csrf-token'],
             'x-guest-token': headersDict['x-guest-token']
         }
 
         
         # check for cookies
         if cookies != "":
-            # get dummy URL to set cookies
-            driver.get("https://twitter.com")
-            cookies = self.cookieDict(cookies)
-            for key, value in cookies.items():
-                driver.add_cookie({'name': key, 'value': value, "domain": ".twitter.com"})
+            self.__cookies = self.cookieDict(cookies)
         else:
-            cookies = self.cookieDict(headersDict['cookie'])
+            self.__cookies = self.cookieDict(headersDict['cookie'])
         print("Done!")
 
-
-        return headers, headersDict, cookies, reqUrl, userID
-
-    def closeSession(self):
-        self.__session.close()
+    def __resetData(self):
         self.__headers = None
         self.__openingResp = None
         self.__userResp = None
         self.__reqUrl = None
         self.__cookies = None
-        self.proxies = None
-
-    def getAllAccData(self):
-        """
-        returns all (unfiltered) data for the account
-        """
-        return self.__openingResp.json()
+  
+    
+    
     
-    # get Tweet data multiple Accs
-    async def __getTweetsPlainAsync(self, handle, id):
-        e1 = 0
-        while e1 < 5:
+    
+    # get Twitter data methodes
+    ## get user data
+    async def __getUserPlainAsync(self, client: httpx.AsyncClient, handle, id):
+        retries = 0
+        while retries < 5:
             try:
                 urlTwitter = f"https://api.twitter.com/graphql/CkON7wJrKLwEVV59ClcmjA/UserTweets?variables=%7B%22userId%22%3A%22{id}%22%2C%22count%22%3A40%2C%22includePromotedContent%22%3Atrue%2C%22withQuickPromoteEligibilityTweetFields%22%3Atrue%2C%22withSuperFollowsUserFields%22%3Atrue%2C%22withDownvotePerspective%22%3Afalse%2C%22withReactionsMetadata%22%3Afalse%2C%22withReactionsPerspective%22%3Afalse%2C%22withSuperFollowsTweetFields%22%3Atrue%2C%22withVoice%22%3Atrue%2C%22withV2Timeline%22%3Atrue%7D&features=%7B%22responsive_web_twitter_blue_verified_badge_is_enabled%22%3Atrue%2C%22responsive_web_graphql_exclude_directive_enabled%22%3Atrue%2C%22verified_phone_label_enabled%22%3Afalse%2C%22responsive_web_graphql_timeline_navigation_enabled%22%3Atrue%2C%22responsive_web_graphql_skip_user_profile_image_extensions_enabled%22%3Afalse%2C%22tweetypie_unmention_optimization_enabled%22%3Atrue%2C%22vibe_api_enabled%22%3Atrue%2C%22responsive_web_edit_tweet_api_enabled%22%3Atrue%2C%22graphql_is_translatable_rweb_tweet_is_translatable_enabled%22%3Atrue%2C%22view_counts_everywhere_api_enabled%22%3Atrue%2C%22longform_notetweets_consumption_enabled%22%3Atrue%2C%22tweet_awards_web_tipping_enabled%22%3Afalse%2C%22freedom_of_speech_not_reach_fetch_enabled%22%3Afalse%2C%22standardized_nudges_misinfo%22%3Atrue%2C%22tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled%22%3Afalse%2C%22interactive_text_enabled%22%3Atrue%2C%22responsive_web_text_conversations_enabled%22%3Afalse%2C%22longform_notetweets_richtext_consumption_enabled%22%3Afalse%2C%22responsive_web_enhance_cards_enabled%22%3Afalse%7D"
-                async with aiohttp.ClientSession() as s:
-                    async with s.get(urlTwitter, headers=self.__headers) as resp:
-                        data = await resp.json()
-                        data = {"handle": handle, "id": id, "resp": data['data']['user']['result']['timeline_v2']['timeline']['instructions'][1]['entries']}
+                resp = await client.get(urlTwitter, headers=self.__headers)
+                data = resp.json()
+                data = {"handle": handle, "id": id, "resp": data}
+                break
+            except Exception as e:
+                raise Exception(e)
+        return data
+    
+    
+    async def __getUserPlainMain(self):
+        try:
+            async with httpx.AsyncClient(proxies=self.changeProxy()) as client:
+                coroutines = []
+                for data in self._IDList:
+                    coroutines.append(self.__getUserPlainAsync(client, data['handle'], data['id']))
+                info = await asyncio.gather(*coroutines)
+        except Exception as e:
+                raise Exception(e)
+        return info
+    
+    def getUserPlain(self):
+        """
+        get all (unfiltered) data from every account in your handle list ("unnecessary" data and ads included)
+        
+        :return: [{"handle": handle1, "id": id1, "resp": data1}, {"handle": handle2, "id": id2, "resp": data2},]
+        """
+        retries = 0
+        while retries < 5:
+            try:
+                resp = asyncio.run(self.__getUserPlainMain())
                 break
             except:
-                print(traceback.format_exc())
+                #print(traceback.format_exc())
                 print("failed to scrape tweets. Trying again with new data")
-                e1 = e1 + 1
-                self.__proxyCounter = self.__proxyCounter + 1
-                __twitterData = self.getTwitterGuestData(cookies=self.__accCookies)
-                self.__headers = __twitterData[0]
-                self.__headersDict = __twitterData[1]
-                self.__cookies = __twitterData[2]
+                retries += 1
+                self.__proxyCounter += 1
+                self.getTwitterGuestData(cookies=self.__accCookies)
+                
+        return resp
+    
+    ## get twitter data
+    async def __getTweetsPlainAsync(self, client: httpx.AsyncClient, handle, id):
+        retries = 0
+        while retries < 5:
+            try:
+                urlTwitter = f"https://api.twitter.com/graphql/CkON7wJrKLwEVV59ClcmjA/UserTweets?variables=%7B%22userId%22%3A%22{id}%22%2C%22count%22%3A40%2C%22includePromotedContent%22%3Atrue%2C%22withQuickPromoteEligibilityTweetFields%22%3Atrue%2C%22withSuperFollowsUserFields%22%3Atrue%2C%22withDownvotePerspective%22%3Afalse%2C%22withReactionsMetadata%22%3Afalse%2C%22withReactionsPerspective%22%3Afalse%2C%22withSuperFollowsTweetFields%22%3Atrue%2C%22withVoice%22%3Atrue%2C%22withV2Timeline%22%3Atrue%7D&features=%7B%22responsive_web_twitter_blue_verified_badge_is_enabled%22%3Atrue%2C%22responsive_web_graphql_exclude_directive_enabled%22%3Atrue%2C%22verified_phone_label_enabled%22%3Afalse%2C%22responsive_web_graphql_timeline_navigation_enabled%22%3Atrue%2C%22responsive_web_graphql_skip_user_profile_image_extensions_enabled%22%3Afalse%2C%22tweetypie_unmention_optimization_enabled%22%3Atrue%2C%22vibe_api_enabled%22%3Atrue%2C%22responsive_web_edit_tweet_api_enabled%22%3Atrue%2C%22graphql_is_translatable_rweb_tweet_is_translatable_enabled%22%3Atrue%2C%22view_counts_everywhere_api_enabled%22%3Atrue%2C%22longform_notetweets_consumption_enabled%22%3Atrue%2C%22tweet_awards_web_tipping_enabled%22%3Afalse%2C%22freedom_of_speech_not_reach_fetch_enabled%22%3Afalse%2C%22standardized_nudges_misinfo%22%3Atrue%2C%22tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled%22%3Afalse%2C%22interactive_text_enabled%22%3Atrue%2C%22responsive_web_text_conversations_enabled%22%3Afalse%2C%22longform_notetweets_richtext_consumption_enabled%22%3Afalse%2C%22responsive_web_enhance_cards_enabled%22%3Afalse%7D"
+                resp = await client.get(urlTwitter, headers=self.__headers)
+                data = resp.json()
+                data = {"handle": handle, "id": id, "resp": data['data']['user']['result']['timeline_v2']['timeline']['instructions'][1]['entries']}
+                break
+            except Exception as e:
+                raise Exception(e)
         return data
     
     
     async def __getTweetsPlainMain(self):
-        coroutines = []
-        for data in self._IDList:
-            coroutines.append(self.__getTweetsPlainAsync(data['handle'], data['id']))
-        info = await asyncio.gather(*coroutines)
+        try:
+            async with httpx.AsyncClient(proxies=self.changeProxy()) as client:
+                coroutines = []
+                for data in self._IDList:
+                    coroutines.append(self.__getTweetsPlainAsync(client, data['handle'], data['id']))
+                info = await asyncio.gather(*coroutines)
+        except Exception as e:
+                raise Exception(e)
         return info
     
-    def getTweetsPlainMultiple(self):
+    def getTweetsPlain(self):
         """
         get all (unfiltered) tweets from every account in your handle list (unnecessary data and ads included)
         
-        call with asyncio.run(scraper.getTweetsPlainMultiple())
+        :return: [{"handle": handle1, "id": id1, "resp": {1}}, {"handle": handle2, "id": id2, "resp": {2}}]
         """
-        resp = asyncio.run(self.__getTweetsPlainMain())
+        retries = 0
+        while retries < 5:
+            try:
+                resp = asyncio.run(self.__getTweetsPlainMain())
+                break
+            except:
+                #print(traceback.format_exc())
+                print("failed to scrape tweets. Trying again with new data")
+                retries += 1
+                self.__proxyCounter += 1
+                self.getTwitterGuestData(cookies=self.__accCookies)
+                
         return resp
-    
-    def getTweetsTextMultiple(self):
+
+    def getTweetsText(self):
         """
         get text from all tweets from every account in your handle list
+        
+        :return: [{'entryId': entryId1, 'retweet': retweet1, 'text': text1}, {'entryId': entryId2, 'retweet': retweet2, 'text': text2}]
         """
-        resp = asyncio.run(self.__getTweetsPlainMain())
+        retries = 0
+        while retries < 5:
+            try:
+                resp = asyncio.run(self.__getTweetsPlainMain())
+                break
+            except:
+                #print(traceback.format_exc())
+                print("failed to scrape tweets. Trying again with new data")
+                retries += 1
+                self.__proxyCounter += 1
+                self.getTwitterGuestData(cookies=self.__accCookies)
     
         accountTweets = []
         for handle in resp:
             tweets = []
             for tweet in handle['resp']:
                 if "promotedTweet" not in tweet['entryId']:
                     try:
                         tweets.append({
                             'entryId': tweet['entryId'],
-                            'retweet': self.getRetweetInfo(tweet),
+                            'retweet': self.filterRetweetInfo(tweet),
                             'text': tweet['content']['itemContent']['tweet_results']['result']['legacy']['full_text']})
                     except:
                         continue
             accountTweets.append({
                 "handle": handle['handle'],
                 "id": handle['id'],
                 "tweets": tweets
             })
         return accountTweets
+  
     
     
-
-    # get Tweet data
-        
-    def getRetweetInfo(self, singlePlainTweet, getRetweetInfo=False):
+    
+    
+    # filter methodes
+    ## filter Tweet data
+    def filterRetweetInfo(self, singlePlainTweet, getRetweetInfo=False):
         """
-        checks if the tweet is a retweet (returns True/False/TweetInfo)
+        checks if the tweet is a retweet (returns True, False or the TweetInfo (if you use getRetweetInfo=True))
 
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         :param getRetweetInfo: default=False -> get all info about the retweetet tweet
         """
 
         if 'retweeted_status_result' in singlePlainTweet['content']['itemContent']['tweet_results']['result']['legacy']:
             if getRetweetInfo:
                 return singlePlainTweet['content']['itemContent']['tweet_results']['result']['legacy']['retweeted_status_result']
             else:
                 return True
         else:
             return False
-
-    def getTweetsPlain(self):
-        """
-        get all (unfiltered) tweets from an account (unnecessary data included)
-        """
-        e1 = 0
-        while e1 < 5:
-            try:
-                resp = self.__session.get(url=self.__reqUrl, headers=self.__headers, cookies=self.__cookies, proxies=self.changeProxy())
-                jresp = resp.json()['data']['user']['result']['timeline_v2']['timeline']['instructions'][1]['entries']
-                break
-            except:
-                #print(traceback.format_exc())
-                print("failed to scrape tweets. Trying again with new data")
-                e1 = e1 + 1
-                self.__proxyCounter = self.__proxyCounter + 1
-                __twitterData = self.getTwitterGuestData(cookies=self.__accCookies)
-                self.__headers = __twitterData[0]
-                self.__headersDict = __twitterData[1]
-                self.__cookies = __twitterData[2]
-        return jresp
-
-    def getTweetsText(self):
-        """
-        get text from all tweets from an account
-        """
-        resp = self.getTweetsPlain()
-        tweets = []
-        for tweet in resp:
-            if "promotedTweet" not in tweet['entryId']:
-                try:
-                    tweets.append({
-                        'entryId': tweet['entryId'],
-                        'retweet': self.getRetweetInfo(tweet),
-                        'text': tweet['content']['itemContent']['tweet_results']['result']['legacy']['full_text']})
-                except:
-                    continue
-        return tweets
-
-    def getCreatedAt(self, singlePlainTweet):
+        
+    def filterTweetCreatedAt(self, singlePlainTweet):
         """
-        returns createTimeDate of a tweet
+        returns creation date of a tweet
 
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         """
         return singlePlainTweet['content']['itemContent']['tweet_results']['result']['legacy']['created_at']
 
-    def getID(self, singlePlainTweet):
+    def filterTweetID(self, singlePlainTweet):
         """
         returns the ID of a tweet
 
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         """
         return singlePlainTweet['content']['itemContent']['tweet_results']['result']['legacy']['id_str']
 
-    def getRetweetCount(self, singlePlainTweet):
+    def filterRetweetCount(self, singlePlainTweet):
         """
         returns how many times the tweet has been retweeted
 
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         """
         return singlePlainTweet['content']['itemContent']['tweet_results']['result']['legacy']['retweet_count']
 
-    def getReplyCount(self, singlePlainTweet):
+    def filterReplyCount(self, singlePlainTweet):
         """
         returns how many replies the tweet has
 
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         """
         return singlePlainTweet['content']['itemContent']['tweet_results']['result']['legacy']['reply_count']
 
-    def getViews(self, singlePlainTweet):
+    def filterViews(self, singlePlainTweet):
         """
         returns how many views the tweet has
 
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         """
         return singlePlainTweet['content']['itemContent']['tweet_results']['result']['views']['count']
 
-    def getPinnedTweetInfo(self):
+    ## filter Account data
+    def __defaultAccountFilter(self, singleUserPlain):
+        return singleUserPlain['resp']['data']['user']['result']['timeline_v2']['timeline']['instructions'][1]['entries'][0]['content']['itemContent']['tweet_results']['result']['core']['user_results']['result']
+    
+    def filterPinnedTweetInfo(self, singleUserPlain):
         """
-        returns all (unfiltered) information about the pinned tweet
+        returns all (unfiltered) information about the pinned tweet of an Account
+        
+        :param getUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
         """
-        return \
-        self.__openingResp['data']['user']['result']['timeline_v2']['timeline']['instructions'][2]['entry']['content']['itemContent']['tweet_results']['result']
-
-    # get User data
-    def isBusinessAccount(self):
+        return singleUserPlain['data']['user']['result']['timeline_v2']['timeline']['instructions'][1]['entries'][0]['content']['itemContent']['tweet_results']['result']
+        
+    def filterIsBusinessAccount(self, singleUserPlain):
         """
         returns if the account is a business account
+        
+        :param getUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
         """
-        return self.__userResp['business_account']
-
-    def hasNftAvatar(self):
-        """
-        returns if the account has an NFT avatar
-        """
-        return self.__userResp['has_nft_avatar']
+        return self.__defaultAccountFilter(singleUserPlain)['business_account']
 
-    def userID(self):
+    def filterUserID(self, singleUserPlain):
         """
         returns the id of an account
+        
+        :param getUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
         """
-        return self.__userResp['id']
+        return self.__defaultAccountFilter(singleUserPlain)['id']
 
-    def isBlueVerified(self):
+    def filterIsBlueVerified(self, singleUserPlain):
         """
         returns if the account is verified with a twitter blue check
+        
+        :param getUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
         """
-        return self.__userResp['is_blue_verified']
+        return self.__defaultAccountFilter(singleUserPlain)['is_blue_verified']
 
-    def createdAt(self):
+    def filterAccountCreationDate(self, singleUserPlain):
         """
         returns the creation time of an account
+        
+        :param getUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
         """
-        return self.__userResp['legacy']['created_at']
+        return self.__defaultAccountFilter(singleUserPlain)['legacy']['created_at']
 
-    def description(self):
+    def filterDescription(self, singleUserPlain):
         """
         returns the description of an account
+        
+        :param getUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
         """
-        return self.__userResp['legacy']['description']
+        return self.__defaultAccountFilter(singleUserPlain)['legacy']['description']
 
-    def getAllUserData(self):
+    def getUserSpecificData(self, singleUserPlain):
         """
         returns all (unfiltered) data about an account
+        
+        :param getUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
         """
-        return self.__userResp
+        return self.__defaultAccountFilter(singleUserPlain)
```

### Comparing `ReverseTwitterScraper-0.4/ReverseTwitterScraper.egg-info/PKG-INFO` & `ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ReverseTwitterScraper
-Version: 0.4
+Version: 0.5
 Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
 Home-page: https://github.com/1220moritz/reverse-twitter-scraper
 Author: 1220moritz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ReverseTwitterScraper
-ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and Requests module to scrape tweets.
+ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and httpx to scrape tweets and other account data.
 
 ## Links
 GitHub: https://github.com/1220moritz/reverse-twitter-scraper  
 PyPI: https://pypi.org/project/ReverseTwitterScraper/
 
 ## Installation
 To install the package, simply run the following command:
@@ -37,40 +37,38 @@
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
 cookies = ""
 timeout = 5
 proxy_list = []
 
 # single account
-twitter_handle = "elonmusk"
-scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, timeout, proxy_list)
-tweets = scraper.getAllTweetsText()
+twitter_handle = ["elonmusk"]
+scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
+tweets = scraper.getTweetsText()
 
 # multiple accounts
 twitter_handles = ["elonmusk", "POTUS", "latestinspace"]
-scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, timeout, proxy_list)
-tweets = scraper.getTweetsTextMultiple()
+scraper = TwitterScraper(twitter_handles, chromedriver_path, cookies, proxy_list)
+tweets = scraper.getTweetsText()
 
 print(tweets)
 ```
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
-Finally, we call the getAllTweetsText() method to get the tweets of the specified Twitter account.
+Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
 
 ## Parameters
 The TwitterScraper class takes the following parameters:
 
-- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to elonmusk.
+- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
 
 - chromedriverPath: The path of the Chrome driver executable file. This file is required to use the Selenium module.
 
 - cookies: (Optional) The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
 
-- timeout: (Optional) The time (in seconds) to wait for the page to load. The default value is 5 seconds.
-
 - proxyList: (Optional) A list of proxies to use for scraping. The list should contain proxy addresses in the format ip:port:user:pw.
 
 
 ## How to get account cookies:
 Following a private "target" account is necessary to access its data. Then, account cookies can be used to scrape the account.
 1. Open the Chrome browser and go to the Twitter website.
 2. If you're not already logged in, log in to your Twitter account.
@@ -81,74 +79,76 @@
 7. In your Python code, create a new instance of the TwitterScraper class and paste the cookie value as the value of the "cookies" parameter.
 8. That's it! You can now use the TwitterScraper class to scrape data from your Twitter account.  
 
 By following these steps, you should be able to retrieve the necessary cookies from your Twitter account and use them in your Python code to scrape data.
 
 ## Methodes:
 
-### getTweetsPlainMultiple()
-      this is only if you want to scrape multiple twitter acccounts
+## get twitter data
+### getUserPlain()
+      get all (unfiltered) data from every account in your handle list ("unnecessary" data and ads included)
+      returns [{"handle": handle1, "id": id1, "resp": data1}, {"handle": handle2, "id": id2, "resp": data2},]
+
+### getTweetsPlain()
       get all (unfiltered) tweets from every account in your handle list (unnecessary data and ads included)
+      returns [{"handle": handle1, "id": id1, "resp": {1}}, {"handle": handle2, "id": id2, "resp": {2}}]
      
-### getTweetsTextMultiple()
-      this is only if you want to scrape multiple twitter acccounts
+### getTweetsText()
       get text from all tweets from every account in your handle list
+      returns [{'entryId': entryId1, 'retweet': retweet1, 'text': text1}, {'entryId': entryId2, 'retweet': retweet2, 'text': text2}]
 
-### getAllAccData()
-      returns all (unfiltered) data for the account
 
-### getRetweetInfo(singlePlainTweet, getRetweetInfo=False):
-        checks if the tweet is a retweet (returns True/False/TweetInfo)
-
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+## filter Tweet data
+### filterRetweetInfo(singlePlainTweet, getRetweetInfo=False):
+        checks if the tweet is a retweet (returns True, False or the TweetInfo (if you use getRetweetInfo=True))
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
         :param getRetweetInfo: default=False -> get all info about the retweetet tweet
-        
-### getAllTweetsPlain()
-      get all tweets from an account (unnecessary data included)
-
-
-### getAllTweetsText()
-      get a dict with text, tweetID and retweetInfo from all tweets from an account
       
-### getCreatedAt(singlePlainTweet)
+### filterTweetCreatedAt(singlePlainTweet)
     returns createTimeDate of a tweet
-    :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+    :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getID(singlePlainTweet)
+### filterTweetID(singlePlainTweet)
         returns the ID of a tweet
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getRetweetCount(singlePlainTweet)
+### filterRetweetCount(singlePlainTweet)
         returns how many times the tweet has been retweeted
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getReplyCount( singlePlainTweet)
+### filterReplyCount( singlePlainTweet)
         returns how many replies the tweet has
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
 
-### getViews(singlePlainTweet)
+### filterViews(singlePlainTweet)
         returns how many views the tweet has
-        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getAllTweetsPlain to get the info
+        :param singlePlainTweet: plain (unfiltered) info of a tweet. Use getTweetsPlain() to get the info
+
 
-### getPinnedTweetInfo()
+## filter Account data
+### filterPinnedTweetInfo(singleUserPlain)
         returns all (unfiltered) information about the pinned tweet
+		:param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### isBusinessAccount()
+### filterIsBusinessAccount(singleUserPlain)
         returns if the account is a business account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### hasNftAvatar()
-        returns if the account has an NFT avatar
-
-### userID()
-        returns the userID of the account
+### filterUserID(singleUserPlain)
+        returns the id of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### isBlueVerified()
+### filterIsBlueVerified(singleUserPlain)
         returns if the account is verified with a twitter blue check
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### createdAt()
+### filterAccountCreationDate(singleUserPlain)
         returns the creation time of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### description()
+### filterDescription(singleUserPlain)
         returns the description of an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
-### getAllUserData()
+### getUserSpecificData(singleUserPlain)
         returns all (unfiltered) data about an account
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
```

### Comparing `ReverseTwitterScraper-0.4/setup.py` & `ReverseTwitterScraper-0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ReverseTwitterScraper",
-    version="0.4",
+    version="0.5",
     author="1220moritz",
     description="A Python package for scraping Twitter data without API. With proxy and account-cookie support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/1220moritz/reverse-twitter-scraper",
       install_requires=[
           'selenium-wire',
           'selenium',
-          "requests",
+          "httpx",
           "asyncio",
-          "aiohttp"
+          "traceback"
       ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

