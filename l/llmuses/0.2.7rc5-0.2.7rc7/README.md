# Comparing `tmp/llmuses-0.2.7rc5.tar.gz` & `tmp/llmuses-0.2.7rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmuses-0.2.7rc5.tar", last modified: Fri Mar 29 11:11:13 2024, max compression
+gzip compressed data, was "llmuses-0.2.7rc7.tar", last modified: Tue Apr  9 14:35:54 2024, max compression
```

## Comparing `llmuses-0.2.7rc5.tar` & `llmuses-0.2.7rc7.tar`

### file list

```diff
@@ -1,166 +1,167 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.631012 llmuses-0.2.7rc5/
--rw-r--r--   0 jason      (501) staff       (20)    11944 2024-03-29 11:11:13.630472 llmuses-0.2.7rc5/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)    11285 2024-03-29 11:11:12.000000 llmuses-0.2.7rc5/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.408922 llmuses-0.2.7rc5/llmuses/
--rw-r--r--   0 jason      (501) staff       (20)      106 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.415386 llmuses-0.2.7rc5/llmuses/benchmarks/
--rw-r--r--   0 jason      (501) staff       (20)      158 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.418783 llmuses-0.2.7rc5/llmuses/benchmarks/arc/
--rw-r--r--   0 jason      (501) staff       (20)      308 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/arc/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     5608 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/arc/ai2_arc.py
--rw-r--r--   0 jason      (501) staff       (20)     8983 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/arc/arc_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.420791 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/
--rw-r--r--   0 jason      (501) staff       (20)      300 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    10792 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/bbh_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.460873 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/
--rwxr-xr-x   0 jason      (501) staff       (20)     1780 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3652 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     1166 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3567 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2404 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     4476 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     4830 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2120 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2146 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/navigate.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     1417 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2294 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3480 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     6140 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/snarks.txt
--rwxr-xr-x   0 jason      (501) staff       (20)      820 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3022 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2944 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2163 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt
--rw-r--r--   0 jason      (501) staff       (20)     2155 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/benchmarks/benchmark.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.466459 llmuses-0.2.7rc5/llmuses/benchmarks/ceval/
--rw-r--r--   0 jason      (501) staff       (20)      337 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/ceval/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    15540 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/ceval/ceval_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     5063 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/ceval/ceval_exam.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.469565 llmuses-0.2.7rc5/llmuses/benchmarks/competition_math/
--rw-r--r--   0 jason      (501) staff       (20)      387 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/competition_math/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     2678 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/competition_math/competition_math.py
--rw-r--r--   0 jason      (501) staff       (20)    19079 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/competition_math/competition_math_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)    10047 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/data_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.471894 llmuses-0.2.7rc5/llmuses/benchmarks/general_qa/
--rw-r--r--   0 jason      (501) staff       (20)      340 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/benchmarks/general_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     5584 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/general_qa/general_qa_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.475208 llmuses-0.2.7rc5/llmuses/benchmarks/gsm8k/
--rw-r--r--   0 jason      (501) staff       (20)      309 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/gsm8k/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4282 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/gsm8k/gsm8k.py
--rw-r--r--   0 jason      (501) staff       (20)    13761 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/gsm8k/gsm8k_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.477688 llmuses-0.2.7rc5/llmuses/benchmarks/hellaswag/
--rw-r--r--   0 jason      (501) staff       (20)      351 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/hellaswag/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4690 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/hellaswag/hellaswag.py
--rw-r--r--   0 jason      (501) staff       (20)     8547 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/hellaswag/hellaswag_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.480026 llmuses-0.2.7rc5/llmuses/benchmarks/humaneval/
--rw-r--r--   0 jason      (501) staff       (20)      329 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/humaneval/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3482 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/humaneval/humaneval.py
--rw-r--r--   0 jason      (501) staff       (20)     1661 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/humaneval/humaneval_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.482817 llmuses-0.2.7rc5/llmuses/benchmarks/mmlu/
--rw-r--r--   0 jason      (501) staff       (20)      331 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/mmlu/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     5256 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/mmlu/mmlu.py
--rw-r--r--   0 jason      (501) staff       (20)    16340 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/mmlu/mmlu_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.485660 llmuses-0.2.7rc5/llmuses/benchmarks/race/
--rw-r--r--   0 jason      (501) staff       (20)      331 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/benchmarks/race/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3835 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/benchmarks/race/race.py
--rw-r--r--   0 jason      (501) staff       (20)     9892 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/race/race_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.492481 llmuses-0.2.7rc5/llmuses/benchmarks/trivia_qa/
--rw-r--r--   0 jason      (501) staff       (20)      345 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/benchmarks/trivia_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3296 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/benchmarks/trivia_qa/trivia_qa.py
--rw-r--r--   0 jason      (501) staff       (20)     7653 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.500109 llmuses-0.2.7rc5/llmuses/benchmarks/truthful_qa/
--rw-r--r--   0 jason      (501) staff       (20)      361 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/truthful_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7017 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/benchmarks/truthful_qa/truthful_qa.py
--rw-r--r--   0 jason      (501) staff       (20)    14944 2024-03-29 08:36:55.000000 llmuses-0.2.7rc5/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     3284 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/cache.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.558606 llmuses-0.2.7rc5/llmuses/cli/
--rw-r--r--   0 jason      (501) staff       (20)       50 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/cli/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)      404 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/cli/base.py
--rw-r--r--   0 jason      (501) staff       (20)      549 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/cli/cli.py
--rw-r--r--   0 jason      (501) staff       (20)     3865 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/cli/start_server.py
--rw-r--r--   0 jason      (501) staff       (20)     5919 2024-03-29 11:10:00.000000 llmuses-0.2.7rc5/llmuses/config.py
--rw-r--r--   0 jason      (501) staff       (20)     2632 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/constants.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.565631 llmuses-0.2.7rc5/llmuses/evaluator/
--rw-r--r--   0 jason      (501) staff       (20)      101 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/evaluator/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    28339 2024-03-29 08:44:25.000000 llmuses-0.2.7rc5/llmuses/evaluator/evaluator.py
--rw-r--r--   0 jason      (501) staff       (20)     5760 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/evaluator/rating_eval.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.567589 llmuses-0.2.7rc5/llmuses/evaluator/reviewer/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/evaluator/reviewer/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    17034 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/evaluator/reviewer/auto_reviewer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.573775 llmuses-0.2.7rc5/llmuses/metrics/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/metrics/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.575695 llmuses-0.2.7rc5/llmuses/metrics/bundled_rouge_score/
--rw-r--r--   0 jason      (501) staff       (20)      650 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/metrics/bundled_rouge_score/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    11450 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/metrics/bundled_rouge_score/rouge_scorer.py
--rw-r--r--   0 jason      (501) staff       (20)     3462 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/metrics/code_metric.py
--rw-r--r--   0 jason      (501) staff       (20)     1986 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/metrics/math_accuracy.py
--rw-r--r--   0 jason      (501) staff       (20)    12545 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/metrics/metrics.py
--rw-r--r--   0 jason      (501) staff       (20)     4516 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/metrics/rouge_metric.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.580147 llmuses-0.2.7rc5/llmuses/models/
--rw-r--r--   0 jason      (501) staff       (20)      141 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.581767 llmuses-0.2.7rc5/llmuses/models/custom/
--rw-r--r--   0 jason      (501) staff       (20)      101 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/models/custom/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     1380 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/models/custom/custom_model.py
--rw-r--r--   0 jason      (501) staff       (20)     1321 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/models/dummy_chat_model.py
--rw-r--r--   0 jason      (501) staff       (20)     3020 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/models/model.py
--rw-r--r--   0 jason      (501) staff       (20)    21702 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/models/model_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     3448 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/models/openai_model.py
--rw-r--r--   0 jason      (501) staff       (20)    25273 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/models/template.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.596717 llmuses-0.2.7rc5/llmuses/perf/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     1034 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/_logging.py
--rw-r--r--   0 jason      (501) staff       (20)     1080 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/dashscope_message.py
--rw-r--r--   0 jason      (501) staff       (20)     1057 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/generate_zhipu_token.py
--rw-r--r--   0 jason      (501) staff       (20)    29573 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/http_client.py
--rw-r--r--   0 jason      (501) staff       (20)     3685 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/monitor.py
--rw-r--r--   0 jason      (501) staff       (20)     1153 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/server_sent_event.py
--rw-r--r--   0 jason      (501) staff       (20)     1092 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/vllm_qwen_openai_completion.py
--rw-r--r--   0 jason      (501) staff       (20)     1043 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/perf/zhipu_message.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.598437 llmuses-0.2.7rc5/llmuses/preprocess/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/preprocess/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.600844 llmuses-0.2.7rc5/llmuses/preprocess/tokenizers/
--rw-r--r--   0 jason      (501) staff       (20)        0 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/preprocess/tokenizers/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7810 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/preprocess/tokenizers/gpt2_tokenizer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.602397 llmuses-0.2.7rc5/llmuses/registry/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/registry/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.620730 llmuses-0.2.7rc5/llmuses/registry/tasks/
--rw-r--r--   0 jason      (501) staff       (20)      701 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/arc.yaml
--rw-r--r--   0 jason      (501) staff       (20)      700 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/bbh.yaml
--rw-r--r--   0 jason      (501) staff       (20)      774 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/bbh_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)      702 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/ceval.yaml
--rw-r--r--   0 jason      (501) staff       (20)      768 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/ceval_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)      806 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml
--rw-r--r--   0 jason      (501) staff       (20)      703 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/gsm8k.yaml
--rw-r--r--   0 jason      (501) staff       (20)      701 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/mmlu.yaml
--rw-r--r--   0 jason      (501) staff       (20)      777 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/registry/tasks/mmlu_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)    14152 2024-03-29 07:45:31.000000 llmuses-0.2.7rc5/llmuses/run.py
--rw-r--r--   0 jason      (501) staff       (20)     8511 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/run_arena.py
--rw-r--r--   0 jason      (501) staff       (20)     5996 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/run_ms.py
--rw-r--r--   0 jason      (501) staff       (20)     3227 2024-03-29 09:07:23.000000 llmuses-0.2.7rc5/llmuses/summarizer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.623890 llmuses-0.2.7rc5/llmuses/tools/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/tools/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3233 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/tools/combine_reports.py
--rw-r--r--   0 jason      (501) staff       (20)     3277 2024-03-06 09:18:31.000000 llmuses-0.2.7rc5/llmuses/tools/gen_mmlu_subject_mapping.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.629485 llmuses-0.2.7rc5/llmuses/utils/
--rw-r--r--   0 jason      (501) staff       (20)       85 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/utils/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7668 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/utils/arena_utils.py
--rw-r--r--   0 jason      (501) staff       (20)     2993 2024-03-18 05:46:13.000000 llmuses-0.2.7rc5/llmuses/utils/completion_parsers.py
--rw-r--r--   0 jason      (501) staff       (20)     1855 2023-12-18 07:51:14.000000 llmuses-0.2.7rc5/llmuses/utils/logger.py
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-03-28 05:57:39.000000 llmuses-0.2.7rc5/llmuses/utils/task_cfg_parser.py
--rw-r--r--   0 jason      (501) staff       (20)    11952 2024-03-28 12:39:09.000000 llmuses-0.2.7rc5/llmuses/utils/utils.py
--rw-r--r--   0 jason      (501) staff       (20)      121 2024-03-29 11:11:08.000000 llmuses-0.2.7rc5/llmuses/version.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-03-29 11:11:13.412532 llmuses-0.2.7rc5/llmuses.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)    11944 2024-03-29 11:11:12.000000 llmuses-0.2.7rc5/llmuses.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     5276 2024-03-29 11:11:13.000000 llmuses-0.2.7rc5/llmuses.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-03-29 11:11:12.000000 llmuses-0.2.7rc5/llmuses.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)        8 2024-03-29 11:11:12.000000 llmuses-0.2.7rc5/llmuses.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-03-29 11:11:13.631130 llmuses-0.2.7rc5/setup.cfg
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.521258 llmuses-0.2.7rc7/
+-rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-09 14:35:54.520803 llmuses-0.2.7rc7/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)    11285 2024-04-09 14:35:53.000000 llmuses-0.2.7rc7/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.357623 llmuses-0.2.7rc7/llmuses/
+-rw-r--r--   0 jason      (501) staff       (20)      106 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.361796 llmuses-0.2.7rc7/llmuses/benchmarks/
+-rw-r--r--   0 jason      (501) staff       (20)      158 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.363385 llmuses-0.2.7rc7/llmuses/benchmarks/arc/
+-rw-r--r--   0 jason      (501) staff       (20)      308 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/arc/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     5608 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/arc/ai2_arc.py
+-rw-r--r--   0 jason      (501) staff       (20)     8983 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/arc/arc_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.364366 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/
+-rw-r--r--   0 jason      (501) staff       (20)      300 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    10792 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/bbh_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.379438 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/
+-rwxr-xr-x   0 jason      (501) staff       (20)     1780 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3652 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     1166 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3567 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     4476 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     4830 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2120 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2146 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/navigate.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     1417 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2294 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3480 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     6140 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/snarks.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)      820 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3022 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2944 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2163 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt
+-rw-r--r--   0 jason      (501) staff       (20)     2155 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/benchmark.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.381573 llmuses-0.2.7rc7/llmuses/benchmarks/ceval/
+-rw-r--r--   0 jason      (501) staff       (20)      337 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/ceval/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    15844 2024-04-09 10:23:04.000000 llmuses-0.2.7rc7/llmuses/benchmarks/ceval/ceval_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     5063 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/ceval/ceval_exam.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.383577 llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/
+-rw-r--r--   0 jason      (501) staff       (20)      387 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     2678 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/competition_math.py
+-rw-r--r--   0 jason      (501) staff       (20)    19079 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/competition_math_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)    10091 2024-04-09 13:29:59.000000 llmuses-0.2.7rc7/llmuses/benchmarks/data_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.385090 llmuses-0.2.7rc7/llmuses/benchmarks/general_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      340 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/general_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     5660 2024-04-09 13:33:11.000000 llmuses-0.2.7rc7/llmuses/benchmarks/general_qa/general_qa_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.386667 llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/
+-rw-r--r--   0 jason      (501) staff       (20)      309 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4282 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/gsm8k.py
+-rw-r--r--   0 jason      (501) staff       (20)    13761 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/gsm8k_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.388450 llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/
+-rw-r--r--   0 jason      (501) staff       (20)      351 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4690 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/hellaswag.py
+-rw-r--r--   0 jason      (501) staff       (20)     8547 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/hellaswag_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.390079 llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/
+-rw-r--r--   0 jason      (501) staff       (20)      329 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3482 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/humaneval.py
+-rw-r--r--   0 jason      (501) staff       (20)     1661 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/humaneval_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.391749 llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/
+-rw-r--r--   0 jason      (501) staff       (20)      331 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     5256 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/mmlu.py
+-rw-r--r--   0 jason      (501) staff       (20)    16393 2024-04-09 12:38:11.000000 llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/mmlu_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.394599 llmuses-0.2.7rc7/llmuses/benchmarks/race/
+-rw-r--r--   0 jason      (501) staff       (20)      331 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/race/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3835 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/race/race.py
+-rw-r--r--   0 jason      (501) staff       (20)     9892 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/race/race_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.397321 llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      345 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3296 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/trivia_qa.py
+-rw-r--r--   0 jason      (501) staff       (20)     7653 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.400086 llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      361 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7017 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/truthful_qa.py
+-rw-r--r--   0 jason      (501) staff       (20)    14944 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     3284 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cache.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.403710 llmuses-0.2.7rc7/llmuses/cli/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cli/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)      404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cli/base.py
+-rw-r--r--   0 jason      (501) staff       (20)      549 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cli/cli.py
+-rw-r--r--   0 jason      (501) staff       (20)     3865 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cli/start_server.py
+-rw-r--r--   0 jason      (501) staff       (20)     6552 2024-04-09 13:25:19.000000 llmuses-0.2.7rc7/llmuses/config.py
+-rw-r--r--   0 jason      (501) staff       (20)     2632 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/constants.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.406218 llmuses-0.2.7rc7/llmuses/evaluator/
+-rw-r--r--   0 jason      (501) staff       (20)      101 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/evaluator/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    28598 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/evaluator/evaluator.py
+-rw-r--r--   0 jason      (501) staff       (20)     5760 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/evaluator/rating_eval.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.407437 llmuses-0.2.7rc7/llmuses/evaluator/reviewer/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/evaluator/reviewer/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    17034 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/evaluator/reviewer/auto_reviewer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.410904 llmuses-0.2.7rc7/llmuses/metrics/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.411972 llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/
+-rw-r--r--   0 jason      (501) staff       (20)      650 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    11450 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/rouge_scorer.py
+-rw-r--r--   0 jason      (501) staff       (20)     3462 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/code_metric.py
+-rw-r--r--   0 jason      (501) staff       (20)     1986 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/math_accuracy.py
+-rw-r--r--   0 jason      (501) staff       (20)    12545 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/metrics/metrics.py
+-rw-r--r--   0 jason      (501) staff       (20)     4516 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/metrics/rouge_metric.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.499073 llmuses-0.2.7rc7/llmuses/models/
+-rw-r--r--   0 jason      (501) staff       (20)      141 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.501116 llmuses-0.2.7rc7/llmuses/models/custom/
+-rw-r--r--   0 jason      (501) staff       (20)      101 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/models/custom/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     1380 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/models/custom/custom_model.py
+-rw-r--r--   0 jason      (501) staff       (20)     1321 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/models/dummy_chat_model.py
+-rw-r--r--   0 jason      (501) staff       (20)     3020 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/models/model.py
+-rw-r--r--   0 jason      (501) staff       (20)    21702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/models/model_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     3448 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/models/openai_model.py
+-rw-r--r--   0 jason      (501) staff       (20)    25273 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/models/template.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.508537 llmuses-0.2.7rc7/llmuses/perf/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     1034 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/_logging.py
+-rw-r--r--   0 jason      (501) staff       (20)     1080 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/dashscope_message.py
+-rw-r--r--   0 jason      (501) staff       (20)     1057 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/generate_zhipu_token.py
+-rw-r--r--   0 jason      (501) staff       (20)    29573 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/http_client.py
+-rw-r--r--   0 jason      (501) staff       (20)     3685 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/monitor.py
+-rw-r--r--   0 jason      (501) staff       (20)     1153 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/server_sent_event.py
+-rw-r--r--   0 jason      (501) staff       (20)     1092 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/vllm_qwen_openai_completion.py
+-rw-r--r--   0 jason      (501) staff       (20)     1043 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/zhipu_message.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.509146 llmuses-0.2.7rc7/llmuses/preprocess/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/preprocess/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.510367 llmuses-0.2.7rc7/llmuses/preprocess/tokenizers/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/preprocess/tokenizers/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7810 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/preprocess/tokenizers/gpt2_tokenizer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.510954 llmuses-0.2.7rc7/llmuses/registry/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/registry/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.516050 llmuses-0.2.7rc7/llmuses/registry/tasks/
+-rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/arc.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      700 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/bbh.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      774 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/bbh_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/ceval.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      768 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/ceval_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      806 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 13:25:19.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/general_qa.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      703 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/gsm8k.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/mmlu.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      777 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/mmlu_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)    14577 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/run.py
+-rw-r--r--   0 jason      (501) staff       (20)     8511 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/run_arena.py
+-rw-r--r--   0 jason      (501) staff       (20)     5996 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/run_ms.py
+-rw-r--r--   0 jason      (501) staff       (20)     3227 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/summarizer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.517475 llmuses-0.2.7rc7/llmuses/tools/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/tools/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3233 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/tools/combine_reports.py
+-rw-r--r--   0 jason      (501) staff       (20)     3277 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/tools/gen_mmlu_subject_mapping.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.520291 llmuses-0.2.7rc7/llmuses/utils/
+-rw-r--r--   0 jason      (501) staff       (20)       85 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/utils/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7668 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/utils/arena_utils.py
+-rw-r--r--   0 jason      (501) staff       (20)     2993 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/utils/completion_parsers.py
+-rw-r--r--   0 jason      (501) staff       (20)     1855 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/utils/logger.py
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/utils/task_cfg_parser.py
+-rw-r--r--   0 jason      (501) staff       (20)    11952 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/utils/utils.py
+-rw-r--r--   0 jason      (501) staff       (20)      121 2024-04-09 14:35:35.000000 llmuses-0.2.7rc7/llmuses/version.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.360145 llmuses-0.2.7rc7/llmuses.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-09 14:35:53.000000 llmuses-0.2.7rc7/llmuses.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     5315 2024-04-09 14:35:54.000000 llmuses-0.2.7rc7/llmuses.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-04-09 14:35:53.000000 llmuses-0.2.7rc7/llmuses.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)        8 2024-04-09 14:35:53.000000 llmuses-0.2.7rc7/llmuses.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-04-09 14:35:54.521361 llmuses-0.2.7rc7/setup.cfg
```

### Comparing `llmuses-0.2.7rc5/PKG-INFO` & `llmuses-0.2.7rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmuses
-Version: 0.2.7rc5
+Version: 0.2.7rc7
 Summary: LLMs Evaluation Framework
 Home-page: 
 Author: ModelScope team
 Author-email: contact@modelscope.cn
 Keywords: python,llm,evaluation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmuses-0.2.7rc5/README.md` & `llmuses-0.2.7rc7/README.md`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/arc/ai2_arc.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/arc/ai2_arc.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/arc/arc_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/arc/arc_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/bbh_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/bbh_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/navigate.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/navigate.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/snarks.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/snarks.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt` & `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/benchmark.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/ceval/ceval_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/ceval/ceval_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,16 @@
             subset_list = SUBSET_LIST
 
         if metric_list is None:
             metric_list = [{'name': 'WeightedAverageAccuracy', 'object': weighted_mean}]
 
         if few_shot_num is None:
             # Use 5-shot by default
-            logger.info(f'Set 5-shot examples by default for C-Eval.')
-            few_shot_num = 5
+            logger.info(f'Set 0-shot examples by default for C-Eval.')
+            few_shot_num = 0
 
         if few_shot_num > 5:
             logger.warning(f'few_shot_num <= 5 for C-Eval, but got {few_shot_num}. Use 5-shot by default.')
             few_shot_num = 5
 
         super().__init__(subset_list=subset_list,
                          metric_list=metric_list,
@@ -206,14 +206,17 @@
         if len(few_shot_prompts) > 0:
             context: str = '\n'.join(few_shot_prompts) + '\n'
         else:
             context = ''
 
         full_prompt: str = context.strip() + self._format_example(input_d=input_d, include_answer=False)
 
+        subject_name: str = SUBJECT_MAPPING.get(subset_name)[1] if SUBJECT_MAPPING.get(subset_name) else subset_name
+        full_prompt = f"以下是中国关于{subject_name}考试的单项选择题，请选出其中的正确答案。\n" + full_prompt
+
         return {'data': [full_prompt], 'multi_choices': self.choices}
 
     def get_gold_answer(self, input_d: dict) -> str:
         # Get the gold choice
         return input_d.get('answer', '')
 
     def parse_pred_result(self, result: str, raw_input_d: dict = None, eval_type: str = 'checkpoint') -> str:
@@ -292,15 +295,15 @@
         total_num: int = sum([num for _, num in subset_score_map.values()])
         weighted_avg_acc: float = sum([score * num for score, num in subset_score_map.values()]) / total_num
         weighted_avg_acc = normalize_score(score=weighted_avg_acc)
 
         # Get domain-subject mapping
         subject_review_map = {}
         for subset_name, (subset_score, num) in subset_score_map.items():
-            domain_name: str = SUBJECT_MAPPING.get(subset_name)[2]
+            domain_name: str = SUBJECT_MAPPING.get(subset_name)[2] if SUBJECT_MAPPING.get(subset_name) else 'DEFAULT'
             if domain_name in subject_review_map:
                 subject_review_map[domain_name].append((subset_name, subset_score, num))
             else:
                 subject_review_map[domain_name] = [(subset_name, subset_score, num)]
 
         # Get domain score
         category_list = []
@@ -327,11 +330,11 @@
     @classmethod
     def _format_example(cls, input_d: dict, include_answer=True):
         example = '问题：' + input_d['question']
         for choice in cls.choices:
             example += f'\n{choice}. {input_d[f"{choice}"]}'
 
         if include_answer:
-            example += '\n答案：' + input_d['answer'] + '\n\n'
+            example += '\n答案: ' + input_d['answer'] + '\n\n'
         else:
-            example += '\n答案：'
+            example += '\n答案: '
         return example
```

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/ceval/ceval_exam.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/ceval/ceval_exam.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/competition_math/competition_math.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/competition_math.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/competition_math/competition_math_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/competition_math_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/data_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/data_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,25 +101,25 @@
             {'subset_name': [prompt_d_1, prompt_d_2, ...]}
             prompt_d_i (dict): refer to the output of gen_prompt method.
 
         e.g. train -- few-shot data, test -- target dataset to evaluate.
         """
         res_dict: dict = {}
 
-        if self.few_shot_num < 0:
+        if self.few_shot_num and self.few_shot_num < 0:
             raise ValueError(f'Invalid shot_num: {self.few_shot_num} for few-shot evaluation.')
 
         logger.info(f'\n** Use default settings: \n'
                     f'>few_shot_num: {self.few_shot_num}, '
                     f'>few_shot_split: {self.train_split}, '
                     f'>target_eval_split: {self.eval_split}')
 
         for sub_name, sub_data_dict in data_dict.items():
             few_shot_data = []
-            if self.few_shot_num > 0:
+            if self.few_shot_num and self.few_shot_num > 0:
                 few_shot_random: bool = self.config_kwargs.get('few_shot_random', True)
                 few_shot_data = self.get_fewshot_examples(
                     [item for item in sub_data_dict[self.train_split]],
                     self.few_shot_num,
                     few_shot_random=few_shot_random)
 
             res_dict[sub_name] = []
```

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/general_qa/general_qa_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/general_qa/general_qa_adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
+import glob
+import os.path
 
 from llmuses.benchmarks.data_adapter import DataAdapter
 from llmuses.metrics.metrics import bleu_ngram_one_sample, weighted_mean
 from llmuses.metrics.rouge_metric import compute_rouge_score_one_sample_zh
+from llmuses.utils import jsonl_to_list
 from llmuses.utils.logger import get_logger
 from typing import Any, Optional
 from collections import defaultdict
 import json
 
 logger = get_logger()
 
@@ -16,15 +19,15 @@
 
 class GeneralQAAdapter(DataAdapter):
     # TODO: set few_shot_num
 
     def __init__(self,
                  subset_list: list = None,
                  metric_list: list = None,
-                 train_split: str = 'train',
+                 train_split: str = None,
                  eval_split: str = 'test',
                  **kwargs):
         if subset_list is None:
             subset_list = SUBSET_LIST
 
         if metric_list is None:
             metric_list = [{'name': 'WeightedAverageBLEU', 'object': weighted_mean}]
@@ -35,55 +38,53 @@
                          eval_split=eval_split,
                          **kwargs)
     
     def load(self,
              dataset_name_or_path: str,
              subset_list: list = None,
              **kwargs) -> dict:
-        data_dict = {}
 
-        split_list = [split for split in [self.train_split, self.eval_split] if split is not None]
-        for sub_name in subset_list:
-            data_dict[sub_name] = {}
-
-            try:
-                with open(dataset_name_or_path, 'r') as f:
-                    data = json.load(f)
-            except Exception as e:
-                raise e
-            
-            for split in split_list:
-                dataset = data[split]
-                data_dict[sub_name].update({split: dataset})
+        file_list = glob.glob(os.path.join(dataset_name_or_path, '*.jsonl'))
+        data_list = []
+        try:
+            for file_path in file_list:
+                data_list.extend(jsonl_to_list(file_path))
+        except Exception as e:
+            raise ValueError(f"Failed to load data from {dataset_name_or_path}, got error: {e}")
+
+        data_dict = {'default': {'test': data_list}}
 
         return data_dict
     
     def gen_prompt(self, input_d: dict, subset_name: str, few_shot_list: list, **kwargs) -> dict:
         """
         Args:
