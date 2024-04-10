# Comparing `tmp/khoj_assistant-1.9.1.dev5.tar.gz` & `tmp/khoj_assistant-1.9.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Apr  7 09:49:07 2024, max compression
+gzip compressed data, last modified: Mon Apr  8 06:13:34 2024, max compression
```

## Comparing `khoj_assistant-1.9.1.dev5.tar` & `khoj_assistant-1.9.1.dev8.tar`

### file list

```diff
@@ -1,183 +1,183 @@
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/__init__.py
--rw-r--r--   0        0        0    14394 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/configure.py
--rw-r--r--   0        0        0     5330 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/main.py
--rwxr-xr-x   0        0        0      664 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/manage.py
--rw-r--r--   0        0        0     2832 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/app/README.md
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/app/__init__.py
--rw-r--r--   0        0        0     4534 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/app/settings.py
--rw-r--r--   0        0        0      869 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/app/urls.py
--rw-r--r--   0        0        0      388 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/app/wsgi.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/__init__.py
--rw-r--r--   0        0        0     5523 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/admin.py
--rw-r--r--   0        0        0      153 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/apps.py
--rw-r--r--   0        0        0       60 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/tests.py
--rw-r--r--   0        0        0    33625 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/adapters/__init__.py
--rw-r--r--   0        0        0     4077 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0001_khojuser.py
--rw-r--r--   0        0        0     1195 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0002_googleuser.py
--rw-r--r--   0        0        0      224 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0003_vector_extension.py
--rw-r--r--   0        0        0     8202 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0004_content_types_and_more.py
--rw-r--r--   0        0        0      429 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0005_embeddings_corpus_id.py
--rw-r--r--   0        0        0     1131 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0006_embeddingsdates.py
--rw-r--r--   0        0        0      917 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0007_add_conversation.py
--rw-r--r--   0        0        0      399 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
--rw-r--r--   0        0        0      876 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0009_khojapiuser.py
--rw-r--r--   0        0        0     3347 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
--rw-r--r--   0        0        0      773 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
--rw-r--r--   0        0        0      331 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0011_merge_20231102_0138.py
--rw-r--r--   0        0        0      552 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0012_entry_file_source.py
--rw-r--r--   0        0        0     1311 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0013_subscription.py
--rw-r--r--   0        0        0      411 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0014_alter_googleuser_picture.py
--rw-r--r--   0        0        0      584 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0015_alter_subscription_user.py
--rw-r--r--   0        0        0      429 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
--rw-r--r--   0        0        0     1219 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0017_searchmodel.py
--rw-r--r--   0        0        0     1152 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
--rw-r--r--   0        0        0      843 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
--rw-r--r--   0        0        0     1190 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0020_reflectivequestion.py
--rw-r--r--   0        0        0     1504 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
--rw-r--r--   0        0        0      904 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
--rw-r--r--   0        0        0     1122 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0023_usersearchmodelconfig.py
--rw-r--r--   0        0        0      405 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0024_alter_entry_embeddings.py
--rw-r--r--   0        0        0     1573 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
--rw-r--r--   0        0        0      691 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      731 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      375 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0027_merge_20240118_1324.py
--rw-r--r--   0        0        0      405 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
--rw-r--r--   0        0        0      934 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0029_userrequests.py
--rw-r--r--   0        0        0     1252 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0030_conversation_slug_and_title.py
--rw-r--r--   0        0        0     2033 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0031_agent_conversation_agent.py
--rw-r--r--   0        0        0      812 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0031_alter_googleuser_locale.py
--rw-r--r--   0        0        0      317 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0032_merge_20240322_0427.py
--rw-r--r--   0        0        0      369 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
--rw-r--r--   0        0        0     1251 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/__init__.py
--rw-r--r--   0        0        0    11129 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/database/models/__init__.py
--rw-r--r--   0        0        0     1651 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     8953 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/agent.html
--rw-r--r--   0        0        0     6672 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/agents.html
--rw-r--r--   0        0        0    11089 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0   112026 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    38365 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     5367 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/content_source_computer_input.html
--rw-r--r--   0        0        0     7225 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/content_source_github_input.html
--rw-r--r--   0        0        0     3497 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/content_source_notion_input.html
--rw-r--r--   0        0        0     1628 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0     4218 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/login.html
--rw-r--r--   0        0        0     2910 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0    18326 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/search.html
--rw-r--r--   0        0        0     2168 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/utils.html
--rw-r--r--   0        0        0     5160 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73396 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0     1222 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/utils.js
--rw-r--r--   0        0        0    51584 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0    10517 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/computer.png
--rw-r--r--   0        0        0      549 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0      503 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/copy-solid.svg
--rw-r--r--   0        0        0      746 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/copy_button.svg
--rw-r--r--   0        0        0    19662 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/credit-card.png
--rw-r--r--   0        0        0   205167 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    30234 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/favicon-256x256.png
--rw-r--r--   0        0        0    31531 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0     1100 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/key.svg
--rw-r--r--   0        0        0    13011 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0    29856 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
--rw-r--r--   0        0        0  1301428 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0      616 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/microphone-solid.svg
--rw-r--r--   0        0        0     1578 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     1736 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/openai-logomark.svg
--rw-r--r--   0        0        0     7946 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0     2945 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/plaintext.svg
--rw-r--r--   0        0        0     1877 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/question-mark-icon.svg
--rw-r--r--   0        0        0     1319 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/stop-solid.svg
--rw-r--r--   0        0        0      503 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/trash-solid.svg
--rw-r--r--   0        0        0     2233 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/user-silhouette.svg
--rw-r--r--   0        0        0      951 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/web.svg
--rw-r--r--   0        0        0     2417 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/whatsapp.svg
--rw-r--r--   0        0        0   591182 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
--rw-r--r--   0        0        0   197173 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
--rw-r--r--   0        0        0   268309 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
--rw-r--r--   0        0        0   406179 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
--rw-r--r--   0        0        0    82985 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
--rw-r--r--   0        0        0   236285 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/migrations/__init__.py
--rw-r--r--   0        0        0     1928 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_offline_chat_default_model.py
--rw-r--r--   0        0        0     2034 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_offline_chat_default_model_2.py
--rw-r--r--   0        0        0     2510 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_offline_chat_schema.py
--rw-r--r--   0        0        0      975 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_offline_model.py
--rw-r--r--   0        0        0     2025 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_processor_config_openai.py
--rw-r--r--   0        0        0     5132 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_server_pg.py
--rw-r--r--   0        0        0      569 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_version.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4715 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/__init__.py
--rw-r--r--   0        0        0    12604 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/text_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/github/__init__.py
--rw-r--r--   0        0        0    14040 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/github/github_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/markdown/__init__.py
--rw-r--r--   0        0        0     5690 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/markdown/markdown_to_entries.py
--rw-r--r--   0        0        0     9906 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/notion/notion_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/org_mode/__init__.py
--rw-r--r--   0        0        0     6377 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/org_mode/org_to_entries.py
--rw-r--r--   0        0        0    18246 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/pdf/__init__.py
--rw-r--r--   0        0        0     4660 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/pdf/pdf_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/plaintext/__init__.py
--rw-r--r--   0        0        0     3717 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/content/plaintext/plaintext_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0    21189 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0    10226 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/offline/__init__.py
--rw-r--r--   0        0        0     8579 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/offline/chat_model.py
--rw-r--r--   0        0        0     1793 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/offline/utils.py
--rw-r--r--   0        0        0      470 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/offline/whisper.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/openai/__init__.py
--rw-r--r--   0        0        0     6896 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/openai/gpt.py
--rw-r--r--   0        0        0     3284 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/openai/utils.py
--rw-r--r--   0        0        0      432 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/openai/whisper.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/tools/__init__.py
--rw-r--r--   0        0        0     5929 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/processor/tools/online_search.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    13865 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1443 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/api_agents.py
--rw-r--r--   0        0        0    25148 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/api_chat.py
--rw-r--r--   0        0        0    10827 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/api_config.py
--rw-r--r--   0        0        0     2208 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/api_phone.py
--rw-r--r--   0        0        0     4569 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/auth.py
--rw-r--r--   0        0        0    28306 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0    10974 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/indexer.py
--rw-r--r--   0        0        0     3137 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/notion.py
--rw-r--r--   0        0        0     1151 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/storage.py
--rw-r--r--   0        0        0     4285 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/subscription.py
--rw-r--r--   0        0        0     1081 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/twilio.py
--rw-r--r--   0        0        0    13329 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      358 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0    10101 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0      939 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     1005 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0     8916 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     3466 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     1740 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/config.py
--rw-r--r--   0        0        0      791 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     9519 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/fs_syncer.py
--rw-r--r--   0        0        0    12034 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     7245 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/initialization.py
--rw-r--r--   0        0        0     1192 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2009 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4028 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1309 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1430 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      565 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/.gitignore
--rw-r--r--   0        0        0    34523 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/LICENSE
--rw-r--r--   0        0        0     2378 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/README.md
--rw-r--r--   0        0        0     3456 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/pyproject.toml
--rw-r--r--   0        0        0     5629 2024-04-07 09:49:07.000000 khoj_assistant-1.9.1.dev5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/__init__.py
+-rw-r--r--   0        0        0    14394 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/configure.py
+-rw-r--r--   0        0        0     5330 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/main.py
+-rwxr-xr-x   0        0        0      664 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/manage.py
+-rw-r--r--   0        0        0     2832 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/settings.py
+-rw-r--r--   0        0        0      869 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/urls.py
+-rw-r--r--   0        0        0      388 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/wsgi.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/__init__.py
+-rw-r--r--   0        0        0     5523 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/admin.py
+-rw-r--r--   0        0        0      153 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/apps.py
+-rw-r--r--   0        0        0       60 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/tests.py
+-rw-r--r--   0        0        0    33625 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/adapters/__init__.py
+-rw-r--r--   0        0        0     4077 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0001_khojuser.py
+-rw-r--r--   0        0        0     1195 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0002_googleuser.py
+-rw-r--r--   0        0        0      224 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0003_vector_extension.py
+-rw-r--r--   0        0        0     8202 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0004_content_types_and_more.py
+-rw-r--r--   0        0        0      429 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0005_embeddings_corpus_id.py
+-rw-r--r--   0        0        0     1131 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0006_embeddingsdates.py
+-rw-r--r--   0        0        0      917 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0007_add_conversation.py
+-rw-r--r--   0        0        0      399 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
+-rw-r--r--   0        0        0      876 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0009_khojapiuser.py
+-rw-r--r--   0        0        0     3347 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
+-rw-r--r--   0        0        0      773 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
+-rw-r--r--   0        0        0      331 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0011_merge_20231102_0138.py
+-rw-r--r--   0        0        0      552 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0012_entry_file_source.py
+-rw-r--r--   0        0        0     1311 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0013_subscription.py
+-rw-r--r--   0        0        0      411 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0014_alter_googleuser_picture.py
+-rw-r--r--   0        0        0      584 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0015_alter_subscription_user.py
+-rw-r--r--   0        0        0      429 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
+-rw-r--r--   0        0        0     1219 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0017_searchmodel.py
+-rw-r--r--   0        0        0     1152 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
+-rw-r--r--   0        0        0      843 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
+-rw-r--r--   0        0        0     1190 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0020_reflectivequestion.py
+-rw-r--r--   0        0        0     1504 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
+-rw-r--r--   0        0        0      904 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
+-rw-r--r--   0        0        0     1122 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0023_usersearchmodelconfig.py
+-rw-r--r--   0        0        0      405 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0024_alter_entry_embeddings.py
+-rw-r--r--   0        0        0     1573 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
+-rw-r--r--   0        0        0      691 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      731 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      375 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0027_merge_20240118_1324.py
+-rw-r--r--   0        0        0      405 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
+-rw-r--r--   0        0        0      934 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0029_userrequests.py
+-rw-r--r--   0        0        0     1252 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0030_conversation_slug_and_title.py
+-rw-r--r--   0        0        0     2033 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0031_agent_conversation_agent.py
+-rw-r--r--   0        0        0      812 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0031_alter_googleuser_locale.py
+-rw-r--r--   0        0        0      317 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0032_merge_20240322_0427.py
+-rw-r--r--   0        0        0      369 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
+-rw-r--r--   0        0        0     1251 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/__init__.py
+-rw-r--r--   0        0        0    11129 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/models/__init__.py
+-rw-r--r--   0        0        0     1651 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     8953 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/agent.html
+-rw-r--r--   0        0        0     6672 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/agents.html
+-rw-r--r--   0        0        0    11089 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0   112026 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    38365 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     5367 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_computer_input.html
+-rw-r--r--   0        0        0     7225 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_github_input.html
+-rw-r--r--   0        0        0     3497 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_notion_input.html
+-rw-r--r--   0        0        0     1628 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0     4218 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/login.html
+-rw-r--r--   0        0        0     2910 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0    18326 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/search.html
+-rw-r--r--   0        0        0     2168 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/utils.html
+-rw-r--r--   0        0        0     5160 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73396 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0     1222 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/utils.js
+-rw-r--r--   0        0        0    51584 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0    10517 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/computer.png
+-rw-r--r--   0        0        0      549 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0      503 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/copy-solid.svg
+-rw-r--r--   0        0        0      746 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/copy_button.svg
+-rw-r--r--   0        0        0    19662 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/credit-card.png
+-rw-r--r--   0        0        0   205167 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    30234 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-256x256.png
+-rw-r--r--   0        0        0    31531 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0     1100 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/key.svg
+-rw-r--r--   0        0        0    13011 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0    29856 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
+-rw-r--r--   0        0        0  1301428 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0      616 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/microphone-solid.svg
+-rw-r--r--   0        0        0     1578 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     1736 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/openai-logomark.svg
+-rw-r--r--   0        0        0     7946 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0     2945 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/plaintext.svg
+-rw-r--r--   0        0        0     1877 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/question-mark-icon.svg
+-rw-r--r--   0        0        0     1319 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/stop-solid.svg
+-rw-r--r--   0        0        0      503 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/trash-solid.svg
+-rw-r--r--   0        0        0     2233 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/user-silhouette.svg
+-rw-r--r--   0        0        0      951 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/web.svg
+-rw-r--r--   0        0        0     2417 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/whatsapp.svg
+-rw-r--r--   0        0        0   591182 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
+-rw-r--r--   0        0        0   197173 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
+-rw-r--r--   0        0        0   268309 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
+-rw-r--r--   0        0        0   406179 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
+-rw-r--r--   0        0        0    82985 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
+-rw-r--r--   0        0        0   236285 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_default_model.py
+-rw-r--r--   0        0        0     2034 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_default_model_2.py
+-rw-r--r--   0        0        0     2510 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_schema.py
+-rw-r--r--   0        0        0      975 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_model.py
+-rw-r--r--   0        0        0     2025 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_processor_config_openai.py
+-rw-r--r--   0        0        0     5132 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_server_pg.py
+-rw-r--r--   0        0        0      569 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_version.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4715 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/__init__.py
+-rw-r--r--   0        0        0    12604 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/text_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/github/__init__.py
+-rw-r--r--   0        0        0    14040 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/github/github_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/markdown/__init__.py
+-rw-r--r--   0        0        0     5690 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/markdown/markdown_to_entries.py
+-rw-r--r--   0        0        0     9906 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/notion/notion_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/__init__.py
+-rw-r--r--   0        0        0     6377 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/org_to_entries.py
+-rw-r--r--   0        0        0    18246 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/pdf/__init__.py
+-rw-r--r--   0        0        0     4660 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/pdf/pdf_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/plaintext/__init__.py
+-rw-r--r--   0        0        0     3717 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/plaintext/plaintext_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0    21189 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0    10226 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/__init__.py
+-rw-r--r--   0        0        0     8579 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/chat_model.py
+-rw-r--r--   0        0        0     1793 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/utils.py
+-rw-r--r--   0        0        0      470 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/__init__.py
+-rw-r--r--   0        0        0     6896 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/gpt.py
+-rw-r--r--   0        0        0     3284 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/utils.py
+-rw-r--r--   0        0        0      432 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/tools/__init__.py
+-rw-r--r--   0        0        0     5929 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/tools/online_search.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13865 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1443 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api_agents.py
+-rw-r--r--   0        0        0    25148 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api_chat.py
+-rw-r--r--   0        0        0    10827 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api_config.py
+-rw-r--r--   0        0        0     2208 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api_phone.py
+-rw-r--r--   0        0        0     4569 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/auth.py
+-rw-r--r--   0        0        0    28306 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0    10974 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/indexer.py
+-rw-r--r--   0        0        0     3137 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/notion.py
+-rw-r--r--   0        0        0     1151 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/storage.py
+-rw-r--r--   0        0        0     4285 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/subscription.py
+-rw-r--r--   0        0        0     1081 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/twilio.py
+-rw-r--r--   0        0        0    13329 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0    10101 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0      939 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     1005 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0     8916 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     3466 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     1740 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/config.py
+-rw-r--r--   0        0        0      791 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     9519 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/fs_syncer.py
+-rw-r--r--   0        0        0    12034 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     7245 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/initialization.py
+-rw-r--r--   0        0        0     1192 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2009 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4028 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1309 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1430 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      565 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/.gitignore
+-rw-r--r--   0        0        0    34523 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/LICENSE
+-rw-r--r--   0        0        0     2378 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/README.md
+-rw-r--r--   0        0        0     3525 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/pyproject.toml
+-rw-r--r--   0        0        0     5705 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/PKG-INFO
```

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/configure.py` & `khoj_assistant-1.9.1.dev8/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/main.py` & `khoj_assistant-1.9.1.dev8/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/manage.py` & `khoj_assistant-1.9.1.dev8/src/khoj/manage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/app/README.md` & `khoj_assistant-1.9.1.dev8/src/khoj/app/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/app/settings.py` & `khoj_assistant-1.9.1.dev8/src/khoj/app/settings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/app/urls.py` & `khoj_assistant-1.9.1.dev8/src/khoj/app/urls.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/admin.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/admin.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/adapters/__init__.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0001_khojuser.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0001_khojuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0002_googleuser.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0002_googleuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0004_content_types_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0004_content_types_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0006_embeddingsdates.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0006_embeddingsdates.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0007_add_conversation.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0007_add_conversation.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0009_khojapiuser.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0009_khojapiuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0012_entry_file_source.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0012_entry_file_source.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0013_subscription.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0013_subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0015_alter_subscription_user.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0015_alter_subscription_user.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0017_searchmodel.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0017_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0020_reflectivequestion.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0020_reflectivequestion.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0022_texttoimagemodelconfig.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0022_texttoimagemodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0023_usersearchmodelconfig.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0023_usersearchmodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0029_userrequests.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0029_userrequests.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0030_conversation_slug_and_title.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0030_conversation_slug_and_title.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0031_agent_conversation_agent.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0031_agent_conversation_agent.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0031_alter_googleuser_locale.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0031_alter_googleuser_locale.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/database/models/__init__.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/404.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/agent.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/agent.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/agents.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/agents.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/base_config.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/chat.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/config.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/content_source_computer_input.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_computer_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/content_source_github_input.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/content_source_notion_input.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/khoj.webmanifest` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/khoj.webmanifest`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/login.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/login.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/search.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/search.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/utils.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/utils.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/utils.js` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/utils.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/computer.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/computer.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/copy_button.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/copy_button.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/credit-card.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/credit-card.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/favicon-256x256.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/key.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/key.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/microphone-solid.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/microphone-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/openai-logomark.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/openai-logomark.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/plaintext.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/plaintext.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/question-mark-icon.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/question-mark-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/stop-solid.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/stop-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/user-silhouette.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/user-silhouette.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/web.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/web.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/icons/whatsapp.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/whatsapp.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_offline_chat_default_model.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_default_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_offline_chat_default_model_2.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_default_model_2.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_offline_chat_schema.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_schema.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_offline_model.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_processor_config_openai.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_processor_config_openai.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_server_pg.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_server_pg.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/migrations/migrate_version.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_version.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/embeddings.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/embeddings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/content/text_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/text_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/content/github/github_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/github/github_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/content/markdown/markdown_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/markdown/markdown_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/content/notion/notion_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/notion/notion_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/content/org_mode/org_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/org_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/content/org_mode/orgnode.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/content/pdf/pdf_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/pdf/pdf_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/content/plaintext/plaintext_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/plaintext/plaintext_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/utils.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/offline/chat_model.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/chat_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/offline/utils.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/openai/gpt.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/conversation/openai/utils.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/processor/tools/online_search.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/tools/online_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/api.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/api_agents.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api_agents.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/api_chat.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api_chat.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/api_config.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api_config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/api_phone.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api_phone.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/auth.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/auth.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/helpers.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/indexer.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/indexer.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/notion.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/notion.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/storage.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/storage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/subscription.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/twilio.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/twilio.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/routers/web_client.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/search_filter/date_filter.py` & `khoj_assistant-1.9.1.dev8/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/search_filter/file_filter.py` & `khoj_assistant-1.9.1.dev8/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/search_filter/word_filter.py` & `khoj_assistant-1.9.1.dev8/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/search_type/text_search.py` & `khoj_assistant-1.9.1.dev8/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/cli.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/config.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/constants.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/fs_syncer.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/fs_syncer.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/helpers.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/initialization.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/initialization.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/jsonl.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/models.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/rawconfig.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/state.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/src/khoj/utils/yaml.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/.gitignore` & `khoj_assistant-1.9.1.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/LICENSE` & `khoj_assistant-1.9.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/README.md` & `khoj_assistant-1.9.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev5/pyproject.toml` & `khoj_assistant-1.9.1.dev8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Intended Audience :: Information Technology",
 ]
 dependencies = [
     "beautifulsoup4 ~= 4.12.3",
@@ -43,20 +44,20 @@
     "python-multipart >= 0.0.7",
     "jinja2 == 3.1.3",
     "openai >= 1.0.0",
     "tiktoken >= 0.3.2",
     "tenacity >= 8.2.2",
     "pillow ~= 9.5.0",
     "pydantic >= 2.0.0",
-    "pyyaml == 6.0",
+    "pyyaml ~= 6.0",
     "rich >= 13.3.1",
     "schedule == 1.1.0",
     "sentence-transformers == 2.5.1",
     "transformers >= 4.28.0",
-    "torch == 2.0.1",
+    "torch == 2.2.2",
     "uvicorn == 0.17.6",
     "aiohttp ~= 3.9.0",
     "langchain <= 0.2.0",
     "langchain-openai >= 0.0.5",
     "requests >= 2.26.0",
     "anyio == 3.7.1",
     "pymupdf >= 1.23.5",
@@ -66,15 +67,15 @@
     "itsdangerous == 2.1.2",
     "httpx == 0.25.0",
     "pgvector == 0.2.4",
     "psycopg2-binary == 2.9.9",
     "gunicorn == 21.2.0",
     "lxml == 4.9.3",
     "tzdata == 2023.3",
-    "rapidocr-onnxruntime == 1.3.11",
+    "rapidocr-onnxruntime == 1.3.11; python_version<'3.12'",
     "openai-whisper >= 20231117",
     "django-phonenumber-field == 7.3.0",
     "phonenumbers == 8.13.27",
     "markdownify ~= 0.11.6",
     "websockets == 12.0",
 ]
 dynamic = ["version"]
