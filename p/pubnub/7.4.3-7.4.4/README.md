# Comparing `tmp/pubnub-7.4.3.tar.gz` & `tmp/pubnub-7.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubnub-7.4.3.tar", last modified: Thu Mar 28 14:56:55 2024, max compression
+gzip compressed data, was "pubnub-7.4.4.tar", last modified: Wed Apr 10 16:47:46 2024, max compression
```

## Comparing `pubnub-7.4.3.tar` & `pubnub-7.4.4.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.815835 pubnub-7.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-28 14:56:28.000000 pubnub-7.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-28 14:56:55.815835 pubnub-7.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-03-28 14:56:28.000000 pubnub-7.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.795835 pubnub-7.4.3/pubnub/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/crypto_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/dtos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.795835 pubnub-7.4.3/pubnub/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.799835 pubnub-7.4.3/pubnub/endpoints/access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/access/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/access/grant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/access/grant_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/access/revoke_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.799835 pubnub-7.4.3/pubnub/endpoints/channel_groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/channel_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/channel_groups/remove_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.799835 pubnub-7.4.3/pubnub/endpoints/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.799835 pubnub-7.4.3/pubnub/endpoints/entities/membership/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/membership/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/membership/add_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/membership/fetch_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/membership/remove_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/membership/update_memberships.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.799835 pubnub-7.4.3/pubnub/endpoints/entities/space/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/space/create_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/space/fetch_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/space/fetch_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/space/remove_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/space/update_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.799835 pubnub-7.4.3/pubnub/endpoints/entities/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/user/create_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/user/fetch_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/user/fetch_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/user/remove_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/entities/user/update_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/fetch_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.803835 pubnub-7.4.3/pubnub/endpoints/file_operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/delete_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/download_file_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/fetch_upload_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/file_based_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/list_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/publish_file_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/file_operations/send_file_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/history_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.803835 pubnub-7.4.3/pubnub/endpoints/message_actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/message_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/message_actions/add_message_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/message_actions/get_message_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/message_actions/remove_message_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/message_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.803835 pubnub-7.4.3/pubnub/endpoints/objects_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.803835 pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/get_all_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/get_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/remove_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/set_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.803835 pubnub-7.4.3/pubnub/endpoints/objects_v2/members/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/members/get_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/members/manage_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/members/remove_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/members/set_channel_members.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.803835 pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/get_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/manage_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/remove_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/set_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/objects_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.807835 pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/get_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/remove_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/set_uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.807835 pubnub-7.4.3/pubnub/endpoints/presence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/presence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/presence/get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/presence/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/presence/here_now.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/presence/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/presence/set_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/presence/where_now.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.807835 pubnub-7.4.3/pubnub/endpoints/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/pubsub/fire.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/pubsub/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/pubsub/subscribe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.807835 pubnub-7.4.3/pubnub/endpoints/push/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/push/add_channels_to_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/push/list_push_provisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/push/remove_channels_from_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/push/remove_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/endpoints/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.807835 pubnub-7.4.3/pubnub/event_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/effects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.807835 pubnub-7.4.3/pubnub/event_engine/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/models/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/models/invocations.py
--rw-r--r--   0 runner    (1001) docker     (127)    37253 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/models/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/event_engine/statemachine.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19670 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.807835 pubnub-7.4.3/pubnub/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.811835 pubnub-7.4.3/pubnub/models/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/access_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.811835 pubnub-7.4.3/pubnub/models/consumer/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/entities/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/entities/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/entities/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/entities/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/entities/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/message_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/message_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.811835 pubnub-7.4.3/pubnub/models/consumer/objects_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/objects_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/objects_v2/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/objects_v2/channel_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/objects_v2/memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/objects_v2/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/objects_v2/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/objects_v2/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/pn_error_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/push.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.815835 pubnub-7.4.3/pubnub/models/consumer/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/v3/access_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/v3/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/v3/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/v3/pn_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/v3/space.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/v3/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/consumer/v3/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.815835 pubnub-7.4.3/pubnub/models/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/server/subscribe.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/models/subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/pnconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/pubnub.py
--rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/pubnub_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/pubnub_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.815835 pubnub-7.4.3/pubnub/request_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/request_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/request_handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/request_handlers/requests_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-03-28 14:56:28.000000 pubnub-7.4.3/pubnub/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:56:55.815835 pubnub-7.4.3/pubnub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-28 14:56:55.000000 pubnub-7.4.3/pubnub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-03-28 14:56:55.000000 pubnub-7.4.3/pubnub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:56:55.000000 pubnub-7.4.3/pubnub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:56:55.000000 pubnub-7.4.3/pubnub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 14:56:55.000000 pubnub-7.4.3/pubnub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 14:56:55.000000 pubnub-7.4.3/pubnub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-28 14:56:55.815835 pubnub-7.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-28 14:56:28.000000 pubnub-7.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.838263 pubnub-7.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-10 16:47:34.000000 pubnub-7.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-10 16:47:46.838263 pubnub-7.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-10 16:47:34.000000 pubnub-7.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.818263 pubnub-7.4.4/pubnub/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/crypto_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/dtos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.818263 pubnub-7.4.4/pubnub/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/grant_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/revoke_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/channel_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/remove_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/entities/membership/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/add_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/fetch_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/remove_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/update_memberships.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/entities/space/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/create_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/fetch_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/fetch_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/remove_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/update_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/entities/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/fetch_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/fetch_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/remove_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/update_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/fetch_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/file_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/download_file_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/fetch_upload_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/file_based_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/publish_file_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/send_file_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/history_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/message_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_actions/add_message_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_actions/get_message_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_actions/remove_message_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/get_all_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/get_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/remove_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/set_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/get_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/manage_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/remove_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/set_channel_members.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/get_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/manage_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/remove_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/set_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/objects_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/get_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/remove_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/set_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/endpoints/presence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/here_now.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/set_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/where_now.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/endpoints/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/pubsub/fire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/pubsub/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/pubsub/subscribe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/endpoints/push/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/add_channels_to_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/list_push_provisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/remove_channels_from_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/remove_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/event_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20582 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/effects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/event_engine/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/models/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41947 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/models/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/statemachine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19670 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.834263 pubnub-7.4.4/pubnub/models/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/access_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.834263 pubnub-7.4.4/pubnub/models/consumer/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/message_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/message_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.834263 pubnub-7.4.4/pubnub/models/consumer/objects_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/pn_error_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.834263 pubnub-7.4.4/pubnub/models/consumer/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/access_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/pn_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.838263 pubnub-7.4.4/pubnub/models/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/server/subscribe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/pnconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/pubnub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30155 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/pubnub_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/pubnub_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.838263 pubnub-7.4.4/pubnub/request_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/request_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/request_handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/request_handlers/requests_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.838263 pubnub-7.4.4/pubnub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 16:47:46.838263 pubnub-7.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 16:47:34.000000 pubnub-7.4.4/setup.py
```

### Comparing `pubnub-7.4.3/LICENSE` & `pubnub-7.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/PKG-INFO` & `pubnub-7.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubnub
-Version: 7.4.3
+Version: 7.4.4
 Summary: PubNub Real-time push service in the cloud
 Home-page: http://pubnub.com
 Author: PubNub
 Author-email: support@pubnub.com
 License: PubNub Software Development Kit License
 Project-URL: Source, https://github.com/pubnub/python
 Project-URL: Documentation, https://www.pubnub.com/docs/sdks/python