-            input_d: {'history': [], 'input': '', 'output': ''}
+            input_d: {'history': [], 'question': '', 'answer': ''}
 
         Returns:
             {'data': [prompt]}
 
         """
         # prompt = f"'<|im_start|>user\n{input_d['input']}<|im_end|>\n<|im_start|>assistant\n'"
-        prompt = input_d['input']
+        history = input_d.get('history', [])
+        prompt = input_d['question']
+        if len(history) > 0:
+            prompt = '\n'.join(history) + '\n' + prompt
         return {'data': [prompt]}
     
     def get_gold_answer(self, input_d: dict) -> str:
         """
         Args:
-            input_d: {'history': [], 'input': '', 'output': ''}
+            input_d: {'history': [], 'question': '', 'answer': ''}
 
         Returns:
             gold_answer: str
 
         """
-        return input_d.get('output', '')
+        return input_d.get('answer', '')
     
     def parse_pred_result(self, result: str, raw_input_d: dict = None, eval_type: str = 'checkpoint') -> str:
         """
         Args:
             result: str
 
         Returns:
```

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/gsm8k/gsm8k.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/gsm8k.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/gsm8k/gsm8k_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/gsm8k_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/hellaswag/hellaswag.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/hellaswag.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/hellaswag/hellaswag_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/hellaswag_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/humaneval/humaneval.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/humaneval.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/humaneval/humaneval_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/humaneval_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/mmlu/mmlu.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/mmlu.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/mmlu/mmlu_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/mmlu_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         total_num: int = sum([num for _, num in subset_score_map.values()])
         weighted_avg_acc: float = sum([score * num for score, num in subset_score_map.values()]) / total_num
         weighted_avg_acc = normalize_score(score=weighted_avg_acc)
 
         # Get domain-subject mapping
         subject_review_map = {}
         for subset_name, (subset_score, num) in subset_score_map.items():
-            domain_name: str = SUBJECT_MAPPING.get(subset_name)[2]
+            domain_name: str = SUBJECT_MAPPING.get(subset_name)[2] if SUBJECT_MAPPING.get(subset_name) else subset_name
             if domain_name in subject_review_map:
                 subject_review_map[domain_name].append((subset_name, subset_score, num))
             else:
                 subject_review_map[domain_name] = [(subset_name, subset_score, num)]
 
         # Get domain score
         category_list = []
```

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/race/race.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/race/race.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/race/race_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/race/race_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/trivia_qa/trivia_qa.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/trivia_qa.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/truthful_qa/truthful_qa.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/truthful_qa.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py` & `llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/cache.py` & `llmuses-0.2.7rc7/llmuses/cache.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/cli/cli.py` & `llmuses-0.2.7rc7/llmuses/cli/cli.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/cli/start_server.py` & `llmuses-0.2.7rc7/llmuses/cli/start_server.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/config.py` & `llmuses-0.2.7rc7/llmuses/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 registry_tasks = {
     'arc': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/arc.yaml')),
     'gsm8k': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/gsm8k.yaml')),
     'mmlu': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/mmlu.yaml')),
     'ceval': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/ceval.yaml')),
     'bbh': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/bbh.yaml')),
+    'general_qa': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/general_qa.yaml')),
 
     # 'bbh_mini': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/bbh_mini.yaml')),
     # 'mmlu_mini': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/mmlu_mini.yaml')),
     # 'ceval_mini': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/ceval_mini.yaml')),
 
 }
 