```

### Comparing `khoj_assistant-1.9.1.dev5/PKG-INFO` & `khoj_assistant-1.9.1.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: khoj-assistant
-Version: 1.9.1.dev5
+Version: 1.9.1.dev8
 Summary: An AI copilot for your Second Brain
 Project-URL: Homepage, https://khoj.dev
 Project-URL: Documentation, https://docs.khoj.dev
 Project-URL: Code, https://github.com/khoj-ai/khoj
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Requires-Python: >=3.9
 Requires-Dist: aiohttp~=3.9.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: authlib==1.2.1
@@ -44,23 +45,23 @@
 Requires-Dist: pgvector==0.2.4
 Requires-Dist: phonenumbers==8.13.27
 Requires-Dist: pillow~=9.5.0
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: pymupdf>=1.23.5
 Requires-Dist: python-multipart>=0.0.7
-Requires-Dist: pyyaml==6.0
-Requires-Dist: rapidocr-onnxruntime==1.3.11
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: rapidocr-onnxruntime==1.3.11; python_version < '3.12'
 Requires-Dist: requests>=2.26.0
 Requires-Dist: rich>=13.3.1
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentence-transformers==2.5.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: tiktoken>=0.3.2
-Requires-Dist: torch==2.0.1
+Requires-Dist: torch==2.2.2
 Requires-Dist: transformers>=4.28.0
 Requires-Dist: tzdata==2023.3
 Requires-Dist: uvicorn==0.17.6
 Requires-Dist: websockets==12.0
 Provides-Extra: dev
 Requires-Dist: black>=23.1.0; extra == 'dev'
 Requires-Dist: factory-boy>=3.2.1; extra == 'dev'
```

