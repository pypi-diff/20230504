# Comparing `tmp/twitter_api_py-0.3.3.tar.gz` & `tmp/twitter_api_py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_api_py-0.3.3.tar", max compression
+gzip compressed data, was "twitter_api_py-0.4.0.tar", max compression
```

## Comparing `twitter_api_py-0.3.3.tar` & `twitter_api_py-0.4.0.tar`

### file list

```diff
@@ -1,216 +1,269 @@
--rw-r--r--   0        0        0     1497 2023-05-01 07:19:33.892883 twitter_api_py-0.3.3/LICENSE
--rw-r--r--   0        0        0     2126 2023-05-02 15:01:57.648446 twitter_api_py-0.3.3/README.md
--rw-r--r--   0        0        0     1516 2023-05-02 17:57:54.763964 twitter_api_py-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      480 2023-05-02 15:47:39.640660 twitter_api_py-0.3.3/twitter_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/__init__.py
--rw-r--r--   0        0        0     1039 2023-05-01 05:03:58.580612 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
--rw-r--r--   0        0        0      310 2023-05-01 05:01:04.629161 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
--rw-r--r--   0        0        0     1386 2023-05-01 15:37:14.131307 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
--rw-r--r--   0        0        0      305 2023-05-01 05:01:45.139500 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
--rw-r--r--   0        0        0      806 2023-05-01 05:02:17.969774 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
--rw-r--r--   0        0        0      314 2023-05-01 05:02:27.359852 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
--rw-r--r--   0        0        0     1209 2023-05-01 05:02:59.990124 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
--rw-r--r--   0        0        0      310 2023-05-01 05:03:15.690255 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
--rw-r--r--   0        0        0      829 2023-05-01 05:03:36.810430 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
--rw-r--r--   0        0        0      305 2023-05-01 05:03:51.400552 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.3.3/twitter_api/client/oauth_session/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/__init__.py
--rw-r--r--   0        0        0      364 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
--rw-r--r--   0        0        0     1139 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
--rw-r--r--   0        0        0      450 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
--rw-r--r--   0        0        0      792 2023-05-02 16:12:13.062596 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
--rw-r--r--   0        0        0      432 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
--rw-r--r--   0        0        0      721 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
--rw-r--r--   0        0        0      391 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
--rw-r--r--   0        0        0      797 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
--rw-r--r--   0        0        0      500 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
--rw-r--r--   0        0        0      750 2023-05-02 16:12:03.602519 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
--rw-r--r--   0        0        0      647 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/session_resources.py
--rw-r--r--   0        0        0      375 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
--rw-r--r--   0        0        0     1792 2023-05-02 16:41:17.966730 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
--rw-r--r--   0        0        0     3884 2023-05-02 17:57:16.613654 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
--rw-r--r--   0        0        0     1325 2023-05-02 16:41:04.896624 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_session.py
--rw-r--r--   0        0        0     1560 2023-05-02 16:43:35.267843 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
--rw-r--r--   0        0        0     3396 2023-05-02 16:43:15.727684 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
--rw-r--r--   0        0        0      866 2023-05-02 16:43:44.697919 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_session.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.3.3/twitter_api/client/request/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-24 12:44:19.060255 twitter_api_py-0.3.3/twitter_api/client/request/request_async_client.py
--rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.3.3/twitter_api/client/request/request_async_mock_client.py
--rw-r--r--   0        0        0     5182 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/request/request_async_real_client.py
--rw-r--r--   0        0        0     1967 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/request/request_client.py
--rw-r--r--   0        0        0     3368 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/request/request_mock_client.py
--rw-r--r--   0        0        0     7253 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/request/request_real_client.py
--rw-r--r--   0        0        0    32303 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_client.py
--rw-r--r--   0        0        0    14518 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_mock_client.py
--rw-r--r--   0        0        0    14743 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_real_client.py
--rw-r--r--   0        0        0    32062 2023-05-02 16:44:11.348135 twitter_api_py-0.3.3/twitter_api/client/twitter_api_client.py
--rw-r--r--   0        0        0    26895 2023-05-02 15:47:39.640660 twitter_api_py-0.3.3/twitter_api/client/twitter_api_mock_client.py
--rw-r--r--   0        0        0    13583 2023-05-02 16:40:53.436531 twitter_api_py-0.3.3/twitter_api/client/twitter_api_real_client.py
--rw-r--r--   0        0        0    10588 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/error.py
--rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.3.3/twitter_api/rate_limit/__init__.py
--rw-r--r--   0        0        0      603 2023-05-01 15:29:32.247704 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/__init__.py
--rw-r--r--   0        0        0     2232 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
--rw-r--r--   0        0        0      976 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
--rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
--rw-r--r--   0        0        0     3316 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
--rw-r--r--   0        0        0      705 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
--rw-r--r--   0        0        0     1232 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/rate_limit_manager.py
--rw-r--r--   0        0        0     3303 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/rate_limit.py
--rw-r--r--   0        0        0      291 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/rate_limit_info.py
--rw-r--r--   0        0        0       91 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/rate_limit_target.py
--rw-r--r--   0        0        0      281 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/api_resources.py
--rw-r--r--   0        0        0      437 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/oauth2_invalidate_token/__init__.py
--rw-r--r--   0        0        0     2295 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
--rw-r--r--   0        0        0      332 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/oauth2_token/__init__.py
--rw-r--r--   0        0        0     2187 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/oauth2_token/post_oauth2_token.py
--rw-r--r--   0        0        0      541 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversation_messages/__init__.py
--rw-r--r--   0        0        0     2316 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
--rw-r--r--   0        0        0      441 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations/__init__.py
--rw-r--r--   0        0        0     2164 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
--rw-r--r--   0        0        0      673 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
--rw-r--r--   0        0        0     8906 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
--rw-r--r--   0        0        0      676 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
--rw-r--r--   0        0        0     2390 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
--rw-r--r--   0        0        0      429 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/__init__.py
--rw-r--r--   0        0        0     1438 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/delete_v2_tweet.py
--rw-r--r--   0        0        0     3088 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/get_v2_tweet.py
--rw-r--r--   0        0        0      458 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
--rw-r--r--   0        0        0     6560 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
--rw-r--r--   0        0        0      428 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/__init__.py
--rw-r--r--   0        0        0     2977 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/get_v2_tweets.py
--rw-r--r--   0        0        0     2926 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/post_v2_tweets.py
--rw-r--r--   0        0        0      438 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_all/__init__.py
--rw-r--r--   0        0        0     5900 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
--rw-r--r--   0        0        0      471 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_recent/__init__.py
--rw-r--r--   0        0        0     5999 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
--rw-r--r--   0        0        0      471 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream/__init__.py
--rw-r--r--   0        0        0     3615 2023-05-02 15:14:15.304418 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
--rw-r--r--   0        0        0      770 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0     3096 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0      275 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user/get_v2_user.py
--rw-r--r--   0        0        0      371 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_followers/__init__.py
--rw-r--r--   0        0        0     6509 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
--rw-r--r--   0        0        0      376 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_following/__init__.py
--rw-r--r--   0        0        0     1909 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_following/post_v2_user_following.py
--rw-r--r--   0        0        0      391 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_liked_tweets/__init__.py
--rw-r--r--   0        0        0     7930 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
--rw-r--r--   0        0        0      367 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_retweets/__init__.py
--rw-r--r--   0        0        0     1911 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
--rw-r--r--   0        0        0      331 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_tweets/__init__.py
--rw-r--r--   0        0        0     8343 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
--rw-r--r--   0        0        0      279 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users/__init__.py
--rw-r--r--   0        0        0     2680 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users/get_v2_users.py
--rw-r--r--   0        0        0      299 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users_by/__init__.py
--rw-r--r--   0        0        0     2755 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users_by/get_v2_users_by.py
--rw-r--r--   0        0        0      396 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users_by_username/__init__.py
--rw-r--r--   0        0        0     3025 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.3.3/twitter_api/types/__init__.py
--rw-r--r--   0        0        0      386 2023-04-09 09:46:11.323030 twitter_api_py-0.3.3/twitter_api/types/chainable.py
--rw-r--r--   0        0        0      697 2023-04-26 11:13:40.460129 twitter_api_py-0.3.3/twitter_api/types/comma_separatable.py
--rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.3.3/twitter_api/types/endpoint.py
--rw-r--r--   0        0        0     1580 2023-05-02 17:35:22.073007 twitter_api_py-0.3.3/twitter_api/types/extra_permissive_model.py
--rw-r--r--   0        0        0      570 2023-05-02 15:47:39.640660 twitter_api_py-0.3.3/twitter_api/types/generic_client.py
--rw-r--r--   0        0        0      616 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/types/http.py
--rw-r--r--   0        0        0      734 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/types/httpx.py
--rw-r--r--   0        0        0     2362 2023-04-20 12:43:51.415589 twitter_api_py-0.3.3/twitter_api/types/model.py
--rw-r--r--   0        0        0     1942 2023-05-01 15:41:37.413361 twitter_api_py-0.3.3/twitter_api/types/oauth.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/types/oauth1/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-02 17:48:22.619331 twitter_api_py-0.3.3/twitter_api/types/oauth1/oauth1_access_token.py
--rw-r--r--   0        0        0     3473 2023-05-02 16:25:30.009051 twitter_api_py-0.3.3/twitter_api/types/oauth1/oauth1_authorization.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/types/oauth2/__init__.py
--rw-r--r--   0        0        0     1974 2023-05-02 17:51:03.780634 twitter_api_py-0.3.3/twitter_api/types/oauth2/oauth2_access_token.py
--rw-r--r--   0        0        0     3592 2023-05-02 16:26:12.579396 twitter_api_py-0.3.3/twitter_api/types/oauth2/oauth2_authorization.py
--rw-r--r--   0        0        0       63 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/types/pagination_token.py
--rw-r--r--   0        0        0     3529 2023-05-02 14:56:28.715783 twitter_api_py-0.3.3/twitter_api/types/paging.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/__init__.py
--rw-r--r--   0        0        0      337 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation.py
--rw-r--r--   0        0        0      201 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
--rw-r--r--   0        0        0       64 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
--rw-r--r--   0        0        0      594 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/__init__.py
--rw-r--r--   0        0        0      331 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/dm_event_expansion.py
--rw-r--r--   0        0        0      437 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/dm_event_field.py
--rw-r--r--   0        0        0       57 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/dm_event_id.py
--rw-r--r--   0        0        0      238 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/dm_event_type.py
--rw-r--r--   0        0        0      315 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_domain.py
--rw-r--r--   0        0        0      248 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_entity.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_geo/__init__.py
--rw-r--r--   0        0        0      209 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_geo/geo.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/__init__.py
--rw-r--r--   0        0        0     1356 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media.py
--rw-r--r--   0        0        0      570 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_field.py
--rw-r--r--   0        0        0      100 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_id.py
--rw-r--r--   0        0        0       56 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_key.py
--rw-r--r--   0        0        0      376 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_non_public_metrics.py
--rw-r--r--   0        0        0      411 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_organic_metrics.py
--rw-r--r--   0        0        0      412 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_promoted_metrics.py
--rw-r--r--   0        0        0      190 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_public_metrics.py
--rw-r--r--   0        0        0      211 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_variants.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_place/__init__.py
--rw-r--r--   0        0        0      635 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_place/place.py
--rw-r--r--   0        0        0      348 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_place/place_field.py
--rw-r--r--   0        0        0       94 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_place/place_id.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/__init__.py
--rw-r--r--   0        0        0      593 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll.py
--rw-r--r--   0        0        0      272 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll_field.py
--rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll_id.py
--rw-r--r--   0        0        0      164 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll_option.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet.py
--rw-r--r--   0        0        0      392 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities.py
--rw-r--r--   0        0        0      913 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description.py
--rw-r--r--   0        0        0      184 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
--rw-r--r--   0        0        0      184 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
--rw-r--r--   0        0        0      246 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
--rw-r--r--   0        0        0      258 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description_url.py
--rw-r--r--   0        0        0      338 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_url.py
--rw-r--r--   0        0        0      254 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_includes.py
--rw-r--r--   0        0        0      219 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_public_metrics.py
--rw-r--r--   0        0        0      352 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_rule/__init__.py
--rw-r--r--   0        0        0      311 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_rule/rule.py
--rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_rule/rule_id.py
--rw-r--r--   0        0        0       55 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_rule/rule_tag.py
--rw-r--r--   0        0        0     1411 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_scope.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/__init__.py
--rw-r--r--   0        0        0     6434 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet.py
--rw-r--r--   0        0        0      309 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_attachments.py
--rw-r--r--   0        0        0      229 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_context_annotation.py
--rw-r--r--   0        0        0      314 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_edit_controls.py
--rw-r--r--   0        0        0      720 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities.py
--rw-r--r--   0        0        0      333 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_annotation.py
--rw-r--r--   0        0        0      247 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
--rw-r--r--   0        0        0      247 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
--rw-r--r--   0        0        0      313 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_mention.py
--rw-r--r--   0        0        0      415 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_url.py
--rw-r--r--   0        0        0      632 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_expansion.py
--rw-r--r--   0        0        0     1910 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_field.py
--rw-r--r--   0        0        0      288 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_geo.py
--rw-r--r--   0        0        0      231 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
--rw-r--r--   0        0        0      100 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_id.py
--rw-r--r--   0        0        0      287 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
--rw-r--r--   0        0        0      285 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_organic_metrics.py
--rw-r--r--   0        0        0      286 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
--rw-r--r--   0        0        0      437 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_public_metrics.py
--rw-r--r--   0        0        0      256 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
--rw-r--r--   0        0        0     7049 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_response_body.py
--rw-r--r--   0        0        0      387 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/__init__.py
--rw-r--r--   0        0        0      969 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user.py
--rw-r--r--   0        0        0      157 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user_expantion.py
--rw-r--r--   0        0        0      608 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user_field.py
--rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user_id.py
--rw-r--r--   0        0        0       97 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user_verified_type.py
--rw-r--r--   0        0        0      128 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/username.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.3.3/twitter_api/utils/__init__.py
--rw-r--r--   0        0        0      123 2023-04-23 15:17:02.699271 twitter_api_py-0.3.3/twitter_api/utils/_datetime.py
--rw-r--r--   0        0        0      716 2023-04-27 14:28:44.162902 twitter_api_py-0.3.3/twitter_api/utils/_functional.py
--rw-r--r--   0        0        0      904 2023-04-25 11:39:31.648198 twitter_api_py-0.3.3/twitter_api/utils/_oauth.py
--rw-r--r--   0        0        0      775 2023-05-01 04:02:26.399958 twitter_api_py-0.3.3/twitter_api/utils/json.py
--rw-r--r--   0        0        0      630 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/warning.py
--rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 twitter_api_py-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-03 13:16:42.851501 twitter_api_py-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2126 2023-05-03 13:16:42.851501 twitter_api_py-0.4.0/README.md
+-rw-r--r--   0        0        0     1516 2023-05-04 13:43:23.393237 twitter_api_py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      480 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
+-rw-r--r--   0        0        0     1388 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
+-rw-r--r--   0        0        0      306 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
+-rw-r--r--   0        0        0      808 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
+-rw-r--r--   0        0        0      315 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
+-rw-r--r--   0        0        0     1211 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
+-rw-r--r--   0        0        0      831 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
+-rw-r--r--   0        0        0      306 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.4.0/twitter_api/client/oauth_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
+-rw-r--r--   0        0        0     1140 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
+-rw-r--r--   0        0        0      451 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
+-rw-r--r--   0        0        0      433 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
+-rw-r--r--   0        0        0      392 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
+-rw-r--r--   0        0        0      798 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
+-rw-r--r--   0        0        0      501 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
+-rw-r--r--   0        0        0      648 2023-05-03 13:16:42.861501 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/session_resources.py
+-rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
+-rw-r--r--   0        0        0     1596 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
+-rw-r--r--   0        0        0     1793 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
+-rw-r--r--   0        0        0     3885 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
+-rw-r--r--   0        0        0     1103 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth1_session.py
+-rw-r--r--   0        0        0     1561 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
+-rw-r--r--   0        0        0     3397 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
+-rw-r--r--   0        0        0      823 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth2_session.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.4.0/twitter_api/client/request/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/request/request_async_client.py
+-rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.4.0/twitter_api/client/request/request_async_mock_client.py
+-rw-r--r--   0        0        0     5182 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/request/request_async_real_client.py
+-rw-r--r--   0        0        0     1967 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/request/request_client.py
+-rw-r--r--   0        0        0     3368 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/request/request_mock_client.py
+-rw-r--r--   0        0        0     7235 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/request/request_real_client.py
+-rw-r--r--   0        0        0    32304 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/twitter_api_async_client.py
+-rw-r--r--   0        0        0    14518 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/twitter_api_async_mock_client.py
+-rw-r--r--   0        0        0    14743 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/twitter_api_async_real_client.py
+-rw-r--r--   0        0        0    32063 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/twitter_api_client.py
+-rw-r--r--   0        0        0    26895 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/twitter_api_mock_client.py
+-rw-r--r--   0        0        0    13583 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/client/twitter_api_real_client.py
+-rw-r--r--   0        0        0    10636 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/error.py
+-rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.4.0/twitter_api/rate_limit/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/rate_limit/manager/__init__.py
+-rw-r--r--   0        0        0     2232 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
+-rw-r--r--   0        0        0      976 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.4.0/twitter_api/rate_limit/manager/handlers/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
+-rw-r--r--   0        0        0     3316 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
+-rw-r--r--   0        0        0      705 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
+-rw-r--r--   0        0        0     1232 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/rate_limit/manager/rate_limit_manager.py
+-rw-r--r--   0        0        0     3303 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/rate_limit/rate_limit.py
+-rw-r--r--   0        0        0      291 2023-05-02 14:52:07.203654 twitter_api_py-0.4.0/twitter_api/rate_limit/rate_limit_info.py
+-rw-r--r--   0        0        0       91 2023-05-02 14:52:07.203654 twitter_api_py-0.4.0/twitter_api/rate_limit/rate_limit_target.py
+-rw-r--r--   0        0        0      281 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/api_resources.py
+-rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/oauth2_invalidate_token/__init__.py
+-rw-r--r--   0        0        0     2295 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
+-rw-r--r--   0        0        0      332 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/oauth2_token/__init__.py
+-rw-r--r--   0        0        0     2187 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/oauth2_token/post_oauth2_token.py
+-rw-r--r--   0        0        0      541 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversation_messages/__init__.py
+-rw-r--r--   0        0        0     2316 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
+-rw-r--r--   0        0        0      441 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
+-rw-r--r--   0        0        0      673 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
+-rw-r--r--   0        0        0     8907 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
+-rw-r--r--   0        0        0      676 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
+-rw-r--r--   0        0        0     2390 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
+-rw-r--r--   0        0        0      429 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     1438 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweet/delete_v2_tweet.py
+-rw-r--r--   0        0        0     3088 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweet/get_v2_tweet.py
+-rw-r--r--   0        0        0      458 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
+-rw-r--r--   0        0        0     6561 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
+-rw-r--r--   0        0        0      428 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets/__init__.py
+-rw-r--r--   0        0        0     2977 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets/get_v2_tweets.py
+-rw-r--r--   0        0        0     2926 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets/post_v2_tweets.py
+-rw-r--r--   0        0        0      438 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_all/__init__.py
+-rw-r--r--   0        0        0     6032 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
+-rw-r--r--   0        0        0      471 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_recent/__init__.py
+-rw-r--r--   0        0        0     6131 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
+-rw-r--r--   0        0        0      471 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream/__init__.py
+-rw-r--r--   0        0        0     3615 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
+-rw-r--r--   0        0        0      770 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0     3096 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0      275 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user/get_v2_user.py
+-rw-r--r--   0        0        0      371 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_followers/__init__.py
+-rw-r--r--   0        0        0     6510 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
+-rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_following/__init__.py
+-rw-r--r--   0        0        0     1909 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_following/post_v2_user_following.py
+-rw-r--r--   0        0        0      391 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_liked_tweets/__init__.py
+-rw-r--r--   0        0        0     7931 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
+-rw-r--r--   0        0        0      367 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_retweets/__init__.py
+-rw-r--r--   0        0        0     1911 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
+-rw-r--r--   0        0        0      331 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_tweets/__init__.py
+-rw-r--r--   0        0        0     8344 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
+-rw-r--r--   0        0        0      279 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_users/__init__.py
+-rw-r--r--   0        0        0     2680 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_users/get_v2_users.py
+-rw-r--r--   0        0        0      299 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_users_by/__init__.py
+-rw-r--r--   0        0        0     2755 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_users_by/get_v2_users_by.py
+-rw-r--r--   0        0        0      396 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_users_by_username/__init__.py
+-rw-r--r--   0        0        0     3025 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.4.0/twitter_api/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/_chainable.py
+-rw-r--r--   0        0        0      570 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/_generic_client.py
+-rw-r--r--   0        0        0     2362 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/_model.py
+-rw-r--r--   0        0        0     3458 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/_paging.py
+-rw-r--r--   0        0        0      697 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/comma_separatable.py
+-rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.4.0/twitter_api/types/endpoint.py
+-rw-r--r--   0        0        0     1581 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/extra_permissive_model.py
+-rw-r--r--   0        0        0      616 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/http.py
+-rw-r--r--   0        0        0      734 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/httpx.py
+-rw-r--r--   0        0        0     1942 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/oauth.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/oauth1/__init__.py
+-rw-r--r--   0        0        0     2037 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/oauth1/oauth1_access_token.py
+-rw-r--r--   0        0        0     3474 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/oauth1/oauth1_authorization.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/oauth2/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/oauth2/oauth2_access_token.py
+-rw-r--r--   0        0        0     3593 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/oauth2/oauth2_authorization.py
+-rw-r--r--   0        0        0       63 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/pagination_token.py
+-rw-r--r--   0        0        0       55 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_cashtag.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_conversation/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_conversation/dm_conversation.py
+-rw-r--r--   0        0        0      201 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
+-rw-r--r--   0        0        0       64 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
+-rw-r--r--   0        0        0      594 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_event/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_event/dm_event_expansion.py
+-rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_event/dm_event_field.py
+-rw-r--r--   0        0        0       57 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_event/dm_event_id.py
+-rw-r--r--   0        0        0      238 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_dm_event/dm_event_type.py
+-rw-r--r--   0        0        0      338 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_domain.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_entity/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_entity/entity.py
+-rw-r--r--   0        0        0       56 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_entity/entity_id.py
+-rw-r--r--   0        0        0       58 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_entity/entity_name.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_geo/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_geo/geo.py
+-rw-r--r--   0        0        0       55 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_hashtag.py
+-rw-r--r--   0        0        0      762 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_language.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_list/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_list/list_id.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/__init__.py
+-rw-r--r--   0        0        0     1356 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media.py
+-rw-r--r--   0        0        0      570 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media_field.py
+-rw-r--r--   0        0        0      100 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media_id.py
+-rw-r--r--   0        0        0       56 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media_key.py
+-rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media_non_public_metrics.py
+-rw-r--r--   0        0        0      411 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media_organic_metrics.py
+-rw-r--r--   0        0        0      412 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media_promoted_metrics.py
+-rw-r--r--   0        0        0      190 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media_public_metrics.py
+-rw-r--r--   0        0        0      211 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_media/media_variants.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_place/__init__.py
+-rw-r--r--   0        0        0      933 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_place/place.py
+-rw-r--r--   0        0        0     2712 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_place/place_country_code.py
+-rw-r--r--   0        0        0      348 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_place/place_field.py
+-rw-r--r--   0        0        0       61 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_place/place_full_name.py
+-rw-r--r--   0        0        0       94 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_place/place_id.py
+-rw-r--r--   0        0        0       57 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_place/place_name.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_poll/__init__.py
+-rw-r--r--   0        0        0      593 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_poll/poll.py
+-rw-r--r--   0        0        0      272 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_poll/poll_field.py
+-rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_poll/poll_id.py
+-rw-r--r--   0        0        0      164 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_poll/poll_option.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet.py
+-rw-r--r--   0        0        0      392 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_entities.py
+-rw-r--r--   0        0        0      913 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_entities_description.py
+-rw-r--r--   0        0        0      237 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
+-rw-r--r--   0        0        0      237 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
+-rw-r--r--   0        0        0      246 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
+-rw-r--r--   0        0        0      258 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_entities_description_url.py
+-rw-r--r--   0        0        0      338 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_entities_url.py
+-rw-r--r--   0        0        0      254 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_includes.py
+-rw-r--r--   0        0        0      219 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_public_metrics.py
+-rw-r--r--   0        0        0      352 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_rule/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_rule/rule.py
+-rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_rule/rule_id.py
+-rw-r--r--   0        0        0       55 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_rule/rule_tag.py
+-rw-r--r--   0        0        0     1411 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_scope.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/_and_operator.py
+-rw-r--r--   0        0        0      305 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/_markable_operator.py
+-rw-r--r--   0        0        0      704 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/_not_operator.py
+-rw-r--r--   0        0        0      364 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/_or_operator.py
+-rw-r--r--   0        0        0      666 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/bounding_box_operator.py
+-rw-r--r--   0        0        0      369 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/cashtag_operator.py
+-rw-r--r--   0        0        0     1361 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/context_operator.py
+-rw-r--r--   0        0        0      410 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/conversation_id_operator.py
+-rw-r--r--   0        0        0      371 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/entity_operator.py
+-rw-r--r--   0        0        0      454 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/from_user_operator.py
+-rw-r--r--   0        0        0     1620 2023-05-04 13:24:33.227263 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/group_operator.py
+-rw-r--r--   0        0        0      240 2023-05-04 13:40:13.473882 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/has_cashtags_operator.py
+-rw-r--r--   0        0        0      230 2023-05-04 13:41:21.463651 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/has_geo_operator.py
+-rw-r--r--   0        0        0      240 2023-05-04 13:40:02.033921 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/has_hashtags_operator.py
+-rw-r--r--   0        0        0      236 2023-05-04 13:40:55.923738 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/has_images_operator.py
+-rw-r--r--   0        0        0      234 2023-05-04 13:40:23.623848 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/has_links_operator.py
+-rw-r--r--   0        0        0      234 2023-05-04 13:40:45.373774 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/has_media_operator.py
+-rw-r--r--   0        0        0      240 2023-05-04 13:40:37.683800 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/has_mentions_operator.py
+-rw-r--r--   0        0        0      243 2023-05-04 13:41:06.593702 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/has_video_link_operator.py
+-rw-r--r--   0        0        0      369 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/hashtag_operator.py
+-rw-r--r--   0        0        0      379 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/in_reply_to_tweet_id_operator.py
+-rw-r--r--   0        0        0      444 2023-05-04 13:39:41.393991 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/is_nullcast_operator.py
+-rw-r--r--   0        0        0      232 2023-05-04 13:37:40.124404 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/is_quote_operator.py
+-rw-r--r--   0        0        0      232 2023-05-04 13:37:03.134530 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/is_reply_operator.py
+-rw-r--r--   0        0        0      236 2023-05-04 13:36:42.674600 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/is_retweet_operator.py
+-rw-r--r--   0        0        0      238 2023-05-04 13:39:12.784088 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/is_verified_operator.py
+-rw-r--r--   0        0        0      446 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/keyword_operator.py
+-rw-r--r--   0        0        0      359 2023-05-04 13:41:34.213608 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/lang_operator.py
+-rw-r--r--   0        0        0      347 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/list_operator.py
+-rw-r--r--   0        0        0      379 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/mention_operator.py
+-rw-r--r--   0        0        0     1062 2023-05-04 13:36:07.904718 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/operator.py
+-rw-r--r--   0        0        0      400 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/place_country_operator.py
+-rw-r--r--   0        0        0      574 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/place_operator.py
+-rw-r--r--   0        0        0     1277 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/point_radius_operator.py
+-rw-r--r--   0        0        0      384 2023-05-04 12:42:31.224094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/quotes_of_tweet_id_operator.py
+-rw-r--r--   0        0        0      462 2023-05-04 12:42:31.234094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/retweet_of_operator.py
+-rw-r--r--   0        0        0      380 2023-05-04 12:42:31.234094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/retweets_of_tweet_id_operator.py
+-rw-r--r--   0        0        0      450 2023-05-04 12:42:31.234094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/to_user_operator.py
+-rw-r--r--   0        0        0      292 2023-05-04 12:42:31.234094 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/operators/url_operator.py
+-rw-r--r--   0        0        0    16361 2023-05-04 13:38:17.014278 twitter_api_py-0.4.0/twitter_api/types/v2_search_query/search_query.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     7856 2023-05-04 12:42:31.234094 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet.py
+-rw-r--r--   0        0        0      309 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_attachments.py
+-rw-r--r--   0        0        0      267 2023-05-04 12:42:31.234094 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_context_annotation.py
+-rw-r--r--   0        0        0      314 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_edit_controls.py
+-rw-r--r--   0        0        0      720 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_entities.py
+-rw-r--r--   0        0        0      333 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_entities_annotation.py
+-rw-r--r--   0        0        0      247 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
+-rw-r--r--   0        0        0      247 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
+-rw-r--r--   0        0        0      313 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_entities_mention.py
+-rw-r--r--   0        0        0      415 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_entities_url.py
+-rw-r--r--   0        0        0      632 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_expansion.py
+-rw-r--r--   0        0        0     1910 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_field.py
+-rw-r--r--   0        0        0      288 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_geo.py
+-rw-r--r--   0        0        0      231 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
+-rw-r--r--   0        0        0      100 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_id.py
+-rw-r--r--   0        0        0      287 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
+-rw-r--r--   0        0        0      285 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_organic_metrics.py
+-rw-r--r--   0        0        0      286 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
+-rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_public_metrics.py
+-rw-r--r--   0        0        0      256 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
+-rw-r--r--   0        0        0     7050 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_response_body.py
+-rw-r--r--   0        0        0      387 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_user/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_user/user.py
+-rw-r--r--   0        0        0      157 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_user/user_expantion.py
+-rw-r--r--   0        0        0      608 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_user/user_field.py
+-rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_user/user_id.py
+-rw-r--r--   0        0        0       97 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_user/user_verified_type.py
+-rw-r--r--   0        0        0      128 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/types/v2_user/username.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.4.0/twitter_api/utils/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/utils/_datetime.py
+-rw-r--r--   0        0        0      716 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/utils/_functional.py
+-rw-r--r--   0        0        0      904 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/utils/_oauth.py
+-rw-r--r--   0        0        0      775 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/utils/json.py
+-rw-r--r--   0        0        0      630 2023-05-03 13:16:42.871502 twitter_api_py-0.4.0/twitter_api/warning.py
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 twitter_api_py-0.4.0/PKG-INFO
```

### Comparing `twitter_api_py-0.3.3/LICENSE` & `twitter_api_py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/README.md` & `twitter_api_py-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/pyproject.toml` & `twitter_api_py-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["yassun4dev <yassun4dev@outlook.com>"]
 description = "Twitter API Client by Typed Python."
 name = "twitter-api-py"
 packages = [{include = "twitter_api"}]
 readme = "README.md"