@@ -57,39 +58,48 @@
     #         'bbh_mini': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/bbh_mini.yaml')),
     #         'mmlu_mini': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/mmlu_mini.yaml')),
     #         'ceval_mini': yaml_to_dict(os.path.join(cur_path, 'registry/tasks/ceval_mini.yaml')),
     #
     #     }
 
     @staticmethod
-    def registry(name: str, data_pattern: str, dataset_dir: str = None) -> None:
+    def registry(name: str, data_pattern: str, dataset_dir: str = None, subset_list: list = None) -> None:
         """
         Register a new task (dataset) for evaluation.
 
         Args:
             name: str, the dataset name.
             data_pattern: str, the data pattern for the task.
                     e.g. `mmlu`, `ceval`, `gsm8k`, ...
                     refer to task_config.list() for all available datasets.
             dataset_dir: str, the directory to store multiple datasets files. e.g. /path/to/data, 
                 then your specific custom dataset directory will be /path/to/data/{name}
+            subset_list: list, the subset list for the dataset.
+                e.g. ['middle_school_politics', 'operating_system']
+                refer to the mmlu for example.  https://github.com/hendrycks/test/blob/master/categories.py
         """
         available_datasets = list(registry_tasks.keys())
         if data_pattern not in available_datasets:
             logger.error(f'No dataset found in available datasets: {available_datasets}, got data_pattern: {data_pattern}')
             return
 
         # Reuse the existing task config and update the datasets
         pattern_config = registry_tasks.get(data_pattern)
 
         custom_config = copy.deepcopy(pattern_config)
         custom_config.update({'datasets': [data_pattern]})
         custom_config.update({'dataset_hub': 'Local'})     # TODO: to support `ModelScope`