```

### Comparing `pubnub-7.4.3/README.md` & `pubnub-7.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/__init__.py` & `pubnub-7.4.4/pubnub/__init__.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/builders.py` & `pubnub-7.4.4/pubnub/builders.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/callbacks.py` & `pubnub-7.4.4/pubnub/callbacks.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/crypto.py` & `pubnub-7.4.4/pubnub/crypto.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/crypto_core.py` & `pubnub-7.4.4/pubnub/crypto_core.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/dtos.py` & `pubnub-7.4.4/pubnub/dtos.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/access/audit.py` & `pubnub-7.4.4/pubnub/endpoints/access/audit.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/access/grant.py` & `pubnub-7.4.4/pubnub/endpoints/access/grant.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/access/grant_token.py` & `pubnub-7.4.4/pubnub/endpoints/access/grant_token.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/access/revoke_token.py` & `pubnub-7.4.4/pubnub/endpoints/access/revoke_token.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py` & `pubnub-7.4.4/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py` & `pubnub-7.4.4/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py` & `pubnub-7.4.4/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/channel_groups/remove_channel_group.py` & `pubnub-7.4.4/pubnub/endpoints/channel_groups/remove_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/endpoint.py` & `pubnub-7.4.4/pubnub/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/endpoint.py` & `pubnub-7.4.4/pubnub/endpoints/entities/endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/membership/add_memberships.py` & `pubnub-7.4.4/pubnub/endpoints/entities/membership/add_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/membership/fetch_memberships.py` & `pubnub-7.4.4/pubnub/endpoints/entities/membership/fetch_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/membership/remove_memberships.py` & `pubnub-7.4.4/pubnub/endpoints/entities/membership/remove_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/membership/update_memberships.py` & `pubnub-7.4.4/pubnub/endpoints/entities/membership/update_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/space/create_space.py` & `pubnub-7.4.4/pubnub/endpoints/entities/space/create_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/space/fetch_space.py` & `pubnub-7.4.4/pubnub/endpoints/entities/space/fetch_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/space/fetch_spaces.py` & `pubnub-7.4.4/pubnub/endpoints/entities/space/fetch_spaces.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/space/remove_space.py` & `pubnub-7.4.4/pubnub/endpoints/entities/space/remove_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/space/update_space.py` & `pubnub-7.4.4/pubnub/endpoints/entities/space/update_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/user/create_user.py` & `pubnub-7.4.4/pubnub/endpoints/entities/user/create_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/user/fetch_user.py` & `pubnub-7.4.4/pubnub/endpoints/entities/user/fetch_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/user/fetch_users.py` & `pubnub-7.4.4/pubnub/endpoints/entities/user/fetch_users.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/user/remove_user.py` & `pubnub-7.4.4/pubnub/endpoints/entities/user/remove_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/entities/user/update_user.py` & `pubnub-7.4.4/pubnub/endpoints/entities/user/update_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/fetch_messages.py` & `pubnub-7.4.4/pubnub/endpoints/fetch_messages.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/delete_file.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/delete_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/download_file.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/download_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/download_file_asyncio.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/download_file_asyncio.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/fetch_upload_details.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/fetch_upload_details.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/get_file_url.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/get_file_url.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/list_files.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/list_files.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/publish_file_message.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/publish_file_message.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/send_file.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/send_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/file_operations/send_file_asyncio.py` & `pubnub-7.4.4/pubnub/endpoints/file_operations/send_file_asyncio.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/history.py` & `pubnub-7.4.4/pubnub/endpoints/history.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/history_delete.py` & `pubnub-7.4.4/pubnub/endpoints/history_delete.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/message_actions/add_message_action.py` & `pubnub-7.4.4/pubnub/endpoints/message_actions/add_message_action.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/message_actions/get_message_actions.py` & `pubnub-7.4.4/pubnub/endpoints/message_actions/get_message_actions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/message_actions/remove_message_action.py` & `pubnub-7.4.4/pubnub/endpoints/message_actions/remove_message_action.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/message_count.py` & `pubnub-7.4.4/pubnub/endpoints/message_count.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/mixins.py` & `pubnub-7.4.4/pubnub/endpoints/mixins.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/get_all_channels.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/get_all_channels.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/get_channel.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/get_channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/remove_channel.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/remove_channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/channel/set_channel.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/set_channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/members/get_channel_members.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/members/get_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/members/manage_channel_members.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/members/manage_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/members/remove_channel_members.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/members/remove_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/members/set_channel_members.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/members/set_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/get_memberships.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/get_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/manage_memberships.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/manage_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/remove_memberships.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/remove_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/memberships/set_memberships.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/set_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/objects_endpoint.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/objects_endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/get_uuid.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/get_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/remove_uuid.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/remove_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/objects_v2/uuid/set_uuid.py` & `pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/set_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/presence/get_state.py` & `pubnub-7.4.4/pubnub/endpoints/presence/get_state.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/presence/heartbeat.py` & `pubnub-7.4.4/pubnub/endpoints/presence/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/presence/here_now.py` & `pubnub-7.4.4/pubnub/endpoints/presence/here_now.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/presence/leave.py` & `pubnub-7.4.4/pubnub/endpoints/presence/leave.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/presence/set_state.py` & `pubnub-7.4.4/pubnub/endpoints/presence/set_state.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/presence/where_now.py` & `pubnub-7.4.4/pubnub/endpoints/presence/where_now.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/pubsub/fire.py` & `pubnub-7.4.4/pubnub/endpoints/pubsub/fire.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/pubsub/publish.py` & `pubnub-7.4.4/pubnub/endpoints/pubsub/publish.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/pubsub/subscribe.py` & `pubnub-7.4.4/pubnub/endpoints/pubsub/subscribe.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/push/add_channels_to_push.py` & `pubnub-7.4.4/pubnub/endpoints/push/add_channels_to_push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/push/list_push_provisions.py` & `pubnub-7.4.4/pubnub/endpoints/push/list_push_provisions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/push/remove_channels_from_push.py` & `pubnub-7.4.4/pubnub/endpoints/push/remove_channels_from_push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/push/remove_device.py` & `pubnub-7.4.4/pubnub/endpoints/push/remove_device.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/signal.py` & `pubnub-7.4.4/pubnub/endpoints/signal.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/endpoints/time.py` & `pubnub-7.4.4/pubnub/endpoints/time.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/enums.py` & `pubnub-7.4.4/pubnub/enums.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/errors.py` & `pubnub-7.4.4/pubnub/errors.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/event_engine/containers.py` & `pubnub-7.4.4/pubnub/event_engine/containers.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/event_engine/dispatcher.py` & `pubnub-7.4.4/pubnub/event_engine/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/event_engine/effects.py` & `pubnub-7.4.4/pubnub/event_engine/effects.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,19 @@
 
     def get_new_stop_event(self):
         event = asyncio.Event()
         self.logger.debug(f'creating new stop_event({id(event)}) for {self.__class__.__name__}')
         return event
 
     def calculate_reconnection_delay(self, attempts):
