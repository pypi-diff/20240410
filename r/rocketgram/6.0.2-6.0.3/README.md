# Comparing `tmp/rocketgram-6.0.2.tar.gz` & `tmp/rocketgram-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketgram-6.0.2.tar", last modified: Wed Mar 13 14:15:38 2024, max compression
+gzip compressed data, was "rocketgram-6.0.3.tar", last modified: Wed Apr 10 14:29:26 2024, max compression
```

## Comparing `rocketgram-6.0.2.tar` & `rocketgram-6.0.3.tar`

### file list

```diff
@@ -1,355 +1,355 @@
--rw-r--r--   0        0        0     1047 2024-03-13 14:15:25.342290 rocketgram-6.0.2/LICENSE
--rw-r--r--   0        0        0     1593 2024-03-13 14:15:25.342290 rocketgram-6.0.2/README.md
--rw-r--r--   0        0        0     2165 2024-03-13 14:15:38.054308 rocketgram-6.0.2/pyproject.toml
--rw-r--r--   0        0        0      572 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/__init__.py
--rw-r--r--   0        0        0    15075 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/__init__.py
--rw-r--r--   0        0        0      777 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/add_sticker_to_set.py
--rw-r--r--   0        0        0     1080 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/animation.py
--rw-r--r--   0        0        0      664 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/answer_callback_query.py
--rw-r--r--   0        0        0      848 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/answer_inline_query.py
--rw-r--r--   0        0        0      594 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/answer_pre_checkout_query.py
--rw-r--r--   0        0        0      691 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/answer_shipping_query.py
--rw-r--r--   0        0        0      934 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/answer_web_app_query.py
--rw-r--r--   0        0        0      553 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/approve_chat_join_request.py
--rw-r--r--   0        0        0     1098 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/audio.py
--rw-r--r--   0        0        0      651 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/ban_chat_member.py
--rw-r--r--   0        0        0      545 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/ban_chat_sender_chat.py
--rw-r--r--   0        0        0      596 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command.py
--rw-r--r--   0        0        0      361 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command_scope.py
--rw-r--r--   0        0        0      566 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0      534 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0      542 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0      555 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_chat.py
--rw-r--r--   0        0        0      608 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0      593 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0      508 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_default.py
--rw-r--r--   0        0        0      615 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_description.py
--rw-r--r--   0        0        0      536 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_name.py
--rw-r--r--   0        0        0      653 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/bot_short_description.py
--rw-r--r--   0        0        0     1006 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/callback_query.py
--rw-r--r--   0        0        0     4223 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat.py
--rw-r--r--   0        0        0      702 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_action_type.py
--rw-r--r--   0        0        0     1797 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_administrator_rights.py
--rw-r--r--   0        0        0      966 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_boost.py
--rw-r--r--   0        0        0      601 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_boost_added.py
--rw-r--r--   0        0        0      976 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_boost_removed.py
--rw-r--r--   0        0        0     1193 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_boost_source.py
--rw-r--r--   0        0        0      352 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_boost_source_type.py
--rw-r--r--   0        0        0      753 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_boost_updated.py
--rw-r--r--   0        0        0     1248 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_invite_link.py
--rw-r--r--   0        0        0     1149 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_join_request.py
--rw-r--r--   0        0        0      664 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_location.py
--rw-r--r--   0        0        0     3657 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_member.py
--rw-r--r--   0        0        0      396 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_member_status_type.py
--rw-r--r--   0        0        0     1468 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_member_updated.py
--rw-r--r--   0        0        0     1700 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_permissions.py
--rw-r--r--   0        0        0      736 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_photo.py
--rw-r--r--   0        0        0      594 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_shared.py
--rw-r--r--   0        0        0      380 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chat_type.py
--rw-r--r--   0        0        0      924 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/chosen_inline_result.py
--rw-r--r--   0        0        0      430 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/close.py
--rw-r--r--   0        0        0      542 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/close_forum_topic.py
--rw-r--r--   0        0        0      536 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/close_general_forum_topic.py
--rw-r--r--   0        0        0      755 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/contact.py
--rw-r--r--   0        0        0     1379 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/copy_message.py
--rw-r--r--   0        0        0     1048 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/copy_messages.py
--rw-r--r--   0        0        0      751 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/create_chat_invite_link.py
--rw-r--r--   0        0        0      894 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/create_forum_topic.py
--rw-r--r--   0        0        0     1265 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/create_invoice_link.py
--rw-r--r--   0        0        0     1137 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/create_new_sticker_set.py
--rw-r--r--   0        0        0      553 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/decline_chat_join_request.py
--rw-r--r--   0        0        0      515 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_chat_photo.py
--rw-r--r--   0        0        0      556 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_chat_sticker_set.py
--rw-r--r--   0        0        0      545 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_forum_topic.py
--rw-r--r--   0        0        0      543 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_message.py
--rw-r--r--   0        0        0      559 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_messages.py
--rw-r--r--   0        0        0      635 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_my_commands.py
--rw-r--r--   0        0        0      493 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_sticker_from_set.py
--rw-r--r--   0        0        0      478 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_sticker_set.py
--rw-r--r--   0        0        0      531 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/delete_webhook.py
--rw-r--r--   0        0        0      708 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/dice.py
--rw-r--r--   0        0        0      503 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/dice_type.py
--rw-r--r--   0        0        0      942 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/document.py
--rw-r--r--   0        0        0      766 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/edit_chat_invite_link.py
--rw-r--r--   0        0        0      627 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/edit_forum_topic.py
--rw-r--r--   0        0        0      547 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/edit_general_forum_topic.py
--rw-r--r--   0        0        0      953 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/edit_message_caption.py
--rw-r--r--   0        0        0      909 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/edit_message_live_location.py
--rw-r--r--   0        0        0     1158 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/edit_message_media.py
--rw-r--r--   0        0        0      734 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/edit_message_reply_markup.py
--rw-r--r--   0        0        0     1036 2024-03-13 14:15:25.342290 rocketgram-6.0.2/src/rocketgram/api/edit_message_text.py
--rw-r--r--   0        0        0      648 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/encrypted_credentials.py
--rw-r--r--   0        0        0     1640 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/encrypted_passport_element.py
--rw-r--r--   0        0        0      633 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/encrypted_passport_element_type.py
--rw-r--r--   0        0        0      670 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/entity_type.py
--rw-r--r--   0        0        0      528 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/export_chat_invite_link.py
--rw-r--r--   0        0        0     5711 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/external_reply_info.py
--rw-r--r--   0        0        0      843 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/file.py
--rw-r--r--   0        0        0      500 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/force_reply.py
--rw-r--r--   0        0        0      732 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/forum_topic.py
--rw-r--r--   0        0        0      513 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/forum_topic_closed.py
--rw-r--r--   0        0        0      690 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/forum_topic_created.py
--rw-r--r--   0        0        0      694 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/forum_topic_edited.py
--rw-r--r--   0        0        0      521 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/forum_topic_reopened.py
--rw-r--r--   0        0        0      717 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/forward_message.py
--rw-r--r--   0        0        0     1073 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/forward_messages.py
--rw-r--r--   0        0        0     1110 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/game.py
--rw-r--r--   0        0        0      667 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/game_high_score.py
--rw-r--r--   0        0        0      573 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/general_forum_topic_hidden.py
--rw-r--r--   0        0        0      581 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0      740 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_chat.py
--rw-r--r--   0        0        0      831 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_chat_administrators.py
--rw-r--r--   0        0        0      793 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_chat_member.py
--rw-r--r--   0        0        0      523 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_chat_member_count.py
--rw-r--r--   0        0        0     1350 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_chat_menu_button.py
--rw-r--r--   0        0        0      815 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0      454 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_file.py
--rw-r--r--   0        0        0      791 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_forum_topic_icon_stickers.py
--rw-r--r--   0        0        0      928 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_game_high_scores.py
--rw-r--r--   0        0        0      679 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_me.py
--rw-r--r--   0        0        0      912 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_my_commands.py
--rw-r--r--   0        0        0      913 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_my_default_administrator_rights.py
--rw-r--r--   0        0        0      822 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_my_description.py
--rw-r--r--   0        0        0      766 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_my_name.py
--rw-r--r--   0        0        0      863 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_my_short_description.py
--rw-r--r--   0        0        0      736 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_sticker_set.py
--rw-r--r--   0        0        0      950 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_updates.py
--rw-r--r--   0        0        0      868 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_user_chat_boosts.py
--rw-r--r--   0        0        0      874 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_user_profile_photos.py
--rw-r--r--   0        0        0      727 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/get_webhook_info.py
--rw-r--r--   0        0        0     1196 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/giveaway.py
--rw-r--r--   0        0        0      836 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/giveaway_completed.py
--rw-r--r--   0        0        0      541 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/giveaway_created.py
--rw-r--r--   0        0        0     1554 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/giveaway_winners.py
--rw-r--r--   0        0        0      533 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/hide_general_forum_topic.py
--rw-r--r--   0        0        0     1621 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_keyboard_button.py
--rw-r--r--   0        0        0      782 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_keyboard_markup.py
--rw-r--r--   0        0        0     1069 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query.py
--rw-r--r--   0        0        0      367 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result.py
--rw-r--r--   0        0        0     1020 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_article.py
--rw-r--r--   0        0        0     1127 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_audio.py
--rw-r--r--   0        0        0     1057 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     1125 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     1079 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_gif.py
--rw-r--r--   0        0        0     1102 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_mpeg4_gif.py
--rw-r--r--   0        0        0     1127 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0      836 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     1072 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     1072 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     1028 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_contact.py
--rw-r--r--   0        0        0     1247 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_document.py
--rw-r--r--   0        0        0      687 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_game.py
--rw-r--r--   0        0        0     1303 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_gif.py
--rw-r--r--   0        0        0     1147 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_location.py
--rw-r--r--   0        0        0     1332 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_mpeg4_gif.py
--rw-r--r--   0        0        0     1205 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_photo.py
--rw-r--r--   0        0        0     1151 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_venue.py
--rw-r--r--   0        0        0     1258 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_video.py
--rw-r--r--   0        0        0     1091 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_result_voice.py
--rw-r--r--   0        0        0      552 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/inline_query_results_button.py
--rw-r--r--   0        0        0      655 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_contact_message_content.py
--rw-r--r--   0        0        0     1219 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_file.py
--rw-r--r--   0        0        0     1272 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_invoice_message_content.py
--rw-r--r--   0        0        0      713 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_location_message_content.py
--rw-r--r--   0        0        0      346 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_media.py
--rw-r--r--   0        0        0     1012 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_media_animation.py
--rw-r--r--   0        0        0      960 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_media_audio.py
--rw-r--r--   0        0        0      927 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_media_document.py
--rw-r--r--   0        0        0      842 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_media_photo.py
--rw-r--r--   0        0        0     1042 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_media_video.py
--rw-r--r--   0        0        0      373 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_message_content.py
--rw-r--r--   0        0        0      620 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_sticker.py
--rw-r--r--   0        0        0      822 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_text_message_content.py
--rw-r--r--   0        0        0      735 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/input_venue_message_content.py
--rw-r--r--   0        0        0      710 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/invoice.py
--rw-r--r--   0        0        0      958 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/keyboard_button.py
--rw-r--r--   0        0        0      444 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/keyboard_button_poll_type.py
--rw-r--r--   0        0        0      869 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/keyboard_button_request_chat.py
--rw-r--r--   0        0        0      571 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/keyboard_button_request_users.py
--rw-r--r--   0        0        0      384 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/labeled_price.py
--rw-r--r--   0        0        0      497 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/leave_chat.py
--rw-r--r--   0        0        0      961 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/link_preview_options.py
--rw-r--r--   0        0        0      865 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/location.py
--rw-r--r--   0        0        0      433 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/log_out.py
--rw-r--r--   0        0        0      845 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/login_url.py
--rw-r--r--   0        0        0      764 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/mask_position.py
--rw-r--r--   0        0        0      344 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/mask_position_point_type.py
--rw-r--r--   0        0        0      346 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/menu_button.py
--rw-r--r--   0        0        0      481 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/menu_button_commands.py
--rw-r--r--   0        0        0      477 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/menu_button_default.py
--rw-r--r--   0        0        0      550 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/menu_button_web_app.py
--rw-r--r--   0        0        0    17805 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message.py
--rw-r--r--   0        0        0      680 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message_auto_delete_timer_changed.py
--rw-r--r--   0        0        0     1055 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message_entity.py
--rw-r--r--   0        0        0      556 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message_id.py
--rw-r--r--   0        0        0     1580 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message_origin.py
--rw-r--r--   0        0        0      366 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message_origin_type.py
--rw-r--r--   0        0        0     1031 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message_reaction_count_updated.py
--rw-r--r--   0        0        0     1336 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message_reaction_updated.py
--rw-r--r--   0        0        0     1741 2024-03-13 14:15:25.346290 rocketgram-6.0.2/src/rocketgram/api/message_type.py
--rw-r--r--   0        0        0      827 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/order_info.py
--rw-r--r--   0        0        0      428 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/parse_mode_type.py
--rw-r--r--   0        0        0      908 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_data.py
--rw-r--r--   0        0        0      376 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error.py
--rw-r--r--   0        0        0      713 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_data_field.py
--rw-r--r--   0        0        0      678 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_file.py
--rw-r--r--   0        0        0      714 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_files.py
--rw-r--r--   0        0        0      699 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_front_side.py
--rw-r--r--   0        0        0      707 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_reverse_side.py
--rw-r--r--   0        0        0      686 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_selfie.py
--rw-r--r--   0        0        0      723 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_translation_file.py
--rw-r--r--   0        0        0      759 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_translation_files.py
--rw-r--r--   0        0        0      709 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/passport_element_error_unspecified.py
--rw-r--r--   0        0        0      791 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/password_file.py
--rw-r--r--   0        0        0      712 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/photo_size.py
--rw-r--r--   0        0        0      590 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/pin_chat_message.py
--rw-r--r--   0        0        0     1695 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/poll.py
--rw-r--r--   0        0        0      834 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/poll_answer.py
--rw-r--r--   0        0        0      590 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/poll_option.py
--rw-r--r--   0        0        0      293 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/poll_type.py
--rw-r--r--   0        0        0     1032 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/pre_checkout_query.py
--rw-r--r--   0        0        0     1223 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/promote_chat_member.py
--rw-r--r--   0        0        0      704 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/proximity_alert_triggered.py
--rw-r--r--   0        0        0      724 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/reaction_count.py
--rw-r--r--   0        0        0      957 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/reaction_type.py
--rw-r--r--   0        0        0      331 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/reaction_type_type.py
--rw-r--r--   0        0        0      545 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/reopen_forum_topic.py
--rw-r--r--   0        0        0      539 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/reopen_general_forum_topic.py
--rw-r--r--   0        0        0      719 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/reply_keyboard_markup.py
--rw-r--r--   0        0        0      444 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/reply_keyboard_remove.py
--rw-r--r--   0        0        0      725 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/reply_parameters.py
--rw-r--r--   0        0        0     2378 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/request.py
--rw-r--r--   0        0        0     1223 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/response.py
--rw-r--r--   0        0        0      678 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/response_parameters.py
--rw-r--r--   0        0        0      762 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/restrict_chat_member.py
--rw-r--r--   0        0        0      571 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     1579 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_animation.py
--rw-r--r--   0        0        0     1519 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_audio.py
--rw-r--r--   0        0        0      638 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_chat_action.py
--rw-r--r--   0        0        0      929 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_contact.py
--rw-r--r--   0        0        0      879 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_dice.py
--rw-r--r--   0        0        0     1492 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_document.py
--rw-r--r--   0        0        0      828 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_game.py
--rw-r--r--   0        0        0     1626 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_invoice.py
--rw-r--r--   0        0        0     1032 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_location.py
--rw-r--r--   0        0        0     1512 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_media_group.py
--rw-r--r--   0        0        0     1142 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_message.py
--rw-r--r--   0        0        0     1291 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_photo.py
--rw-r--r--   0        0        0     1436 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_poll.py
--rw-r--r--   0        0        0     1071 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_sticker.py
--rw-r--r--   0        0        0     1054 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_venue.py
--rw-r--r--   0        0        0     1601 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_video.py
--rw-r--r--   0        0        0     1276 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_video_note.py
--rw-r--r--   0        0        0     1287 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/send_voice.py
--rw-r--r--   0        0        0      612 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/sent_web_app_message.py
--rw-r--r--   0        0        0      589 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_chat_administrator_custom_title.py
--rw-r--r--   0        0        0      572 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_chat_description.py
--rw-r--r--   0        0        0      629 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_chat_menu_button.py
--rw-r--r--   0        0        0      673 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_chat_permissions.py
--rw-r--r--   0        0        0      720 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_chat_photo.py
--rw-r--r--   0        0        0      547 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_chat_sticker_set.py
--rw-r--r--   0        0        0      521 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_chat_title.py
--rw-r--r--   0        0        0      599 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_custom_emoji_sticker_set_thumbnail.py
--rw-r--r--   0        0        0      708 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_game_score.py
--rw-r--r--   0        0        0      688 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_message_reaction.py
--rw-r--r--   0        0        0      687 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_my_commands.py
--rw-r--r--   0        0        0      693 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_my_default_administrator_rights.py
--rw-r--r--   0        0        0      570 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_my_description.py
--rw-r--r--   0        0        0      542 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_my_name.py
--rw-r--r--   0        0        0      591 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_my_short_description.py
--rw-r--r--   0        0        0      616 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_passport_data_errors.py
--rw-r--r--   0        0        0      537 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_sticker_emoji_list.py
--rw-r--r--   0        0        0      559 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_sticker_keywords.py
--rw-r--r--   0        0        0      613 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_sticker_mask_position.py
--rw-r--r--   0        0        0      520 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_sticker_position_in_set.py
--rw-r--r--   0        0        0      791 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_sticker_set_thumbnail.py
--rw-r--r--   0        0        0      499 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_sticker_set_title.py
--rw-r--r--   0        0        0      981 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/set_webhook.py
--rw-r--r--   0        0        0      787 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/shipping_address.py
--rw-r--r--   0        0        0      482 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/shipping_option.py
--rw-r--r--   0        0        0      877 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/shipping_query.py
--rw-r--r--   0        0        0     1777 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/sticker.py
--rw-r--r--   0        0        0      341 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/sticker_format.py
--rw-r--r--   0        0        0     1218 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/sticker_set.py
--rw-r--r--   0        0        0      343 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/sticker_type.py
--rw-r--r--   0        0        0      737 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/stop_message_live_location.py
--rw-r--r--   0        0        0      897 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/stop_poll.py
--rw-r--r--   0        0        0      632 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/story.py
--rw-r--r--   0        0        0     1042 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/successful_payment.py
--rw-r--r--   0        0        0     1037 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/switch_inline_query_chosen_chat.py
--rw-r--r--   0        0        0      887 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/text_quote.py
--rw-r--r--   0        0        0      502 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/thumbnail_mime_type.py
--rw-r--r--   0        0        0      584 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/unban_chat_member.py
--rw-r--r--   0        0        0      551 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/unban_chat_sender_chat.py
--rw-r--r--   0        0        0      539 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/unhide_general_forum_topic.py
--rw-r--r--   0        0        0      530 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/unpin_all_chat_messages.py
--rw-r--r--   0        0        0      575 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/unpin_all_forum_topic_messages.py
--rw-r--r--   0        0        0      569 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/unpin_all_general_forum_topic_messages.py
--rw-r--r--   0        0        0      538 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/unpin_chat_message.py
--rw-r--r--   0        0        0     5440 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/update.py
--rw-r--r--   0        0        0      782 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/update_type.py
--rw-r--r--   0        0        0      786 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/upload_sticker_file.py
--rw-r--r--   0        0        0     1201 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/user.py
--rw-r--r--   0        0        0      729 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/user_chat_boosts.py
--rw-r--r--   0        0        0      749 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/user_profile_photos.py
--rw-r--r--   0        0        0      594 2024-03-13 14:15:25.350290 rocketgram-6.0.2/src/rocketgram/api/user_shared.py
--rw-r--r--   0        0        0     3137 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/utils.py
--rw-r--r--   0        0        0      947 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/venue.py
--rw-r--r--   0        0        0     1052 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/video.py
--rw-r--r--   0        0        0      588 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/video_chat_ended.py
--rw-r--r--   0        0        0      708 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/video_chat_participants_invited.py
--rw-r--r--   0        0        0      745 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/video_chat_scheduled.py
--rw-r--r--   0        0        0      561 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/video_chat_started.py
--rw-r--r--   0        0        0      910 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/video_note.py
--rw-r--r--   0        0        0      741 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/voice.py
--rw-r--r--   0        0        0      590 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/web_app_data.py
--rw-r--r--   0        0        0      575 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/web_app_info.py
--rw-r--r--   0        0        0     1722 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/webhook_info.py
--rw-r--r--   0        0        0      811 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/api/write_access_allowed.py
--rw-r--r--   0        0        0     6692 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/bot.py
--rw-r--r--   0        0        0      304 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/connectors/__init__.py
--rw-r--r--   0        0        0     2719 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/connectors/aiohttp.py
--rw-r--r--   0        0        0     1373 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/connectors/connector.py
--rw-r--r--   0        0        0    11207 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/context.py
--rw-r--r--   0        0        0     2994 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/errors.py
--rw-r--r--   0        0        0      375 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/executors/__init__.py
--rw-r--r--   0        0        0     2986 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/executors/aiohttp.py
--rw-r--r--   0        0        0     2765 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/executors/executor.py
--rw-r--r--   0        0        0     5304 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/executors/updates.py
--rw-r--r--   0        0        0     6606 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/executors/webhook.py
--rw-r--r--   0        0        0      690 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/json_adapters/__init__.py
--rw-r--r--   0        0        0      434 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/json_adapters/base_adapter.py
--rw-r--r--   0        0        0      346 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/json_adapters/orjson_adapter.py
--rw-r--r--   0        0        0      342 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/json_adapters/standard_json_adapter.py
--rw-r--r--   0        0        0      342 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/json_adapters/ujson_adapter.py
--rw-r--r--   0        0        0      317 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/keyboards/__init__.py
--rw-r--r--   0        0        0      316 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/keyboards/errors.py
--rw-r--r--   0        0        0     2661 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/keyboards/inline.py
--rw-r--r--   0        0        0     4026 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/keyboards/keyboard.py
--rw-r--r--   0        0        0     4448 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/keyboards/reply.py
--rw-r--r--   0        0        0      309 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/middlewares/__init__.py
--rw-r--r--   0        0        0      843 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/middlewares/defaultvalues.py
--rw-r--r--   0        0        0     1321 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/middlewares/limiter.py
--rw-r--r--   0        0        0     1851 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/middlewares/middleware.py
--rw-r--r--   0        0        0      165 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/middlewares/prometheus.py
--rw-r--r--   0        0        0      220 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/__init__.py
--rw-r--r--   0        0        0      367 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/dispatcher/__init__.py
--rw-r--r--   0        0        0     4938 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/dispatcher/base.py
--rw-r--r--   0        0        0     6590 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/dispatcher/commonfilters.py
--rw-r--r--   0        0        0      861 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/dispatcher/commonwaiters.py
--rw-r--r--   0        0        0     7426 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/dispatcher/dispatcher.py
--rw-r--r--   0        0        0     2628 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/dispatcher/filters.py
--rw-r--r--   0        0        0     1576 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/dispatcher/waiters.py
--rw-r--r--   0        0        0      390 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/routers/router.py
--rw-r--r--   0        0        0      189 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/tools/__init__.py
--rw-r--r--   0        0        0     1074 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/tools/parser/__init__.py
--rw-r--r--   0        0        0     1720 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/tools/parser/parser.py
--rw-r--r--   0        0        0     6760 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/tools/parser/style.py
--rw-r--r--   0        0        0      202 2024-03-13 14:15:25.354290 rocketgram-6.0.2/src/rocketgram/version.py
--rw-r--r--   0        0        0     2427 2024-03-13 14:15:25.354290 rocketgram-6.0.2/tests/api/parsing/private/callback_data.yaml
--rw-r--r--   0        0        0     4399 2024-03-13 14:15:25.354290 rocketgram-6.0.2/tests/api/parsing/private/callback_game.yaml
--rw-r--r--   0        0        0     3752 2024-03-13 14:15:25.354290 rocketgram-6.0.2/tests/api/parsing/private/message_photo.yaml
--rw-r--r--   0        0        0     1591 2024-03-13 14:15:25.354290 rocketgram-6.0.2/tests/api/parsing/private/message_text.yaml
--rw-r--r--   0        0        0     3618 2024-03-13 14:15:25.354290 rocketgram-6.0.2/tests/api/parsing/test_parsing.py
--rw-r--r--   0        0        0     2321 2024-03-13 14:15:25.354290 rocketgram-6.0.2/tests/dispatcher/commonfilters/test_command.py
--rw-r--r--   0        0        0     4663 1970-01-01 00:00:00.000000 rocketgram-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1047 2024-04-10 14:29:14.423030 rocketgram-6.0.3/LICENSE
+-rw-r--r--   0        0        0     1593 2024-04-10 14:29:14.423030 rocketgram-6.0.3/README.md
+-rw-r--r--   0        0        0     2165 2024-04-10 14:29:26.994887 rocketgram-6.0.3/pyproject.toml
+-rw-r--r--   0        0        0      572 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/__init__.py
+-rw-r--r--   0        0        0    15075 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/__init__.py
+-rw-r--r--   0        0        0      777 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/add_sticker_to_set.py
+-rw-r--r--   0        0        0     1080 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/animation.py
+-rw-r--r--   0        0        0      664 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/answer_callback_query.py
+-rw-r--r--   0        0        0      848 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/answer_inline_query.py
+-rw-r--r--   0        0        0      594 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/answer_pre_checkout_query.py
+-rw-r--r--   0        0        0      691 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/answer_shipping_query.py
+-rw-r--r--   0        0        0      934 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/answer_web_app_query.py
+-rw-r--r--   0        0        0      553 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/approve_chat_join_request.py
+-rw-r--r--   0        0        0     1098 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/audio.py
+-rw-r--r--   0        0        0      651 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/ban_chat_member.py
+-rw-r--r--   0        0        0      545 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/ban_chat_sender_chat.py
+-rw-r--r--   0        0        0      596 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command.py
+-rw-r--r--   0        0        0      361 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command_scope.py
+-rw-r--r--   0        0        0      566 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0      534 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0      542 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0      555 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_chat.py
+-rw-r--r--   0        0        0      608 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0      593 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0      508 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_default.py
+-rw-r--r--   0        0        0      615 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_description.py
+-rw-r--r--   0        0        0      536 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_name.py
+-rw-r--r--   0        0        0      653 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/bot_short_description.py
+-rw-r--r--   0        0        0     1006 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/callback_query.py
+-rw-r--r--   0        0        0     4223 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat.py
+-rw-r--r--   0        0        0      702 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_action_type.py
+-rw-r--r--   0        0        0     1797 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_administrator_rights.py
+-rw-r--r--   0        0        0      966 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_boost.py
+-rw-r--r--   0        0        0      601 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_boost_added.py
+-rw-r--r--   0        0        0      976 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_boost_removed.py
+-rw-r--r--   0        0        0     1193 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_boost_source.py
+-rw-r--r--   0        0        0      352 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_boost_source_type.py
+-rw-r--r--   0        0        0      753 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_boost_updated.py
+-rw-r--r--   0        0        0     1248 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_invite_link.py
+-rw-r--r--   0        0        0     1149 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_join_request.py
+-rw-r--r--   0        0        0      664 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_location.py
+-rw-r--r--   0        0        0     3657 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_member.py
+-rw-r--r--   0        0        0      396 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_member_status_type.py
+-rw-r--r--   0        0        0     1468 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_member_updated.py
+-rw-r--r--   0        0        0     1700 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_permissions.py
+-rw-r--r--   0        0        0      736 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_photo.py
+-rw-r--r--   0        0        0      594 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_shared.py
+-rw-r--r--   0        0        0      380 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chat_type.py
+-rw-r--r--   0        0        0      924 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/chosen_inline_result.py
+-rw-r--r--   0        0        0      430 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/close.py
+-rw-r--r--   0        0        0      542 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/close_forum_topic.py
+-rw-r--r--   0        0        0      536 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/close_general_forum_topic.py
+-rw-r--r--   0        0        0      755 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/contact.py
+-rw-r--r--   0        0        0     1379 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/copy_message.py
+-rw-r--r--   0        0        0     1048 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/copy_messages.py
+-rw-r--r--   0        0        0      751 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/create_chat_invite_link.py
+-rw-r--r--   0        0        0      894 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/create_forum_topic.py
+-rw-r--r--   0        0        0     1265 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/create_invoice_link.py
+-rw-r--r--   0        0        0     1137 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/create_new_sticker_set.py
+-rw-r--r--   0        0        0      553 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/decline_chat_join_request.py
+-rw-r--r--   0        0        0      515 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_chat_photo.py
+-rw-r--r--   0        0        0      556 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_chat_sticker_set.py
+-rw-r--r--   0        0        0      545 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_forum_topic.py
+-rw-r--r--   0        0        0      543 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_message.py
+-rw-r--r--   0        0        0      559 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_messages.py
+-rw-r--r--   0        0        0      635 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_my_commands.py
+-rw-r--r--   0        0        0      493 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_sticker_from_set.py
+-rw-r--r--   0        0        0      478 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_sticker_set.py
+-rw-r--r--   0        0        0      531 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/delete_webhook.py
+-rw-r--r--   0        0        0      708 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/dice.py
+-rw-r--r--   0        0        0      503 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/dice_type.py
+-rw-r--r--   0        0        0      942 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/document.py
+-rw-r--r--   0        0        0      766 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/edit_chat_invite_link.py
+-rw-r--r--   0        0        0      627 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/edit_forum_topic.py
+-rw-r--r--   0        0        0      547 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/edit_general_forum_topic.py
+-rw-r--r--   0        0        0      953 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/edit_message_caption.py
+-rw-r--r--   0        0        0      909 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/edit_message_live_location.py
+-rw-r--r--   0        0        0     1158 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/edit_message_media.py
+-rw-r--r--   0        0        0      734 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     1036 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/edit_message_text.py
+-rw-r--r--   0        0        0      648 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/encrypted_credentials.py
+-rw-r--r--   0        0        0     1640 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/encrypted_passport_element.py
+-rw-r--r--   0        0        0      633 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/encrypted_passport_element_type.py
+-rw-r--r--   0        0        0      670 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/entity_type.py
+-rw-r--r--   0        0        0      528 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/export_chat_invite_link.py
+-rw-r--r--   0        0        0     5711 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/external_reply_info.py
+-rw-r--r--   0        0        0      843 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/file.py
+-rw-r--r--   0        0        0      500 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/force_reply.py
+-rw-r--r--   0        0        0      732 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/forum_topic.py
+-rw-r--r--   0        0        0      513 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/forum_topic_closed.py
+-rw-r--r--   0        0        0      704 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/forum_topic_created.py
+-rw-r--r--   0        0        0      694 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/forum_topic_edited.py
+-rw-r--r--   0        0        0      521 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/forum_topic_reopened.py
+-rw-r--r--   0        0        0      717 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/forward_message.py
+-rw-r--r--   0        0        0     1073 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/forward_messages.py
+-rw-r--r--   0        0        0     1110 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/game.py
+-rw-r--r--   0        0        0      667 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/game_high_score.py
+-rw-r--r--   0        0        0      573 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0      581 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0      740 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/get_chat.py
+-rw-r--r--   0        0        0      831 2024-04-10 14:29:14.427029 rocketgram-6.0.3/src/rocketgram/api/get_chat_administrators.py
+-rw-r--r--   0        0        0      793 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_chat_member.py
+-rw-r--r--   0        0        0      523 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_chat_member_count.py
+-rw-r--r--   0        0        0     1350 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_chat_menu_button.py
+-rw-r--r--   0        0        0      815 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0      454 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_file.py
+-rw-r--r--   0        0        0      791 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_forum_topic_icon_stickers.py
+-rw-r--r--   0        0        0      928 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_game_high_scores.py
+-rw-r--r--   0        0        0      679 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_me.py
+-rw-r--r--   0        0        0      912 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_my_commands.py
+-rw-r--r--   0        0        0      913 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_my_default_administrator_rights.py
+-rw-r--r--   0        0        0      822 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_my_description.py
+-rw-r--r--   0        0        0      766 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_my_name.py
+-rw-r--r--   0        0        0      863 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_my_short_description.py
+-rw-r--r--   0        0        0      736 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_sticker_set.py
+-rw-r--r--   0        0        0      950 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_updates.py
+-rw-r--r--   0        0        0      868 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_user_chat_boosts.py
+-rw-r--r--   0        0        0      874 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_user_profile_photos.py
+-rw-r--r--   0        0        0      727 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/get_webhook_info.py
+-rw-r--r--   0        0        0     1196 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/giveaway.py
+-rw-r--r--   0        0        0      836 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/giveaway_completed.py
+-rw-r--r--   0        0        0      541 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/giveaway_created.py
+-rw-r--r--   0        0        0     1554 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/giveaway_winners.py
+-rw-r--r--   0        0        0      533 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/hide_general_forum_topic.py
+-rw-r--r--   0        0        0     1621 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_keyboard_button.py
+-rw-r--r--   0        0        0      782 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_keyboard_markup.py
+-rw-r--r--   0        0        0     1069 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query.py
+-rw-r--r--   0        0        0      367 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result.py
+-rw-r--r--   0        0        0     1020 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_article.py
+-rw-r--r--   0        0        0     1127 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_audio.py
+-rw-r--r--   0        0        0     1057 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     1125 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     1079 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_gif.py
+-rw-r--r--   0        0        0     1102 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_mpeg4_gif.py
+-rw-r--r--   0        0        0     1127 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0      836 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     1072 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     1072 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     1028 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_contact.py
+-rw-r--r--   0        0        0     1247 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_document.py
+-rw-r--r--   0        0        0      687 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_game.py
+-rw-r--r--   0        0        0     1303 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_gif.py
+-rw-r--r--   0        0        0     1147 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_location.py
+-rw-r--r--   0        0        0     1332 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_mpeg4_gif.py
+-rw-r--r--   0        0        0     1205 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_photo.py
+-rw-r--r--   0        0        0     1151 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_venue.py
+-rw-r--r--   0        0        0     1258 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_video.py
+-rw-r--r--   0        0        0     1091 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_result_voice.py
+-rw-r--r--   0        0        0      552 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/inline_query_results_button.py
+-rw-r--r--   0        0        0      655 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_contact_message_content.py
+-rw-r--r--   0        0        0     1219 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_file.py
+-rw-r--r--   0        0        0     1272 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_invoice_message_content.py
+-rw-r--r--   0        0        0      713 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_location_message_content.py
+-rw-r--r--   0        0        0      346 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_media.py
+-rw-r--r--   0        0        0     1012 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_media_animation.py
+-rw-r--r--   0        0        0      960 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_media_audio.py
+-rw-r--r--   0        0        0      927 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_media_document.py
+-rw-r--r--   0        0        0      842 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_media_photo.py
+-rw-r--r--   0        0        0     1042 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_media_video.py
+-rw-r--r--   0        0        0      373 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_message_content.py
+-rw-r--r--   0        0        0      620 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_sticker.py
+-rw-r--r--   0        0        0      822 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_text_message_content.py
+-rw-r--r--   0        0        0      735 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/input_venue_message_content.py
+-rw-r--r--   0        0        0      710 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/invoice.py
+-rw-r--r--   0        0        0      958 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/keyboard_button.py
+-rw-r--r--   0        0        0      444 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/keyboard_button_poll_type.py
+-rw-r--r--   0        0        0      869 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/keyboard_button_request_chat.py
+-rw-r--r--   0        0        0      571 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/keyboard_button_request_users.py
+-rw-r--r--   0        0        0      384 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/labeled_price.py
+-rw-r--r--   0        0        0      497 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/leave_chat.py
+-rw-r--r--   0        0        0      961 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/link_preview_options.py
+-rw-r--r--   0        0        0      865 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/location.py
+-rw-r--r--   0        0        0      433 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/log_out.py
+-rw-r--r--   0        0        0      845 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/login_url.py
+-rw-r--r--   0        0        0      764 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/mask_position.py
+-rw-r--r--   0        0        0      344 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/mask_position_point_type.py
+-rw-r--r--   0        0        0      346 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/menu_button.py
+-rw-r--r--   0        0        0      481 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/menu_button_commands.py
+-rw-r--r--   0        0        0      477 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/menu_button_default.py
+-rw-r--r--   0        0        0      550 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/menu_button_web_app.py
+-rw-r--r--   0        0        0    17805 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message.py
+-rw-r--r--   0        0        0      680 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message_auto_delete_timer_changed.py
+-rw-r--r--   0        0        0     1055 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message_entity.py
+-rw-r--r--   0        0        0      556 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message_id.py
+-rw-r--r--   0        0        0     1580 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message_origin.py
+-rw-r--r--   0        0        0      366 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message_origin_type.py
+-rw-r--r--   0        0        0     1031 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     1336 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message_reaction_updated.py
+-rw-r--r--   0        0        0     1741 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/message_type.py
+-rw-r--r--   0        0        0      827 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/order_info.py
+-rw-r--r--   0        0        0      428 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/parse_mode_type.py
+-rw-r--r--   0        0        0      908 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_data.py
+-rw-r--r--   0        0        0      376 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error.py
+-rw-r--r--   0        0        0      713 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_data_field.py
+-rw-r--r--   0        0        0      678 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_file.py
+-rw-r--r--   0        0        0      714 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_files.py
+-rw-r--r--   0        0        0      699 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_front_side.py
+-rw-r--r--   0        0        0      707 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_reverse_side.py
+-rw-r--r--   0        0        0      686 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_selfie.py
+-rw-r--r--   0        0        0      723 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_translation_file.py
+-rw-r--r--   0        0        0      759 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_translation_files.py
+-rw-r--r--   0        0        0      709 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/passport_element_error_unspecified.py
+-rw-r--r--   0        0        0      791 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/password_file.py
+-rw-r--r--   0        0        0      712 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/photo_size.py
+-rw-r--r--   0        0        0      590 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/pin_chat_message.py
+-rw-r--r--   0        0        0     1695 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/poll.py
+-rw-r--r--   0        0        0      834 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/poll_answer.py
+-rw-r--r--   0        0        0      590 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/poll_option.py
+-rw-r--r--   0        0        0      293 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/poll_type.py
+-rw-r--r--   0        0        0     1032 2024-04-10 14:29:14.431029 rocketgram-6.0.3/src/rocketgram/api/pre_checkout_query.py
+-rw-r--r--   0        0        0     1223 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/promote_chat_member.py
+-rw-r--r--   0        0        0      704 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/proximity_alert_triggered.py
+-rw-r--r--   0        0        0      724 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/reaction_count.py
+-rw-r--r--   0        0        0      957 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/reaction_type.py
+-rw-r--r--   0        0        0      331 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/reaction_type_type.py
+-rw-r--r--   0        0        0      545 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/reopen_forum_topic.py
+-rw-r--r--   0        0        0      539 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/reopen_general_forum_topic.py
+-rw-r--r--   0        0        0      719 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/reply_keyboard_markup.py
+-rw-r--r--   0        0        0      444 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/reply_keyboard_remove.py
+-rw-r--r--   0        0        0      725 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/reply_parameters.py
+-rw-r--r--   0        0        0     2378 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/request.py
+-rw-r--r--   0        0        0     1223 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/response.py
+-rw-r--r--   0        0        0      678 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/response_parameters.py
+-rw-r--r--   0        0        0      762 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/restrict_chat_member.py
+-rw-r--r--   0        0        0      571 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     1579 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_animation.py
+-rw-r--r--   0        0        0     1519 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_audio.py
+-rw-r--r--   0        0        0      638 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_chat_action.py
+-rw-r--r--   0        0        0      929 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_contact.py
+-rw-r--r--   0        0        0      879 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_dice.py
+-rw-r--r--   0        0        0     1492 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_document.py
+-rw-r--r--   0        0        0      828 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_game.py
+-rw-r--r--   0        0        0     1626 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_invoice.py
+-rw-r--r--   0        0        0     1032 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_location.py
+-rw-r--r--   0        0        0     1512 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_media_group.py
+-rw-r--r--   0        0        0     1142 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_message.py
+-rw-r--r--   0        0        0     1291 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_photo.py
+-rw-r--r--   0        0        0     1436 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_poll.py
+-rw-r--r--   0        0        0     1071 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_sticker.py
+-rw-r--r--   0        0        0     1054 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_venue.py
+-rw-r--r--   0        0        0     1601 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_video.py
+-rw-r--r--   0        0        0     1276 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_video_note.py
+-rw-r--r--   0        0        0     1287 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/send_voice.py
+-rw-r--r--   0        0        0      612 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/sent_web_app_message.py
+-rw-r--r--   0        0        0      589 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_chat_administrator_custom_title.py
+-rw-r--r--   0        0        0      572 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_chat_description.py
+-rw-r--r--   0        0        0      629 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_chat_menu_button.py
+-rw-r--r--   0        0        0      673 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_chat_permissions.py
+-rw-r--r--   0        0        0      720 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_chat_photo.py
+-rw-r--r--   0        0        0      547 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_chat_sticker_set.py
+-rw-r--r--   0        0        0      521 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_chat_title.py
+-rw-r--r--   0        0        0      599 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_custom_emoji_sticker_set_thumbnail.py
+-rw-r--r--   0        0        0      708 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_game_score.py
+-rw-r--r--   0        0        0      688 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_message_reaction.py
+-rw-r--r--   0        0        0      687 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_my_commands.py
+-rw-r--r--   0        0        0      693 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_my_default_administrator_rights.py
+-rw-r--r--   0        0        0      570 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_my_description.py
+-rw-r--r--   0        0        0      542 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_my_name.py
+-rw-r--r--   0        0        0      591 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_my_short_description.py
+-rw-r--r--   0        0        0      616 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_passport_data_errors.py
+-rw-r--r--   0        0        0      537 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_sticker_emoji_list.py
+-rw-r--r--   0        0        0      559 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_sticker_keywords.py
+-rw-r--r--   0        0        0      613 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_sticker_mask_position.py
+-rw-r--r--   0        0        0      520 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_sticker_position_in_set.py
+-rw-r--r--   0        0        0      791 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_sticker_set_thumbnail.py
+-rw-r--r--   0        0        0      499 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_sticker_set_title.py
+-rw-r--r--   0        0        0      981 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/set_webhook.py
+-rw-r--r--   0        0        0      787 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/shipping_address.py
+-rw-r--r--   0        0        0      482 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/shipping_option.py
+-rw-r--r--   0        0        0      877 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/shipping_query.py
+-rw-r--r--   0        0        0     1777 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/sticker.py
+-rw-r--r--   0        0        0      341 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/sticker_format.py
+-rw-r--r--   0        0        0     1218 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/sticker_set.py
+-rw-r--r--   0        0        0      343 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/sticker_type.py
+-rw-r--r--   0        0        0      737 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/stop_message_live_location.py
+-rw-r--r--   0        0        0      897 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/stop_poll.py
+-rw-r--r--   0        0        0      632 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/story.py
+-rw-r--r--   0        0        0     1042 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/successful_payment.py
+-rw-r--r--   0        0        0     1037 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/switch_inline_query_chosen_chat.py
+-rw-r--r--   0        0        0      887 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/text_quote.py
+-rw-r--r--   0        0        0      502 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/thumbnail_mime_type.py
+-rw-r--r--   0        0        0      584 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/unban_chat_member.py
+-rw-r--r--   0        0        0      551 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/unban_chat_sender_chat.py
+-rw-r--r--   0        0        0      539 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/unhide_general_forum_topic.py
+-rw-r--r--   0        0        0      530 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0      575 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/unpin_all_forum_topic_messages.py
+-rw-r--r--   0        0        0      569 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/unpin_all_general_forum_topic_messages.py
+-rw-r--r--   0        0        0      538 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/unpin_chat_message.py
+-rw-r--r--   0        0        0     5440 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/update.py
+-rw-r--r--   0        0        0      782 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/update_type.py
+-rw-r--r--   0        0        0      786 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/upload_sticker_file.py
+-rw-r--r--   0        0        0     1201 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/user.py
+-rw-r--r--   0        0        0      729 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/user_chat_boosts.py
+-rw-r--r--   0        0        0      749 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/user_profile_photos.py
+-rw-r--r--   0        0        0      594 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/user_shared.py
+-rw-r--r--   0        0        0     3137 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/utils.py
+-rw-r--r--   0        0        0      947 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/venue.py
+-rw-r--r--   0        0        0     1052 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/video.py
+-rw-r--r--   0        0        0      588 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/video_chat_ended.py
+-rw-r--r--   0        0        0      708 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/video_chat_participants_invited.py
+-rw-r--r--   0        0        0      745 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/video_chat_scheduled.py
+-rw-r--r--   0        0        0      561 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/video_chat_started.py
+-rw-r--r--   0        0        0      910 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/video_note.py
+-rw-r--r--   0        0        0      741 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/voice.py
+-rw-r--r--   0        0        0      590 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/web_app_data.py
+-rw-r--r--   0        0        0      575 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/web_app_info.py
+-rw-r--r--   0        0        0     1722 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/webhook_info.py
+-rw-r--r--   0        0        0      811 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/api/write_access_allowed.py
+-rw-r--r--   0        0        0     6692 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/bot.py
+-rw-r--r--   0        0        0      304 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/connectors/__init__.py
+-rw-r--r--   0        0        0     2719 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/connectors/aiohttp.py
+-rw-r--r--   0        0        0     1373 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/connectors/connector.py
+-rw-r--r--   0        0        0    11207 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/context.py
+-rw-r--r--   0        0        0     2994 2024-04-10 14:29:14.435029 rocketgram-6.0.3/src/rocketgram/errors.py
+-rw-r--r--   0        0        0      375 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/executors/__init__.py
+-rw-r--r--   0        0        0     2986 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/executors/aiohttp.py
+-rw-r--r--   0        0        0     2765 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/executors/executor.py
+-rw-r--r--   0        0        0     5304 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/executors/updates.py
+-rw-r--r--   0        0        0     6606 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/executors/webhook.py
+-rw-r--r--   0        0        0      690 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/json_adapters/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/json_adapters/base_adapter.py
+-rw-r--r--   0        0        0      346 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/json_adapters/orjson_adapter.py
+-rw-r--r--   0        0        0      342 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/json_adapters/standard_json_adapter.py
+-rw-r--r--   0        0        0      342 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/json_adapters/ujson_adapter.py
+-rw-r--r--   0        0        0      317 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/keyboards/__init__.py
+-rw-r--r--   0        0        0      316 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/keyboards/errors.py
+-rw-r--r--   0        0        0     2661 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/keyboards/inline.py
+-rw-r--r--   0        0        0     4026 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/keyboards/keyboard.py
+-rw-r--r--   0        0        0     4448 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/keyboards/reply.py
+-rw-r--r--   0        0        0      309 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/middlewares/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/middlewares/defaultvalues.py
+-rw-r--r--   0        0        0     1321 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/middlewares/limiter.py
+-rw-r--r--   0        0        0     1851 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/middlewares/middleware.py
+-rw-r--r--   0        0        0      165 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/middlewares/prometheus.py
+-rw-r--r--   0        0        0      220 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/dispatcher/__init__.py
+-rw-r--r--   0        0        0     4938 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/dispatcher/base.py
+-rw-r--r--   0        0        0     6590 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/dispatcher/commonfilters.py
+-rw-r--r--   0        0        0      861 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/dispatcher/commonwaiters.py
+-rw-r--r--   0        0        0     7426 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/dispatcher/dispatcher.py
+-rw-r--r--   0        0        0     2628 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/dispatcher/filters.py
+-rw-r--r--   0        0        0     1576 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/dispatcher/waiters.py
+-rw-r--r--   0        0        0      390 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/routers/router.py
+-rw-r--r--   0        0        0      189 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/tools/__init__.py
+-rw-r--r--   0        0        0     1074 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/tools/parser/__init__.py
+-rw-r--r--   0        0        0     1720 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/tools/parser/parser.py
+-rw-r--r--   0        0        0     6760 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/tools/parser/style.py
+-rw-r--r--   0        0        0      202 2024-04-10 14:29:14.439029 rocketgram-6.0.3/src/rocketgram/version.py
+-rw-r--r--   0        0        0     2427 2024-04-10 14:29:14.439029 rocketgram-6.0.3/tests/api/parsing/private/callback_data.yaml
+-rw-r--r--   0        0        0     4399 2024-04-10 14:29:14.439029 rocketgram-6.0.3/tests/api/parsing/private/callback_game.yaml
+-rw-r--r--   0        0        0     3752 2024-04-10 14:29:14.439029 rocketgram-6.0.3/tests/api/parsing/private/message_photo.yaml
+-rw-r--r--   0        0        0     1591 2024-04-10 14:29:14.439029 rocketgram-6.0.3/tests/api/parsing/private/message_text.yaml
+-rw-r--r--   0        0        0     3618 2024-04-10 14:29:14.439029 rocketgram-6.0.3/tests/api/parsing/test_parsing.py
+-rw-r--r--   0        0        0     2321 2024-04-10 14:29:14.439029 rocketgram-6.0.3/tests/dispatcher/commonfilters/test_command.py
+-rw-r--r--   0        0        0     4663 1970-01-01 00:00:00.000000 rocketgram-6.0.3/PKG-INFO
```

### Comparing `rocketgram-6.0.2/LICENSE` & `rocketgram-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/README.md` & `rocketgram-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/pyproject.toml` & `rocketgram-6.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rocketgram"
-version = "6.0.2"
+version = "6.0.3"
 description = "Modern and powerful asynchronous telegram bot framework."
 keywords = [
     "telegram",
     "bot",
     "framework",
     "rocketgram",
     "async",
```

### Comparing `rocketgram-6.0.2/src/rocketgram/__init__.py` & `rocketgram-6.0.3/src/rocketgram/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/__init__.py` & `rocketgram-6.0.3/src/rocketgram/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/add_sticker_to_set.py` & `rocketgram-6.0.3/src/rocketgram/api/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/animation.py` & `rocketgram-6.0.3/src/rocketgram/api/animation.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/answer_callback_query.py` & `rocketgram-6.0.3/src/rocketgram/api/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/answer_inline_query.py` & `rocketgram-6.0.3/src/rocketgram/api/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/answer_pre_checkout_query.py` & `rocketgram-6.0.3/src/rocketgram/api/answer_pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/answer_shipping_query.py` & `rocketgram-6.0.3/src/rocketgram/api/answer_shipping_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/answer_web_app_query.py` & `rocketgram-6.0.3/src/rocketgram/api/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/approve_chat_join_request.py` & `rocketgram-6.0.3/src/rocketgram/api/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/audio.py` & `rocketgram-6.0.3/src/rocketgram/api/audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/ban_chat_member.py` & `rocketgram-6.0.3/src/rocketgram/api/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/ban_chat_sender_chat.py` & `rocketgram-6.0.3/src/rocketgram/api/ban_chat_sender_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_command.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_command.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_all_chat_administrators.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_all_group_chats.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_all_private_chats.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_chat.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_chat_administrators.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_command_scope_chat_member.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_description.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_name.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_name.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/bot_short_description.py` & `rocketgram-6.0.3/src/rocketgram/api/bot_short_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/callback_query.py` & `rocketgram-6.0.3/src/rocketgram/api/callback_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat.py` & `rocketgram-6.0.3/src/rocketgram/api/chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_action_type.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_action_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_administrator_rights.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_administrator_rights.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_boost.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_boost.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_boost_added.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_boost_added.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_boost_removed.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_boost_removed.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_boost_source.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_boost_source.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_boost_updated.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_boost_updated.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_invite_link.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_join_request.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_location.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_member.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_member_updated.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_permissions.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_photo.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chat_shared.py` & `rocketgram-6.0.3/src/rocketgram/api/chat_shared.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/chosen_inline_result.py` & `rocketgram-6.0.3/src/rocketgram/api/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/close_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/close_general_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/close_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/contact.py` & `rocketgram-6.0.3/src/rocketgram/api/contact.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/copy_message.py` & `rocketgram-6.0.3/src/rocketgram/api/copy_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/copy_messages.py` & `rocketgram-6.0.3/src/rocketgram/api/copy_messages.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/create_chat_invite_link.py` & `rocketgram-6.0.3/src/rocketgram/api/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/create_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/create_invoice_link.py` & `rocketgram-6.0.3/src/rocketgram/api/create_invoice_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/create_new_sticker_set.py` & `rocketgram-6.0.3/src/rocketgram/api/create_new_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/decline_chat_join_request.py` & `rocketgram-6.0.3/src/rocketgram/api/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/delete_chat_photo.py` & `rocketgram-6.0.3/src/rocketgram/api/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/delete_chat_sticker_set.py` & `rocketgram-6.0.3/src/rocketgram/api/delete_chat_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/delete_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/delete_message.py` & `rocketgram-6.0.3/src/rocketgram/api/delete_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/delete_messages.py` & `rocketgram-6.0.3/src/rocketgram/api/delete_messages.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/delete_my_commands.py` & `rocketgram-6.0.3/src/rocketgram/api/delete_my_commands.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/delete_webhook.py` & `rocketgram-6.0.3/src/rocketgram/api/delete_webhook.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/dice.py` & `rocketgram-6.0.3/src/rocketgram/api/dice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/document.py` & `rocketgram-6.0.3/src/rocketgram/api/document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/edit_chat_invite_link.py` & `rocketgram-6.0.3/src/rocketgram/api/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/edit_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/edit_general_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/edit_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/edit_message_caption.py` & `rocketgram-6.0.3/src/rocketgram/api/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/edit_message_live_location.py` & `rocketgram-6.0.3/src/rocketgram/api/edit_message_live_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/edit_message_media.py` & `rocketgram-6.0.3/src/rocketgram/api/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/edit_message_reply_markup.py` & `rocketgram-6.0.3/src/rocketgram/api/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/edit_message_text.py` & `rocketgram-6.0.3/src/rocketgram/api/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/encrypted_credentials.py` & `rocketgram-6.0.3/src/rocketgram/api/encrypted_credentials.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/encrypted_passport_element.py` & `rocketgram-6.0.3/src/rocketgram/api/encrypted_passport_element.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/encrypted_passport_element_type.py` & `rocketgram-6.0.3/src/rocketgram/api/encrypted_passport_element_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/entity_type.py` & `rocketgram-6.0.3/src/rocketgram/api/entity_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/export_chat_invite_link.py` & `rocketgram-6.0.3/src/rocketgram/api/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/external_reply_info.py` & `rocketgram-6.0.3/src/rocketgram/api/external_reply_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/file.py` & `rocketgram-6.0.3/src/rocketgram/api/file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/forum_topic_closed.py` & `rocketgram-6.0.3/src/rocketgram/api/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/forum_topic_created.py` & `rocketgram-6.0.3/src/rocketgram/api/forum_topic_edited.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 
 from dataclasses import dataclass
 from typing import Optional
 
 
 @dataclass(frozen=True)
-class ForumTopicCreated:
+class ForumTopicEdited:
     """\
-    Represents ForumTopicCreated object:
-    https://core.telegram.org/bots/api#forumtopiccreated
+    Represents ForumTopicEdited object:
+    https://core.telegram.org/bots/api#forumtopicedited
     """
 
-    name: str
-    icon_color: int
+    name: Optional[str]
     icon_custom_emoji_id: Optional[str]
 
     @classmethod
-    def parse(cls, data: dict) -> Optional['ForumTopicCreated']:
+    def parse(cls, data: dict) -> Optional['ForumTopicEdited']:
         if data is None:
             return None
 
-        return cls(data['name'], data['icon_color'], data.get('icon_custom_emoji_id'))
+        return cls(
+            data.get('name'),
+            data.get('icon_custom_emoji_id')
+        )
```

### Comparing `rocketgram-6.0.2/src/rocketgram/api/forum_topic_edited.py` & `rocketgram-6.0.3/src/rocketgram/api/login_url.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Copyright (C) 2015-2024 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Dict
 
 
 @dataclass(frozen=True)
-class ForumTopicEdited:
+class LoginUrl:
     """\
-    Represents ForumTopicEdited object:
-    https://core.telegram.org/bots/api#forumtopicedited
+    Represents LoginUrl keyboard object:
+    https://core.telegram.org/bots/api#loginurl
     """
 
-    name: Optional[str]
-    icon_custom_emoji_id: Optional[str]
+    url: str
+    forward_text: Optional[str] = None
+    bot_username: Optional[str] = None
+    request_write_access: Optional[bool] = None
 
     @classmethod
-    def parse(cls, data: dict) -> Optional['ForumTopicEdited']:
+    def parse(cls, data: Optional[Dict]) -> Optional['LoginUrl']:
         if data is None:
             return None
 
-        return cls(
-            data.get('name'),
-            data.get('icon_custom_emoji_id')
-        )
+        return cls(url=data['url'], forward_text=data.get('forward_text'), bot_username=data.get('bot_username'),
+                   request_write_access=data.get('request_write_access'))
```

### Comparing `rocketgram-6.0.2/src/rocketgram/api/forum_topic_reopened.py` & `rocketgram-6.0.3/src/rocketgram/api/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/forward_message.py` & `rocketgram-6.0.3/src/rocketgram/api/forward_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/forward_messages.py` & `rocketgram-6.0.3/src/rocketgram/api/forward_messages.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/game.py` & `rocketgram-6.0.3/src/rocketgram/api/game.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/game_high_score.py` & `rocketgram-6.0.3/src/rocketgram/api/game_high_score.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/general_forum_topic_hidden.py` & `rocketgram-6.0.3/src/rocketgram/api/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/general_forum_topic_unhidden.py` & `rocketgram-6.0.3/src/rocketgram/api/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_chat.py` & `rocketgram-6.0.3/src/rocketgram/api/get_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_chat_administrators.py` & `rocketgram-6.0.3/src/rocketgram/api/get_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_chat_member.py` & `rocketgram-6.0.3/src/rocketgram/api/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_chat_member_count.py` & `rocketgram-6.0.3/src/rocketgram/api/get_chat_member_count.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_chat_menu_button.py` & `rocketgram-6.0.3/src/rocketgram/api/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_custom_emoji_stickers.py` & `rocketgram-6.0.3/src/rocketgram/api/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_forum_topic_icon_stickers.py` & `rocketgram-6.0.3/src/rocketgram/api/get_forum_topic_icon_stickers.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_game_high_scores.py` & `rocketgram-6.0.3/src/rocketgram/api/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_me.py` & `rocketgram-6.0.3/src/rocketgram/api/get_me.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_my_commands.py` & `rocketgram-6.0.3/src/rocketgram/api/get_my_commands.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_my_default_administrator_rights.py` & `rocketgram-6.0.3/src/rocketgram/api/get_my_default_administrator_rights.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_my_description.py` & `rocketgram-6.0.3/src/rocketgram/api/get_my_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_my_name.py` & `rocketgram-6.0.3/src/rocketgram/api/get_my_name.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_my_short_description.py` & `rocketgram-6.0.3/src/rocketgram/api/get_my_short_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_sticker_set.py` & `rocketgram-6.0.3/src/rocketgram/api/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_updates.py` & `rocketgram-6.0.3/src/rocketgram/api/get_updates.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_user_chat_boosts.py` & `rocketgram-6.0.3/src/rocketgram/api/get_user_chat_boosts.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_user_profile_photos.py` & `rocketgram-6.0.3/src/rocketgram/api/get_user_profile_photos.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/get_webhook_info.py` & `rocketgram-6.0.3/src/rocketgram/api/get_webhook_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/giveaway.py` & `rocketgram-6.0.3/src/rocketgram/api/giveaway.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/giveaway_completed.py` & `rocketgram-6.0.3/src/rocketgram/api/giveaway_completed.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/giveaway_created.py` & `rocketgram-6.0.3/src/rocketgram/api/giveaway_created.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/giveaway_winners.py` & `rocketgram-6.0.3/src/rocketgram/api/giveaway_winners.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/hide_general_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/hide_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_keyboard_button.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_keyboard_markup.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_article.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_audio.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_audio.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_document.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_gif.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_gif.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_mpeg4_gif.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_mpeg4_gif.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_photo.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_sticker.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_video.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_cached_voice.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_contact.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_document.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_game.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_game.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_gif.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_gif.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_location.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_mpeg4_gif.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_mpeg4_gif.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_photo.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_venue.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_video.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_result_voice.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/inline_query_results_button.py` & `rocketgram-6.0.3/src/rocketgram/api/inline_query_results_button.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_contact_message_content.py` & `rocketgram-6.0.3/src/rocketgram/api/input_contact_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_file.py` & `rocketgram-6.0.3/src/rocketgram/api/input_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_invoice_message_content.py` & `rocketgram-6.0.3/src/rocketgram/api/input_invoice_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_location_message_content.py` & `rocketgram-6.0.3/src/rocketgram/api/input_location_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_media_animation.py` & `rocketgram-6.0.3/src/rocketgram/api/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_media_audio.py` & `rocketgram-6.0.3/src/rocketgram/api/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_media_document.py` & `rocketgram-6.0.3/src/rocketgram/api/input_media_document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_media_photo.py` & `rocketgram-6.0.3/src/rocketgram/api/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_media_video.py` & `rocketgram-6.0.3/src/rocketgram/api/input_media_video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_sticker.py` & `rocketgram-6.0.3/src/rocketgram/api/input_sticker.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_text_message_content.py` & `rocketgram-6.0.3/src/rocketgram/api/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/input_venue_message_content.py` & `rocketgram-6.0.3/src/rocketgram/api/input_venue_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/invoice.py` & `rocketgram-6.0.3/src/rocketgram/api/invoice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/keyboard_button.py` & `rocketgram-6.0.3/src/rocketgram/api/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/keyboard_button_request_chat.py` & `rocketgram-6.0.3/src/rocketgram/api/keyboard_button_request_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/keyboard_button_request_users.py` & `rocketgram-6.0.3/src/rocketgram/api/keyboard_button_request_users.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/link_preview_options.py` & `rocketgram-6.0.3/src/rocketgram/api/link_preview_options.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/location.py` & `rocketgram-6.0.3/src/rocketgram/api/location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/login_url.py` & `rocketgram-6.0.3/src/rocketgram/api/successful_payment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # Copyright (C) 2015-2024 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import Optional, Dict
+from typing import Optional
+
+from .order_info import OrderInfo
 
 
 @dataclass(frozen=True)
-class LoginUrl:
+class SuccessfulPayment:
     """\
-    Represents LoginUrl keyboard object:
-    https://core.telegram.org/bots/api#loginurl
+    Represents SuccessfulPayment object:
+    https://core.telegram.org/bots/api#successfulpayment
     """
 
-    url: str
-    forward_text: Optional[str] = None
-    bot_username: Optional[str] = None
-    request_write_access: Optional[bool] = None
+    currency: str
+    total_amount: int
+    invoice_payload: str
+    shipping_option_id: Optional[str]
+    order_info: Optional[OrderInfo]
+    telegram_payment_charge_id: str
+    provider_payment_charge_id: str
 
     @classmethod
-    def parse(cls, data: Optional[Dict]) -> Optional['LoginUrl']:
+    def parse(cls, data: dict) -> Optional['SuccessfulPayment']:
         if data is None:
             return None
 
-        return cls(url=data['url'], forward_text=data.get('forward_text'), bot_username=data.get('bot_username'),
-                   request_write_access=data.get('request_write_access'))
+        return cls(data['currency'], data['total_amount'], data['invoice_payload'], data.get('shipping_option_id'),
+                   OrderInfo.parse(data.get('order_info')), data['telegram_payment_charge_id'],
+                   data['provider_payment_charge_id'])
```

### Comparing `rocketgram-6.0.2/src/rocketgram/api/mask_position.py` & `rocketgram-6.0.3/src/rocketgram/api/mask_position.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/menu_button_web_app.py` & `rocketgram-6.0.3/src/rocketgram/api/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/message.py` & `rocketgram-6.0.3/src/rocketgram/api/message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/message_auto_delete_timer_changed.py` & `rocketgram-6.0.3/src/rocketgram/api/message_auto_delete_timer_changed.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/message_entity.py` & `rocketgram-6.0.3/src/rocketgram/api/message_entity.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/message_id.py` & `rocketgram-6.0.3/src/rocketgram/api/message_id.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/message_origin.py` & `rocketgram-6.0.3/src/rocketgram/api/message_origin.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/message_reaction_count_updated.py` & `rocketgram-6.0.3/src/rocketgram/api/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/message_reaction_updated.py` & `rocketgram-6.0.3/src/rocketgram/api/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/message_type.py` & `rocketgram-6.0.3/src/rocketgram/api/message_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/order_info.py` & `rocketgram-6.0.3/src/rocketgram/api/order_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_data.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_data.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_data_field.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_data_field.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_file.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_files.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_files.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_front_side.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_front_side.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_reverse_side.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_reverse_side.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_selfie.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_selfie.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_translation_file.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_translation_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_translation_files.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_translation_files.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/passport_element_error_unspecified.py` & `rocketgram-6.0.3/src/rocketgram/api/passport_element_error_unspecified.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/password_file.py` & `rocketgram-6.0.3/src/rocketgram/api/password_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/photo_size.py` & `rocketgram-6.0.3/src/rocketgram/api/photo_size.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/pin_chat_message.py` & `rocketgram-6.0.3/src/rocketgram/api/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/poll.py` & `rocketgram-6.0.3/src/rocketgram/api/poll.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/poll_answer.py` & `rocketgram-6.0.3/src/rocketgram/api/poll_answer.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/poll_option.py` & `rocketgram-6.0.3/src/rocketgram/api/poll_option.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/pre_checkout_query.py` & `rocketgram-6.0.3/src/rocketgram/api/pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/promote_chat_member.py` & `rocketgram-6.0.3/src/rocketgram/api/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/proximity_alert_triggered.py` & `rocketgram-6.0.3/src/rocketgram/api/proximity_alert_triggered.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/reaction_count.py` & `rocketgram-6.0.3/src/rocketgram/api/reaction_count.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/reaction_type.py` & `rocketgram-6.0.3/src/rocketgram/api/reaction_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/reopen_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/reopen_general_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/reopen_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/reply_keyboard_markup.py` & `rocketgram-6.0.3/src/rocketgram/api/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/reply_parameters.py` & `rocketgram-6.0.3/src/rocketgram/api/reply_parameters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/request.py` & `rocketgram-6.0.3/src/rocketgram/api/request.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/response.py` & `rocketgram-6.0.3/src/rocketgram/api/response.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/response_parameters.py` & `rocketgram-6.0.3/src/rocketgram/api/response_parameters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/restrict_chat_member.py` & `rocketgram-6.0.3/src/rocketgram/api/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/revoke_chat_invite_link.py` & `rocketgram-6.0.3/src/rocketgram/api/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_animation.py` & `rocketgram-6.0.3/src/rocketgram/api/send_animation.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_audio.py` & `rocketgram-6.0.3/src/rocketgram/api/send_audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_chat_action.py` & `rocketgram-6.0.3/src/rocketgram/api/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_contact.py` & `rocketgram-6.0.3/src/rocketgram/api/send_contact.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_dice.py` & `rocketgram-6.0.3/src/rocketgram/api/send_dice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_document.py` & `rocketgram-6.0.3/src/rocketgram/api/send_document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_game.py` & `rocketgram-6.0.3/src/rocketgram/api/send_game.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_invoice.py` & `rocketgram-6.0.3/src/rocketgram/api/send_invoice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_location.py` & `rocketgram-6.0.3/src/rocketgram/api/send_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_media_group.py` & `rocketgram-6.0.3/src/rocketgram/api/send_media_group.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_message.py` & `rocketgram-6.0.3/src/rocketgram/api/send_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_photo.py` & `rocketgram-6.0.3/src/rocketgram/api/send_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_poll.py` & `rocketgram-6.0.3/src/rocketgram/api/send_poll.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_sticker.py` & `rocketgram-6.0.3/src/rocketgram/api/send_sticker.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_venue.py` & `rocketgram-6.0.3/src/rocketgram/api/send_venue.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_video.py` & `rocketgram-6.0.3/src/rocketgram/api/send_video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_video_note.py` & `rocketgram-6.0.3/src/rocketgram/api/send_video_note.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/send_voice.py` & `rocketgram-6.0.3/src/rocketgram/api/send_voice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/sent_web_app_message.py` & `rocketgram-6.0.3/src/rocketgram/api/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_chat_administrator_custom_title.py` & `rocketgram-6.0.3/src/rocketgram/api/set_chat_administrator_custom_title.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_chat_description.py` & `rocketgram-6.0.3/src/rocketgram/api/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_chat_menu_button.py` & `rocketgram-6.0.3/src/rocketgram/api/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_chat_permissions.py` & `rocketgram-6.0.3/src/rocketgram/api/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_chat_photo.py` & `rocketgram-6.0.3/src/rocketgram/api/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_chat_sticker_set.py` & `rocketgram-6.0.3/src/rocketgram/api/set_chat_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_chat_title.py` & `rocketgram-6.0.3/src/rocketgram/api/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_custom_emoji_sticker_set_thumbnail.py` & `rocketgram-6.0.3/src/rocketgram/api/set_custom_emoji_sticker_set_thumbnail.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_game_score.py` & `rocketgram-6.0.3/src/rocketgram/api/set_game_score.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_message_reaction.py` & `rocketgram-6.0.3/src/rocketgram/api/set_message_reaction.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_my_commands.py` & `rocketgram-6.0.3/src/rocketgram/api/set_my_commands.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_my_default_administrator_rights.py` & `rocketgram-6.0.3/src/rocketgram/api/set_my_default_administrator_rights.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_my_description.py` & `rocketgram-6.0.3/src/rocketgram/api/set_my_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_my_name.py` & `rocketgram-6.0.3/src/rocketgram/api/set_my_name.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_my_short_description.py` & `rocketgram-6.0.3/src/rocketgram/api/set_my_short_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_passport_data_errors.py` & `rocketgram-6.0.3/src/rocketgram/api/set_passport_data_errors.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_sticker_emoji_list.py` & `rocketgram-6.0.3/src/rocketgram/api/set_sticker_emoji_list.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_sticker_keywords.py` & `rocketgram-6.0.3/src/rocketgram/api/set_sticker_keywords.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_sticker_mask_position.py` & `rocketgram-6.0.3/src/rocketgram/api/set_sticker_mask_position.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_sticker_position_in_set.py` & `rocketgram-6.0.3/src/rocketgram/api/set_sticker_position_in_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_sticker_set_thumbnail.py` & `rocketgram-6.0.3/src/rocketgram/api/set_sticker_set_thumbnail.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/set_webhook.py` & `rocketgram-6.0.3/src/rocketgram/api/set_webhook.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/shipping_address.py` & `rocketgram-6.0.3/src/rocketgram/api/shipping_address.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/shipping_query.py` & `rocketgram-6.0.3/src/rocketgram/api/shipping_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/sticker.py` & `rocketgram-6.0.3/src/rocketgram/api/sticker.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/sticker_set.py` & `rocketgram-6.0.3/src/rocketgram/api/sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/stop_message_live_location.py` & `rocketgram-6.0.3/src/rocketgram/api/stop_message_live_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/stop_poll.py` & `rocketgram-6.0.3/src/rocketgram/api/stop_poll.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/story.py` & `rocketgram-6.0.3/src/rocketgram/api/story.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/successful_payment.py` & `rocketgram-6.0.3/src/rocketgram/api/voice.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,33 +2,28 @@
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
 from typing import Optional
 
-from .order_info import OrderInfo
-
 
 @dataclass(frozen=True)
-class SuccessfulPayment:
+class Voice:
     """\
-    Represents SuccessfulPayment object:
-    https://core.telegram.org/bots/api#successfulpayment
+    Represents Voice object:
+    https://core.telegram.org/bots/api#voice
     """
 
-    currency: str
-    total_amount: int
-    invoice_payload: str
-    shipping_option_id: Optional[str]
-    order_info: Optional[OrderInfo]
-    telegram_payment_charge_id: str
-    provider_payment_charge_id: str
+    file_id: str
+    file_unique_id: str
+    duration: int
+    mime_type: Optional[str]
+    file_size: Optional[int]
 
     @classmethod
-    def parse(cls, data: dict) -> Optional['SuccessfulPayment']:
+    def parse(cls, data: dict) -> Optional['Voice']:
         if data is None:
             return None
 
-        return cls(data['currency'], data['total_amount'], data['invoice_payload'], data.get('shipping_option_id'),
-                   OrderInfo.parse(data.get('order_info')), data['telegram_payment_charge_id'],
-                   data['provider_payment_charge_id'])
+        return cls(data['file_id'], data['file_unique_id'], data['duration'], data.get('mime_type'),
+                   data.get('file_size'))
```

### Comparing `rocketgram-6.0.2/src/rocketgram/api/switch_inline_query_chosen_chat.py` & `rocketgram-6.0.3/src/rocketgram/api/switch_inline_query_chosen_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/text_quote.py` & `rocketgram-6.0.3/src/rocketgram/api/text_quote.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/unban_chat_member.py` & `rocketgram-6.0.3/src/rocketgram/api/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/unban_chat_sender_chat.py` & `rocketgram-6.0.3/src/rocketgram/api/unban_chat_sender_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/unhide_general_forum_topic.py` & `rocketgram-6.0.3/src/rocketgram/api/unhide_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/unpin_all_chat_messages.py` & `rocketgram-6.0.3/src/rocketgram/api/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/unpin_all_forum_topic_messages.py` & `rocketgram-6.0.3/src/rocketgram/api/unpin_all_forum_topic_messages.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/unpin_all_general_forum_topic_messages.py` & `rocketgram-6.0.3/src/rocketgram/api/unpin_all_general_forum_topic_messages.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/unpin_chat_message.py` & `rocketgram-6.0.3/src/rocketgram/api/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/update.py` & `rocketgram-6.0.3/src/rocketgram/api/update.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/update_type.py` & `rocketgram-6.0.3/src/rocketgram/api/update_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/upload_sticker_file.py` & `rocketgram-6.0.3/src/rocketgram/api/upload_sticker_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/user.py` & `rocketgram-6.0.3/src/rocketgram/api/user.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/user_chat_boosts.py` & `rocketgram-6.0.3/src/rocketgram/api/user_chat_boosts.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/user_profile_photos.py` & `rocketgram-6.0.3/src/rocketgram/api/user_profile_photos.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/user_shared.py` & `rocketgram-6.0.3/src/rocketgram/api/user_shared.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/utils.py` & `rocketgram-6.0.3/src/rocketgram/api/utils.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/venue.py` & `rocketgram-6.0.3/src/rocketgram/api/venue.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/video.py` & `rocketgram-6.0.3/src/rocketgram/api/video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/video_chat_ended.py` & `rocketgram-6.0.3/src/rocketgram/api/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/video_chat_participants_invited.py` & `rocketgram-6.0.3/src/rocketgram/api/video_chat_participants_invited.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/video_chat_scheduled.py` & `rocketgram-6.0.3/src/rocketgram/api/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/video_chat_started.py` & `rocketgram-6.0.3/src/rocketgram/api/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/video_note.py` & `rocketgram-6.0.3/src/rocketgram/api/video_note.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/web_app_data.py` & `rocketgram-6.0.3/src/rocketgram/api/web_app_data.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/web_app_info.py` & `rocketgram-6.0.3/src/rocketgram/api/web_app_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/webhook_info.py` & `rocketgram-6.0.3/src/rocketgram/api/webhook_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/api/write_access_allowed.py` & `rocketgram-6.0.3/src/rocketgram/api/write_access_allowed.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/bot.py` & `rocketgram-6.0.3/src/rocketgram/bot.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/connectors/aiohttp.py` & `rocketgram-6.0.3/src/rocketgram/connectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/connectors/connector.py` & `rocketgram-6.0.3/src/rocketgram/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/context.py` & `rocketgram-6.0.3/src/rocketgram/context.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/errors.py` & `rocketgram-6.0.3/src/rocketgram/errors.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/executors/aiohttp.py` & `rocketgram-6.0.3/src/rocketgram/executors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/executors/executor.py` & `rocketgram-6.0.3/src/rocketgram/executors/executor.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/executors/updates.py` & `rocketgram-6.0.3/src/rocketgram/executors/updates.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/executors/webhook.py` & `rocketgram-6.0.3/src/rocketgram/executors/webhook.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/json_adapters/__init__.py` & `rocketgram-6.0.3/src/rocketgram/json_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/keyboards/inline.py` & `rocketgram-6.0.3/src/rocketgram/keyboards/inline.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/keyboards/keyboard.py` & `rocketgram-6.0.3/src/rocketgram/keyboards/keyboard.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/keyboards/reply.py` & `rocketgram-6.0.3/src/rocketgram/keyboards/reply.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/middlewares/defaultvalues.py` & `rocketgram-6.0.3/src/rocketgram/middlewares/defaultvalues.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/middlewares/limiter.py` & `rocketgram-6.0.3/src/rocketgram/middlewares/limiter.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/middlewares/middleware.py` & `rocketgram-6.0.3/src/rocketgram/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/routers/dispatcher/base.py` & `rocketgram-6.0.3/src/rocketgram/routers/dispatcher/base.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/routers/dispatcher/commonfilters.py` & `rocketgram-6.0.3/src/rocketgram/routers/dispatcher/commonfilters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/routers/dispatcher/commonwaiters.py` & `rocketgram-6.0.3/src/rocketgram/routers/dispatcher/commonwaiters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/routers/dispatcher/dispatcher.py` & `rocketgram-6.0.3/src/rocketgram/routers/dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/routers/dispatcher/filters.py` & `rocketgram-6.0.3/src/rocketgram/routers/dispatcher/filters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/routers/dispatcher/waiters.py` & `rocketgram-6.0.3/src/rocketgram/routers/dispatcher/waiters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/tools/parser/__init__.py` & `rocketgram-6.0.3/src/rocketgram/tools/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/tools/parser/parser.py` & `rocketgram-6.0.3/src/rocketgram/tools/parser/parser.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/src/rocketgram/tools/parser/style.py` & `rocketgram-6.0.3/src/rocketgram/tools/parser/style.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/tests/api/parsing/private/callback_data.yaml` & `rocketgram-6.0.3/tests/api/parsing/private/callback_data.yaml`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/tests/api/parsing/private/callback_game.yaml` & `rocketgram-6.0.3/tests/api/parsing/private/callback_game.yaml`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/tests/api/parsing/private/message_photo.yaml` & `rocketgram-6.0.3/tests/api/parsing/private/message_photo.yaml`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/tests/api/parsing/private/message_text.yaml` & `rocketgram-6.0.3/tests/api/parsing/private/message_text.yaml`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/tests/api/parsing/test_parsing.py` & `rocketgram-6.0.3/tests/api/parsing/test_parsing.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/tests/dispatcher/commonfilters/test_command.py` & `rocketgram-6.0.3/tests/dispatcher/commonfilters/test_command.py`

 * *Files identical despite different names*

### Comparing `rocketgram-6.0.2/PKG-INFO` & `rocketgram-6.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketgram
-Version: 6.0.2
+Version: 6.0.3
 Summary: Modern and powerful asynchronous telegram bot framework.
 Keywords: telegram bot framework rocketgram async asyncio rocket
 Home-page: https://github.com/vd2org/wultiplexor
 Author-Email: Vd <rocketgram@vd2.org>
 License: Copyright 2015-2024 Vd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