+        custom_config.update({'dataset_args': {data_pattern: {}}})
+
         if dataset_dir is not None:
-            custom_config.update({'dataset_args': {data_pattern: {'local_path': os.path.join(dataset_dir, name)}}})
+            custom_config['dataset_args'][data_pattern].update({'local_path': dataset_dir})
+
+        if subset_list is not None:
+            # custom_config['dataset_args'].get(data_pattern, {}).update({'subset_list': subset_list})
+            custom_config['dataset_args'][data_pattern].update({'subset_list': subset_list})
 
         registry_tasks.update({name: custom_config})
         logger.info(f'** Registered task: {name} with data pattern: {data_pattern}')
 
     def to_dict(self):
         # Note: to avoid serialization error for some model instance
         _tmp_model = copy.copy(self.model)
```

### Comparing `llmuses-0.2.7rc5/llmuses/constants.py` & `llmuses-0.2.7rc7/llmuses/constants.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/evaluator/evaluator.py` & `llmuses-0.2.7rc7/llmuses/evaluator/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,14 +477,17 @@
                                                   'task_output_config.yaml')
         overall_task_cfg_file = os.path.abspath(overall_task_cfg_file)
 
         # TODO: check the robustness of dump yaml
         try:
             logger.info(f'** Dumping overall task config to {overall_task_cfg_file} ...')
             logger.info(f'** The overall task config:\n {self.overall_task_cfg}')