-        if self.reconnection_policy is PNReconnectionPolicy.LINEAR:
+        if self.reconnection_policy is PNReconnectionPolicy.EXPONENTIAL:
+            delay = int(math.pow(2, attempts - 5 * math.floor((attempts - 1) / 5)) - 1)
+        else:
             delay = self.interval
 
-        elif self.reconnection_policy is PNReconnectionPolicy.EXPONENTIAL:
-            delay = int(math.pow(2, attempts - 5 * math.floor((attempts - 1) / 5)) - 1)
         return delay
 
 
 class HandshakeEffect(Effect):
     def run(self):
         channels = self.invocation.channels
         groups = self.invocation.groups
@@ -84,17 +84,17 @@
         if feature_enabled('PN_MAINTAIN_PRESENCE_STATE') and hasattr(self.pubnub, 'state_container'):
             state_container = self.pubnub.state_container
             request.state(state_container.get_state(channels))
 
         request.timetoken(0)
         response = await request.future()
 
-        if isinstance(response, PubNubException):
+        if isinstance(response, Exception):
             self.logger.warning(f'Handshake failed: {str(response)}')
-            handshake_failure = events.HandshakeFailureEvent(str(response), 1, timetoken=timetoken)
+            handshake_failure = events.HandshakeFailureEvent(response, 1, timetoken=timetoken)
             self.event_engine.trigger(handshake_failure)
         elif response.status.error:
             self.logger.warning(f'Handshake failed: {response.status.error_data.__dict__}')
             handshake_failure = events.HandshakeFailureEvent(response.status.error_data, 1, timetoken=timetoken)
             self.event_engine.trigger(handshake_failure)
         else:
             cursor = response.result['t']