-version = "0.3.3"
+version = "0.4.0"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/twitter-api-py"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Generic
 
 from twitter_api.client.oauth_session.resources.oauth1_access_token import (
     Oauth1AccessTokenResources,
     Oauth1AccessTokenUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
-from twitter_api.types.chainable import Chainable
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._chainable import Chainable
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import CallbackUrl
 
 
 class TwitterOAuth1AccessTokenClient(Chainable, Generic[TwitterApiGenericClient]):
     def __init__(
         self,
         authorization_response_url: CallbackUrl,
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 )
 from twitter_api.client.oauth_session.resources.oauth1_authorize import (
     OAuth1AuthorizeSessionResources,
     Oauth1AuthorizeUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
 from twitter_api.error import NeverError
-from twitter_api.types.chainable import Chainable
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._chainable import Chainable
+from twitter_api.types._generic_client import TwitterApiGenericClient
 
 
 class TwitterOAuth1AuthorizeClient(Chainable, Generic[TwitterApiGenericClient]):
     def __init__(self, session: TwitterOAuth1Session[TwitterApiGenericClient]) -> None:
         self._session = session
 
     def request(
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Generic
 
 from twitter_api.client.oauth_session.resources.oauth1_request_token import (
     OAuth1RequestTokenSessionResources,
     Oauth1RequestTokenUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
-from twitter_api.types.chainable import Chainable
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._chainable import Chainable
+from twitter_api.types._generic_client import TwitterApiGenericClient
 
 
 class TwitterOAuth1RequestTokenClient(Chainable, Generic[TwitterApiGenericClient]):
     def __init__(self, session: TwitterOAuth1Session[TwitterApiGenericClient]) -> None:
         self._session = session
 
     def request(
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Generic
 
 from twitter_api.client.oauth_session.resources.v2_oauth2_token import (
     V2OAuth2TokenRerources,
     V2Oauth2TokenUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
-from twitter_api.types.chainable import Chainable
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._chainable import Chainable
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import CallbackUrl
 
 
 class TwitterOAuth2AccessTokenClient(Chainable, Generic[TwitterApiGenericClient]):
     def __init__(
         self,
         authorization_response_url: CallbackUrl,
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Generic
 
 from twitter_api.client.oauth_session.resources.oauth2_authorize import (
     OAuth2AuthorizeSessionResources,
     Oauth2AuthorizeUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
-from twitter_api.types.chainable import Chainable
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._chainable import Chainable
+from twitter_api.types._generic_client import TwitterApiGenericClient
 
 
 @dataclass
 class TwitterOAuth2AuthorizeClient(Chainable, Generic[TwitterApiGenericClient]):
     def __init__(self, session: TwitterOAuth2Session[TwitterApiGenericClient]) -> None:
         self._session = session
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth1SessionResources,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import CallbackUrl
 from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 
 
 class PostOauth1AccessTokenResources(OAuth1SessionResources[TwitterApiGenericClient]):
     def __init__(
         self,
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth1SessionResources,
 )
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
 
 
-class GenerateAuthorizationUrlOAuth1AuthenticateSessionResources(
+class GenerateAuthorizationUrlOAuth1AuthorizeSessionResources(
     OAuth1SessionResources[TwitterApiGenericClient]
 ):
     def generate_authorization_url(self):
         """
         OAuth 1.0a の 2 番目のステップ。
-        ユーザーアクセストークンのセットを生成するために、
-        Twitter 認証画面へのアクセス用 URL を生成する。
+        ユーザーアクセストークンのセットを生成するために使用する。
 
-        refer: https://developer.twitter.com/en/docs/authentication/api-reference/authenticate
+        refer: https://developer.twitter.com/en/docs/authentication/api-reference/authorize
         """
 
         return self._session.generate_authorization_url(
-            "https://api.twitter.com/oauth/authenticate",
+            "https://api.twitter.com/oauth/authorize"
         )
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth1SessionResources,
 )
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
 
 
-class GenerateAuthorizationUrlOAuth1AuthorizeSessionResources(
+class GenerateAuthorizationUrlOAuth1AuthenticateSessionResources(
     OAuth1SessionResources[TwitterApiGenericClient]
 ):
     def generate_authorization_url(self):
         """
         OAuth 1.0a の 2 番目のステップ。
-        ユーザーアクセストークンのセットを生成するために使用する。
+        ユーザーアクセストークンのセットを生成するために、
+        Twitter 認証画面へのアクセス用 URL を生成する。
 
-        refer: https://developer.twitter.com/en/docs/authentication/api-reference/authorize
+        refer: https://developer.twitter.com/en/docs/authentication/api-reference/authenticate
         """
 
         return self._session.generate_authorization_url(
-            "https://api.twitter.com/oauth/authorize"
+            "https://api.twitter.com/oauth/authenticate",
         )
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
     TwitterOAuth1AuthorizeClient,
 )
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth1SessionResources,
 )
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
 
 
 class PostOAuth1RequestTokenSessionResources(
     OAuth1SessionResources[TwitterApiGenericClient]
 ):
     def post(self) -> TwitterOAuth1AuthorizeClient[TwitterApiGenericClient]:
         """
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth2SessionResources,
 )
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
 
 
 class GenerateAuthorizationUrlOAuth2AuthorizeSessionResources(
     OAuth2SessionResources[TwitterApiGenericClient],
 ):
     def generate_authorization_url(self):
         """
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/session_resources.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth2_session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,26 @@
-from typing import Generic
+from abc import ABCMeta, abstractmethod
+from typing import Generic, cast
 
-from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
-from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
+from twitter_api.types.oauth import CallbackUrl
 
 
-class OAuth1SessionResources(Generic[TwitterApiGenericClient]):
-    def __init__(self, session: TwitterOAuth1Session[TwitterApiGenericClient]) -> None:
-        self._session = session
+class TwitterOAuth2Session(Generic[TwitterApiGenericClient], metaclass=ABCMeta):
+    @abstractmethod
+    def generate_authorization_url(
+        self,
+    ):
+        from twitter_api.types.oauth2.oauth2_authorization import OAuth2Authorization
 
+        return cast(OAuth2Authorization[TwitterApiGenericClient], ...)
 
-class OAuth2SessionResources(Generic[TwitterApiGenericClient]):
-    def __init__(self, session: TwitterOAuth2Session[TwitterApiGenericClient]) -> None:
-        self._session = session
+    @abstractmethod
+    def fetch_token(
+        self,
+        authorization_response_url: CallbackUrl,
+        state: str,
+        code_verifier: str,
+    ):
+        from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
+
+        return cast(OAuth2AccessToken[TwitterApiGenericClient], ...)
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Generic
 
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth2SessionResources,
 )
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import CallbackUrl
 from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
 
 ENDPOINT = Endpoint("POST", "https://api.twitter.com/2/oauth2/token")
 
 
 class PostV2OAuth2TokenRerources(
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from twitter_api.client.oauth_session.resources.oauth1_authenticate import (
     OauthAuth1enticateUrl,
 )
 from twitter_api.client.oauth_session.resources.oauth1_authorize import (
     Oauth1AuthorizeUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
-from twitter_api.types.generic_client import TwitterApiGenericMockClient
+from twitter_api.types._generic_client import TwitterApiGenericMockClient
 from twitter_api.types.oauth import AccessSecret, AccessToken, CallbackUrl
 
 
 class TwitterOAuth1MockSession(TwitterOAuth1Session[TwitterApiGenericMockClient]):
     def __init__(
         self,
         client_generator: Callable[
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_real_session.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Oauth1AuthorizeUrl,
 )
 from twitter_api.client.oauth_session.resources.oauth1_request_token import (
     Oauth1RequestTokenUrl,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
 from twitter_api.types import httpx
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import (
     AccessSecret,
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
 )
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_session.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-from abc import ABCMeta, abstractmethod
-from typing import Generic
+from datetime import datetime
+from typing import Callable
 
-from twitter_api.types.generic_client import TwitterApiGenericClient
-from twitter_api.types.http import Url
-from twitter_api.types.oauth import CallbackUrl
+from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
+from twitter_api.types._generic_client import TwitterApiGenericMockClient
+from twitter_api.types.oauth import AccessToken, CallbackUrl
+from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
+from twitter_api.types.v2_scope import Scope
 
 
-class TwitterOAuth1Session(Generic[TwitterApiGenericClient], metaclass=ABCMeta):
-    @abstractmethod
-    def request_token(self):
-        from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
-            TwitterOAuth1AuthorizeClient,
-        )
-
-        _: TwitterOAuth1AuthorizeClient[TwitterApiGenericClient] = ...  # type: ignore
-
-        return _
-
-    @abstractmethod
-    def generate_authorization_url(
+class TwitterOAuth2MockSession(TwitterOAuth2Session[TwitterApiGenericMockClient]):
+    def __init__(
         self,
-        url: Url,
-    ):
-        from twitter_api.types.oauth1.oauth1_authorization import OAuth1Authorization
-
-        _: OAuth1Authorization[TwitterApiGenericClient] = ...  # type: ignore
-
-        return _
+        client_generator: Callable[[AccessToken], TwitterApiGenericMockClient],
+        *,
+        scope: list[Scope],
+    ) -> None:
+        self._client_generator = client_generator
+        self._scope = scope
+
+    def generate_authorization_url(self):
+        from twitter_api.types.oauth2.oauth2_authorization import OAuth2Authorization
+
+        return OAuth2Authorization(
+            authorization_url="https://authorization.url.com",
+            state="state",
+            code_verifier="code_verifier",
+            session=self,
+        )
 
-    @abstractmethod
     def fetch_token(
         self,
         authorization_response_url: CallbackUrl,
-    ):
-        # NOTE: 本来実装は不要だが、モジュールの循環読み込みを防ぐため、
-        #       偽のデータを作っている。
-        from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
-
-        _: OAuth1AccessToken[TwitterApiGenericClient] = ...  # type: ignore
-
-        return _
+        state: str,
+        code_verifier: str,
+    ) -> OAuth2AccessToken:
+        expires_in = 7200
+        return OAuth2AccessToken(
+            token_type="bearer",
+            expires_in=expires_in,
+            expires_at=int(datetime.now().timestamp()) + expires_in,
+            access_token="access_token",
+            scope=self._scope,
+            _client_generator=self._client_generator,
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,93 @@
-from datetime import datetime
-from typing import Callable
+from typing import Any, Callable, Generic, Mapping, Optional
 
+from authlib.integrations.httpx_client.oauth2_client import OAuth2Client
+
+from twitter_api.client.oauth_session.resources.oauth2_authorize import (
+    Oauth2AuthorizeUrl,
+)
+from twitter_api.client.oauth_session.resources.v2_oauth2_token import V2Oauth2TokenUrl
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
-from twitter_api.types.generic_client import TwitterApiGenericMockClient
-from twitter_api.types.oauth import AccessToken, CallbackUrl
+from twitter_api.types import httpx
+from twitter_api.types._generic_client import TwitterApiGenericClient
+from twitter_api.types.oauth import AccessToken, CallbackUrl, ClientId, ClientSecret
 from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
+from twitter_api.types.oauth2.oauth2_authorization import OAuth2Authorization
 from twitter_api.types.v2_scope import Scope
+from twitter_api.utils._oauth import generate_code_verifier
 
 
-class TwitterOAuth2MockSession(TwitterOAuth2Session[TwitterApiGenericMockClient]):
+class TwitterOAuth2RealSession(TwitterOAuth2Session, Generic[TwitterApiGenericClient]):
     def __init__(
         self,
-        client_generator: Callable[[AccessToken], TwitterApiGenericMockClient],
+        client_generator: Callable[[AccessToken], TwitterApiGenericClient],
         *,
-        scope: list[Scope],
+        client_id: ClientId,
+        client_secret: ClientSecret,
+        callback_url: CallbackUrl,
+        scope: Optional[list[Scope]],
+        event_hooks: Optional[Mapping[str, list[httpx.EventHook]]],
+        limits: httpx.Limits,
+        mounts: Optional[Mapping[str, httpx.BaseTransport]],
+        proxies: Optional[httpx.ProxiesTypes],
+        timeout: httpx.TimeoutTypes,
+        transport: Optional[httpx.BaseTransport],
+        verify: httpx.VerifyTypes,
     ) -> None:
         self._client_generator = client_generator
-        self._scope = scope
+        self._session = OAuth2Client(
+            client_id=client_id,
+            client_secret=client_secret,
+            redirect_uri=callback_url,
+            scope=scope,
+            code_challenge_method="S256",
+            event_hooks=event_hooks,
+            limits=limits,
+            mounts=mounts,
+            proxies=proxies,
+            timeout=timeout,
+            transport=transport,
+            verify=verify,
+        )
 
-    def generate_authorization_url(self):
-        from twitter_api.types.oauth2.oauth2_authorization import OAuth2Authorization
+    def generate_authorization_url(
+        self,
+    ) -> OAuth2Authorization[TwitterApiGenericClient]:
+        url: Oauth2AuthorizeUrl = "https://twitter.com/i/oauth2/authorize"
+        code_verifier = generate_code_verifier()
+
+        authorization_url, state = self._session.create_authorization_url(
+            url, code_verifier=code_verifier
+        )
 
         return OAuth2Authorization(
-            authorization_url="https://authorization.url.com",
-            state="state",
-            code_verifier="code_verifier",
+            authorization_url=authorization_url,
+            state=state,
+            code_verifier=code_verifier,
             session=self,
         )
 
     def fetch_token(
         self,
         authorization_response_url: CallbackUrl,
         state: str,
         code_verifier: str,
-    ) -> OAuth2AccessToken:
-        expires_in = 7200
+    ) -> OAuth2AccessToken[TwitterApiGenericClient]:
+        url: V2Oauth2TokenUrl = "https://api.twitter.com/2/oauth2/token"
+
+        response = self._session.fetch_token(
+            url=url,
+            authorization_response=authorization_response_url,
+            state=state,
+            code_verifier=code_verifier,
+        )
+
+        scope: Any = response.pop("scope", "").split(" ")
+
+        # 認証のプロセスがすべて終了したので、コネクションを閉じておく。
+        self._session.close()
+
         return OAuth2AccessToken(
-            token_type="bearer",
-            expires_in=expires_in,
-            expires_at=int(datetime.now().timestamp()) + expires_in,
-            access_token="access_token",
-            scope=self._scope,
+            scope=scope,
             _client_generator=self._client_generator,
+            **response,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_session.py` & `twitter_api_py-0.4.0/twitter_api/client/oauth_session/twitter_oauth1_session.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from abc import ABCMeta, abstractmethod
-from typing import Generic
+from typing import Generic, cast
 
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
+from twitter_api.types.http import Url
 from twitter_api.types.oauth import CallbackUrl
 
 
-class TwitterOAuth2Session(Generic[TwitterApiGenericClient], metaclass=ABCMeta):
+class TwitterOAuth1Session(Generic[TwitterApiGenericClient], metaclass=ABCMeta):
+    @abstractmethod
+    def request_token(self):
+        from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
+            TwitterOAuth1AuthorizeClient,
+        )
+
+        return cast(TwitterOAuth1AuthorizeClient[TwitterApiGenericClient], ...)
+
     @abstractmethod
     def generate_authorization_url(
         self,
+        url: Url,
     ):
-        from twitter_api.types.oauth2.oauth2_authorization import OAuth2Authorization
+        from twitter_api.types.oauth1.oauth1_authorization import OAuth1Authorization
 
-        _: OAuth2Authorization[TwitterApiGenericClient] = ...  # type: ignore
-
-        return _
+        return cast(OAuth1Authorization[TwitterApiGenericClient], ...)
 
     @abstractmethod
     def fetch_token(
         self,
         authorization_response_url: CallbackUrl,
-        state: str,
-        code_verifier: str,
     ):
-        from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
-
-        _: OAuth2AccessToken[TwitterApiGenericClient] = ...  # type: ignore
+        from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 
-        return _
+        return cast(OAuth1AccessToken[TwitterApiGenericClient], ...)
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/request/request_async_client.py` & `twitter_api_py-0.4.0/twitter_api/client/request/request_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/client/request/request_async_real_client.py` & `twitter_api_py-0.4.0/twitter_api/client/request/request_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/client/request/request_client.py` & `twitter_api_py-0.4.0/twitter_api/client/request/request_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/client/request/request_mock_client.py` & `twitter_api_py-0.4.0/twitter_api/client/request/request_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/client/request/request_real_client.py` & `twitter_api_py-0.4.0/twitter_api/client/request/request_real_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             if response.is_error:
                 raise TwitterApiResponseFailed(
                     endpoint,
                     url=url,
                     request_headers=headers,
                     query=query,
                     request_body=body if body is not None else None,
-                    response_status_code=response.status_code,
+                    status_code=response.status_code,
                     response_body=response.content,
                 )
             else:
                 raise TwitterApiResponseModelBodyDecodeError(
                     endpoint,
                     response.content,
                 )
@@ -215,15 +215,15 @@
     if response.is_error:
         raise TwitterApiResponseFailed(
             endpoint,
             url=url,
             request_headers=headers,
             query=query,
             request_body=body if body is not None else None,
-            response_status_code=response.status_code,
+            status_code=response.status_code,
             response_body=data,
         )
 
     # If only errors will raise
     if "errors" in data and len(data.keys()) == 1:
         raise TwitterApiResponseError(
             endpoint,
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_client.py` & `twitter_api_py-0.4.0/twitter_api/client/twitter_api_async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 from twitter_api.resources.v2_users import AsyncV2UsersResources, V2UsersUrl
 from twitter_api.resources.v2_users_by import AsyncV2UsersByResources, V2UsersByUrl
 from twitter_api.resources.v2_users_by_username import (
     AsyncV2UsersByUsernameResources,
     V2UsersByUsernameUrl,
 )
 from twitter_api.types import httpx
-from twitter_api.types.chainable import Chainable
+from twitter_api.types._chainable import Chainable
 from twitter_api.types.oauth import (
     AccessSecret,
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
     ClientId,
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_mock_client.py` & `twitter_api_py-0.4.0/twitter_api/client/twitter_api_async_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_real_client.py` & `twitter_api_py-0.4.0/twitter_api/client/twitter_api_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/client/twitter_api_client.py` & `twitter_api_py-0.4.0/twitter_api/client/twitter_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 from twitter_api.resources.v2_users import V2UsersResources, V2UsersUrl
 from twitter_api.resources.v2_users_by import V2UsersByResources, V2UsersByUrl
 from twitter_api.resources.v2_users_by_username import (
     V2UsersByUsernameResources,
     V2UsersByUsernameUrl,
 )
 from twitter_api.types import httpx
-from twitter_api.types.chainable import Chainable
+from twitter_api.types._chainable import Chainable
 from twitter_api.types.oauth import (
     AccessSecret,
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
     ClientId,
```

### Comparing `twitter_api_py-0.3.3/twitter_api/client/twitter_api_mock_client.py` & `twitter_api_py-0.4.0/twitter_api/client/twitter_api_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/client/twitter_api_real_client.py` & `twitter_api_py-0.4.0/twitter_api/client/twitter_api_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/error.py` & `twitter_api_py-0.4.0/twitter_api/error.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,71 +88,71 @@
             レスポンスデータを定義した後で、API を呼んでください。
             """
         )
 
 
 class MockInjectionResponseWrong(TwitterApiError):
     def __init__(self, endpoint: Endpoint, expected_endpoint: Endpoint):
-        self._endpoint = endpoint
-        self._expected_endpoint = expected_endpoint
+        self.endpoint = endpoint
+        self.expected_endpoint = expected_endpoint
 
     @property
     def message(self) -> str:
         return "出力したいレスポンスのエンドポイントが異なっています。"
 
     @property
     def info(self) -> TwitterApiExceptionInfo:
         return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
             message=self.message,
             **dict(
-                expected_endpoint=self._expected_endpoint,
-                endpoint=self._endpoint,
+                expected_endpoint=self.expected_endpoint,
+                endpoint=self.endpoint,
             ),
         )
 
 
 class TwitterApiResponseModelBodyDecodeError(TwitterApiError):
     def __init__(self, endpoint: Endpoint, content: bytes, **extra):
-        self._endpoint = endpoint
-        self._content = content
+        self.endpoint = endpoint
+        self.content = content
         self._extra = extra
 
     @property
     def message(self) -> str:
         return "Twitter API の応答のボディを JSON でパースできませんでした。"
 
     @property
     def info(self) -> TwitterApiExceptionInfo:
         return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
             message=self.message,
-            **dict(endpoint=self._endpoint, content=self._content),
+            **dict(endpoint=self.endpoint, content=self.content),
             **exclude_none(self._extra),
         )
 
 
 class TwitterApiResponseFailed(TwitterApiError):
     def __init__(
         self,
         endpoint: Endpoint,
         url: str,
         request_headers: Optional[Headers],
         query: Optional[QuryParameters],
         request_body: Optional[RequestJsonBody],
-        response_status_code: int,
+        status_code: int,
         response_body: Optional[Union[ResponseJsonBody, bytes]],
     ):
-        self._endpoint = endpoint
-        self._url = url
-        self._request_headers = request_headers
-        self._query = query
-        self._request_body = request_body
-        self.status_code = response_status_code
-        self._response_body = response_body
+        self.endpoint = endpoint
+        self.url = url
+        self.request_headers = request_headers
+        self.query = query
+        self.request_body = request_body
+        self.status_code = status_code
+        self.response_body = response_body
 
     @property
     def message(self) -> str:
         match self.status_code:
             case TwitterApiErrorCode.OK.value:
                 return "API が成功しています。"
             case TwitterApiErrorCode.NotModified.value:
@@ -188,116 +188,118 @@
 
     @property
     def info(self) -> TwitterApiExceptionInfo:
         return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
             message=self.message,
             **OrderedDict(
-                endpoint=self._endpoint,
-                url=self._url,
-                reqeust_headers=exclude_none(self._request_headers),
-                query=exclude_none(self._query),
-                request_body=exclude_none(self._request_body),
-                response_status_code=self.status_code,
+                endpoint=self.endpoint,
+                url=self.url,
+                reqeust_headers=exclude_none(self.request_headers),
+                query=exclude_none(self.query),
+                request_body=exclude_none(self.request_body),
+                status_code=self.status_code,
                 response_body=(
-                    exclude_none(self._response_body)
-                    if not isinstance(self._response_body, bytes)
-                    else self._response_body
+                    exclude_none(self.response_body)
+                    if not isinstance(self.response_body, bytes)
+                    else self.response_body
                 ),
             ),
         )
 
 
 class TwitterApiResponseError(TwitterApiError):
-    def __init__(self, endpoint: Endpoint, data: Any, **extra):
-        self._endpoint = endpoint
-        self._data = data
+    def __init__(self, endpoint: Endpoint, response_body: Any, **extra):
+        self.endpoint = endpoint
+        self.response_body = response_body
         self._extra = extra
 
     @property
     def message(self) -> str:
         return "Twitter API の応答でエラーが返りました。"
 
     @property
     def info(self) -> TwitterApiExceptionInfo:
         return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
             message=self.message,
             **dict(
-                endpoint=self._endpoint,
-                data=exclude_none(self._data),
+                endpoint=self.endpoint,
+                response_body=exclude_none(self.response_body),
             ),
             **exclude_none(self._extra),
         )
 
 
 class TwitterApiResponseValidationError(TwitterApiError):
     def __init__(
         self, endpoint: Endpoint, response_body: Any, error: pydantic.ValidationError
     ):
-        self._endpoint = endpoint
-        self._response_body = response_body
-        self._error = error
+        self.endpoint = endpoint
+        self.response_body = response_body
+        self.error = error
 
     @property
     def message(self) -> str:
         return "Twitter API の応答の型が想定とは一致していません。"
 
     @property
     def info(self) -> TwitterApiExceptionInfo:
-        response_body = exclude_none(self._response_body)
+        response_body = exclude_none(self.response_body)
 
         # 文字が長すぎる場合、切り取る。
         response_body_str = json.dumps(response_body, ensure_ascii=False)
         max_length = 1000
         if len(response_body_str) > max_length:
             response_body = response_body_str[: max_length - 3] + "..."
 
         return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
             message=self.message,
             **dict(
-                endpoint=self._endpoint,
+                endpoint=self.endpoint,
                 response_body=response_body,
-                error=self._error.errors(),
+                errors=self.error.errors(),
             ),
         )
 
 
 class TwitterApiOAuthTokenV1NotFound(TwitterApiError):
-    def __init__(self, endpoint, data: Any, **extra):
-        self._endpoint = endpoint
-        self._data = data
+    def __init__(self, endpoint, response_body: Any, **extra):
+        self.endpoint = endpoint
+        self.response_body = response_body
         self._extra = extra
 
     @property
     def message(self) -> str:
         return "OAuth V1 のトークンが見つかりませんでした。"
 
     @property
     def info(self) -> TwitterApiExceptionInfo:
         return TwitterApiExceptionInfo(
             type=self.__class__.__name__,
             message=self.message,
             **dict(
-                endpoint=self._endpoint,
-                data=exclude_none(self._data),
+                endpoint=self.endpoint,
+                response_body=exclude_none(self.response_body),
             ),
             **exclude_none(self._extra),
         )
 
 
 class TwitterApiOAuthVersionWrong(TwitterApiError):
     def __init__(self, *, version: OAuthVersion, expected_version: OAuthVersion):
-        self._version = version
-        self._expected_version = expected_version
+        self.version = version
+        self.expected_version = expected_version
 
     @property
     def message(self) -> str:
-        return f'OAuth のバージョンは "{self._version}" ではなく "{self._expected_version}" である必要があります。'
+        return (
+            f'OAuth のバージョンは "{self.version}" ではなく "{self.expected_version}" である必要があります。'
+        )
 
 
 class RateLimitOverError(TwitterApiError):
     def __init__(self, rate_limit: RateLimitInfo) -> None:
         self._rate_limit = rate_limit
 
     @property
```

### Comparing `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/__init__.py` & `twitter_api_py-0.4.0/twitter_api/rate_limit/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/dict_rate_limit_manager.py` & `twitter_api_py-0.4.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py` & `twitter_api_py-0.4.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py` & `twitter_api_py-0.4.0/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py` & `twitter_api_py-0.4.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py` & `twitter_api_py-0.4.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/rate_limit_manager.py` & `twitter_api_py-0.4.0/twitter_api/rate_limit/manager/rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/rate_limit/rate_limit.py` & `twitter_api_py-0.4.0/twitter_api/rate_limit/rate_limit.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py` & `twitter_api_py-0.4.0/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/oauth2_token/post_oauth2_token.py` & `twitter_api_py-0.4.0/twitter_api/resources/oauth2_token/post_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversation_messages/__init__.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversation_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
-from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
-from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
-from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.paging import (
+from twitter_api.types._paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
+from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_dm_conversation.dm_conversation_id import DmConversationId
 from twitter_api.types.v2_dm_event.dm_event_expansion import DmEventExpansion
 from twitter_api.types.v2_dm_event.dm_event_field import DmEventField
 from twitter_api.types.v2_dm_event.dm_event_id import DmEventId
 from twitter_api.types.v2_dm_event.dm_event_type import DmEventType
 from twitter_api.types.v2_media.media_key import MediaKey
 from twitter_api.types.v2_scope import oauth2_scopes
```

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/delete_v2_tweet.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweet/delete_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/get_v2_tweet.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweet/get_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
-from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
-from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
-from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.paging import (
+from twitter_api.types._paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
+from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_retweet.retweet import Retweet
 from twitter_api.types.v2_scope import oauth2_scopes
 from twitter_api.types.v2_tweet.tweet import Tweet
 from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.types.v2_user.user_field import UserField
```

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/get_v2_tweets.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweets/get_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/post_v2_tweets.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweets/post_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 from datetime import datetime
-from typing import AsyncGenerator, Generator, Literal, NotRequired, Optional, TypedDict
+from typing import (
+    AsyncGenerator,
+    Generator,
+    Literal,
+    NotRequired,
+    Optional,
+    TypedDict,
+    Union,
+)
 from urllib import parse
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
-from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
-from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.paging import (
+from twitter_api.types._paging import (
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
+from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_media.media_field import MediaField
 from twitter_api.types.v2_place.place_field import PlaceField
 from twitter_api.types.v2_poll.poll_field import PollField
 from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_search_query.search_query import SearchQuery
 from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
 from twitter_api.types.v2_user.user_field import UserField
 from twitter_api.utils._datetime import rfc3339
 from twitter_api.utils._functional import map_optional
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/all")
 
 GetV2TweetsSearchAllQueryParameters = TypedDict(
     "GetV2TweetsSearchAllQueryParameters",
     {
-        "query": str,
+        "query": Union[SearchQuery, str],
         "start_time": NotRequired[Optional[datetime]],
         "end_time": NotRequired[Optional[datetime]],
         "since_id": NotRequired[Optional[TweetId]],
         "until_id": NotRequired[Optional[TweetId]],
         "sort_order": NotRequired[Optional[Literal["recency", "relevancy"]]],
         "next_token": NotRequired[Optional[PaginationToken]],
         "max_results": NotRequired[Optional[int]],
```

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 from datetime import datetime
-from typing import AsyncGenerator, Generator, Literal, NotRequired, Optional, TypedDict
+from typing import (
+    AsyncGenerator,
+    Generator,
+    Literal,
+    NotRequired,
+    Optional,
+    TypedDict,
+    Union,
+)
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
-from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
-from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.paging import (
+from twitter_api.types._paging import (
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
+from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_media.media_field import MediaField
 from twitter_api.types.v2_place.place_field import PlaceField
 from twitter_api.types.v2_poll.poll_field import PollField
 from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_search_query.search_query import SearchQuery
 from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
 from twitter_api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
 from twitter_api.types.v2_user.user_field import UserField
 from twitter_api.utils._datetime import rfc3339
 from twitter_api.utils._functional import map_optional
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/recent")
 
 GetV2TweetsSearchRecentQueryParameters = TypedDict(
     "GetV2TweetsSearchRecentQueryParameters",
     {
-        "query": str,
+        "query": Union[SearchQuery, str],
         "start_time": NotRequired[Optional[datetime]],
         "end_time": NotRequired[Optional[datetime]],
         "since_id": NotRequired[Optional[TweetId]],
         "until_id": NotRequired[Optional[TweetId]],
         "sort_order": NotRequired[Optional[Literal["recency", "relevancy"]]],
         "next_token": NotRequired[Optional[PaginationToken]],
         "max_results": NotRequired[Optional[int]],
```

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_user/get_v2_user.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_user/get_v2_user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_user_followers/get_v2_user_followers.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_user_followers/get_v2_user_followers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
-from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
-from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
-from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.paging import (
+from twitter_api.types._paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
+from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_scope import oauth2_scopes
 from twitter_api.types.v2_tweet.tweet import Tweet
 from twitter_api.types.v2_tweet.tweet_field import TweetField
 from twitter_api.types.v2_user.user import User
 from twitter_api.types.v2_user.user_expantion import UserExpansion
 from twitter_api.types.v2_user.user_field import UserField
 from twitter_api.types.v2_user.user_id import UserId
```

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_user_following/post_v2_user_following.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_user_following/post_v2_user_following.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
-from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
-from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
-from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.paging import (
+from twitter_api.types._paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
+from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_media.media import Media
 from twitter_api.types.v2_media.media_field import MediaField
 from twitter_api.types.v2_place.place import Place
 from twitter_api.types.v2_place.place_field import PlaceField
 from twitter_api.types.v2_poll.poll import Poll
 from twitter_api.types.v2_poll.poll_field import PollField
 from twitter_api.types.v2_scope import oauth2_scopes
```

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,25 @@
     TypedDict,
 )
 
 from pydantic import Field
 
 from twitter_api.rate_limit.rate_limit import rate_limit
 from twitter_api.resources.api_resources import ApiResources
-from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
-from twitter_api.types.endpoint import Endpoint
-from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
-from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.paging import (
+from twitter_api.types._paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
+from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.v2_media.media import Media
 from twitter_api.types.v2_media.media_field import MediaField
 from twitter_api.types.v2_place.place import Place
 from twitter_api.types.v2_place.place_field import PlaceField
 from twitter_api.types.v2_poll.poll import Poll
 from twitter_api.types.v2_poll.poll_field import PollField
 from twitter_api.types.v2_scope import oauth2_scopes
```

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_users/get_v2_users.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_users/get_v2_users.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_users_by/get_v2_users_by.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_users_by/get_v2_users_by.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py` & `twitter_api_py-0.4.0/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/comma_separatable.py` & `twitter_api_py-0.4.0/twitter_api/types/comma_separatable.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/extra_permissive_model.py` & `twitter_api_py-0.4.0/twitter_api/types/extra_permissive_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 from pydantic import Extra
 
-from .model import Model
+from ._model import Model
 
 
 class ExtraPermissiveModel(Model):
     """
     予期しないキーに対しても情報を保存させる基底クラス。
 
     これが python の標準ライブラリに含まれている dataclass ではなく、
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/generic_client.py` & `twitter_api_py-0.4.0/twitter_api/types/_generic_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/http.py` & `twitter_api_py-0.4.0/twitter_api/types/http.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/httpx.py` & `twitter_api_py-0.4.0/twitter_api/types/httpx.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/model.py` & `twitter_api_py-0.4.0/twitter_api/types/_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/oauth.py` & `twitter_api_py-0.4.0/twitter_api/types/oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/oauth1/oauth1_access_token.py` & `twitter_api_py-0.4.0/twitter_api/types/oauth1/oauth1_access_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     Callable,
     Generic,
     Mapping,
     Optional,
     Union,
 )
 
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
-from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import AccessSecret, AccessToken
 from twitter_api.types.v2_user.user_id import UserId
 from twitter_api.types.v2_user.username import Username
 
 if TYPE_CHECKING:
     IntStr = Union[int, str]
     AbstractSetIntStr = AbstractSet[IntStr]
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/oauth1/oauth1_authorization.py` & `twitter_api_py-0.4.0/twitter_api/types/oauth1/oauth1_authorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from textwrap import dedent
 from typing import Callable, Generic, Optional, TextIO
 
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.http import Url
 
 
 class _OAuth1Authorization(Generic[TwitterApiGenericClient]):
     def __init__(
         self,
         *,
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/oauth2/oauth2_access_token.py` & `twitter_api_py-0.4.0/twitter_api/types/oauth2/oauth2_access_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Mapping,
     Optional,
     Union,
 )
 
 from typing_extensions import Literal
 
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
-from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import AccessToken
 from twitter_api.types.v2_scope import Scope
 
 if TYPE_CHECKING:
     IntStr = Union[int, str]
     AbstractSetIntStr = AbstractSet[IntStr]
     MappingIntStrAny = Mapping[IntStr, Any]
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/oauth2/oauth2_authorization.py` & `twitter_api_py-0.4.0/twitter_api/types/oauth2/oauth2_authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from textwrap import dedent
 from typing import Callable, Generic, Optional, TextIO
 
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
-from twitter_api.types.generic_client import TwitterApiGenericClient
+from twitter_api.types._generic_client import TwitterApiGenericClient
 from twitter_api.types.http import Url
 
 
 class _OAuth2Authorization(Generic[TwitterApiGenericClient]):
     def __init__(
         self,
         *,
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/paging.py` & `twitter_api_py-0.4.0/twitter_api/types/_paging.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Callable,
     Coroutine,
     Generator,
     Optional,
     Self,
     TypedDict,
     TypeVar,
+    cast,
 )
 
 from twitter_api.types.pagination_token import PaginationToken
 
 
 class PageResponseBody(metaclass=ABCMeta):
     @property
@@ -40,24 +41,21 @@
     ],
     query: Optional[AnyQueryParameters],
     pagination_token_key: str,
 ) -> Generator[AnyPageResponseBody, None, None]:
     """
     ページングされたレスポンスを返す API に対して、ページングをイテレータで返す。
     """
-    if query is None:
-        _query: AnyQueryParameters = {pagination_token_key: None}  # type: ignore
-    else:
-        _query = query
+    _query = cast(dict, query if query is not None else {pagination_token_key: None})
 
     next_token = _query.get(pagination_token_key)
 
     while True:
-        _query[pagination_token_key] = next_token  # type: ignore
-        response_body = get_func(_query)
+        _query[pagination_token_key] = next_token
+        response_body = get_func(cast(AnyQueryParameters, _query))
 
         yield response_body
 
         next_token = response_body.meta_next_token
 
         if next_token is None:
             return
@@ -90,23 +88,21 @@
     ],
     query: Optional[AnyQueryParameters],
     pagination_token_key: str,
 ) -> AsyncGenerator[AnyPageResponseBody, None]:
     """
     ページングされたレスポンスを返す API に対して、ページングをイテレータで返す。
     """
-    if query is None:
-        _query: AnyQueryParameters = {pagination_token_key: None}  # type: ignore
-    else:
-        _query = query
+    _query = cast(dict, query if query is not None else {pagination_token_key: None})
+
     next_token = _query.get(pagination_token_key)
 
     while True:
-        _query[pagination_token_key] = next_token  # type: ignore
-        response_body = await get_func(_query)
+        _query[pagination_token_key] = next_token
+        response_body = await get_func(cast(AnyQueryParameters, _query))
 
         yield response_body
 
         next_token = response_body.meta_next_token
 
         if next_token is None:
             return
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation_message.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_dm_conversation/dm_conversation_message.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_media/media.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_media/media.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_media/media_field.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_media/media_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_place/place.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_place/place.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.v2_geo.geo import Geo
-from twitter_api.types.v2_place.place_id import PlaceId
+from twitter_api.types.v2_place.place_country_code import PlaceCountryCode
+from twitter_api.types.v2_place.place_name import PlaceName
+
+from .place_full_name import PlaceFullName
+from .place_id import PlaceId
 
 
 class Place(ExtraPermissiveModel):
     """
     場所情報。
 
     refer: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/place
     """
 
     id: PlaceId
-    full_name: str
-    name: Optional[str] = None
+    name: PlaceName
+    full_name: PlaceFullName
     contained_within: Optional[list[Any]] = None
     country: Optional[str] = None
-    country_code: Optional[str] = None
+    # NOTE: 公式ではない国のコードを返す可能性があるため、 str も受け入れておく。
+    country_code: Optional[Union[PlaceCountryCode, str]] = None
     geo: Optional[Geo] = None
     place_type: Optional[str] = None
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_poll/poll.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_retweet/retweet_entities_description.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_scope.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_scope.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import textwrap
 from datetime import datetime
 from typing import Optional
 
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_tweet.tweet_entities_cashtag import TweetEntitiesCashtag
+from twitter_api.types.v2_tweet.tweet_entities_hashtag import TweetEntitiesHashtag
 from twitter_api.types.v2_tweet.tweet_entities_mention import TweetEntitiesMention
 from twitter_api.types.v2_tweet.tweet_entities_url import TweetEntitiesUrl
 
 from ..v2_user.user_id import UserId
 from .tweet_attachments import TweetAttachments
 from .tweet_context_annotation import TweetContextAnnotation
 from .tweet_edit_controls import TweetEditControls
@@ -195,7 +197,51 @@
             return None
 
         for tweet in self.referenced_tweets:
             if tweet.type == "replied_to":
                 return True
 
         return False
+
+    @property
+    def entities_hashtags(self) -> Optional[list[TweetEntitiesHashtag]]:
+        """
+        ハッシュタグ情報。
+        """
+        if self.entities is None or self.entities.hashtags is None:
+            return None
+
+        return self.entities.hashtags
+
+    @property
+    def has_hashtags(self) -> Optional[bool]:
+        """
+        ハッシュタグがついているかどうか。
+
+        None の場合、判断できる情報がない。
+        """
+        if self.entities is None or self.entities.hashtags is None:
+            return None
+
+        return len(self.entities.hashtags) != 0
+
+    @property
+    def entities_cashtags(self) -> Optional[list[TweetEntitiesCashtag]]:
+        """
+        キャッシュタグ情報。
+        """
+        if self.entities is None or self.entities.cashtags is None:
+            return None
+
+        return self.entities.cashtags
+
+    @property
+    def has_cashtags(self) -> Optional[bool]:
+        """
+        キャッシュタグがついているかどうか。
+
+        None の場合、判断できる情報がない。
+        """
+        if self.entities is None or self.entities.cashtags is None:
+            return None
+
+        return len(self.entities.cashtags) != 0
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_entities.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_expansion.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_expansion.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_field.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_response_body.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_tweet/tweet_response_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABCMeta, abstractmethod
 from typing import Optional, Self, Union
 
 from pydantic import Field
 
+from twitter_api.types._paging import PageResponseBody
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.pagination_token import PaginationToken
-from twitter_api.types.paging import PageResponseBody
 from twitter_api.types.v2_media.media import Media
 from twitter_api.types.v2_place.place import Place
 from twitter_api.types.v2_poll.poll import Poll
 from twitter_api.types.v2_tweet.tweet import Tweet
 from twitter_api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.types.v2_user.user import User
```

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_user/user.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_user/user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/types/v2_user/user_field.py` & `twitter_api_py-0.4.0/twitter_api/types/v2_user/user_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/utils/_functional.py` & `twitter_api_py-0.4.0/twitter_api/utils/_functional.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/utils/_oauth.py` & `twitter_api_py-0.4.0/twitter_api/utils/_oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/utils/json.py` & `twitter_api_py-0.4.0/twitter_api/utils/json.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/twitter_api/warning.py` & `twitter_api_py-0.4.0/twitter_api/warning.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.3/PKG-INFO` & `twitter_api_py-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-py
-Version: 0.3.3
+Version: 0.4.0
 Summary: Twitter API Client by Typed Python.
 Home-page: https://github.com/yassun4dev/twitter-api-py
 License: BSD-3-Clause
 Author: yassun4dev
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