+            if 'model' in self.overall_task_cfg and not isinstance(self.overall_task_cfg['model'], str):
+                self.overall_task_cfg['model'] = None
+                logger.info(f'>> Overwrite overall_task_cfg for `model` due to it is not a string')
             dict_to_yaml(self.overall_task_cfg, overall_task_cfg_file)
         except Exception as e:
             logger.warning(f'Failed to dump overall task config: {e}')
 
         # Note: deprecated
         # self.save_cache()
         # self.clear_cache()
```

### Comparing `llmuses-0.2.7rc5/llmuses/evaluator/rating_eval.py` & `llmuses-0.2.7rc7/llmuses/evaluator/rating_eval.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/evaluator/reviewer/auto_reviewer.py` & `llmuses-0.2.7rc7/llmuses/evaluator/reviewer/auto_reviewer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/metrics/bundled_rouge_score/__init__.py` & `llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/__init__.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/metrics/bundled_rouge_score/rouge_scorer.py` & `llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/rouge_scorer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/metrics/code_metric.py` & `llmuses-0.2.7rc7/llmuses/metrics/code_metric.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/metrics/math_accuracy.py` & `llmuses-0.2.7rc7/llmuses/metrics/math_accuracy.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/metrics/metrics.py` & `llmuses-0.2.7rc7/llmuses/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/metrics/rouge_metric.py` & `llmuses-0.2.7rc7/llmuses/metrics/rouge_metric.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/models/custom/custom_model.py` & `llmuses-0.2.7rc7/llmuses/models/custom/custom_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/models/dummy_chat_model.py` & `llmuses-0.2.7rc7/llmuses/models/dummy_chat_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/models/model.py` & `llmuses-0.2.7rc7/llmuses/models/model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/models/model_adapter.py` & `llmuses-0.2.7rc7/llmuses/models/model_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/models/openai_model.py` & `llmuses-0.2.7rc7/llmuses/models/openai_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/models/template.py` & `llmuses-0.2.7rc7/llmuses/models/template.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/perf/_logging.py` & `llmuses-0.2.7rc7/llmuses/perf/_logging.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/perf/dashscope_message.py` & `llmuses-0.2.7rc7/llmuses/perf/dashscope_message.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/perf/generate_zhipu_token.py` & `llmuses-0.2.7rc7/llmuses/perf/generate_zhipu_token.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/perf/http_client.py` & `llmuses-0.2.7rc7/llmuses/perf/http_client.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/perf/monitor.py` & `llmuses-0.2.7rc7/llmuses/perf/monitor.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/perf/server_sent_event.py` & `llmuses-0.2.7rc7/llmuses/perf/server_sent_event.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/perf/vllm_qwen_openai_completion.py` & `llmuses-0.2.7rc7/llmuses/perf/vllm_qwen_openai_completion.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/perf/zhipu_message.py` & `llmuses-0.2.7rc7/llmuses/perf/zhipu_message.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/preprocess/tokenizers/gpt2_tokenizer.py` & `llmuses-0.2.7rc7/llmuses/preprocess/tokenizers/gpt2_tokenizer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/arc.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/arc.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/bbh.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/bbh.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/bbh_mini.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/bbh_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/ceval.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/ceval.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/ceval_mini.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/ceval_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/gsm8k.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/gsm8k.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/mmlu.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/mmlu.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/registry/tasks/mmlu_mini.yaml` & `llmuses-0.2.7rc7/llmuses/registry/tasks/mmlu_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/run.py` & `llmuses-0.2.7rc7/llmuses/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch        # noqa
 
 from llmuses.config import TaskConfig
 from llmuses.constants import DEFAULT_ROOT_CACHE_DIR
 from llmuses.evaluator import Evaluator
 from llmuses.evaluator.evaluator import HumanevalEvaluator
 from llmuses.models.custom import CustomModel
