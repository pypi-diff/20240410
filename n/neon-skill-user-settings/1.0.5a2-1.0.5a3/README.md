# Comparing `tmp/neon-skill-user_settings-1.0.5a2.tar.gz` & `tmp/neon-skill-user_settings-1.0.5a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-user_settings-1.0.5a2.tar", last modified: Mon Feb  5 22:35:04 2024, max compression
+gzip compressed data, was "neon-skill-user_settings-1.0.5a3.tar", last modified: Wed Apr 10 18:20:19 2024, max compression
```

## Comparing `neon-skill-user_settings-1.0.5a2.tar` & `neon-skill-user_settings-1.0.5a3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.794201 neon-skill-user_settings-1.0.5a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-02-05 22:35:04.794201 neon-skill-user_settings-1.0.5a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    53706 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.770201 neon-skill-user_settings-1.0.5a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.774201 neon-skill-user_settings-1.0.5a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.786200 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/also_change_location_tz.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/birthday_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/birthday_is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/birthday_not_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/birthday_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/change_location_tz.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/date_format_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/date_format_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/dialog_mode_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/dialog_mode_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_already_set_same.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_confirmation.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_overwrite.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/email_set_error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/error_change_username.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/happy_birthday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/hesitation_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/hesitation_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/language_change_confirmation.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/language_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/language_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/language_not_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/language_not_recognized.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/language_not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/language_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/language_setting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/location_is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/location_not_found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/location_uknown_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/location_unknown_online.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/name_confirm_change.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/name_is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/name_no_username.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/name_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/name_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/name_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/name_set_full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/name_set_part.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/only_one_language.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/speech_speed_faster.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/speech_speed_limit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/speech_speed_normal.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/speech_speed_slower.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/time_format_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/time_format_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/transcription_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/transcription_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/units_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/units_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_at.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_audio.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_email_title.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_faster.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_female.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_first_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_full_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_imperial.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_last_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_limited.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_male.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_metric.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_middle_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_preferred_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_primary.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_random.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_secondary.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_slower.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_speak.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_stt.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_text.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_timezone.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_understand.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/dialog/word_username.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.786200 neon-skill-user_settings-1.0.5a2/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/intent/language_settings.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/intent/language_stt.intent
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/intent/language_tts.intent
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/intent/when_is_my_birthday.intent
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/intent/where_am_i.intent
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/intent/who_am_i.intent
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/languages.value
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.786200 neon-skill-user_settings-1.0.5a2/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/regex/language.rx
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/regex/name.rx
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/regex/place.rx
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/regex/primary_tts.rx
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/regex/secondary_tts.rx
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/regex/setting.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.794201 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/at.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/audio.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/birthday.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/date.voc
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/deny.voc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/dialog_mode.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/dmy.voc
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/dot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/email.voc
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/faster.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/female.voc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/first_name.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/full.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/full_name.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/half.voc
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/hesitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/imperial.voc
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/language.voc
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/language_settings.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/language_stt.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/language_tts.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/last_name.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/limited.voc
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/location.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/male.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/mdy.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/metric.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/middle_name.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/my.voc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/my_name_is.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/name.voc
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/no_secondary_language.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/normally.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/permit.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/preferred.voc
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/preferred_name.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/random.voc
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/retention.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/second.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/slower.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/speak_to_me.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/tell_me_my.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/text.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/timezone.voc
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/units.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/username.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/locale/en-us/vocab/ymd.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.794201 neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-02-05 22:35:04.000000 neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-02-05 22:35:04.000000 neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 22:35:04.000000 neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-05 22:35:04.000000 neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-05 22:35:04.000000 neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-05 22:35:04.000000 neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 22:35:04.794201 neon-skill-user_settings-1.0.5a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.794201 neon-skill-user_settings-1.0.5a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    81103 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:35:04.794201 neon-skill-user_settings-1.0.5a2/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/ui/SYSTEM_InputBox.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-05 22:35:01.000000 neon-skill-user_settings-1.0.5a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.023613 neon-skill-user_settings-1.0.5a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-10 18:20:19.023613 neon-skill-user_settings-1.0.5a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    53707 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.003613 neon-skill-user_settings-1.0.5a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.003613 neon-skill-user_settings-1.0.5a3/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.015613 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/also_change_location_tz.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/birthday_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/birthday_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/birthday_not_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/birthday_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/change_location_tz.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/date_format_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/date_format_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/dialog_mode_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/dialog_mode_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_already_set_same.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_confirmation.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_overwrite.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/email_set_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/error_change_username.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/happy_birthday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/hesitation_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/hesitation_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/language_change_confirmation.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/language_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/language_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/language_not_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/language_not_recognized.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/language_not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/language_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/language_setting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/location_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/location_not_found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/location_uknown_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/location_unknown_online.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/name_confirm_change.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/name_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/name_no_username.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/name_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/name_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/name_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/name_set_full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/name_set_part.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/only_one_language.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/speech_speed_faster.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/speech_speed_limit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/speech_speed_normal.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/speech_speed_slower.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/time_format_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/time_format_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/transcription_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/transcription_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/units_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/units_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_at.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_audio.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_email_title.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_faster.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_female.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_first_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_full_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_imperial.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_last_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_limited.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_male.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_metric.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_middle_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_preferred_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_primary.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_random.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_secondary.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_slower.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_speak.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_stt.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_text.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_timezone.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_understand.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/dialog/word_username.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.015613 neon-skill-user_settings-1.0.5a3/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/intent/language_settings.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/intent/language_stt.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/intent/language_tts.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/intent/when_is_my_birthday.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/intent/where_am_i.intent
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/intent/who_am_i.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/languages.value
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.015613 neon-skill-user_settings-1.0.5a3/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/regex/language.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/regex/name.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/regex/place.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/regex/primary_tts.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/regex/secondary_tts.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/regex/setting.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.023613 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/at.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/audio.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/birthday.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/date.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/deny.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/dialog_mode.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/dmy.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/dot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/email.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/faster.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/female.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/first_name.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/full.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/full_name.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/half.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/hesitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/imperial.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/language.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/language_settings.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/language_stt.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/language_tts.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/last_name.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/limited.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/location.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/male.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/mdy.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/metric.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/middle_name.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/my.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/my_name_is.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/name.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/no_secondary_language.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/normally.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/permit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/preferred.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/preferred_name.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/random.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/retention.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/second.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/slower.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/speak_to_me.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/tell_me_my.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/text.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/timezone.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/units.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/username.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/locale/en-us/vocab/ymd.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.023613 neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-10 18:20:18.000000 neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-10 18:20:18.000000 neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:20:18.000000 neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 18:20:18.000000 neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 18:20:18.000000 neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 18:20:18.000000 neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:20:19.023613 neon-skill-user_settings-1.0.5a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.023613 neon-skill-user_settings-1.0.5a3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    81103 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:20:19.023613 neon-skill-user_settings-1.0.5a3/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/ui/SYSTEM_InputBox.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-10 18:20:13.000000 neon-skill-user_settings-1.0.5a3/version.py
```

### Comparing `neon-skill-user_settings-1.0.5a2/LICENSE.md` & `neon-skill-user_settings-1.0.5a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.5a2/PKG-INFO` & `neon-skill-user_settings-1.0.5a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-user_settings
-Version: 1.0.5a2
+Version: 1.0.5a3
 Home-page: https://github.com/NeonGeckoCom/skill-user_settings
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-user_settings-1.0.5a2/README.md` & `neon-skill-user_settings-1.0.5a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.5a2/__init__.py` & `neon-skill-user_settings-1.0.5a3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1069,15 +1069,15 @@
         if self.voc_match(request, "female"):
             return "female"
         LOG.info(f"no gender in request: {request}")
         return None
 
     def _spoken_email(self, email_addr: str):
         """
-        Get a pronouncable email address string
+        Get a pronounceable email address string
         """
         return email_addr.replace('.', f' {self.translate("word_dot")} ')\
             .replace('@', f' {self.translate("word_at")} ')
 
     @staticmethod
     def _get_name_parts(name: str, user_profile: dict) -> dict:
         """
```

### Comparing `neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/PKG-INFO` & `neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-user-settings
-Version: 1.0.5a2
+Version: 1.0.5a3
 Home-page: https://github.com/NeonGeckoCom/skill-user_settings
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-user_settings-1.0.5a2/neon_skill_user_settings.egg-info/SOURCES.txt` & `neon-skill-user_settings-1.0.5a3/neon_skill_user_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.5a2/setup.py` & `neon-skill-user_settings-1.0.5a3/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.5a2/skill.json` & `neon-skill-user_settings-1.0.5a3/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.5a2/test/test_skill.py` & `neon-skill-user_settings-1.0.5a3/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.5a2/ui/SYSTEM_InputBox.qml` & `neon-skill-user_settings-1.0.5a3/ui/SYSTEM_InputBox.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.5a2/version.py` & `neon-skill-user_settings-1.0.5a3/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.5a2"
+__version__ = "1.0.5a3"
```

