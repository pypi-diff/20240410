# Comparing `tmp/guardrails_ai-0.4.2.tar.gz` & `tmp/guardrails_ai-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrails_ai-0.4.2.tar", max compression
+gzip compressed data, was "guardrails_ai-0.4.3.tar", max compression
```

## Comparing `guardrails_ai-0.4.2.tar` & `guardrails_ai-0.4.3.tar`

### file list

```diff
@@ -1,129 +1,134 @@
--rw-r--r--   0        0        0    11357 2024-03-19 20:34:38.658962 guardrails_ai-0.4.2/LICENSE
--rw-r--r--   0        0        0     6848 2024-03-19 20:34:38.658962 guardrails_ai-0.4.2/README.md
--rw-r--r--   0        0        0      641 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/__init__.py
--rw-r--r--   0        0        0     1583 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/api_client.py
--rw-r--r--   0        0        0        0 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/applications/__init__.py
--rw-r--r--   0        0        0     7243 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/applications/text2sql.py
--rw-r--r--   0        0        0      783 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/applications/text2sql.rail
--rw-r--r--   0        0        0      288 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/__init__.py
--rw-r--r--   0        0        0     1694 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/credentials.py
--rw-r--r--   0        0        0      156 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/generic/__init__.py
--rw-r--r--   0        0        0     1450 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/generic/serializeable.py
--rw-r--r--   0        0        0     2826 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/generic/stack.py
--rw-r--r--   0        0        0      346 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/history/__init__.py
--rw-r--r--   0        0        0    14482 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/history/call.py
--rw-r--r--   0        0        0      936 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/history/call_inputs.py
--rw-r--r--   0        0        0     1737 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/history/inputs.py
--rw-r--r--   0        0        0     8172 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/history/iteration.py
--rw-r--r--   0        0        0     4281 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/history/outputs.py
--rw-r--r--   0        0        0      128 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/input_type.py
--rw-r--r--   0        0        0       76 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/output_type.py
--rw-r--r--   0        0        0     3335 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/classes/validation_outcome.py
--rw-r--r--   0        0        0      324 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/__init__.py
--rw-r--r--   0        0        0     2420 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/configure.py
--rw-r--r--   0        0        0       41 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/guardrails.py
--rw-r--r--   0        0        0      189 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/hub/__init__.py
--rw-r--r--   0        0        0     6757 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/hub/create_validator.py
--rw-r--r--   0        0        0       42 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/hub/hub.py
--rw-r--r--   0        0        0     8430 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/hub/install.py
--rw-r--r--   0        0        0     1706 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/hub/submit.py
--rw-r--r--   0        0        0      494 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/logger.py
--rw-r--r--   0        0        0       61 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/server/__init__.py
--rw-r--r--   0        0        0      907 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/server/auth.py
--rw-r--r--   0        0        0     5006 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/server/hub_client.py
--rw-r--r--   0        0        0     1841 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/server/module_manifest.py
--rw-r--r--   0        0        0     1067 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/cli/validate.py
--rw-r--r--   0        0        0      226 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/constants/__init__.py
--rw-r--r--   0        0        0     8367 2024-03-19 20:34:38.774964 guardrails_ai-0.4.2/guardrails/constants.xml
--rw-r--r--   0        0        0    19090 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/datatypes.py
--rw-r--r--   0        0        0     8898 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/document_store.py
--rw-r--r--   0        0        0     7092 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/embedding.py
--rw-r--r--   0        0        0      512 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/errors/__init__.py
--rw-r--r--   0        0        0    52438 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/guard.py
--rw-r--r--   0        0        0       96 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/hub/__init__.py
--rw-r--r--   0        0        0    27170 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/llm_providers.py
--rw-r--r--   0        0        0     2738 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/logger.py
--rw-r--r--   0        0        0      245 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/logging_utils.py
--rw-r--r--   0        0        0      114 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/namespace_template.py
--rw-r--r--   0        0        0      115 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/prompt/__init__.py
--rw-r--r--   0        0        0     3946 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/prompt/base_prompt.py
--rw-r--r--   0        0        0     1411 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/prompt/instructions.py
--rw-r--r--   0        0        0      894 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/prompt/prompt.py
--rw-r--r--   0        0        0    11267 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/rail.py
--rw-r--r--   0        0        0    45788 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/run.py
--rw-r--r--   0        0        0      257 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/schema/__init__.py
--rw-r--r--   0        0        0    18617 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/schema/json_schema.py
--rw-r--r--   0        0        0     5708 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/schema/schema.py
--rw-r--r--   0        0        0     9467 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/schema/string_schema.py
--rw-r--r--   0        0        0     1953 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/stores/context.py
--rw-r--r--   0        0        0      168 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/__init__.py
--rw-r--r--   0        0        0       88 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/args.py
--rw-r--r--   0        0        0      472 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/casting_utils.py
--rw-r--r--   0        0        0     1555 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/constants.py
--rw-r--r--   0        0        0      236 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/dataclass.py
--rw-r--r--   0        0        0     4924 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/docs_utils.py
--rw-r--r--   0        0        0      274 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/exception_utils.py
--rw-r--r--   0        0        0     4435 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/hub_telemetry_utils.py
--rw-r--r--   0        0        0    11220 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/json_utils.py
--rw-r--r--   0        0        0       89 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/kwargs.py
--rw-r--r--   0        0        0      288 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/llm_response.py
--rw-r--r--   0        0        0     3244 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/logs_utils.py
--rw-r--r--   0        0        0     4903 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/misc.py
--rw-r--r--   0        0        0      337 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/on_fail.py
--rw-r--r--   0        0        0     1077 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/openai_utils/__init__.py
--rw-r--r--   0        0        0     1390 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/openai_utils/base.py
--rw-r--r--   0        0        0     2792 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/openai_utils/streaming_utils.py
--rw-r--r--   0        0        0    10818 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/openai_utils/v0.py
--rw-r--r--   0        0        0    11107 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/openai_utils/v1.py
--rw-r--r--   0        0        0     2497 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/parsing_utils.py
--rw-r--r--   0        0        0      757 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/pydantic_utils/__init__.py
--rw-r--r--   0        0        0    18047 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/pydantic_utils/v1.py
--rw-r--r--   0        0        0    17599 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/pydantic_utils/v2.py
--rw-r--r--   0        0        0     7721 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/reask_utils.py
--rw-r--r--   0        0        0     1247 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/safe_get.py
--rw-r--r--   0        0        0     4013 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/sql_utils.py
--rw-r--r--   0        0        0    10841 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/telemetry_utils.py
--rw-r--r--   0        0        0     1488 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/validator_utils.py
--rw-r--r--   0        0        0      507 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/utils/xml_utils.py
--rw-r--r--   0        0        0    18325 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validator_base.py
--rw-r--r--   0        0        0    15848 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validator_service.py
--rw-r--r--   0        0        0     3946 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/__init__.py
--rw-r--r--   0        0        0     1425 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/bug_free_python.py
--rw-r--r--   0        0        0     1703 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/bug_free_sql.py
--rw-r--r--   0        0        0     5567 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/competitor_check.py
--rw-r--r--   0        0        0     7026 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/detect_secrets.py
--rw-r--r--   0        0        0     1819 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/endpoint_is_reachable.py
--rw-r--r--   0        0        0     1335 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/ends_with.py
--rw-r--r--   0        0        0     1884 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/exclude_sql_predicates.py
--rw-r--r--   0        0        0     5533 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/extracted_summary_sentences_match.py
--rw-r--r--   0        0        0     4778 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/extractive_summary.py
--rw-r--r--   0        0        0     3869 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/is_high_quality_translation.py
--rw-r--r--   0        0        0     1540 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/is_profanity_free.py
--rw-r--r--   0        0        0     1091 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/lower_case.py
--rw-r--r--   0        0        0    10671 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/on_topic.py
--rw-r--r--   0        0        0     1204 2024-03-19 20:34:38.778964 guardrails_ai-0.4.2/guardrails/validators/one_line.py
--rw-r--r--   0        0        0     5160 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/pii_filter.py
--rw-r--r--   0        0        0    24837 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/provenance.py
--rw-r--r--   0        0        0     1755 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/pydantic_field_validator.py
--rw-r--r--   0        0        0     3304 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/qa_relevance_llm_eval.py
--rw-r--r--   0        0        0     1769 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/reading_time.py
--rw-r--r--   0        0        0     2455 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/regex_match.py
--rw-r--r--   0        0        0     3075 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/remove_redundant_sentences.py
--rw-r--r--   0        0        0     4572 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/saliency_check.py
--rw-r--r--   0        0        0     3438 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/similar_to_document.py
--rw-r--r--   0        0        0     6425 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/similar_to_list.py
--rw-r--r--   0        0        0     1654 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/sql_column_presence.py
--rw-r--r--   0        0        0     7376 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/toxic_language.py
--rw-r--r--   0        0        0     1422 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/two_words.py
--rw-r--r--   0        0        0     1091 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/upper_case.py
--rw-r--r--   0        0        0     1452 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/valid_choices.py
--rw-r--r--   0        0        0     3198 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/valid_length.py
--rw-r--r--   0        0        0     1946 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/valid_range.py
--rw-r--r--   0        0        0     1407 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/valid_url.py
--rw-r--r--   0        0        0      808 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validators/validators.py
--rw-r--r--   0        0        0    15047 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/validatorsattr.py
--rw-r--r--   0        0        0       93 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/vectordb/__init__.py
--rw-r--r--   0        0        0     2996 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/vectordb/base.py
--rw-r--r--   0        0        0     3338 2024-03-19 20:34:38.782964 guardrails_ai-0.4.2/guardrails/vectordb/faiss.py
--rw-r--r--   0        0        0     3542 2024-03-19 20:34:38.786964 guardrails_ai-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    10095 1970-01-01 00:00:00.000000 guardrails_ai-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 01:03:46.759287 guardrails_ai-0.4.3/LICENSE
+-rw-r--r--   0        0        0     7671 2024-04-10 01:03:46.759287 guardrails_ai-0.4.3/README.md
+-rw-r--r--   0        0        0      675 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/__init__.py
+-rw-r--r--   0        0        0     1628 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/api_client.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/applications/__init__.py
+-rw-r--r--   0        0        0     7243 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/applications/text2sql.py
+-rw-r--r--   0        0        0      783 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/applications/text2sql.rail
+-rw-r--r--   0        0        0      288 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/__init__.py
+-rw-r--r--   0        0        0     1694 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/credentials.py
+-rw-r--r--   0        0        0      156 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/generic/__init__.py
+-rw-r--r--   0        0        0     1450 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/generic/serializeable.py
+-rw-r--r--   0        0        0     2826 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/generic/stack.py
+-rw-r--r--   0        0        0      346 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/__init__.py
+-rw-r--r--   0        0        0    15186 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/call.py
+-rw-r--r--   0        0        0      936 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/call_inputs.py
+-rw-r--r--   0        0        0     1737 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/inputs.py
+-rw-r--r--   0        0        0     8287 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/iteration.py
+-rw-r--r--   0        0        0     4281 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/outputs.py
+-rw-r--r--   0        0        0      128 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/input_type.py
+-rw-r--r--   0        0        0       76 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/output_type.py
+-rw-r--r--   0        0        0     3335 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/validation_outcome.py
+-rw-r--r--   0        0        0      324 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/__init__.py
+-rw-r--r--   0        0        0     2420 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/configure.py
+-rw-r--r--   0        0        0       41 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/guardrails.py
+-rw-r--r--   0        0        0      189 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/hub/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/hub/console.py
+-rw-r--r--   0        0        0     6757 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/hub/create_validator.py
+-rw-r--r--   0        0        0       42 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/hub/hub.py
+-rw-r--r--   0        0        0     9899 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/hub/install.py
+-rw-r--r--   0        0        0     1706 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/hub/submit.py
+-rw-r--r--   0        0        0      425 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/logger.py
+-rw-r--r--   0        0        0       61 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/server/__init__.py
+-rw-r--r--   0        0        0      907 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/server/auth.py
+-rw-r--r--   0        0        0     5006 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/server/hub_client.py
+-rw-r--r--   0        0        0     1841 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/server/module_manifest.py
+-rw-r--r--   0        0        0     1067 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/validate.py
+-rw-r--r--   0        0        0      226 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/constants/__init__.py
+-rw-r--r--   0        0        0     8367 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/constants.xml
+-rw-r--r--   0        0        0    19090 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/datatypes.py
+-rw-r--r--   0        0        0     8898 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/document_store.py
+-rw-r--r--   0        0        0     7092 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/embedding.py
+-rw-r--r--   0        0        0      512 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/errors/__init__.py
+-rw-r--r--   0        0        0    52741 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/guard.py
+-rw-r--r--   0        0        0       96 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/hub/__init__.py
+-rw-r--r--   0        0        0    29727 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/llm_providers.py
+-rw-r--r--   0        0        0     2738 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/logger.py
+-rw-r--r--   0        0        0      245 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/logging_utils.py
+-rw-r--r--   0        0        0      114 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/namespace_template.py
+-rw-r--r--   0        0        0      115 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/prompt/__init__.py
+-rw-r--r--   0        0        0     3946 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/prompt/base_prompt.py
+-rw-r--r--   0        0        0     1411 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/prompt/instructions.py
+-rw-r--r--   0        0        0      894 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/prompt/prompt.py
+-rw-r--r--   0        0        0    11267 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/rail.py
+-rw-r--r--   0        0        0      339 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/__init__.py
+-rw-r--r--   0        0        0    15370 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/async_runner.py
+-rw-r--r--   0        0        0    21453 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/runner.py
+-rw-r--r--   0        0        0     9662 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/stream_runner.py
+-rw-r--r--   0        0        0      441 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/utils.py
+-rw-r--r--   0        0        0      257 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/schema/__init__.py
+-rw-r--r--   0        0        0    18617 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/schema/json_schema.py
+-rw-r--r--   0        0        0     5708 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/schema/schema.py
+-rw-r--r--   0        0        0     9467 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/schema/string_schema.py
+-rw-r--r--   0        0        0     1953 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/stores/context.py
+-rw-r--r--   0        0        0      168 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/args.py
+-rw-r--r--   0        0        0      472 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/casting_utils.py
+-rw-r--r--   0        0        0     1555 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/constants.py
+-rw-r--r--   0        0        0      236 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/dataclass.py
+-rw-r--r--   0        0        0     4924 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/docs_utils.py
+-rw-r--r--   0        0        0      274 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/exception_utils.py
+-rw-r--r--   0        0        0     4435 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/hub_telemetry_utils.py
+-rw-r--r--   0        0        0    11220 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/json_utils.py
+-rw-r--r--   0        0        0       89 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/kwargs.py
+-rw-r--r--   0        0        0      288 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/llm_response.py
+-rw-r--r--   0        0        0     3244 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/logs_utils.py
+-rw-r--r--   0        0        0     4903 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/misc.py
+-rw-r--r--   0        0        0      337 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/on_fail.py
+-rw-r--r--   0        0        0     1077 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/__init__.py
+-rw-r--r--   0        0        0     1390 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/base.py
+-rw-r--r--   0        0        0     2792 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/streaming_utils.py
+-rw-r--r--   0        0        0    10818 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/v0.py
+-rw-r--r--   0        0        0    11107 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/v1.py
+-rw-r--r--   0        0        0     2497 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/parsing_utils.py
+-rw-r--r--   0        0        0      757 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/__init__.py
+-rw-r--r--   0        0        0    18102 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/v1.py
+-rw-r--r--   0        0        0    17654 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/v2.py
+-rw-r--r--   0        0        0     7721 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/reask_utils.py
+-rw-r--r--   0        0        0     1247 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/safe_get.py
+-rw-r--r--   0        0        0     4013 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/sql_utils.py
+-rw-r--r--   0        0        0    10841 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/telemetry_utils.py
+-rw-r--r--   0        0        0     1488 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/validator_utils.py
+-rw-r--r--   0        0        0      507 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/xml_utils.py
+-rw-r--r--   0        0        0    18967 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/validator_base.py
+-rw-r--r--   0        0        0    16056 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/validator_service.py
+-rw-r--r--   0        0        0     3946 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/validators/__init__.py
+-rw-r--r--   0        0        0     1425 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/bug_free_python.py
+-rw-r--r--   0        0        0     1703 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/bug_free_sql.py
+-rw-r--r--   0        0        0     5567 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/competitor_check.py
+-rw-r--r--   0        0        0     7037 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/detect_secrets.py
+-rw-r--r--   0        0        0     1857 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/endpoint_is_reachable.py
+-rw-r--r--   0        0        0     1373 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/ends_with.py
+-rw-r--r--   0        0        0     1884 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/exclude_sql_predicates.py
+-rw-r--r--   0        0        0     5533 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/extracted_summary_sentences_match.py
+-rw-r--r--   0        0        0     4778 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/extractive_summary.py
+-rw-r--r--   0        0        0     3869 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/is_high_quality_translation.py
+-rw-r--r--   0        0        0     1540 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/is_profanity_free.py
+-rw-r--r--   0        0        0     1091 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/lower_case.py
+-rw-r--r--   0        0        0    10671 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/on_topic.py
+-rw-r--r--   0        0        0     1204 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/one_line.py
+-rw-r--r--   0        0        0     5160 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/pii_filter.py
+-rw-r--r--   0        0        0    24837 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/provenance.py
+-rw-r--r--   0        0        0     1755 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/pydantic_field_validator.py
+-rw-r--r--   0        0        0     3304 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/qa_relevance_llm_eval.py
+-rw-r--r--   0        0        0     1784 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/reading_time.py
+-rw-r--r--   0        0        0     2455 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/regex_match.py
+-rw-r--r--   0        0        0     3075 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/remove_redundant_sentences.py
+-rw-r--r--   0        0        0     4572 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/saliency_check.py
+-rw-r--r--   0        0        0     3438 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/similar_to_document.py
+-rw-r--r--   0        0        0     6425 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/similar_to_list.py
+-rw-r--r--   0        0        0     1654 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/sql_column_presence.py
+-rw-r--r--   0        0        0     7376 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/toxic_language.py
+-rw-r--r--   0        0        0     1422 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/two_words.py
+-rw-r--r--   0        0        0     1091 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/upper_case.py
+-rw-r--r--   0        0        0     1452 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/valid_choices.py
+-rw-r--r--   0        0        0     3198 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/valid_length.py
+-rw-r--r--   0        0        0     1946 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/valid_range.py
+-rw-r--r--   0        0        0     1407 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/valid_url.py
+-rw-r--r--   0        0        0      808 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/validators.py
+-rw-r--r--   0        0        0    15075 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validatorsattr.py
+-rw-r--r--   0        0        0       93 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/vectordb/__init__.py
+-rw-r--r--   0        0        0     2996 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/vectordb/base.py
+-rw-r--r--   0        0        0     3338 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/vectordb/faiss.py
+-rw-r--r--   0        0        0     3488 2024-04-10 01:03:46.887288 guardrails_ai-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    11005 1970-01-01 00:00:00.000000 guardrails_ai-0.4.3/PKG-INFO
```

### Comparing `guardrails_ai-0.4.2/LICENSE` & `guardrails_ai-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/README.md` & `guardrails_ai-0.4.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -60,49 +60,69 @@
 
     ```bash
     guardrails hub install hub://guardrails/regex_match
     ```
 3. Create a Guard from the installed guardrail.
 
     ```python
-    # Import Guard and Validator
+    from guardrails import Guard, OnFailAction
     from guardrails.hub import RegexMatch
-    from guardrails import Guard
 
-    # Initialize the Guard with 
-    val = Guard().use(
-        RegexMatch(regex="^[A-Z][a-z]*$")
+    guard = Guard().use(
+        RegexMatch, regex="\(?\d{3}\)?-? *\d{3}-? *-?\d{4}", on_fail=OnFailAction.EXCEPTION
     )
 
-    guard.parse("Caesar")  # Guardrail Passes
-    guard.parse("Caesar is a great leader")  # Guardrail Fails
+    guard.validate("123-456-7890")  # Guardrail passes
+
+    try:
+        guard.validate("1234-789-0000")  # Guardrail fails
+    except Exception as e:
+        print(e)
+    ```
+    Output:
+    ```console
+    Validation failed for field with errors: Result must match \(?\d{3}\)?-? *\d{3}-? *-?\d{4}
     ```
 4. Run multiple guardrails within a Guard.
     First, install the necessary guardrails from Guardrails Hub.
 
     ```bash
     guardrails hub install hub://guardrails/competitor_check
     guardrails hub install hub://guardrails/toxic_language
     ```
 
     Then, create a Guard from the installed guardrails.
     
     ```python
-    from guardrails.hub import RegexMatch, ValidLength
-    from guardrails import Guard
+    from guardrails import Guard, OnFailAction
+    from guardrails.hub import CompetitorCheck, ToxicLanguage
 
-    guard = Guard().use(
-        RegexMatch(regex="^[A-Z][a-z]*$"),
-        ValidLength(min=1, max=32)
+    guard = Guard().use_many(
+        CompetitorCheck(["Apple", "Microsoft", "Google"], on_fail=OnFailAction.EXCEPTION),
+        ToxicLanguage(threshold=0.5, validation_method="sentence", on_fail=OnFailAction.EXCEPTION),),
     )
 
-    guard.parse("Caesar")  # Guardrail Passes
-    guard.parse("Caesar is a great leader")  # Guardrail Fails
+    guard.validate(
+        """An apple a day keeps a doctor away.
+        This is good advice for keeping your health."""
+    )  # Both the guardrails pass
+
+    try:
+        guard.validate(
+            """Shut the hell up! Apple just released a new iPhone."""
+        )  # Both the guardrails fail
+    except Exception as e:
+        print(e)
     ```