-from llmuses.utils import import_module_util
+from llmuses.utils import import_module_util, yaml_to_dict
 from llmuses.utils.logger import get_logger
 
 logger = get_logger()
 
 """
 Run evaluation for LLMs.
 """
@@ -97,19 +97,23 @@
                         help='Dry run in single processing mode.',
                         action='store_true',
                         default=False)
     parser.add_argument('--mem-cache',
                         help='To use memory cache or not.',
                         action='store_true',
                         default=False)
+    # parser.add_argument('--use-cache',
+    #                     help='To reuse the cache or not. Default to True.',
+    #                     action='store_true',
+    #                     default=True)
     parser.add_argument('--use-cache',
-                        help='To reuse the cache or not. Default to True.',
-                        action='store_true',
-                        default=True)
-    parser.add_argument('--stage',      # TODO
+                        help='To reuse the cache or not. Default to `true`.',
+                        type=str,
+                        default='true')
+    parser.add_argument('--stage',
                         help='The stage of evaluation pipeline, '
                              'can be `all`, `infer`, `review`. Default to `all`.',
                         type=str,
                         default='all')
 
     args = parser.parse_args()
 
@@ -142,18 +146,23 @@
         eval_results = []
         for one_task_cfg in task_cfg:
             eval_results.append(run_task(one_task_cfg))
         return eval_results
 
     if isinstance(task_cfg, TaskConfig):
         task_cfg = task_cfg.to_dict()