@@ -288,15 +288,15 @@
 
         response = await request.future()
 
         if isinstance(response, PubNubException):
             self.logger.warning(f'Heartbeat failed: {str(response)}')
             self.event_engine.trigger(events.HeartbeatFailureEvent(channels=channels, groups=groups,
                                                                    reason=response.status.error_data, attempt=1))
-        elif response.status.error:
+        elif response.status and response.status.error:
             self.logger.warning(f'Heartbeat failed: {response.status.error_data.__dict__}')
             self.event_engine.trigger(events.HeartbeatFailureEvent(channels=channels, groups=groups,
                                                                    reason=response.status.error_data, attempt=1))
         else:
             self.event_engine.trigger(events.HeartbeatSuccessEvent(channels=channels, groups=groups))
 
 
@@ -423,9 +423,10 @@
         for message in invocation.messages:
             subscribe_message = SubscribeMessage().from_json(message)
             self.message_worker._process_incoming_payload(subscribe_message)
 
     def emit_status(self, invocation: invocations.EmitStatusInvocation):
         pn_status = PNStatus()
         pn_status.category = invocation.status
+        pn_status.operation = invocation.operation
         pn_status.error = False
         self.pubnub._subscription_manager._listener_manager.announce_status(pn_status)
```

### Comparing `pubnub-7.4.3/pubnub/event_engine/models/events.py` & `pubnub-7.4.4/pubnub/event_engine/models/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,29 +98,34 @@
     pass
 
 
 class ReconnectEvent(PNEvent):
     pass
 
 
+class UnsubscribeAllEvent(PNEvent):
+    pass
+
+
 """
     Presence Events
 """
 
 
 class HeartbeatJoinedEvent(PNChannelGroupsEvent):
     pass
 
 
 class HeartbeatReconnectEvent(PNEvent):
     pass
 
 
 class HeartbeatLeftAllEvent(PNEvent):
-    pass
+    def __init__(self, suppress_leave: bool = False) -> None:
+        self.suppress_leave = suppress_leave
 
 
 class HeartbeatLeftEvent(PNChannelGroupsEvent):
     def __init__(self, channels: List[str], groups: List[str], suppress_leave: bool = False) -> None:
         PNChannelGroupsEvent.__init__(self, channels, groups)
         self.suppress_leave = suppress_leave
```

### Comparing `pubnub-7.4.3/pubnub/event_engine/models/invocations.py` & `pubnub-7.4.4/pubnub/event_engine/models/invocations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Union
 from pubnub.exceptions import PubNubException
-from pubnub.enums import PNStatusCategory
+from pubnub.enums import PNOperationType, PNStatusCategory
 
 
 class PNInvocation:
     pass
 
 
 class PNManageableInvocation(PNInvocation):
@@ -86,17 +86,18 @@
 class EmitMessagesInvocation(PNEmittableInvocation):
     def __init__(self, messages: Union[None, List[str]]) -> None:
         super().__init__()
         self.messages = messages
 
 
 class EmitStatusInvocation(PNEmittableInvocation):
-    def __init__(self, status: Union[None, PNStatusCategory]) -> None:
+    def __init__(self, status: Union[None, PNStatusCategory], operation: Union[None, PNOperationType] = None) -> None:
         super().__init__()
         self.status = status
+        self.operation = operation
 
 
 """
     Presence Effects
 """
```

### Comparing `pubnub-7.4.3/pubnub/event_engine/models/states.py` & `pubnub-7.4.4/pubnub/event_engine/models/states.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pubnub.enums import PNStatusCategory
+from pubnub.enums import PNOperationType, PNStatusCategory
 from pubnub.event_engine.models import invocations
 from pubnub.event_engine.models.invocations import PNInvocation
 from pubnub.event_engine.models import events
 from pubnub.exceptions import PubNubException
 from typing import List, Union
 
 