+    Output:
+    ```console
+    Validation failed for field with errors: Found the following competitors: [['Apple']]. Please avoid naming those competitors next time, The following sentences in your response were found to be toxic:
 
+    - Shut the hell up!
+    ```
 
 ### Use Guardrails to generate structured data from LLMs
 
 
 Let's go through an example where we ask an LLM to generate fake pet names. To do this, we'll create a Pydantic [BaseModel](https://docs.pydantic.dev/latest/api/base_model/) that represents the structure of the output we want.
 
 ```py
@@ -129,15 +149,15 @@
 guard = Guard.from_pydantic(output_class=Pet, prompt=prompt)
 
 validated_output, *rest = guard(
     llm_api=openai.completions.create,
     engine="gpt-3.5-turbo-instruct"
 )
 
-print(f"{validated_output}")
+print(validated_output)
 ```
 
 This prints: 
 ```
 {
     "pet_type": "dog",
     "name": "Buddy
```

### Comparing `guardrails_ai-0.4.2/guardrails/__init__.py` & `guardrails_ai-0.4.3/guardrails/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 from guardrails.guard import Guard
 from guardrails.llm_providers import PromptCallableBase
 from guardrails.logging_utils import configure_logging
 from guardrails.prompt import Instructions, Prompt
 from guardrails.rail import Rail
 from guardrails.utils import constants, docs_utils
-from guardrails.validator_base import Validator, register_validator
+from guardrails.validator_base import OnFailAction, Validator, register_validator
 
 __all__ = [
     "Guard",
     "PromptCallableBase",
     "Rail",
     "Validator",
+    "OnFailAction",
     "register_validator",
     "constants",
     "docs_utils",
     "configure_logging",
     "Prompt",
     "Instructions",
 ]
```

### Comparing `guardrails_ai-0.4.2/guardrails/api_client.py` & `guardrails_ai-0.4.3/guardrails/api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,18 @@
             if base_url is not None
             else os.environ.get("GUARDRAILS_BASE_URL", "http://localhost:8000")
         )
         self.api_key = (
             api_key if api_key is not None else os.environ.get("GUARDRAILS_API_KEY", "")
         )
         self._client = AuthenticatedClient(
-            _base_url=self.base_url,
-            _follow_redirects=True,
+            base_url=self.base_url,  # type: ignore
+            follow_redirects=True,  # type: ignore
             token=self.api_key,
-            _timeout=Timeout(300),
+            timeout=Timeout(300),  # type: ignore
         )
 
     def upsert_guard(self, guard: Guard):
         update_guard.sync(guard_name=guard.name, client=self._client, body=guard)
 
     def validate(
         self,
```

### Comparing `guardrails_ai-0.4.2/guardrails/applications/text2sql.py` & `guardrails_ai-0.4.3/guardrails/applications/text2sql.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/applications/text2sql.rail` & `guardrails_ai-0.4.3/guardrails/applications/text2sql.rail`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/classes/credentials.py` & `guardrails_ai-0.4.3/guardrails/classes/credentials.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/classes/generic/serializeable.py` & `guardrails_ai-0.4.3/guardrails/classes/generic/serializeable.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/classes/generic/stack.py` & `guardrails_ai-0.4.3/guardrails/classes/generic/stack.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/classes/history/call.py` & `guardrails_ai-0.4.3/guardrails/classes/history/call.py`

 * *Files 6% similar despite different names*

```diff
@@ -265,18 +265,36 @@
         completed.
 
         This property contains the aggregate validated output after all
         validation stages have been completed. Some values in the
         validated output may be "fixed" values that were corrected
         during validation.
 
-        This will only have a value if the Guard is in a passing state.
+        This will only have a value if the Guard is in a passing state
+        OR if the action is no-op.
         """
         if self.status == pass_status:
             return self.fixed_output
+        last_iteration = self.iterations.last
+        if (
+            not self.status == pass_status
+            and last_iteration
+            and last_iteration.failed_validations
+        ):
+            # check that all failed validations are noop or none
+            all_noop = True
+            for failed_validation in last_iteration.failed_validations:
+                if (
+                    failed_validation.value_after_validation
+                    is not failed_validation.value_before_validation
+                ):
+                    all_noop = False
+                    break
+            if all_noop:
+                return last_iteration.guarded_output
 
     @property
     @deprecated(
         """'Call.validated_output' is deprecated and will be removed in \
 versions 0.5.0 and beyond. Use 'guarded_output' instead."""
     )
     def validated_output(self) -> Optional[Union[str, Dict]]:
```

### Comparing `guardrails_ai-0.4.2/guardrails/classes/history/call_inputs.py` & `guardrails_ai-0.4.3/guardrails/classes/history/call_inputs.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/classes/history/inputs.py` & `guardrails_ai-0.4.3/guardrails/classes/history/inputs.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/classes/history/iteration.py` & `guardrails_ai-0.4.3/guardrails/classes/history/iteration.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,15 +211,17 @@
                     style="on #F0F8FF",
                 ),
                 Panel(table, title="Message History", style="on #E7DFEB"),
                 Panel(
                     self.raw_output or "", title="Raw LLM Output", style="on #F5F5DC"
                 ),
                 Panel(
-                    pretty_repr(self.validation_response),
+                    self.validation_response
+                    if isinstance(self.validation_response, str)
+                    else pretty_repr(self.validation_response),
                     title="Validated Output",
                     style="on #F0FFF0",
                 ),
             )
 
     def __str__(self) -> str:
         return pretty_repr(self)
