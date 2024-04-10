# Comparing `tmp/llmuses-0.2.7rc7.tar.gz` & `tmp/llmuses-0.2.7rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmuses-0.2.7rc7.tar", last modified: Tue Apr  9 14:35:54 2024, max compression
+gzip compressed data, was "llmuses-0.2.7rc8.tar", last modified: Wed Apr 10 07:35:06 2024, max compression
```

## Comparing `llmuses-0.2.7rc7.tar` & `llmuses-0.2.7rc8.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.521258 llmuses-0.2.7rc7/
--rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-09 14:35:54.520803 llmuses-0.2.7rc7/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)    11285 2024-04-09 14:35:53.000000 llmuses-0.2.7rc7/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.357623 llmuses-0.2.7rc7/llmuses/
--rw-r--r--   0 jason      (501) staff       (20)      106 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.361796 llmuses-0.2.7rc7/llmuses/benchmarks/
--rw-r--r--   0 jason      (501) staff       (20)      158 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.363385 llmuses-0.2.7rc7/llmuses/benchmarks/arc/
--rw-r--r--   0 jason      (501) staff       (20)      308 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/arc/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     5608 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/arc/ai2_arc.py
--rw-r--r--   0 jason      (501) staff       (20)     8983 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/arc/arc_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.364366 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/
--rw-r--r--   0 jason      (501) staff       (20)      300 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    10792 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/bbh_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.379438 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/
--rwxr-xr-x   0 jason      (501) staff       (20)     1780 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3652 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     1166 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3567 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     4476 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     4830 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2120 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2146 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/navigate.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     1417 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2294 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3480 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     6140 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/snarks.txt
--rwxr-xr-x   0 jason      (501) staff       (20)      820 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3022 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2944 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2163 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt
--rw-r--r--   0 jason      (501) staff       (20)     2155 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/benchmark.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.381573 llmuses-0.2.7rc7/llmuses/benchmarks/ceval/
--rw-r--r--   0 jason      (501) staff       (20)      337 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/ceval/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    15844 2024-04-09 10:23:04.000000 llmuses-0.2.7rc7/llmuses/benchmarks/ceval/ceval_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     5063 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/ceval/ceval_exam.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.383577 llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/
--rw-r--r--   0 jason      (501) staff       (20)      387 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     2678 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/competition_math.py
--rw-r--r--   0 jason      (501) staff       (20)    19079 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/competition_math_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)    10091 2024-04-09 13:29:59.000000 llmuses-0.2.7rc7/llmuses/benchmarks/data_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.385090 llmuses-0.2.7rc7/llmuses/benchmarks/general_qa/
--rw-r--r--   0 jason      (501) staff       (20)      340 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/general_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     5660 2024-04-09 13:33:11.000000 llmuses-0.2.7rc7/llmuses/benchmarks/general_qa/general_qa_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.386667 llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/
--rw-r--r--   0 jason      (501) staff       (20)      309 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4282 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/gsm8k.py
--rw-r--r--   0 jason      (501) staff       (20)    13761 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/gsm8k_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.388450 llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/
--rw-r--r--   0 jason      (501) staff       (20)      351 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4690 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/hellaswag.py
--rw-r--r--   0 jason      (501) staff       (20)     8547 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/hellaswag_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.390079 llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/
--rw-r--r--   0 jason      (501) staff       (20)      329 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3482 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/humaneval.py
--rw-r--r--   0 jason      (501) staff       (20)     1661 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/humaneval_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.391749 llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/
--rw-r--r--   0 jason      (501) staff       (20)      331 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     5256 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/mmlu.py
--rw-r--r--   0 jason      (501) staff       (20)    16393 2024-04-09 12:38:11.000000 llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/mmlu_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.394599 llmuses-0.2.7rc7/llmuses/benchmarks/race/
--rw-r--r--   0 jason      (501) staff       (20)      331 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/race/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3835 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/race/race.py
--rw-r--r--   0 jason      (501) staff       (20)     9892 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/race/race_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.397321 llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/
--rw-r--r--   0 jason      (501) staff       (20)      345 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3296 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/trivia_qa.py
--rw-r--r--   0 jason      (501) staff       (20)     7653 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.400086 llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/
--rw-r--r--   0 jason      (501) staff       (20)      361 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7017 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/truthful_qa.py
--rw-r--r--   0 jason      (501) staff       (20)    14944 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     3284 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cache.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.403710 llmuses-0.2.7rc7/llmuses/cli/
--rw-r--r--   0 jason      (501) staff       (20)       50 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cli/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)      404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cli/base.py
--rw-r--r--   0 jason      (501) staff       (20)      549 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cli/cli.py
--rw-r--r--   0 jason      (501) staff       (20)     3865 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/cli/start_server.py
--rw-r--r--   0 jason      (501) staff       (20)     6552 2024-04-09 13:25:19.000000 llmuses-0.2.7rc7/llmuses/config.py
--rw-r--r--   0 jason      (501) staff       (20)     2632 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/constants.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.406218 llmuses-0.2.7rc7/llmuses/evaluator/
--rw-r--r--   0 jason      (501) staff       (20)      101 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/evaluator/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    28598 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/evaluator/evaluator.py
--rw-r--r--   0 jason      (501) staff       (20)     5760 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/evaluator/rating_eval.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.407437 llmuses-0.2.7rc7/llmuses/evaluator/reviewer/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/evaluator/reviewer/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    17034 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/evaluator/reviewer/auto_reviewer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.410904 llmuses-0.2.7rc7/llmuses/metrics/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.411972 llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/
--rw-r--r--   0 jason      (501) staff       (20)      650 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    11450 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/rouge_scorer.py
--rw-r--r--   0 jason      (501) staff       (20)     3462 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/code_metric.py
--rw-r--r--   0 jason      (501) staff       (20)     1986 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/metrics/math_accuracy.py
--rw-r--r--   0 jason      (501) staff       (20)    12545 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/metrics/metrics.py
--rw-r--r--   0 jason      (501) staff       (20)     4516 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/metrics/rouge_metric.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.499073 llmuses-0.2.7rc7/llmuses/models/
--rw-r--r--   0 jason      (501) staff       (20)      141 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.501116 llmuses-0.2.7rc7/llmuses/models/custom/
--rw-r--r--   0 jason      (501) staff       (20)      101 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/models/custom/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     1380 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/models/custom/custom_model.py
--rw-r--r--   0 jason      (501) staff       (20)     1321 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/models/dummy_chat_model.py
--rw-r--r--   0 jason      (501) staff       (20)     3020 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/models/model.py
--rw-r--r--   0 jason      (501) staff       (20)    21702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/models/model_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     3448 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/models/openai_model.py
--rw-r--r--   0 jason      (501) staff       (20)    25273 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/models/template.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.508537 llmuses-0.2.7rc7/llmuses/perf/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     1034 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/_logging.py
--rw-r--r--   0 jason      (501) staff       (20)     1080 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/dashscope_message.py
--rw-r--r--   0 jason      (501) staff       (20)     1057 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/generate_zhipu_token.py
--rw-r--r--   0 jason      (501) staff       (20)    29573 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/http_client.py
--rw-r--r--   0 jason      (501) staff       (20)     3685 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/monitor.py
--rw-r--r--   0 jason      (501) staff       (20)     1153 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/server_sent_event.py
--rw-r--r--   0 jason      (501) staff       (20)     1092 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/vllm_qwen_openai_completion.py
--rw-r--r--   0 jason      (501) staff       (20)     1043 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/perf/zhipu_message.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.509146 llmuses-0.2.7rc7/llmuses/preprocess/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/preprocess/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.510367 llmuses-0.2.7rc7/llmuses/preprocess/tokenizers/
--rw-r--r--   0 jason      (501) staff       (20)        0 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/preprocess/tokenizers/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7810 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/preprocess/tokenizers/gpt2_tokenizer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.510954 llmuses-0.2.7rc7/llmuses/registry/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/registry/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.516050 llmuses-0.2.7rc7/llmuses/registry/tasks/
--rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/arc.yaml
--rw-r--r--   0 jason      (501) staff       (20)      700 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/bbh.yaml
--rw-r--r--   0 jason      (501) staff       (20)      774 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/bbh_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/ceval.yaml
--rw-r--r--   0 jason      (501) staff       (20)      768 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/ceval_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)      806 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml
--rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 13:25:19.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/general_qa.yaml
--rw-r--r--   0 jason      (501) staff       (20)      703 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/gsm8k.yaml
--rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/mmlu.yaml
--rw-r--r--   0 jason      (501) staff       (20)      777 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/registry/tasks/mmlu_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)    14577 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/run.py
--rw-r--r--   0 jason      (501) staff       (20)     8511 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/run_arena.py
--rw-r--r--   0 jason      (501) staff       (20)     5996 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/run_ms.py
--rw-r--r--   0 jason      (501) staff       (20)     3227 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/summarizer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.517475 llmuses-0.2.7rc7/llmuses/tools/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/tools/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3233 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/tools/combine_reports.py
--rw-r--r--   0 jason      (501) staff       (20)     3277 2024-04-01 07:18:15.000000 llmuses-0.2.7rc7/llmuses/tools/gen_mmlu_subject_mapping.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.520291 llmuses-0.2.7rc7/llmuses/utils/
--rw-r--r--   0 jason      (501) staff       (20)       85 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/utils/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7668 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/utils/arena_utils.py
--rw-r--r--   0 jason      (501) staff       (20)     2993 2024-03-18 05:46:13.000000 llmuses-0.2.7rc7/llmuses/utils/completion_parsers.py
--rw-r--r--   0 jason      (501) staff       (20)     1855 2023-12-18 07:51:14.000000 llmuses-0.2.7rc7/llmuses/utils/logger.py
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/utils/task_cfg_parser.py
--rw-r--r--   0 jason      (501) staff       (20)    11952 2024-04-09 03:19:53.000000 llmuses-0.2.7rc7/llmuses/utils/utils.py
--rw-r--r--   0 jason      (501) staff       (20)      121 2024-04-09 14:35:35.000000 llmuses-0.2.7rc7/llmuses/version.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-09 14:35:54.360145 llmuses-0.2.7rc7/llmuses.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-09 14:35:53.000000 llmuses-0.2.7rc7/llmuses.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     5315 2024-04-09 14:35:54.000000 llmuses-0.2.7rc7/llmuses.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-04-09 14:35:53.000000 llmuses-0.2.7rc7/llmuses.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)        8 2024-04-09 14:35:53.000000 llmuses-0.2.7rc7/llmuses.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-04-09 14:35:54.521361 llmuses-0.2.7rc7/setup.cfg
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.305132 llmuses-0.2.7rc8/
+-rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-10 07:35:06.304745 llmuses-0.2.7rc8/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)    11285 2024-04-10 07:35:05.000000 llmuses-0.2.7rc8/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.230765 llmuses-0.2.7rc8/llmuses/
+-rw-r--r--   0 jason      (501) staff       (20)      106 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.233787 llmuses-0.2.7rc8/llmuses/benchmarks/
+-rw-r--r--   0 jason      (501) staff       (20)      158 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.235146 llmuses-0.2.7rc8/llmuses/benchmarks/arc/
+-rw-r--r--   0 jason      (501) staff       (20)      308 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/arc/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     5608 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/arc/ai2_arc.py
+-rw-r--r--   0 jason      (501) staff       (20)     8983 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/arc/arc_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.236594 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/
+-rw-r--r--   0 jason      (501) staff       (20)      300 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    10792 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/bbh_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.253681 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/
+-rwxr-xr-x   0 jason      (501) staff       (20)     1780 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3652 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     1166 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3567 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     4476 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     4830 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2120 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2146 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/navigate.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     1417 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2294 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3480 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     6140 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/snarks.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)      820 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3022 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2944 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2163 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt
+-rw-r--r--   0 jason      (501) staff       (20)     2155 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/benchmark.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.255445 llmuses-0.2.7rc8/llmuses/benchmarks/ceval/
+-rw-r--r--   0 jason      (501) staff       (20)      337 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/ceval/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    15844 2024-04-09 10:23:04.000000 llmuses-0.2.7rc8/llmuses/benchmarks/ceval/ceval_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     5063 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/ceval/ceval_exam.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.257622 llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/
+-rw-r--r--   0 jason      (501) staff       (20)      387 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     2678 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/competition_math.py
+-rw-r--r--   0 jason      (501) staff       (20)    19079 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/competition_math_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)    10091 2024-04-09 13:29:59.000000 llmuses-0.2.7rc8/llmuses/benchmarks/data_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.259332 llmuses-0.2.7rc8/llmuses/benchmarks/general_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      340 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/general_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     6087 2024-04-10 07:29:44.000000 llmuses-0.2.7rc8/llmuses/benchmarks/general_qa/general_qa_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.261947 llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/
+-rw-r--r--   0 jason      (501) staff       (20)      309 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4282 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/gsm8k.py
+-rw-r--r--   0 jason      (501) staff       (20)    13761 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/gsm8k_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.264678 llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/
+-rw-r--r--   0 jason      (501) staff       (20)      351 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4690 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/hellaswag.py
+-rw-r--r--   0 jason      (501) staff       (20)     8547 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/hellaswag_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.266946 llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/
+-rw-r--r--   0 jason      (501) staff       (20)      329 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3482 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/humaneval.py
+-rw-r--r--   0 jason      (501) staff       (20)     1661 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/humaneval_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.269402 llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/
+-rw-r--r--   0 jason      (501) staff       (20)      331 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     5256 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/mmlu.py
+-rw-r--r--   0 jason      (501) staff       (20)    16393 2024-04-09 12:38:11.000000 llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/mmlu_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.271353 llmuses-0.2.7rc8/llmuses/benchmarks/race/
+-rw-r--r--   0 jason      (501) staff       (20)      331 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/race/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3835 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/race/race.py
+-rw-r--r--   0 jason      (501) staff       (20)     9892 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/race/race_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.273146 llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      345 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3296 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/trivia_qa.py
+-rw-r--r--   0 jason      (501) staff       (20)     7653 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.274581 llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      361 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7017 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/truthful_qa.py
+-rw-r--r--   0 jason      (501) staff       (20)    14944 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     3284 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cache.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.276501 llmuses-0.2.7rc8/llmuses/cli/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cli/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)      404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cli/base.py
+-rw-r--r--   0 jason      (501) staff       (20)      549 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cli/cli.py
+-rw-r--r--   0 jason      (501) staff       (20)     3865 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cli/start_server.py
+-rw-r--r--   0 jason      (501) staff       (20)     6552 2024-04-09 13:25:19.000000 llmuses-0.2.7rc8/llmuses/config.py
+-rw-r--r--   0 jason      (501) staff       (20)     2632 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/constants.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.277975 llmuses-0.2.7rc8/llmuses/evaluator/
+-rw-r--r--   0 jason      (501) staff       (20)      101 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/evaluator/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    28598 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/evaluator/evaluator.py
+-rw-r--r--   0 jason      (501) staff       (20)     5760 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/evaluator/rating_eval.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.279020 llmuses-0.2.7rc8/llmuses/evaluator/reviewer/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/evaluator/reviewer/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    17034 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/evaluator/reviewer/auto_reviewer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.281610 llmuses-0.2.7rc8/llmuses/metrics/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.282563 llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/
+-rw-r--r--   0 jason      (501) staff       (20)      650 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    11450 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/rouge_scorer.py
+-rw-r--r--   0 jason      (501) staff       (20)     3462 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/code_metric.py
+-rw-r--r--   0 jason      (501) staff       (20)     1986 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/math_accuracy.py
+-rw-r--r--   0 jason      (501) staff       (20)    12545 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/metrics/metrics.py
+-rw-r--r--   0 jason      (501) staff       (20)     4516 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/metrics/rouge_metric.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.285526 llmuses-0.2.7rc8/llmuses/models/
+-rw-r--r--   0 jason      (501) staff       (20)      141 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.286906 llmuses-0.2.7rc8/llmuses/models/custom/
+-rw-r--r--   0 jason      (501) staff       (20)      101 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/models/custom/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     1380 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/models/custom/custom_model.py
+-rw-r--r--   0 jason      (501) staff       (20)     1321 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/models/dummy_chat_model.py
+-rw-r--r--   0 jason      (501) staff       (20)     3020 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/models/model.py
+-rw-r--r--   0 jason      (501) staff       (20)    21702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/models/model_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     3448 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/models/openai_model.py
+-rw-r--r--   0 jason      (501) staff       (20)    25273 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/models/template.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.291862 llmuses-0.2.7rc8/llmuses/perf/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     1034 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/_logging.py
+-rw-r--r--   0 jason      (501) staff       (20)     1080 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/dashscope_message.py
+-rw-r--r--   0 jason      (501) staff       (20)     1057 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/generate_zhipu_token.py
+-rw-r--r--   0 jason      (501) staff       (20)    29573 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/http_client.py
+-rw-r--r--   0 jason      (501) staff       (20)     3685 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/monitor.py
+-rw-r--r--   0 jason      (501) staff       (20)     1153 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/server_sent_event.py
+-rw-r--r--   0 jason      (501) staff       (20)     1092 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/vllm_qwen_openai_completion.py
+-rw-r--r--   0 jason      (501) staff       (20)     1043 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/zhipu_message.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.292376 llmuses-0.2.7rc8/llmuses/preprocess/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/preprocess/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.293394 llmuses-0.2.7rc8/llmuses/preprocess/tokenizers/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/preprocess/tokenizers/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7810 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/preprocess/tokenizers/gpt2_tokenizer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.293973 llmuses-0.2.7rc8/llmuses/registry/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/registry/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.299580 llmuses-0.2.7rc8/llmuses/registry/tasks/
+-rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/arc.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      700 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/bbh.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      774 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/bbh_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/ceval.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      768 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/ceval_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      806 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 13:25:19.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/general_qa.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      703 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/gsm8k.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/mmlu.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      777 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/mmlu_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)    14577 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/run.py
+-rw-r--r--   0 jason      (501) staff       (20)     8511 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/run_arena.py
+-rw-r--r--   0 jason      (501) staff       (20)     5996 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/run_ms.py
+-rw-r--r--   0 jason      (501) staff       (20)     3227 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/summarizer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.300935 llmuses-0.2.7rc8/llmuses/tools/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/tools/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3233 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/tools/combine_reports.py
+-rw-r--r--   0 jason      (501) staff       (20)     3277 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/tools/gen_mmlu_subject_mapping.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.304188 llmuses-0.2.7rc8/llmuses/utils/
+-rw-r--r--   0 jason      (501) staff       (20)       85 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/utils/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7668 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/utils/arena_utils.py
+-rw-r--r--   0 jason      (501) staff       (20)     2993 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/utils/completion_parsers.py
+-rw-r--r--   0 jason      (501) staff       (20)     1855 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/utils/logger.py
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/utils/task_cfg_parser.py
+-rw-r--r--   0 jason      (501) staff       (20)    11952 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/utils/utils.py
+-rw-r--r--   0 jason      (501) staff       (20)      121 2024-04-10 07:34:50.000000 llmuses-0.2.7rc8/llmuses/version.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.232517 llmuses-0.2.7rc8/llmuses.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-10 07:35:06.000000 llmuses-0.2.7rc8/llmuses.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     5315 2024-04-10 07:35:06.000000 llmuses-0.2.7rc8/llmuses.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-04-10 07:35:06.000000 llmuses-0.2.7rc8/llmuses.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)        8 2024-04-10 07:35:06.000000 llmuses-0.2.7rc8/llmuses.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-04-10 07:35:06.305217 llmuses-0.2.7rc8/setup.cfg
```

### Comparing `llmuses-0.2.7rc7/PKG-INFO` & `llmuses-0.2.7rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmuses
-Version: 0.2.7rc7
+Version: 0.2.7rc8
 Summary: LLMs Evaluation Framework
 Home-page: 
 Author: ModelScope team
 Author-email: contact@modelscope.cn
 Keywords: python,llm,evaluation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmuses-0.2.7rc7/README.md` & `llmuses-0.2.7rc8/README.md`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/arc/ai2_arc.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/arc/ai2_arc.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/arc/arc_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/arc/arc_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/bbh_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/bbh_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/navigate.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/navigate.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/snarks.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/snarks.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt` & `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/benchmark.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/ceval/ceval_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/ceval/ceval_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/ceval/ceval_exam.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/ceval/ceval_exam.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/competition_math.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/competition_math.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/competition_math/competition_math_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/competition_math_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/data_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/data_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/general_qa/general_qa_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/general_qa/general_qa_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,52 +39,59 @@
                          **kwargs)
     
     def load(self,
              dataset_name_or_path: str,
              subset_list: list = None,
              **kwargs) -> dict:
 
-        file_list = glob.glob(os.path.join(dataset_name_or_path, '*.jsonl'))
+        data_file_list = glob.glob(os.path.join(dataset_name_or_path, '*.jsonl'))
         data_list = []
+
         try:
-            for file_path in file_list:
+            for file_path in data_file_list:
                 data_list.extend(jsonl_to_list(file_path))
         except Exception as e:
             raise ValueError(f"Failed to load data from {dataset_name_or_path}, got error: {e}")
 
         data_dict = {'default': {'test': data_list}}
 
         return data_dict
     
     def gen_prompt(self, input_d: dict, subset_name: str, few_shot_list: list, **kwargs) -> dict:
         """
         Args:
-            input_d: {'history': [], 'question': '', 'answer': ''}
+            input_d:
+                format1: {'history': [['q1', 'a1'], ['q2', 'a2']], 'question': '', 'answer': ''}
+                format2: {'history': [['q1', 'a1'], ['q2', 'a2']], 'query': '', 'response': ''}
 
         Returns:
             {'data': [prompt]}
 
         """
         # prompt = f"'<|im_start|>user\n{input_d['input']}<|im_end|>\n<|im_start|>assistant\n'"
-        history = input_d.get('history', [])
-        prompt = input_d['question']
+        history = input_d.get('history', [])    # history: [['q1', 'a1'], ['q2', 'a2'], ...]
         if len(history) > 0:
-            prompt = '\n'.join(history) + '\n' + prompt
+            logger.warning(f"The history is not included in the prompt for GeneralQA. To be supported in the future.")
+
+        prompt = input_d.get('question', '') or input_d.get('query', '')
+
+        # if len(history) > 0:
+        #     prompt = '\n'.join(history) + '\n' + prompt
         return {'data': [prompt]}
     
     def get_gold_answer(self, input_d: dict) -> str:
         """
         Args:
             input_d: {'history': [], 'question': '', 'answer': ''}
 
         Returns:
             gold_answer: str
 
         """
-        return input_d.get('answer', '')
+        return input_d.get('answer', '') or input_d.get('response', '')
     
     def parse_pred_result(self, result: str, raw_input_d: dict = None, eval_type: str = 'checkpoint') -> str:
         """
         Args:
             result: str
 
         Returns:
```

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/gsm8k.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/gsm8k.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/gsm8k/gsm8k_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/gsm8k_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/hellaswag.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/hellaswag.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/hellaswag/hellaswag_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/hellaswag_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/humaneval.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/humaneval.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/humaneval/humaneval_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/humaneval_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/mmlu.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/mmlu.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/mmlu/mmlu_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/mmlu_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/race/race.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/race/race.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/race/race_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/race/race_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/trivia_qa.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/trivia_qa.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/truthful_qa.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/truthful_qa.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py` & `llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/cache.py` & `llmuses-0.2.7rc8/llmuses/cache.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/cli/cli.py` & `llmuses-0.2.7rc8/llmuses/cli/cli.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/cli/start_server.py` & `llmuses-0.2.7rc8/llmuses/cli/start_server.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/config.py` & `llmuses-0.2.7rc8/llmuses/config.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/constants.py` & `llmuses-0.2.7rc8/llmuses/constants.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/evaluator/evaluator.py` & `llmuses-0.2.7rc8/llmuses/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/evaluator/rating_eval.py` & `llmuses-0.2.7rc8/llmuses/evaluator/rating_eval.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/evaluator/reviewer/auto_reviewer.py` & `llmuses-0.2.7rc8/llmuses/evaluator/reviewer/auto_reviewer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/__init__.py` & `llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/__init__.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/metrics/bundled_rouge_score/rouge_scorer.py` & `llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/rouge_scorer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/metrics/code_metric.py` & `llmuses-0.2.7rc8/llmuses/metrics/code_metric.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/metrics/math_accuracy.py` & `llmuses-0.2.7rc8/llmuses/metrics/math_accuracy.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/metrics/metrics.py` & `llmuses-0.2.7rc8/llmuses/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/metrics/rouge_metric.py` & `llmuses-0.2.7rc8/llmuses/metrics/rouge_metric.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/models/custom/custom_model.py` & `llmuses-0.2.7rc8/llmuses/models/custom/custom_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/models/dummy_chat_model.py` & `llmuses-0.2.7rc8/llmuses/models/dummy_chat_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/models/model.py` & `llmuses-0.2.7rc8/llmuses/models/model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/models/model_adapter.py` & `llmuses-0.2.7rc8/llmuses/models/model_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/models/openai_model.py` & `llmuses-0.2.7rc8/llmuses/models/openai_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/models/template.py` & `llmuses-0.2.7rc8/llmuses/models/template.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/perf/_logging.py` & `llmuses-0.2.7rc8/llmuses/perf/_logging.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/perf/dashscope_message.py` & `llmuses-0.2.7rc8/llmuses/perf/dashscope_message.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/perf/generate_zhipu_token.py` & `llmuses-0.2.7rc8/llmuses/perf/generate_zhipu_token.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/perf/http_client.py` & `llmuses-0.2.7rc8/llmuses/perf/http_client.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/perf/monitor.py` & `llmuses-0.2.7rc8/llmuses/perf/monitor.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/perf/server_sent_event.py` & `llmuses-0.2.7rc8/llmuses/perf/server_sent_event.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/perf/vllm_qwen_openai_completion.py` & `llmuses-0.2.7rc8/llmuses/perf/vllm_qwen_openai_completion.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/perf/zhipu_message.py` & `llmuses-0.2.7rc8/llmuses/perf/zhipu_message.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/preprocess/tokenizers/gpt2_tokenizer.py` & `llmuses-0.2.7rc8/llmuses/preprocess/tokenizers/gpt2_tokenizer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/arc.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/arc.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/bbh.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/bbh.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/bbh_mini.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/bbh_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/ceval.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/ceval.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/ceval_mini.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/ceval_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/general_qa.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/general_qa.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/gsm8k.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/gsm8k.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/mmlu.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/mmlu.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/registry/tasks/mmlu_mini.yaml` & `llmuses-0.2.7rc8/llmuses/registry/tasks/mmlu_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/run.py` & `llmuses-0.2.7rc8/llmuses/run.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/run_arena.py` & `llmuses-0.2.7rc8/llmuses/run_arena.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/run_ms.py` & `llmuses-0.2.7rc8/llmuses/run_ms.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/summarizer.py` & `llmuses-0.2.7rc8/llmuses/summarizer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/tools/combine_reports.py` & `llmuses-0.2.7rc8/llmuses/tools/combine_reports.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/tools/gen_mmlu_subject_mapping.py` & `llmuses-0.2.7rc8/llmuses/tools/gen_mmlu_subject_mapping.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/utils/arena_utils.py` & `llmuses-0.2.7rc8/llmuses/utils/arena_utils.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/utils/completion_parsers.py` & `llmuses-0.2.7rc8/llmuses/utils/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/utils/logger.py` & `llmuses-0.2.7rc8/llmuses/utils/logger.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses/utils/utils.py` & `llmuses-0.2.7rc8/llmuses/utils/utils.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc7/llmuses.egg-info/PKG-INFO` & `llmuses-0.2.7rc8/llmuses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmuses
-Version: 0.2.7rc7
+Version: 0.2.7rc8
 Summary: LLMs Evaluation Framework
 Home-page: 
 Author: ModelScope team
 Author-email: contact@modelscope.cn
 Keywords: python,llm,evaluation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmuses-0.2.7rc7/llmuses.egg-info/SOURCES.txt` & `llmuses-0.2.7rc8/llmuses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