@@ -95,14 +95,15 @@
         super().__init__(context)
         self._transitions = {
             events.HandshakeFailureEvent.__name__: self.reconnecting,
             events.DisconnectEvent.__name__: self.disconnect,
             events.HandshakeSuccessEvent.__name__: self.handshaking_success,
             events.SubscriptionRestoredEvent.__name__: self.subscription_restored,
             events.SubscriptionChangedEvent.__name__: self.subscription_changed,
+            events.UnsubscribeAllEvent.__name__: self.unsubscribe_all,
         }
 
     def on_enter(self, context: Union[None, PNContext]):
         self._context.update(context)
         super().on_enter(self._context)
         return invocations.HandshakeInvocation(self._context.channels,
                                                self._context.groups,
@@ -167,14 +168,29 @@
 
         return PNTransition(
             state=ReceivingState,
             context=self._context,
             invocation=invocations.EmitStatusInvocation(PNStatusCategory.PNConnectedCategory)
         )
 
+    def unsubscribe_all(self, event: events.UnsubscribeAllEvent, context: PNContext) -> PNTransition:
+        self._context.update(context)
+        self._context.timetoken = 0
+        self._context.region = None
+        self._context.attempt = 0
+        self._context.channels = []
+        self._context.groups = []
+
+        return PNTransition(
+            state=UnsubscribedState,
+            context=self._context,
+            invocation=invocations.EmitStatusInvocation(PNStatusCategory.PNAcknowledgmentCategory,
+                                                        operation=PNOperationType.PNUnsubscribeOperation)
+        )
+
 
 class HandshakeReconnectingState(PNState):
     def __init__(self, context: PNContext) -> None:
         super().__init__(context)
         self._transitions = {
             events.DisconnectEvent.__name__: self.disconnect,
             events.HandshakeReconnectGiveupEvent.__name__: self.give_up,
@@ -227,19 +243,26 @@
             context=self._context
         )
 
     def give_up(self, event: events.HandshakeReconnectGiveupEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
         self._context.attempt = event.attempt
         self._context.reason = event.reason
+        status_invocation = None
+
+        if isinstance(event, Exception) and 'status' in event.reason:
+            status_invocation = invocations.EmitStatusInvocation(status=event.reason.status.category,
+                                                                 operation=PNOperationType.PNUnsubscribeOperation)
+        else:
+            status_invocation = invocations.EmitStatusInvocation(PNStatusCategory.PNDisconnectedCategory)
 
         return PNTransition(
             state=HandshakeFailedState,
             context=self._context,
-            invocation=invocations.EmitStatusInvocation(PNStatusCategory.PNDisconnectedCategory)
+            invocation=status_invocation
         )
 
     def subscription_restored(self, event: events.SubscriptionRestoredEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
         self._context.channels = event.channels
         self._context.groups = event.groups
         self._context.with_presence = event.with_presence
@@ -266,14 +289,15 @@
 class HandshakeFailedState(PNState):
     def __init__(self, context: PNContext) -> None:
         super().__init__(context)
         self._transitions = {
             events.SubscriptionChangedEvent.__name__: self.subscription_changed,
             events.ReconnectEvent.__name__: self.reconnect,
             events.SubscriptionRestoredEvent.__name__: self.subscription_restored,
+            events.UnsubscribeAllEvent.__name__: self.unsubscribe_all,
         }
 
     def subscription_changed(self, event: events.SubscriptionChangedEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
         self._context.channels = event.channels
         self._context.groups = event.groups
         self._context.with_presence = event.with_presence
@@ -301,45 +325,77 @@
         self._context.region = event.region
 
         return PNTransition(
             state=ReceivingState,
             context=self._context
         )
 
+    def unsubscribe_all(self, event: events.UnsubscribeAllEvent, context: PNContext) -> PNTransition:
+        self._context.update(context)
+        self._context.timetoken = 0
+        self._context.region = None
+        self._context.attempt = 0
+        self._context.channels = []
+        self._context.groups = []
+
+        return PNTransition(
+            state=UnsubscribedState,
+            context=self._context,
+            invocation=invocations.EmitStatusInvocation(PNStatusCategory.PNAcknowledgmentCategory,
+                                                        operation=PNOperationType.PNUnsubscribeOperation)
+        )
+
 
 class HandshakeStoppedState(PNState):
     def __init__(self, context: PNContext) -> None:
         super().__init__(context)
         self._context.attempt = 0
 
         self._transitions = {
-            events.ReconnectEvent.__name__: self.reconnect
+            events.ReconnectEvent.__name__: self.reconnect,
+            events.UnsubscribeAllEvent.__name__: self.unsubscribe_all,
         }
 
     def reconnect(self, event: events.ReconnectEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
 
         return PNTransition(
             state=HandshakeReconnectingState,
             context=self._context
         )
 
+    def unsubscribe_all(self, event: events.UnsubscribeAllEvent, context: PNContext) -> PNTransition:
+        self._context.update(context)
+        self._context.timetoken = 0
+        self._context.region = None
+        self._context.attempt = 0
+        self._context.channels = []
+        self._context.groups = []
+
+        return PNTransition(
+            state=UnsubscribedState,
+            context=self._context,
+            invocation=invocations.EmitStatusInvocation(PNStatusCategory.PNAcknowledgmentCategory,
+                                                        operation=PNOperationType.PNUnsubscribeOperation)
+        )
+
 
 class ReceivingState(PNState):
     def __init__(self, context: PNContext) -> None:
         super().__init__(context)
         self._context.attempt = 0
 
         self._transitions = {
             events.SubscriptionChangedEvent.__name__: self.subscription_changed,
             events.SubscriptionRestoredEvent.__name__: self.subscription_restored,
             events.ReceiveSuccessEvent.__name__: self.receiving_success,
             events.ReceiveFailureEvent.__name__: self.receiving_failure,
             events.DisconnectEvent.__name__: self.disconnect,
             events.ReconnectEvent.__name__: self.reconnect,
+            events.UnsubscribeAllEvent.__name__: self.unsubscribe_all,
         }
 
     def on_enter(self, context: Union[None, PNContext]):
         super().on_enter(context)
         return invocations.ReceiveMessagesInvocation(context.channels, context.groups,
                                                      timetoken=self._context.timetoken, region=self._context.region)
 
@@ -406,14 +462,29 @@
         self._context.update(context)
 
         return PNTransition(
             state=ReceivingState,
             context=self._context
         )
 
+    def unsubscribe_all(self, event: events.UnsubscribeAllEvent, context: PNContext) -> PNTransition:
+        self._context.update(context)
+        self._context.timetoken = 0
+        self._context.region = None
+        self._context.attempt = 0
+        self._context.channels = []
+        self._context.groups = []
+
+        return PNTransition(
+            state=UnsubscribedState,
+            context=self._context,
+            invocation=invocations.EmitStatusInvocation(PNStatusCategory.PNAcknowledgmentCategory,
+                                                        operation=PNOperationType.PNUnsubscribeOperation)
+        )
+
 
 class ReceiveReconnectingState(PNState):
     def __init__(self, context: PNContext) -> None:
         super().__init__(context)
         self._transitions = {
             events.ReceiveReconnectFailureEvent.__name__: self.reconnect_failure,
             events.SubscriptionChangedEvent.__name__: self.subscription_changed,
@@ -507,14 +578,15 @@
     def __init__(self, context: PNContext) -> None:
         super().__init__(context)
         self._transitions = {
             events.ReceiveReconnectRetryEvent.__name__: self.reconnect_retry,
             events.SubscriptionChangedEvent.__name__: self.subscription_changed,
             events.SubscriptionRestoredEvent.__name__: self.subscription_restored,
             events.ReconnectEvent.__name__: self.reconnect,
+            events.UnsubscribeAllEvent.__name__: self.unsubscribe_all,
         }
 
     def reconnect_retry(self, event: events.ReceiveReconnectRetryEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
 
         return PNTransition(
             state=ReceiveReconnectingState,
@@ -550,32 +622,63 @@
         self._context.region = event.region
 
         return PNTransition(
             state=ReceivingState,
             context=self._context
         )
 
+    def unsubscribe_all(self, event: events.UnsubscribeAllEvent, context: PNContext) -> PNTransition:
+        self._context.update(context)
+        self._context.timetoken = 0
+        self._context.region = None
+        self._context.attempt = 0
+        self._context.channels = []
+        self._context.groups = []
+
+        return PNTransition(
+            state=UnsubscribedState,
+            context=self._context,
+            invocation=invocations.EmitStatusInvocation(PNStatusCategory.PNAcknowledgmentCategory,
+                                                        operation=PNOperationType.PNUnsubscribeOperation)
+        )
+
 
 class ReceiveStoppedState(PNState):
     def __init__(self, context: PNContext) -> None:
         super().__init__(context)
         self._context.attempt = 0
 
         self._transitions = {
-            events.ReconnectEvent.__name__: self.reconnect
+            events.ReconnectEvent.__name__: self.reconnect,
+            events.UnsubscribeAllEvent.__name__: self.unsubscribe_all,
         }
 
     def reconnect(self, event: events.ReconnectEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
 
         return PNTransition(
             state=ReceiveReconnectingState,
             context=self._context
         )
 
+    def unsubscribe_all(self, event: events.UnsubscribeAllEvent, context: PNContext) -> PNTransition:
+        self._context.update(context)
+        self._context.timetoken = 0
+        self._context.region = None
+        self._context.attempt = 0
+        self._context.channels = []
+        self._context.groups = []
+
+        return PNTransition(
+            state=UnsubscribedState,
+            context=self._context,
+            invocation=invocations.EmitStatusInvocation(PNStatusCategory.PNAcknowledgmentCategory,
+                                                        operation=PNOperationType.PNUnsubscribeOperation)
+        )
+
 
 """
 Presence states
 """
 
 
 class HeartbeatInactiveState(PNState):
@@ -707,21 +810,20 @@
             state=HeartbeatStoppedState,
             context=self._context,
             invocation=invocation
         )
 
     def left_all(self, event: events.HeartbeatLeftAllEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
-        self._context.channels = []
-        self._context.groups = []
-
         invocation = None
         if not event.suppress_leave:
-            invocation = invocations.HeartbeatLeaveInvocation(channels=event.channels,
-                                                              groups=event.groups)
+            invocation = invocations.HeartbeatLeaveInvocation(channels=self._context.channels,
+                                                              groups=self._context.groups)
+        self._context.channels = []
+        self._context.groups = []
 
         return PNTransition(
             state=HeartbeatInactiveState,
             context=self._context,
             invocation=invocation
         )
 
@@ -765,21 +867,20 @@
             state=HeartbeatStoppedState,
             context=self._context,
             invocation=invocation
         )
 
     def left_all(self, event: events.HeartbeatLeftAllEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
-        self._context.channels = []
-        self._context.groups = []
-
         invocation = None
         if not event.suppress_leave:
-            invocation = invocations.HeartbeatLeaveInvocation(channels=event.channels,
-                                                              groups=event.groups)
+            invocation = invocations.HeartbeatLeaveInvocation(channels=self._context.channels,
+                                                              groups=self._context.groups)
+        self._context.channels = []
+        self._context.groups = []
 
         return PNTransition(
             state=HeartbeatInactiveState,
             context=self._context,
             invocation=invocation
         )
 
@@ -853,21 +954,20 @@
             state=HeartbeatStoppedState,
             context=self._context,
             invocation=invocation
         )
 
     def left_all(self, event: events.HeartbeatLeftAllEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
-        self._context.channels = []
-        self._context.groups = []
-
         invocation = None
         if not event.suppress_leave:
-            invocation = invocations.HeartbeatLeaveInvocation(channels=event.channels,
-                                                              groups=event.groups)
+            invocation = invocations.HeartbeatLeaveInvocation(channels=self._context.channels,
+                                                              groups=self._context.groups)
+        self._context.channels = []
+        self._context.groups = []
 
         return PNTransition(
             state=HeartbeatInactiveState,
             context=self._context,
             invocation=invocation
         )
 
@@ -1001,20 +1101,19 @@
             state=HeartbeatStoppedState,
             context=self._context,
             invocation=invocation
         )
 
     def left_all(self, event: events.HeartbeatLeftAllEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
-        self._context.channels = []
-        self._context.groups = []
-
         invocation = None
         if not event.suppress_leave:
-            invocation = invocations.HeartbeatLeaveInvocation(channels=event.channels,
-                                                              groups=event.groups)
+            invocation = invocations.HeartbeatLeaveInvocation(channels=self._context.channels,
+                                                              groups=self._context.groups)
+        self._context.channels = []
+        self._context.groups = []
 
         return PNTransition(
             state=HeartbeatInactiveState,
             context=self._context,
             invocation=invocation
         )
```

### Comparing `pubnub-7.4.3/pubnub/event_engine/statemachine.py` & `pubnub-7.4.4/pubnub/event_engine/statemachine.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         else:
             self.logger.warning(f'Unhandled event: {event.get_name()} in {self.get_state_name()}')
 
         self.dispatch_effects()
 
     def dispatch_effects(self):
         for invocation in self._invocations:
-            self.logger.debug(f'Dispatching {invocation.__class__.__name__} {id(invocation)}')
+            self.logger.debug(f'Dispatching {invocation.__class__.__name__} {invocation.__dict__} {id(invocation)}')
             self._dispatcher.dispatch_effect(invocation)
 
         self._invocations.clear()
 
     def stop(self):
         self._enabled = False
```

### Comparing `pubnub-7.4.3/pubnub/exceptions.py` & `pubnub-7.4.4/pubnub/exceptions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/features.py` & `pubnub-7.4.4/pubnub/features.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/managers.py` & `pubnub-7.4.4/pubnub/managers.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/access_manager.py` & `pubnub-7.4.4/pubnub/models/consumer/access_manager.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/channel_group.py` & `pubnub-7.4.4/pubnub/models/consumer/channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/common.py` & `pubnub-7.4.4/pubnub/models/consumer/common.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/entities/membership.py` & `pubnub-7.4.4/pubnub/models/consumer/entities/membership.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/entities/page.py` & `pubnub-7.4.4/pubnub/models/consumer/entities/page.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/entities/space.py` & `pubnub-7.4.4/pubnub/models/consumer/entities/space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/entities/user.py` & `pubnub-7.4.4/pubnub/models/consumer/entities/user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/file.py` & `pubnub-7.4.4/pubnub/models/consumer/file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/history.py` & `pubnub-7.4.4/pubnub/models/consumer/history.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/message_actions.py` & `pubnub-7.4.4/pubnub/models/consumer/message_actions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/objects_v2/channel.py` & `pubnub-7.4.4/pubnub/models/consumer/objects_v2/channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/objects_v2/channel_members.py` & `pubnub-7.4.4/pubnub/models/consumer/objects_v2/channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/objects_v2/memberships.py` & `pubnub-7.4.4/pubnub/models/consumer/objects_v2/memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/objects_v2/page.py` & `pubnub-7.4.4/pubnub/models/consumer/objects_v2/page.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/objects_v2/sort.py` & `pubnub-7.4.4/pubnub/models/consumer/objects_v2/sort.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/objects_v2/uuid.py` & `pubnub-7.4.4/pubnub/models/consumer/objects_v2/uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/presence.py` & `pubnub-7.4.4/pubnub/models/consumer/presence.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/pubsub.py` & `pubnub-7.4.4/pubnub/models/consumer/pubsub.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/push.py` & `pubnub-7.4.4/pubnub/models/consumer/push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/time.py` & `pubnub-7.4.4/pubnub/models/consumer/time.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/v3/access_manager.py` & `pubnub-7.4.4/pubnub/models/consumer/v3/access_manager.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/v3/channel.py` & `pubnub-7.4.4/pubnub/models/consumer/v3/channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/v3/group.py` & `pubnub-7.4.4/pubnub/models/consumer/v3/group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/v3/pn_resource.py` & `pubnub-7.4.4/pubnub/models/consumer/v3/pn_resource.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/v3/space.py` & `pubnub-7.4.4/pubnub/models/consumer/v3/space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/v3/user.py` & `pubnub-7.4.4/pubnub/models/consumer/v3/user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/consumer/v3/uuid.py` & `pubnub-7.4.4/pubnub/models/consumer/v3/uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/models/server/subscribe.py` & `pubnub-7.4.4/pubnub/models/server/subscribe.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/pnconfiguration.py` & `pubnub-7.4.4/pubnub/pnconfiguration.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/pubnub.py` & `pubnub-7.4.4/pubnub/pubnub.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/pubnub_asyncio.py` & `pubnub-7.4.4/pubnub/pubnub_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -587,15 +587,15 @@
         else:
             subscription_event = events.SubscriptionChangedEvent(
                 channels=subscribe_operation.channels_with_pressence,
                 groups=subscribe_operation.groups_with_pressence,
                 with_presence=subscribe_operation.presence_enabled
             )
         self.event_engine.trigger(subscription_event)
-        if self._pubnub.config._heartbeat_interval > 0:
+        if self._pubnub.config.enable_presence_heartbeat and self._pubnub.config._heartbeat_interval > 0:
             self.presence_engine.trigger(events.HeartbeatJoinedEvent(
                 channels=subscribe_operation.channels,
                 groups=subscribe_operation.channel_groups
             ))
 
     def adapt_unsubscribe_builder(self, unsubscribe_operation):
         if not isinstance(unsubscribe_operation, UnsubscribeOperation):
@@ -605,31 +605,50 @@
             self.event_engine.get_context().channels,
             self.event_engine.get_context().with_presence)
 
         groups = unsubscribe_operation.get_subscribed_channel_groups(
             self.event_engine.get_context().groups,
             self.event_engine.get_context().with_presence)
 
-        self.event_engine.trigger(events.SubscriptionChangedEvent(channels=channels, groups=groups))
+        if channels or groups:
+            self.event_engine.trigger(events.SubscriptionChangedEvent(channels=channels, groups=groups))
+        else:
+            self.event_engine.trigger(events.UnsubscribeAllEvent())
 
-        self.presence_engine.trigger(event=events.HeartbeatLeftEvent(
-            channels=unsubscribe_operation.channels,
-            groups=unsubscribe_operation.channel_groups,
-            suppress_leave=self._pubnub.config.suppress_leave_events
-        ))
+        if self._pubnub.config.enable_presence_heartbeat and self._pubnub.config._heartbeat_interval > 0:
+            self.presence_engine.trigger(event=events.HeartbeatLeftEvent(
+                channels=unsubscribe_operation.channels,
+                groups=unsubscribe_operation.channel_groups,
+                suppress_leave=self._pubnub.config.suppress_leave_events
+            ))
 
     def adapt_state_builder(self, state_operation):
         self.state_container.register_state(state_operation.state,
-                                            state_operation.channels,
-                                            state_operation.channel_groups)
+                                            state_operation.channels)
         return super().adapt_state_builder(state_operation)
 
+    def unsubscribe_all(self):
+        self.adapt_unsubscribe_builder(UnsubscribeOperation(
+            channels=self.get_subscribed_channels(),
+            channel_groups=self.get_subscribed_channel_groups()))
+
     def get_custom_params(self):
         return {'ee': 1}
 
+    def get_subscribed_channels(self):
+        return self.event_engine.get_context().channels
+
+    def get_subscribed_channel_groups(self):
+        return self.event_engine.get_context().groups
+
+    def _stop_heartbeat_timer(self):
+        self.presence_engine.trigger(events.HeartbeatLeftAllEvent(
+            suppress_leave=self._pubnub.config.suppress_leave_events))
+        self.presence_engine.stop()
+
 
 class AsyncioSubscribeMessageWorker(SubscribeMessageWorker):
     async def run(self):
         await self._take_message()
 
     async def _take_message(self):
         while True:
```

### Comparing `pubnub-7.4.3/pubnub/pubnub_core.py` & `pubnub-7.4.4/pubnub/pubnub_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 from .managers import TelemetryManager
 
 logger = logging.getLogger("pubnub")
 
 
 class PubNubCore:
     """A base class for PubNub Python API implementations"""
-    SDK_VERSION = "7.4.3"
+    SDK_VERSION = "7.4.4"
     SDK_NAME = "PubNub-Python"
 
     TIMESTAMP_DIVIDER = 1000
     MAX_SEQUENCE = 65535
 
     __metaclass__ = ABCMeta
     __crypto = None
```

### Comparing `pubnub-7.4.3/pubnub/request_handlers/requests_handler.py` & `pubnub-7.4.4/pubnub/request_handlers/requests_handler.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/structures.py` & `pubnub-7.4.4/pubnub/structures.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub/utils.py` & `pubnub-7.4.4/pubnub/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,18 @@
 def is_subscribed_event(status):
     assert isinstance(status, PNStatus)
     return status.category == PNStatusCategory.PNConnectedCategory
 
 
 def is_unsubscribed_event(status):
     assert isinstance(status, PNStatus)
-    return status.category == PNStatusCategory.PNAcknowledgmentCategory \
+    is_disconnect = status.category == PNStatusCategory.PNDisconnectedCategory
+    is_unsubscribe = status.category == PNStatusCategory.PNAcknowledgmentCategory \
         and status.operation == PNOperationType.PNUnsubscribeOperation
+    return is_disconnect or is_unsubscribe
 
 
 def prepare_pam_arguments(unsorted_params):
     sorted_keys = sorted(unsorted_params)
     stringified_arguments = ""
     i = 0
```

### Comparing `pubnub-7.4.3/pubnub/workers.py` & `pubnub-7.4.4/pubnub/workers.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/pubnub.egg-info/PKG-INFO` & `pubnub-7.4.4/pubnub.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubnub
-Version: 7.4.3
+Version: 7.4.4
 Summary: PubNub Real-time push service in the cloud
 Home-page: http://pubnub.com
 Author: PubNub
 Author-email: support@pubnub.com
 License: PubNub Software Development Kit License
 Project-URL: Source, https://github.com/pubnub/python
 Project-URL: Documentation, https://www.pubnub.com/docs/sdks/python
```

### Comparing `pubnub-7.4.3/pubnub.egg-info/SOURCES.txt` & `pubnub-7.4.4/pubnub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.3/setup.py` & `pubnub-7.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pubnub',
-    version='7.4.3',
+    version='7.4.4',
     description='PubNub Real-time push service in the cloud',
     author='PubNub',
     author_email='support@pubnub.com',
     url='http://pubnub.com',
     project_urls={
         'Source': 'https://github.com/pubnub/python',
         'Documentation': 'https://www.pubnub.com/docs/sdks/python',
```