```

### Comparing `guardrails_ai-0.4.2/guardrails/classes/history/outputs.py` & `guardrails_ai-0.4.3/guardrails/classes/history/outputs.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/classes/validation_outcome.py` & `guardrails_ai-0.4.3/guardrails/classes/validation_outcome.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/cli/configure.py` & `guardrails_ai-0.4.3/guardrails/cli/configure.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/cli/hub/create_validator.py` & `guardrails_ai-0.4.3/guardrails/cli/hub/create_validator.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/cli/hub/install.py` & `guardrails_ai-0.4.3/guardrails/cli/hub/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 from guardrails.classes.generic import Stack
 from guardrails.cli.hub.hub import hub_command
 from guardrails.cli.logger import LEVELS, logger
 from guardrails.cli.server.hub_client import get_validator_manifest
 from guardrails.cli.server.module_manifest import ModuleManifest
 
+from .console import console
+
 
 def removesuffix(string: str, suffix: str) -> str:
     if sys.version_info.minor >= 9:
         return string.removesuffix(suffix)  # type: ignore
     else:
         if string.endswith(suffix):
             return string[: -len(suffix)]
@@ -30,25 +32,35 @@
 
 
 def pip_process(
     action: str,
     package: str = "",
     flags: List[str] = [],
     format: Union[Literal["string"], Literal["json"]] = string_format,
-):
+) -> Union[str, dict]:
     try:
         logger.debug(f"running pip {action} {' '.join(flags)} {package}")
         command = [sys.executable, "-m", "pip", action]
         command.extend(flags)
         if package:
             command.append(package)
         output = subprocess.check_output(command)
         logger.debug(f"decoding output from pip {action} {package}")
         if format == json_format:
-            return BytesHeaderParser().parsebytes(output)
+            parsed = BytesHeaderParser().parsebytes(output)
+            try:
+                return json.loads(str(parsed))
+            except Exception:
+                logger.debug(
+                    f"json parse exception in decoding output from pip {action} {package}. Falling back to accumulating the byte stream",  # noqa
+                )
+            accumulator = {}
+            for key, value in parsed.items():
+                accumulator[key] = value
+            return accumulator
         return str(output.decode())
     except subprocess.CalledProcessError as exc:
         logger.error(
             (
                 f"Failed to {action} {package}\n"
                 f"Exit code: {exc.returncode}\n"
                 f"stdout: {exc.output}"
@@ -185,25 +197,30 @@
 
 def install_hub_module(module_manifest: ModuleManifest, site_packages: str):
     install_url = get_install_url(module_manifest)
     install_directory = get_hub_directory(module_manifest, site_packages)
 
     # Install validator module in namespaced directory under guardrails.hub
     download_output = pip_process(
-        "install", install_url, [f"--target={install_directory}", "--no-deps"]
+        "install", install_url, [f"--target={install_directory}", "--no-deps", "-q"]
     )
     logger.info(download_output)
 
     # Install validator module's dependencies in normal site-packages directory
     inspect_output = pip_process(
         "inspect", flags=[f"--path={install_directory}"], format=json_format
     )
-    inspection: dict = json.loads(str(inspect_output))
+
+    # throw if inspect_output is a string. Mostly for pyright
+    if isinstance(inspect_output, str):
+        logger.error("Failed to inspect the installed package!")
+        sys.exit(1)
+
     dependencies = (
-        Stack(*inspection.get("installed", []))
+        Stack(*inspect_output.get("installed", []))
         .at(0, {})
         .get("metadata", {})  # type: ignore
         .get("requires_dist", [])  # type: ignore
     )
     requirements = filter(lambda dep: "extra" not in dep, dependencies)
     for req in requirements:
         req_info = Stack(*req.split(" "))
@@ -221,32 +238,60 @@
         help="URI to the package to install. Example: hub://guardrails/regex_match."
     ),
 ):
     """Install a validator from the Hub."""
     if not package_uri.startswith("hub://"):
         logger.error("Invalid URI!")
         sys.exit(1)
+
+    console.print(f"\nInstalling {package_uri}...\n")
     logger.log(
-        level=LEVELS.get("NOTICE"), msg=f"Installing {package_uri}..."  # type: ignore
+        level=LEVELS.get("SPAM"), msg=f"Installing {package_uri}..."  # type: ignore
     )
+
     # Validation
     module_name = package_uri.replace("hub://", "")
 
     # Prep
-    module_manifest = get_validator_manifest(module_name)
-    site_packages = get_site_packages_location()
+    with console.status("Fetching manifest", spinner="bouncingBar"):
+        module_manifest = get_validator_manifest(module_name)
+        site_packages = get_site_packages_location()
 
     # Install
-    install_hub_module(module_manifest, site_packages)
+    with console.status("Downloading dependencies", spinner="bouncingBar"):
+        install_hub_module(module_manifest, site_packages)
 
     # Post-install
-    run_post_install(module_manifest, site_packages)
-    add_to_hub_inits(module_manifest, site_packages)
-    success_message = Template(
-        """
-
-    Successfully installed ${module_name}!
-
-    See how to use it here: https://hub.guardrailsai.com/validator/${id}
-    """
-    ).safe_substitute(module_name=module_name, id=module_manifest.id)
-    logger.log(level=LEVELS.get("SUCCESS"), msg=success_message)  # type: ignore
+    with console.status("Running post-install setup", spinner="bouncingBar"):
+        run_post_install(module_manifest, site_packages)
+        add_to_hub_inits(module_manifest, site_packages)
+
+    success_message_cli = Template(
+        """✅Successfully installed ${module_name}!
+
+[bold]Import validator:[/bold]
+from guardrails.hub import ${export}
+
+[bold]Get more info:[/bold]
+https://hub.guardrailsai.com/validator/${id}
+"""
+    ).safe_substitute(
+        module_name=package_uri,
+        id=module_manifest.id,
+        export=module_manifest.exports[0],
+    )
+    success_message_logger = Template(
+        """✅Successfully installed ${module_name}!
+
+Import validator:
+from guardrails.hub import ${export}
+
+Get more info:
+https://hub.guardrailsai.com/validator/${id}
+"""
+    ).safe_substitute(
+        module_name=package_uri,
+        id=module_manifest.id,
+        export=module_manifest.exports[0],
+    )
+    console.print(success_message_cli)  # type: ignore
+    logger.log(level=LEVELS.get("SPAM"), msg=success_message_logger)  # type: ignore
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `guardrails_ai-0.4.2/guardrails/cli/hub/submit.py` & `guardrails_ai-0.4.3/guardrails/cli/hub/submit.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/cli/server/auth.py` & `guardrails_ai-0.4.3/guardrails/cli/server/auth.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/cli/server/hub_client.py` & `guardrails_ai-0.4.3/guardrails/cli/server/hub_client.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/cli/server/module_manifest.py` & `guardrails_ai-0.4.3/guardrails/cli/server/module_manifest.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/cli/validate.py` & `guardrails_ai-0.4.3/guardrails/cli/validate.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/constants.xml` & `guardrails_ai-0.4.3/guardrails/constants.xml`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/datatypes.py` & `guardrails_ai-0.4.3/guardrails/datatypes.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/document_store.py` & `guardrails_ai-0.4.3/guardrails/document_store.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/embedding.py` & `guardrails_ai-0.4.3/guardrails/embedding.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/errors/__init__.py` & `guardrails_ai-0.4.3/guardrails/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/guard.py` & `guardrails_ai-0.4.3/guardrails/guard.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
         instructions: Optional[str] = None,
         msg_history: Optional[List[Dict]] = None,
         metadata: Optional[Dict] = None,
         full_schema_reask: Optional[bool] = None,
         stream: Optional[bool] = False,
         *args,
         **kwargs,