+    elif isinstance(task_cfg, str):
+        task_cfg = yaml_to_dict(task_cfg)
+    elif isinstance(task_cfg, dict):
+        logger.info('** Args: Task config is provided with dictionary type. **')
+    else:
+        raise ValueError('** Args: Please provide a valid task config. **')
 
     # Get the output task config
     output_task_cfg = copy.copy(task_cfg)
-    output_task_cfg.update({'model': task_cfg['model'].__class__.__name__})
     logger.info(output_task_cfg)
 
     model_args: dict = task_cfg.get('model_args',
                                     {'revision': 'default', 'precision': torch.float16, 'device_map': 'auto'})
     # Get the GLOBAL default config (infer_cfg) for prediction
     generation_config: dict = task_cfg.get('generation_config',
                                            {'do_sample': False,
@@ -185,15 +194,15 @@
     model_precision = model_args.get('precision', torch.float16)
     if isinstance(model_precision, str):
         model_precision = eval(model_precision)
 
     if mem_cache:
         logger.warning('** DeprecatedWarning: `--mem-cache` is deprecated, please use `--use-cache` instead.')
 
-    logger.info(f'Set use_cache to {use_cache}.')
+    logger.info(f'** Set use_cache to {use_cache}.')
 
     # Get model args
     if dry_run:
         from llmuses.models.dummy_chat_model import DummyChatModel
         model_id: str = 'dummy'
         model_revision: str = 'v1.0.0'
     elif eval_type == 'custom':
@@ -217,16 +226,15 @@
                              'Note that you need to enable the execution code in the human_eval/execution.py first.')
 
         if dry_run:
             from llmuses.models.dummy_chat_model import DummyChatModel
             model_adapter = DummyChatModel(model_cfg=dict())
         elif eval_type == 'custom':
             if not isinstance(model, CustomModel):
-                raise ValueError('Please provide a custom model instance '
-                                 'in format of llmuses.models.custom.CustomModel.')
+                raise ValueError(f'Expected llmuses.models.custom.CustomModel, but got {type(model)}.')
             from llmuses.models.model_adapter import CustomModelAdapter
             model_adapter = CustomModelAdapter(custom_model=model)
         else:
             # Init model adapter
             device_map = model_args.get('device_map', 'auto') if torch.cuda.is_available() else None
             model_adapter = imported_modules['ModelAdapterClass'](model_id=model_id,
                                                                   model_revision=model_revision,
@@ -283,26 +291,27 @@
     return eval_results
 
 
 def main():
     args = parse_args()
 
     # Get task_cfg
+    use_cache: bool = False if args.use_cache.lower() == 'false' else True
     task_cfg = {
         'model_args': parse_str_args(args.model_args),
         'generation_config': parse_str_args(args.generation_config),
         'dataset_args': args.dataset_args,
         'dry_run': args.dry_run,
         'model': args.model,
         'eval_type': args.eval_type,
         'datasets': args.datasets,
         'work_dir': args.work_dir,
         'outputs': args.outputs,
         'mem_cache': args.mem_cache,
-        'use_cache': args.use_cache,
+        'use_cache': use_cache,
         'dataset_hub': args.dataset_hub,
         'dataset_dir': args.dataset_dir,
         'stage': args.stage,
         'limit': args.limit,
         'debug': args.debug
     }
```

### Comparing `llmuses-0.2.7rc5/llmuses/run_arena.py` & `llmuses-0.2.7rc7/llmuses/run_arena.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/run_ms.py` & `llmuses-0.2.7rc7/llmuses/run_ms.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/summarizer.py` & `llmuses-0.2.7rc7/llmuses/summarizer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/tools/combine_reports.py` & `llmuses-0.2.7rc7/llmuses/tools/combine_reports.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/tools/gen_mmlu_subject_mapping.py` & `llmuses-0.2.7rc7/llmuses/tools/gen_mmlu_subject_mapping.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/utils/arena_utils.py` & `llmuses-0.2.7rc7/llmuses/utils/arena_utils.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/utils/completion_parsers.py` & `llmuses-0.2.7rc7/llmuses/utils/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/utils/logger.py` & `llmuses-0.2.7rc7/llmuses/utils/logger.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses/utils/utils.py` & `llmuses-0.2.7rc7/llmuses/utils/utils.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc5/llmuses.egg-info/PKG-INFO` & `llmuses-0.2.7rc7/llmuses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmuses
-Version: 0.2.7rc5
+Version: 0.2.7rc7
 Summary: LLMs Evaluation Framework
 Home-page: 
 Author: ModelScope team
 Author-email: contact@modelscope.cn
 Keywords: python,llm,evaluation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmuses-0.2.7rc5/llmuses.egg-info/SOURCES.txt` & `llmuses-0.2.7rc7/llmuses.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 llmuses/registry/__init__.py
 llmuses/registry/tasks/arc.yaml
 llmuses/registry/tasks/bbh.yaml
 llmuses/registry/tasks/bbh_mini.yaml
 llmuses/registry/tasks/ceval.yaml
 llmuses/registry/tasks/ceval_mini.yaml
 llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml
+llmuses/registry/tasks/general_qa.yaml
 llmuses/registry/tasks/gsm8k.yaml
 llmuses/registry/tasks/mmlu.yaml
 llmuses/registry/tasks/mmlu_mini.yaml
 llmuses/tools/__init__.py
 llmuses/tools/combine_reports.py
 llmuses/tools/gen_mmlu_subject_mapping.py
 llmuses/utils/__init__.py
```