-    ) -> Union[ValidationOutcome[OT], Iterable[str]]:
+    ) -> Union[ValidationOutcome[OT], Iterable[ValidationOutcome[OT]]]:
         ...
 
     @overload
     def __call__(
         self,
         llm_api: Callable[[Any], Awaitable[Any]],
         prompt_params: Optional[Dict] = None,
@@ -495,15 +495,16 @@
         instructions: Optional[str] = None,
         msg_history: Optional[List[Dict]] = None,
         metadata: Optional[Dict] = None,
         full_schema_reask: Optional[bool] = None,
         *args,
         **kwargs,
     ) -> Union[
-        Union[ValidationOutcome[OT], Iterable[str]], Awaitable[ValidationOutcome[OT]]
+        Union[ValidationOutcome[OT], Iterable[ValidationOutcome[OT]]],
+        Awaitable[ValidationOutcome[OT]],
     ]:
         """Call the LLM and validate the output. Pass an async LLM API to
         return a coroutine.
 
         Args:
             llm_api: The LLM API to call
                      (e.g. openai.Completion.create or openai.Completion.acreate)
@@ -659,15 +660,15 @@
         instructions: Optional[str],
         msg_history: Optional[List[Dict]],
         metadata: Dict,
         full_schema_reask: bool,
         call_log: Call,
         *args,
         **kwargs,
-    ) -> Union[ValidationOutcome[OT], Iterable[str]]:
+    ) -> Union[ValidationOutcome[OT], Iterable[ValidationOutcome[OT]]]:
         instructions_obj = instructions or self.instructions
         prompt_obj = prompt or self.prompt
         msg_history_obj = msg_history or []
         if prompt_obj is None:
             if msg_history is not None and not len(msg_history_obj):
                 raise RuntimeError(
                     "You must provide a prompt if msg_history is empty. "
@@ -1425,43 +1426,47 @@
                                 else h.parsed_output
                             ),
                             validation_output=(
                                 h.validated_output.to_dict()
                                 if isinstance(h.validated_output, AnyObject)
                                 else h.validated_output
                             ),
-                            reasks=(
+                            reasks=list(
                                 [
-                                    (
-                                        FieldReAsk(
-                                            incorrect_value=r.to_dict().get(
-                                                "incorrect_value"
-                                            ),
-                                            path=r.to_dict().get("path"),
-                                            fail_results=[
-                                                FailResult(
-                                                    error_message=r.to_dict().get(
-                                                        "error_message"
-                                                    ),
-                                                    fix_value=r.to_dict().get(
-                                                        "fix_value"
-                                                    ),
-                                                )
-                                            ],
-                                        )
-                                        for r in h.reasks  # type: ignore
+                                    FieldReAsk(
+                                        incorrect_value=r.to_dict().get(
+                                            "incorrect_value"
+                                        ),
+                                        path=r.to_dict().get("path"),
+                                        fail_results=[
+                                            FailResult(
+                                                error_message=r.to_dict().get(
+                                                    "error_message"
+                                                ),
+                                                fix_value=r.to_dict().get("fix_value"),
+                                            )
+                                        ],
                                     )
+                                    for r in h.reasks  # type: ignore
                                 ]
                                 if h.reasks != UNSET
                                 else []
                             ),
                         ),
                     )
                     for h in history_events
                 ]
                 call_log.iterations.extend(iterations)
                 if self.history.length == 0:
                     self.history.push(call_log)
 
-            return ValidationOutcome[OT].from_guard_history(call_log)
+            # Our interfaces are too different for this to work right now.
+            # Once we move towards shared interfaces for both the open source
+            # and the api we can re-enable this.
+            # return ValidationOutcome[OT].from_guard_history(call_log)
+            return ValidationOutcome[OT](
+                raw_llm_output=validation_output.raw_llm_response,  # type: ignore
+                validated_output=cast(OT, validation_output.validated_output),
+                validation_passed=validation_output.result,
+            )
         else:
             raise ValueError("Guard does not have an api client!")
```

### Comparing `guardrails_ai-0.4.2/guardrails/llm_providers.py` & `guardrails_ai-0.4.3/guardrails/llm_providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,14 +276,33 @@
         )
         ```
         """  # noqa
 
         if "instructions" in kwargs:
             prompt = kwargs.pop("instructions") + "\n\n" + prompt
 
+        def is_base_cohere_chat(func):
+            try:
+                return (
+                    func.__closure__[1].cell_contents.__func__.__qualname__
+                    == "BaseCohere.chat"
+                )
+            except (AttributeError, IndexError):
+                return False
+
+        # TODO: When cohere totally gets rid of `generate`,
+        #       remove this cond and the final return
+        if is_base_cohere_chat(client_callable):
+            cohere_response = client_callable(
+                message=prompt, model=model, *args, **kwargs
+            )
+            return LLMResponse(
+                output=cohere_response.text,
+            )
+
         cohere_response = client_callable(prompt=prompt, model=model, *args, **kwargs)
         return LLMResponse(
             output=cohere_response[0].text,
         )
 
 
 class AnthropicCallable(PromptCallableBase):
@@ -372,14 +391,24 @@
                 prompt=text,
                 instructions=instructions,
                 msg_history=msg_history,
             ),
             *args,
             **kwargs,
         )
+
+        if kwargs.get("stream", False):
+            # If stream is defined and set to True,
+            # the callable returns a generator object
+            llm_response = cast(Iterable[str], response)
+            return LLMResponse(
+                output="",
+                stream_output=llm_response,
+            )
+
         return LLMResponse(
             output=response.choices[0].message.content,  # type: ignore
             prompt_token_count=response.usage.prompt_tokens,  # type: ignore
             response_token_count=response.usage.completion_tokens,  # type: ignore
         )
 
 
@@ -558,15 +587,15 @@
 
     try:
         import cohere  # noqa: F401 # type: ignore
 
         if (
             isinstance(getattr(llm_api, "__self__", None), cohere.Client)
             and getattr(llm_api, "__name__", None) == "generate"
-        ):
+        ) or getattr(llm_api, "__module__", None) == "cohere.client":
             return CohereCallable(*args, client_callable=llm_api, **kwargs)
     except ImportError:
         pass
 
     try:
         import anthropic.resources  # noqa: F401 # type: ignore
 
@@ -759,14 +788,61 @@
             ),
             *args,
             **fn_kwargs,
             **kwargs,
         )
 
 
+class AsyncLiteLLMCallable(AsyncPromptCallableBase):
+    async def invoke_llm(
+        self,
+        text: str,
+        instructions: Optional[str] = None,
+        *args,
+        **kwargs,
+    ):
+        """Wrapper for Lite LLM completions.
+
+        To use Lite LLM for guardrails, do
+        ```
+        from litellm import completion
+
+        raw_llm_response, validated_response = guard(
+            completion,
+            model="gpt-3.5-turbo",
+            prompt_params={...},
+            temperature=...,
+            ...
+        )
+        ```
+        """
+        try:
+            from litellm import acompletion  # type: ignore
+        except ImportError as e:
+            raise PromptCallableException(
+                "The `litellm` package is not installed. "
+                "Install with `pip install litellm`"
+            ) from e
+
+        response = await acompletion(
+            messages=litellm_messages(
+                prompt=text,
+                instructions=instructions,
+            ),
+            *args,
+            **kwargs,
+        )
+
+        return LLMResponse(
+            output=response.choices[0].message.content,  # type: ignore
+            prompt_token_count=response.usage.prompt_tokens,  # type: ignore
+            response_token_count=response.usage.completion_tokens,  # type: ignore
+        )
+
+
 class AsyncManifestCallable(AsyncPromptCallableBase):
     async def invoke_llm(
         self,
         text: str,
         client: Any,
         instructions: Optional[str] = None,
         *args,
@@ -837,14 +913,22 @@
         import manifest  # noqa: F401 # type: ignore
 
         if isinstance(llm_api, manifest.Manifest):
             return AsyncManifestCallable(*args, client=llm_api, **kwargs)
     except ImportError:
         pass
 
+    try:
+        import litellm
+
+        if llm_api == litellm.acompletion:
+            return AsyncLiteLLMCallable(*args, **kwargs)
+    except ImportError:
+        pass
+
     return AsyncArbitraryCallable(*args, llm_api=llm_api, **kwargs)
 
 
 def model_is_supported_server_side(
     llm_api: Optional[Union[Callable, Callable[[Any], Awaitable[Any]]]] = None,
     *args,
     **kwargs,
```

### Comparing `guardrails_ai-0.4.2/guardrails/logger.py` & `guardrails_ai-0.4.3/guardrails/logger.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/prompt/base_prompt.py` & `guardrails_ai-0.4.3/guardrails/prompt/base_prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/prompt/instructions.py` & `guardrails_ai-0.4.3/guardrails/prompt/instructions.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/prompt/prompt.py` & `guardrails_ai-0.4.3/guardrails/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/rail.py` & `guardrails_ai-0.4.3/guardrails/rail.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/schema/json_schema.py` & `guardrails_ai-0.4.3/guardrails/schema/json_schema.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/schema/schema.py` & `guardrails_ai-0.4.3/guardrails/schema/schema.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/schema/string_schema.py` & `guardrails_ai-0.4.3/guardrails/schema/string_schema.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/stores/context.py` & `guardrails_ai-0.4.3/guardrails/stores/context.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/constants.py` & `guardrails_ai-0.4.3/guardrails/utils/constants.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/docs_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/docs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/hub_telemetry_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/hub_telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/json_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/logs_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/logs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/misc.py` & `guardrails_ai-0.4.3/guardrails/utils/misc.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/openai_utils/__init__.py` & `guardrails_ai-0.4.3/guardrails/utils/openai_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/openai_utils/base.py` & `guardrails_ai-0.4.3/guardrails/utils/openai_utils/base.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/openai_utils/streaming_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/openai_utils/streaming_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/openai_utils/v0.py` & `guardrails_ai-0.4.3/guardrails/utils/openai_utils/v0.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/openai_utils/v1.py` & `guardrails_ai-0.4.3/guardrails/utils/openai_utils/v1.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/parsing_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/pydantic_utils/__init__.py` & `guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/pydantic_utils/v1.py` & `guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from guardrails.datatypes import Float as FloatDataType
 from guardrails.datatypes import Integer as IntegerDataType
 from guardrails.datatypes import List as ListDataType
 from guardrails.datatypes import Object as ObjectDataType
 from guardrails.datatypes import String as StringDataType
 from guardrails.datatypes import Time as TimeDataType
 from guardrails.utils.safe_get import safe_get
-from guardrails.validator_base import Validator
+from guardrails.validator_base import OnFailAction, Validator
 from guardrails.validatorsattr import ValidatorsAttr
 
 
 class ArbitraryModel(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
@@ -214,15 +214,17 @@
 
         for val in vals:
             gd_validator = convert_pydantic_validator_to_guardrails_validator(
                 model, val
             )
             if "validators" not in fld.field_info.extra:
                 fld.field_info.extra["validators"] = []
-            fld.field_info.extra["validators"].append((gd_validator, "reask"))
+            fld.field_info.extra["validators"].append(
+                (gd_validator, OnFailAction.REASK)
+            )
 
     model_fields = {}
     for field_name, field in model.__fields__.items():
         field_copy = deepcopy(field)
 
         if "validators" in field.field_info.extra and not isinstance(
             field.field_info.extra["validators"], list
```

### Comparing `guardrails_ai-0.4.2/guardrails/utils/pydantic_utils/v2.py` & `guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from guardrails.datatypes import Float as FloatDataType
 from guardrails.datatypes import Integer as IntegerDataType
 from guardrails.datatypes import List as ListDataType
 from guardrails.datatypes import Object as ObjectDataType
 from guardrails.datatypes import String as StringDataType
 from guardrails.datatypes import Time as TimeDataType
 from guardrails.utils.safe_get import safe_get
-from guardrails.validator_base import Validator
+from guardrails.validator_base import OnFailAction, Validator
 from guardrails.validatorsattr import ValidatorsAttr
 
 DataTypeT = TypeVar("DataTypeT", bound=DataType)
 
 try:
     from pydantic import Discriminator  # type: ignore
 
@@ -244,15 +244,17 @@
 
         for val in vals:
             gd_validator = convert_pydantic_validator_to_guardrails_validator(
                 model, val
             )
             if "validators" not in fld.field_info.json_schema_extra:
                 fld.json_schema_extra["validators"] = []
-            fld.json_schema_extra["validators"].append((gd_validator, "reask"))
+            fld.json_schema_extra["validators"].append(
+                (gd_validator, OnFailAction.REASK)
+            )
 
     model_fields = {}
     for field_name, field in model.model_fields.items():
         field_copy = deepcopy(field)
         if field.json_schema_extra is None:
             field_copy.json_schema_extra = {}
```

### Comparing `guardrails_ai-0.4.2/guardrails/utils/reask_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/reask_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/safe_get.py` & `guardrails_ai-0.4.3/guardrails/utils/safe_get.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/sql_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/telemetry_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/utils/validator_utils.py` & `guardrails_ai-0.4.3/guardrails/utils/validator_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validator_base.py` & `guardrails_ai-0.4.3/guardrails/validator_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 from collections import defaultdict
 from copy import deepcopy
+from enum import Enum
 from string import Template
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Literal,
@@ -369,26 +370,38 @@
 class FailResult(ValidationResult):
     outcome: Literal["fail"] = "fail"
 
     error_message: str
     fix_value: Optional[Any] = None
 
 
+class OnFailAction(str, Enum):
+    REASK = "reask"
+    FIX = "fix"
+    FILTER = "filter"
+    REFRAIN = "refrain"
+    NOOP = "noop"
+    EXCEPTION = "exception"
+    FIX_REASK = "fix_reask"
+
+
 @dataclass  # type: ignore
 class Validator(Runnable):
     """Base class for validators."""
 
     rail_alias: str = ""
 
     run_in_separate_process = False
     override_value_on_pass = False
     required_metadata_keys = []
     _metadata = {}
 
-    def __init__(self, on_fail: Optional[Union[Callable, str]] = None, **kwargs):
+    def __init__(
+        self, on_fail: Optional[Union[Callable, OnFailAction]] = None, **kwargs
+    ):
         # Raise a warning for deprecated validators
 
         # Get class name and rail_alias
         child_class_name = str(type(self).__name__)
         validator_rail_alias = self.rail_alias
 
         # Check if this rail_alias is deprecated
@@ -405,22 +418,31 @@
             else:
                 warn(
                     f"""{child_class_name} is deprecated and
                     will be removed after version 0.5.x.
                     """,
                     FutureWarning,
                 )
+        self.on_fail_descriptor: Union[str, OnFailAction] = "custom"
 
         if on_fail is None:
-            on_fail = "noop"
-        if isinstance(on_fail, str):
+            on_fail = OnFailAction.NOOP
+        if isinstance(on_fail, OnFailAction):
             self.on_fail_descriptor = on_fail
             self.on_fail_method = None
+        elif (
+            isinstance(on_fail, str)
+            and OnFailAction.__members__.get(on_fail.upper()) is not None
+        ):
+            self.on_fail_descriptor = (
+                OnFailAction.__members__.get(on_fail.upper())
+                or ""  # this default isn't needed, it's just for pyright
+            )
+            self.on_fail_method = None
         else:
-            self.on_fail_descriptor = "custom"
             self.on_fail_method = on_fail
 
         # Store the kwargs for the validator.
         self._kwargs = kwargs
 
         assert (
             self.rail_alias in validators_registry
```

### Comparing `guardrails_ai-0.4.2/guardrails/validator_service.py` & `guardrails_ai-0.4.3/guardrails/validator_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import asyncio
 import itertools
 import os
 from concurrent.futures import ProcessPoolExecutor
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from guardrails.classes.history import Iteration
 from guardrails.datatypes import FieldValidation
 from guardrails.errors import ValidationError
 from guardrails.logger import logger
 from guardrails.utils.hub_telemetry_utils import HubTelemetry
 from guardrails.utils.logs_utils import ValidatorLogs
 from guardrails.utils.reask_utils import FieldReAsk, ReAsk
 from guardrails.utils.safe_get import safe_get
 from guardrails.utils.telemetry_utils import trace_validator
 from guardrails.validator_base import (
     FailResult,
     Filter,
+    OnFailAction,
     PassResult,
     Refrain,
     ValidationResult,
     Validator,
 )
 
 
@@ -55,21 +56,21 @@
         return result
 
     def perform_correction(
         self,
         results: List[FailResult],
         value: Any,
         validator: Validator,
-        on_fail_descriptor: str,
+        on_fail_descriptor: Union[OnFailAction, str],
     ):
-        if on_fail_descriptor == "fix":
+        if on_fail_descriptor == OnFailAction.FIX:
             # FIXME: Should we still return fix_value if it is None?
             # I think we should warn and return the original value.
             return results[0].fix_value
-        elif on_fail_descriptor == "fix_reask":
+        elif on_fail_descriptor == OnFailAction.FIX_REASK:
             # FIXME: Same thing here
             fixed_value = results[0].fix_value
             result = self.execute_validator(
                 validator, fixed_value, results[0].metadata or {}
             )
 
             if isinstance(result, FailResult):
@@ -79,29 +80,29 @@
                 )
 
             return fixed_value
         if on_fail_descriptor == "custom":
             if validator.on_fail_method is None:
                 raise ValueError("on_fail is 'custom' but on_fail_method is None")
             return validator.on_fail_method(value, results)
-        if on_fail_descriptor == "reask":
+        if on_fail_descriptor == OnFailAction.REASK:
             return FieldReAsk(
                 incorrect_value=value,
                 fail_results=results,
             )
-        if on_fail_descriptor == "exception":
+        if on_fail_descriptor == OnFailAction.EXCEPTION:
             raise ValidationError(
                 "Validation failed for field with errors: "
                 + ", ".join([result.error_message for result in results])
             )
-        if on_fail_descriptor == "filter":
+        if on_fail_descriptor == OnFailAction.FILTER:
             return Filter()
-        if on_fail_descriptor == "refrain":
+        if on_fail_descriptor == OnFailAction.REFRAIN:
             return Refrain()
-        if on_fail_descriptor == "noop":
+        if on_fail_descriptor == OnFailAction.NOOP:
             return value
         else:
             raise ValueError(
                 f"Invalid on_fail_descriptor {on_fail_descriptor}, "
                 f"expected 'fix' or 'exception'."
             )
 
@@ -247,15 +248,19 @@
 
 class AsyncValidatorService(ValidatorServiceBase, MultiprocMixin):
     def group_validators(self, validators):
         groups = itertools.groupby(
             validators, key=lambda v: (v.on_fail_descriptor, v.override_value_on_pass)
         )
         for (on_fail_descriptor, override_on_pass), group in groups:
-            if override_on_pass or on_fail_descriptor in ["fix", "fix_reask", "custom"]:
+            if override_on_pass or on_fail_descriptor in [
+                OnFailAction.FIX,
+                OnFailAction.FIX_REASK,
+                "custom",
+            ]:
                 for validator in group:
                     yield on_fail_descriptor, [validator]
             else:
                 yield on_fail_descriptor, list(group)
 
     async def run_validators(
         self,
```

### Comparing `guardrails_ai-0.4.2/guardrails/validators/__init__.py` & `guardrails_ai-0.4.3/guardrails/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/bug_free_python.py` & `guardrails_ai-0.4.3/guardrails/validators/bug_free_python.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/bug_free_sql.py` & `guardrails_ai-0.4.3/guardrails/validators/bug_free_sql.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/competitor_check.py` & `guardrails_ai-0.4.3/guardrails/validators/competitor_check.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/detect_secrets.py` & `guardrails_ai-0.4.3/guardrails/validators/detect_secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         - Multi-line secrets may not be caught. e.g.
             - RSA/SSH keys
 
     Example:
         ```py
 
         guard = Guard.from_string(validators=[
-            DetectSecrets(on_fail="fix")
+            DetectSecrets(on_fail=OnFailAction.FIX)
         ])
         guard.parse(
             llm_output=code_snippet,
         )
         ```
     """
```

### Comparing `guardrails_ai-0.4.2/guardrails/validators/endpoint_is_reachable.py` & `guardrails_ai-0.4.3/guardrails/validators/endpoint_is_reachable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from http import HTTPStatus
 from typing import Any, Dict
 
 from guardrails.logger import logger
 from guardrails.validator_base import (
     FailResult,
     PassResult,
     ValidationResult,
@@ -27,15 +28,15 @@
         logger.debug(f"Validating {value} is a valid URL...")
 
         import requests
 
         # Check that the URL exists and can be reached
         try:
             response = requests.get(value)
-            if response.status_code != 200:
+            if response.status_code != HTTPStatus.OK:
                 return FailResult(
                     error_message=f"URL {value} returned "
                     f"status code {response.status_code}",
                 )
         except requests.exceptions.ConnectionError:
             return FailResult(
                 error_message=f"URL {value} could not be reached",
```

### Comparing `guardrails_ai-0.4.2/guardrails/validators/ends_with.py` & `guardrails_ai-0.4.3/guardrails/validators/ends_with.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict
 
 from guardrails.logger import logger
 from guardrails.validator_base import (
     FailResult,
+    OnFailAction,
     PassResult,
     ValidationResult,
     Validator,
     register_validator,
 )
 
 
@@ -22,15 +23,15 @@
     | Supported data types          | `list`                            |
     | Programmatic fix              | Append the given value to the list. |
 
     Args:
         end: The required last element.
     """
 
-    def __init__(self, end: str, on_fail: str = "fix"):
+    def __init__(self, end: str, on_fail: OnFailAction = OnFailAction.FIX):
         super().__init__(
             on_fail=on_fail,
             end=end,
         )
         self._end = end
 
     def validate(self, value: Any, metadata: Dict) -> ValidationResult:
```

### Comparing `guardrails_ai-0.4.2/guardrails/validators/exclude_sql_predicates.py` & `guardrails_ai-0.4.3/guardrails/validators/exclude_sql_predicates.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/extracted_summary_sentences_match.py` & `guardrails_ai-0.4.3/guardrails/validators/extracted_summary_sentences_match.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/extractive_summary.py` & `guardrails_ai-0.4.3/guardrails/validators/extractive_summary.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/is_high_quality_translation.py` & `guardrails_ai-0.4.3/guardrails/validators/is_high_quality_translation.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/is_profanity_free.py` & `guardrails_ai-0.4.3/guardrails/validators/is_profanity_free.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/lower_case.py` & `guardrails_ai-0.4.3/guardrails/validators/lower_case.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/on_topic.py` & `guardrails_ai-0.4.3/guardrails/validators/on_topic.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/one_line.py` & `guardrails_ai-0.4.3/guardrails/validators/one_line.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/pii_filter.py` & `guardrails_ai-0.4.3/guardrails/validators/pii_filter.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/provenance.py` & `guardrails_ai-0.4.3/guardrails/validators/provenance.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/pydantic_field_validator.py` & `guardrails_ai-0.4.3/guardrails/validators/pydantic_field_validator.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/qa_relevance_llm_eval.py` & `guardrails_ai-0.4.3/guardrails/validators/qa_relevance_llm_eval.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/reading_time.py` & `guardrails_ai-0.4.3/guardrails/validators/reading_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional
+from typing import Any, Callable, Dict, Optional
 
 from guardrails.logger import logger
 from guardrails.validator_base import (
     FailResult,
     PassResult,
     ValidationResult,
     Validator,
@@ -24,15 +24,15 @@
     | Programmatic fix              | None                                |
 
     Args:
 
         reading_time: The maximum reading time in minutes.
     """
 
-    def __init__(self, reading_time: int, on_fail: Optional[str] = None):
+    def __init__(self, reading_time: int, on_fail: Optional[Callable] = None):
         super().__init__(
             on_fail=on_fail,
             reading_time=reading_time,
         )
         self._max_time = reading_time
 
     def validate(self, value: Any, metadata: Dict) -> ValidationResult:
```

### Comparing `guardrails_ai-0.4.2/guardrails/validators/regex_match.py` & `guardrails_ai-0.4.3/guardrails/validators/regex_match.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/remove_redundant_sentences.py` & `guardrails_ai-0.4.3/guardrails/validators/remove_redundant_sentences.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/saliency_check.py` & `guardrails_ai-0.4.3/guardrails/validators/saliency_check.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/similar_to_document.py` & `guardrails_ai-0.4.3/guardrails/validators/similar_to_document.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/similar_to_list.py` & `guardrails_ai-0.4.3/guardrails/validators/similar_to_list.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/sql_column_presence.py` & `guardrails_ai-0.4.3/guardrails/validators/sql_column_presence.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/toxic_language.py` & `guardrails_ai-0.4.3/guardrails/validators/toxic_language.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/two_words.py` & `guardrails_ai-0.4.3/guardrails/validators/two_words.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/upper_case.py` & `guardrails_ai-0.4.3/guardrails/validators/upper_case.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/valid_choices.py` & `guardrails_ai-0.4.3/guardrails/validators/valid_choices.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/valid_length.py` & `guardrails_ai-0.4.3/guardrails/validators/valid_length.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/valid_range.py` & `guardrails_ai-0.4.3/guardrails/validators/valid_range.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/valid_url.py` & `guardrails_ai-0.4.3/guardrails/validators/valid_url.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validators/validators.py` & `guardrails_ai-0.4.3/guardrails/validators/validators.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/validatorsattr.py` & `guardrails_ai-0.4.3/guardrails/validatorsattr.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import lxml.etree as ET
 import pydantic
 
 from guardrails.constants import hub
 from guardrails.utils.xml_utils import cast_xml_to_string
-from guardrails.validator_base import Validator, ValidatorSpec
+from guardrails.validator_base import OnFailAction, Validator, ValidatorSpec
 
 
 class ValidatorsAttr(pydantic.BaseModel):
     """Class for parsing and manipulating the `format` attribute of an element.
 
     The format attribute is a string that contains semi-colon separated
     validators e.g. "valid-url; is-reachable". Each validator is itself either:
@@ -172,15 +172,15 @@
         validator_args = cls.parse(validators_str)
 
         on_fail_handlers = {}
         for key, value in element.attrib.items():
             key = cast_xml_to_string(key)
             if key.startswith("on-fail-"):
                 on_fail_handler_name = key[len("on-fail-") :]
-                on_fail_handler = value
+                on_fail_handler = OnFailAction(value)
                 on_fail_handlers[on_fail_handler_name] = on_fail_handler
 
         validators, unregistered_validators = cls.get_validators(
             validator_args=validator_args,
             tag=tag,
             on_fail_handlers=on_fail_handlers,
             strict=strict,
```

### Comparing `guardrails_ai-0.4.2/guardrails/vectordb/base.py` & `guardrails_ai-0.4.3/guardrails/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/guardrails/vectordb/faiss.py` & `guardrails_ai-0.4.3/guardrails/vectordb/faiss.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.2/pyproject.toml` & `guardrails_ai-0.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guardrails-ai"
-version = "0.4.2"
+version = "0.4.3"
 description = "Adding guardrails to large language models."
 authors = ["Guardrails AI <contact@guardrailsai.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "guardrails", from = "." }
 ]
@@ -32,14 +32,15 @@
 sqlglot = {version = "^19.0.3", optional = true}
 thefuzz = {version = "^0.20.0", optional = true}
 nltk = {version = "^3.8.1", optional = true}
 faiss-cpu = {version = "^1.7.4", optional = true}
 numpy = {version = ">=1.24", optional = true}
 alt-profanity-check = {version = "^1.3.1", optional = true}
 detect-secrets = {version = "^1.4.0", optional = true}
+litellm = {version = "^1.34.38", optional = true}
 manifest-ml = {version = "^0.1.8", optional = true}
 transformers = {version = "^4.36.0", optional = true}
 presidio_analyzer = {version = "^2.2.33", optional = true}
 presidio_anonymizer = {version = "^2.2.33", optional = true}
 spacy-transformers = {version = "^1.3.4", optional = true}
 anthropic = {version = "^0.7.2", optional = true}
 torch = {version = "^2.1.1", optional = true}
@@ -51,26 +52,27 @@
 pydoc-markdown = "4.8.2"
 opentelemetry-sdk = "1.20.0"
 opentelemetry-exporter-otlp-proto-grpc = "1.20.0"
 opentelemetry-exporter-otlp-proto-http = "1.20.0"
 langchain-core = "^0.1.18"
 coloredlogs = "^15.0.1"
 requests = "^2.31.0"
-guardrails-api-client = "^0.1.0"
+guardrails-api-client = "^0.1.1"
 jwt = "^1.3.1"
 
 
 
 [tool.poetry.extras]
 sql = ["sqlvalidator", "sqlalchemy", "sqlglot"]
 summary = ["thefuzz", "nltk"]
 vectordb = ["faiss-cpu", "numpy"]
 profanity = ["alt-profanity-check"]
 detect-secrets = ["detect-secrets"]
 manifest = ["manifest-ml"]
+litellm = ["litellm"]
 high_quality_translation = ["unbabel-comet", "huggingface_hub"]
 toxic_language = ["transformers", "torch"]
 pii = ["presidio_analyzer", "presidio_anonymizer"]
 competitor-check = ["spacy-transformers"]
 anthropic = ["anthropic"]
 docs-build = ["nbdoc", "docspec_python", "pydoc-markdown"]
 
@@ -101,26 +103,20 @@
 mknotebooks = "^0.8.0"
 griffe = "^0.36.9"
 pillow = "^10.1.0"
 cairosvg = "^2.7.1"
 mkdocs-glightbox = "^0.3.4"
 
 [[tool.poetry.source]]
-name = "torch"
-url = "https://download.pytorch.org/whl/cpu"
-priority = "explicit"
-
-[[tool.poetry.source]]
 name = "PyPI"
-priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
-line_length = 88
+line_length = 88
```

### Comparing `guardrails_ai-0.4.2/PKG-INFO` & `guardrails_ai-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardrails-ai
-Version: 0.4.2
+Version: 0.4.3
 Summary: Adding guardrails to large language models.
 License: Apache-2.0
 Author: Guardrails AI
 Author-email: contact@guardrailsai.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -13,32 +13,34 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic
 Provides-Extra: competitor-check
 Provides-Extra: detect-secrets
 Provides-Extra: docs-build
 Provides-Extra: high-quality-translation
+Provides-Extra: litellm
 Provides-Extra: manifest
 Provides-Extra: pii
 Provides-Extra: profanity
 Provides-Extra: sql
 Provides-Extra: summary
 Provides-Extra: toxic-language
 Provides-Extra: vectordb
 Requires-Dist: alt-profanity-check (>=1.3.1,<2.0.0) ; extra == "profanity"
 Requires-Dist: anthropic (>=0.7.2,<0.8.0) ; extra == "anthropic"
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: detect-secrets (>=1.4.0,<2.0.0) ; extra == "detect-secrets"
 Requires-Dist: docspec_python (==2.2.1) ; extra == "docs-build"
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0) ; extra == "vectordb"
 Requires-Dist: griffe (>=0.36.9,<0.37.0)
-Requires-Dist: guardrails-api-client (>=0.1.0,<0.2.0)
+Requires-Dist: guardrails-api-client (>=0.1.1,<0.2.0)
 Requires-Dist: huggingface_hub (>=0.19.3,<0.20.0) ; extra == "high-quality-translation"
 Requires-Dist: jwt (>=1.3.1,<2.0.0)
 Requires-Dist: langchain-core (>=0.1.18,<0.2.0)
+Requires-Dist: litellm (>=1.34.38,<2.0.0) ; extra == "litellm"
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: manifest-ml (>=0.1.8,<0.2.0) ; extra == "manifest"
 Requires-Dist: nbdoc (>=0.0.82,<0.0.83) ; extra == "docs-build"
 Requires-Dist: nltk (>=3.8.1,<4.0.0) ; extra == "summary"
 Requires-Dist: numpy (>=1.24) ; extra == "vectordb"
 Requires-Dist: openai (<2)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.20.0)
@@ -130,49 +132,69 @@
 
     ```bash
     guardrails hub install hub://guardrails/regex_match
     ```
 3. Create a Guard from the installed guardrail.
 
     ```python
-    # Import Guard and Validator
+    from guardrails import Guard, OnFailAction
     from guardrails.hub import RegexMatch
-    from guardrails import Guard
 
-    # Initialize the Guard with 
-    val = Guard().use(
-        RegexMatch(regex="^[A-Z][a-z]*$")
+    guard = Guard().use(
+        RegexMatch, regex="\(?\d{3}\)?-? *\d{3}-? *-?\d{4}", on_fail=OnFailAction.EXCEPTION
     )
 
-    guard.parse("Caesar")  # Guardrail Passes
-    guard.parse("Caesar is a great leader")  # Guardrail Fails
+    guard.validate("123-456-7890")  # Guardrail passes
+
+    try:
+        guard.validate("1234-789-0000")  # Guardrail fails
+    except Exception as e:
+        print(e)
+    ```
+    Output:
+    ```console
+    Validation failed for field with errors: Result must match \(?\d{3}\)?-? *\d{3}-? *-?\d{4}
     ```
 4. Run multiple guardrails within a Guard.
     First, install the necessary guardrails from Guardrails Hub.
 
     ```bash
     guardrails hub install hub://guardrails/competitor_check
     guardrails hub install hub://guardrails/toxic_language
     ```
 
     Then, create a Guard from the installed guardrails.
     
     ```python
-    from guardrails.hub import RegexMatch, ValidLength
-    from guardrails import Guard
+    from guardrails import Guard, OnFailAction
+    from guardrails.hub import CompetitorCheck, ToxicLanguage
 
-    guard = Guard().use(
-        RegexMatch(regex="^[A-Z][a-z]*$"),
-        ValidLength(min=1, max=32)
+    guard = Guard().use_many(
+        CompetitorCheck(["Apple", "Microsoft", "Google"], on_fail=OnFailAction.EXCEPTION),
+        ToxicLanguage(threshold=0.5, validation_method="sentence", on_fail=OnFailAction.EXCEPTION),),
     )
 
-    guard.parse("Caesar")  # Guardrail Passes
-    guard.parse("Caesar is a great leader")  # Guardrail Fails
+    guard.validate(
+        """An apple a day keeps a doctor away.
+        This is good advice for keeping your health."""
+    )  # Both the guardrails pass
+
+    try:
+        guard.validate(
+            """Shut the hell up! Apple just released a new iPhone."""
+        )  # Both the guardrails fail
+    except Exception as e:
+        print(e)
     ```
+    Output:
+    ```console
+    Validation failed for field with errors: Found the following competitors: [['Apple']]. Please avoid naming those competitors next time, The following sentences in your response were found to be toxic:
 
+    - Shut the hell up!
+    ```
 
 ### Use Guardrails to generate structured data from LLMs
 
 
 Let's go through an example where we ask an LLM to generate fake pet names. To do this, we'll create a Pydantic [BaseModel](https://docs.pydantic.dev/latest/api/base_model/) that represents the structure of the output we want.
 
 ```py
@@ -199,15 +221,15 @@
 guard = Guard.from_pydantic(output_class=Pet, prompt=prompt)
 
 validated_output, *rest = guard(
     llm_api=openai.completions.create,
     engine="gpt-3.5-turbo-instruct"
 )
 
-print(f"{validated_output}")
+print(validated_output)
 ```
 
 This prints: 
 ```
 {
     "pet_type": "dog",
     "name": "Buddy
```

