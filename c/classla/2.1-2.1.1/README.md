# Comparing `tmp/classla-2.1.tar.gz` & `tmp/classla-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classla-2.1.tar", last modified: Tue Aug  8 07:48:44 2023, max compression
+gzip compressed data, was "classla-2.1.1.tar", last modified: Wed Apr 10 11:03:18 2024, max compression
```

## Comparing `classla-2.1.tar` & `classla-2.1.1.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.690206 classla-2.1/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      603 2023-08-08 07:48:16.000000 classla-2.1/LICENSE
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    19995 2023-08-08 07:48:44.686206 classla-2.1/PKG-INFO
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    18731 2023-08-08 07:48:16.000000 classla-2.1/README.md
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.630205 classla-2.1/classla/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      950 2023-08-08 07:48:16.000000 classla-2.1/classla/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      101 2023-08-08 07:48:16.000000 classla-2.1/classla/_version.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.638205 classla-2.1/classla/models/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)       84 2023-08-08 07:48:16.000000 classla-2.1/classla/models/_training_logging.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    15100 2023-08-08 07:48:16.000000 classla-2.1/classla/models/charlm.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    26251 2023-08-08 07:48:16.000000 classla-2.1/classla/models/classifier.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.638205 classla-2.1/classla/models/classifiers/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/classifiers/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2224 2023-08-08 07:48:16.000000 classla-2.1/classla/models/classifiers/classifier_args.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    15364 2023-08-08 07:48:16.000000 classla-2.1/classla/models/classifiers/cnn_classifier.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2439 2023-08-08 07:48:16.000000 classla-2.1/classla/models/classifiers/iterate_test.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.646205 classla-2.1/classla/models/common/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3908 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/beam.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3582 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/biaffine.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     6728 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/char_model.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     8385 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/chuliu_edmonds.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2012 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/constant.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     5418 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/crf.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1413 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    36070 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/doc.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2856 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/dropout.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     5089 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/hlstm.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2662 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/loss.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4855 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/packed_lstm.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     5183 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/pretrain.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      221 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/seq2seq_constant.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    11837 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/seq2seq_model.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     8016 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/seq2seq_modules.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3507 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/seq2seq_utils.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      645 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/trainer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     7287 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/utils.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     7916 2023-08-08 07:48:16.000000 classla-2.1/classla/models/common/vocab.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.646205 classla-2.1/classla/models/depparse/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/depparse/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     9232 2023-08-08 07:48:16.000000 classla-2.1/classla/models/depparse/data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    10188 2023-08-08 07:48:16.000000 classla-2.1/classla/models/depparse/model.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      616 2023-08-08 07:48:16.000000 classla-2.1/classla/models/depparse/scorer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     6031 2023-08-08 07:48:16.000000 classla-2.1/classla/models/depparse/trainer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2248 2023-08-08 07:48:16.000000 classla-2.1/classla/models/identity_lemmatizer.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.650205 classla-2.1/classla/models/lemma/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/lemma/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4545 2023-08-08 07:48:16.000000 classla-2.1/classla/models/lemma/data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      631 2023-08-08 07:48:16.000000 classla-2.1/classla/models/lemma/edit.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      460 2023-08-08 07:48:16.000000 classla-2.1/classla/models/lemma/scorer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     9087 2023-08-08 07:48:16.000000 classla-2.1/classla/models/lemma/trainer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      651 2023-08-08 07:48:16.000000 classla-2.1/classla/models/lemma/vocab.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    14569 2023-08-08 07:48:16.000000 classla-2.1/classla/models/lemmatizer.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.650205 classla-2.1/classla/models/mwt/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/mwt/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3550 2023-08-08 07:48:16.000000 classla-2.1/classla/models/mwt/data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      358 2023-08-08 07:48:16.000000 classla-2.1/classla/models/mwt/scorer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     5623 2023-08-08 07:48:16.000000 classla-2.1/classla/models/mwt/trainer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      508 2023-08-08 07:48:16.000000 classla-2.1/classla/models/mwt/vocab.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    11456 2023-08-08 07:48:16.000000 classla-2.1/classla/models/mwt_expander.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.654205 classla-2.1/classla/models/ner/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/ner/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     8846 2023-08-08 07:48:16.000000 classla-2.1/classla/models/ner/data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     6299 2023-08-08 07:48:16.000000 classla-2.1/classla/models/ner/model.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4604 2023-08-08 07:48:16.000000 classla-2.1/classla/models/ner/scorer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     5389 2023-08-08 07:48:16.000000 classla-2.1/classla/models/ner/trainer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3557 2023-08-08 07:48:16.000000 classla-2.1/classla/models/ner/utils.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1557 2023-08-08 07:48:16.000000 classla-2.1/classla/models/ner/vocab.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    11691 2023-08-08 07:48:16.000000 classla-2.1/classla/models/ner_tagger.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    12065 2023-08-08 07:48:16.000000 classla-2.1/classla/models/parser.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.658205 classla-2.1/classla/models/pos/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4059 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/build_xpos_vocab_factory.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     6225 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     9023 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/model.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    13663 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/postprocessor.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      651 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/scorer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     7364 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/trainer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3275 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/vocab.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2120 2023-08-08 07:48:16.000000 classla-2.1/classla/models/pos/xpos_vocab_factory.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.658205 classla-2.1/classla/models/srl/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/models/srl/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     6141 2023-08-08 07:48:16.000000 classla-2.1/classla/models/srl/data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     7526 2023-08-08 07:48:16.000000 classla-2.1/classla/models/srl/model.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1821 2023-08-08 07:48:16.000000 classla-2.1/classla/models/srl/scorer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4509 2023-08-08 07:48:16.000000 classla-2.1/classla/models/srl/trainer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1106 2023-08-08 07:48:16.000000 classla-2.1/classla/models/srl/vocab.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    11382 2023-08-08 07:48:16.000000 classla-2.1/classla/models/srl_tagger.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    15674 2023-08-08 07:48:16.000000 classla-2.1/classla/models/tagger.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.662205 classla-2.1/classla/pipeline/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      206 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/_constants.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     7920 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/core.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2052 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/depparse_processor.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.666206 classla-2.1/classla/pipeline/external/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/external/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2150 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/external/jieba.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2280 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/external/spacy.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2693 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/external/sudachipy.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4093 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/lemma_processor.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1518 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/mwt_processor.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1559 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/ner_processor.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2890 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/pos_processor.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     8296 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/processor.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      129 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/registry.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1763 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/sentiment_processor.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1634 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/srl_processor.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4302 2023-08-08 07:48:16.000000 classla-2.1/classla/pipeline/tokenize_processor.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.666206 classla-2.1/classla/protobuf/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)   182057 2023-08-08 07:48:16.000000 classla-2.1/classla/protobuf/CoreNLP_pb2.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1701 2023-08-08 07:48:16.000000 classla-2.1/classla/protobuf/__init__.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.666206 classla-2.1/classla/resources/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/resources/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    17440 2023-08-08 07:48:16.000000 classla-2.1/classla/resources/common.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4384 2023-08-08 07:48:16.000000 classla-2.1/classla/resources/installation.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     9320 2023-08-08 07:48:16.000000 classla-2.1/classla/resources/prepare_resources.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.670205 classla-2.1/classla/server/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      632 2023-08-08 07:48:16.000000 classla-2.1/classla/server/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4672 2023-08-08 07:48:16.000000 classla-2.1/classla/server/annotator.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    27864 2023-08-08 07:48:16.000000 classla-2.1/classla/server/client.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2619 2023-08-08 07:48:16.000000 classla-2.1/classla/server/main.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2590 2023-08-08 07:48:16.000000 classla-2.1/classla/server/semgrex.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.674206 classla-2.1/classla/utils/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      402 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/avg_sent_len.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     8163 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/conll.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    27954 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/conll18_ud_eval.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1301 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/contract_mwt.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1263 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/helper_func.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      246 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/max_mwt_length.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1788 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/obeliks.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2456 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/postprocess_vietnamese_tokenizer_data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2225 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/prepare_ner_data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     5072 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/prepare_tokenizer_data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1777 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/reldi.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      451 2023-08-08 07:48:16.000000 classla-2.1/classla/utils/select_backoff.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.634204 classla-2.1/classla.egg-info/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    19995 2023-08-08 07:48:44.000000 classla-2.1/classla.egg-info/PKG-INFO
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4927 2023-08-08 07:48:44.000000 classla-2.1/classla.egg-info/SOURCES.txt
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        1 2023-08-08 07:48:44.000000 classla-2.1/classla.egg-info/dependency_links.txt
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      152 2023-08-08 07:48:44.000000 classla-2.1/classla.egg-info/requires.txt
--rw-rw-r--   0 decaf     (1000) decaf     (1000)       40 2023-08-08 07:48:44.000000 classla-2.1/classla.egg-info/top_level.txt
--rw-rw-r--   0 decaf     (1000) decaf     (1000)       38 2023-08-08 07:48:44.690206 classla-2.1/setup.cfg
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4197 2023-08-08 07:48:16.000000 classla-2.1/setup.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.674206 classla-2.1/stanfordnlp/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/stanfordnlp/__init__.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.674206 classla-2.1/stanfordnlp/models/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/stanfordnlp/models/__init__.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.674206 classla-2.1/stanfordnlp/models/common/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:16.000000 classla-2.1/stanfordnlp/models/common/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)       45 2023-08-08 07:48:16.000000 classla-2.1/stanfordnlp/models/common/pretrain.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.682206 classla-2.1/tests/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4600 2023-08-08 07:48:16.000000 classla-2.1/tests/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     8157 2023-08-08 07:48:16.000000 classla-2.1/tests/test_client.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3413 2023-08-08 07:48:16.000000 classla-2.1/tests/test_data_conversion.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1580 2023-08-08 07:48:16.000000 classla-2.1/tests/test_data_objects.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4885 2023-08-08 07:48:16.000000 classla-2.1/tests/test_decorators.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2618 2023-08-08 07:48:16.000000 classla-2.1/tests/test_depparse.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2467 2023-08-08 07:48:16.000000 classla-2.1/tests/test_depparse_data.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1543 2023-08-08 07:48:16.000000 classla-2.1/tests/test_doc.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     6940 2023-08-08 07:48:16.000000 classla-2.1/tests/test_english_pipeline.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1424 2023-08-08 07:48:16.000000 classla-2.1/tests/test_installation.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1126 2023-08-08 07:48:16.000000 classla-2.1/tests/test_lemmatizer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3358 2023-08-08 07:48:16.000000 classla-2.1/tests/test_mwt_expander.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1514 2023-08-08 07:48:16.000000 classla-2.1/tests/test_ner_tagger.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1850 2023-08-08 07:48:16.000000 classla-2.1/tests/test_pretrain.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4607 2023-08-08 07:48:16.000000 classla-2.1/tests/test_protobuf.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3090 2023-08-08 07:48:16.000000 classla-2.1/tests/test_requirements.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     6581 2023-08-08 07:48:16.000000 classla-2.1/tests/test_semgrex.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4239 2023-08-08 07:48:16.000000 classla-2.1/tests/test_server_misc.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    10266 2023-08-08 07:48:16.000000 classla-2.1/tests/test_server_request.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     9727 2023-08-08 07:48:16.000000 classla-2.1/tests/test_server_start.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1038 2023-08-08 07:48:16.000000 classla-2.1/tests/test_tagger.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     8051 2023-08-08 07:48:16.000000 classla-2.1/tests/test_tokenizer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2757 2023-08-08 07:48:16.000000 classla-2.1/tests/test_utils.py
-drwxrwxr-x   0 decaf     (1000) decaf     (1000)        0 2023-08-08 07:48:44.686206 classla-2.1/tests_classla/
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     4574 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/__init__.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      583 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_downloads.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     3067 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_lemmatizer.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)      989 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_ner.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1231 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_parser.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)    11092 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_readme_examples.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     8757 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_slovenian_pipeline.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1099 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_srl.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     1284 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_tagger.py
--rw-rw-r--   0 decaf     (1000) decaf     (1000)     2998 2023-08-08 07:48:16.000000 classla-2.1/tests_classla/test_tokenizer.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.502962 classla-2.1.1/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      603 2024-04-10 10:01:35.000000 classla-2.1.1/LICENSE
+-rw-r--r--   0 prupnik  (1977552579) prupnik  (1977552579)    20597 2024-04-10 11:03:18.501962 classla-2.1.1/PKG-INFO
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    18925 2024-04-10 10:13:11.000000 classla-2.1.1/README.md
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.436961 classla-2.1.1/classla/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      950 2024-04-10 10:01:35.000000 classla-2.1.1/classla/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      103 2024-04-10 10:01:35.000000 classla-2.1.1/classla/_version.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.443961 classla-2.1.1/classla/models/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       84 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/_training_logging.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    15100 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/charlm.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    26251 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/classifier.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.445962 classla-2.1.1/classla/models/classifiers/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/classifiers/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2224 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/classifiers/classifier_args.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    15364 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/classifiers/cnn_classifier.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2439 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/classifiers/iterate_test.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.455962 classla-2.1.1/classla/models/common/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3908 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/beam.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3582 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/biaffine.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     6728 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/char_model.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8385 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/chuliu_edmonds.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2012 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/constant.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     5418 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/crf.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1413 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    36070 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/doc.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2856 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/dropout.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     5089 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/hlstm.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2662 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/loss.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4855 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/packed_lstm.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     5183 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/pretrain.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      221 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/seq2seq_constant.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    11837 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/seq2seq_model.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8016 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/seq2seq_modules.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3507 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/seq2seq_utils.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      645 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/trainer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     7287 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/utils.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     7916 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/common/vocab.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.457962 classla-2.1.1/classla/models/depparse/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/depparse/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     9232 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/depparse/data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    10188 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/depparse/model.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      616 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/depparse/scorer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     6031 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/depparse/trainer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2248 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/identity_lemmatizer.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.460962 classla-2.1.1/classla/models/lemma/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/lemma/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4545 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/lemma/data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      631 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/lemma/edit.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      460 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/lemma/scorer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     9087 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/lemma/trainer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      651 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/lemma/vocab.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    14569 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/lemmatizer.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.462962 classla-2.1.1/classla/models/mwt/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/mwt/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3550 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/mwt/data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      358 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/mwt/scorer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     5623 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/mwt/trainer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      508 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/mwt/vocab.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    11456 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/mwt_expander.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.465962 classla-2.1.1/classla/models/ner/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/ner/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8846 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/ner/data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     6299 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/ner/model.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4604 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/ner/scorer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     5389 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/ner/trainer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3557 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/ner/utils.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1557 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/ner/vocab.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    11691 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/ner_tagger.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    12065 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/parser.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.468962 classla-2.1.1/classla/models/pos/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4059 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/build_xpos_vocab_factory.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     6225 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     9023 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/model.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    13663 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/postprocessor.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      651 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/scorer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     7364 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/trainer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3275 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/vocab.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2120 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/pos/xpos_vocab_factory.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.471962 classla-2.1.1/classla/models/srl/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/srl/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     6141 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/srl/data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     7526 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/srl/model.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1821 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/srl/scorer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4509 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/srl/trainer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1106 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/srl/vocab.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    11382 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/srl_tagger.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    15674 2024-04-10 10:01:35.000000 classla-2.1.1/classla/models/tagger.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.476962 classla-2.1.1/classla/pipeline/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      206 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/_constants.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     7920 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/core.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2052 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/depparse_processor.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.477962 classla-2.1.1/classla/pipeline/external/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/external/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2150 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/external/jieba.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2280 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/external/spacy.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2693 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/external/sudachipy.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4093 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/lemma_processor.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1518 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/mwt_processor.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1559 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/ner_processor.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2890 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/pos_processor.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8296 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/processor.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      129 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/registry.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1763 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/sentiment_processor.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1634 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/srl_processor.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4302 2024-04-10 10:01:35.000000 classla-2.1.1/classla/pipeline/tokenize_processor.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.478962 classla-2.1.1/classla/protobuf/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)   182057 2024-04-10 10:01:35.000000 classla-2.1.1/classla/protobuf/CoreNLP_pb2.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1701 2024-04-10 10:01:35.000000 classla-2.1.1/classla/protobuf/__init__.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.480962 classla-2.1.1/classla/resources/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/resources/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    17440 2024-04-10 10:01:35.000000 classla-2.1.1/classla/resources/common.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4384 2024-04-10 10:01:35.000000 classla-2.1.1/classla/resources/installation.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     9320 2024-04-10 10:01:35.000000 classla-2.1.1/classla/resources/prepare_resources.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.481962 classla-2.1.1/classla/server/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      632 2024-04-10 10:01:35.000000 classla-2.1.1/classla/server/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4672 2024-04-10 10:01:35.000000 classla-2.1.1/classla/server/annotator.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    27864 2024-04-10 10:01:35.000000 classla-2.1.1/classla/server/client.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2619 2024-04-10 10:01:35.000000 classla-2.1.1/classla/server/main.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2590 2024-04-10 10:01:35.000000 classla-2.1.1/classla/server/semgrex.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.486962 classla-2.1.1/classla/utils/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      402 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/avg_sent_len.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8163 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/conll.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    27954 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/conll18_ud_eval.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1301 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/contract_mwt.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1263 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/helper_func.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      246 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/max_mwt_length.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1788 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/obeliks.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2456 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/postprocess_vietnamese_tokenizer_data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2225 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/prepare_ner_data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     5072 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/prepare_tokenizer_data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1777 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/reldi.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      451 2024-04-10 10:01:35.000000 classla-2.1.1/classla/utils/select_backoff.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.501962 classla-2.1.1/classla.egg-info/
+-rw-r--r--   0 prupnik  (1977552579) prupnik  (1977552579)    20597 2024-04-10 11:03:18.000000 classla-2.1.1/classla.egg-info/PKG-INFO
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4927 2024-04-10 11:03:18.000000 classla-2.1.1/classla.egg-info/SOURCES.txt
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        1 2024-04-10 11:03:18.000000 classla-2.1.1/classla.egg-info/dependency_links.txt
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      152 2024-04-10 11:03:18.000000 classla-2.1.1/classla.egg-info/requires.txt
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       40 2024-04-10 11:03:18.000000 classla-2.1.1/classla.egg-info/top_level.txt
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       38 2024-04-10 11:03:18.502962 classla-2.1.1/setup.cfg
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4296 2024-04-10 10:53:00.000000 classla-2.1.1/setup.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.487962 classla-2.1.1/stanfordnlp/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/stanfordnlp/__init__.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.487962 classla-2.1.1/stanfordnlp/models/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/stanfordnlp/models/__init__.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.488962 classla-2.1.1/stanfordnlp/models/common/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 10:01:35.000000 classla-2.1.1/stanfordnlp/models/common/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       45 2024-04-10 10:01:35.000000 classla-2.1.1/stanfordnlp/models/common/pretrain.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.496962 classla-2.1.1/tests/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4600 2024-04-10 10:01:35.000000 classla-2.1.1/tests/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8157 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_client.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3413 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_data_conversion.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1580 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_data_objects.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4885 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_decorators.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2618 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_depparse.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2467 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_depparse_data.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1543 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_doc.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     6940 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_english_pipeline.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1424 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_installation.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1126 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_lemmatizer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3358 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_mwt_expander.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1514 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_ner_tagger.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1850 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_pretrain.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4607 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_protobuf.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3090 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_requirements.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     6581 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_semgrex.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4239 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_server_misc.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    10266 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_server_request.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     9727 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_server_start.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1038 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_tagger.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8051 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_tokenizer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2757 2024-04-10 10:01:35.000000 classla-2.1.1/tests/test_utils.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-10 11:03:18.500962 classla-2.1.1/tests_classla/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4574 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      583 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_downloads.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     3067 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_lemmatizer.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      989 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_ner.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1231 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_parser.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    11092 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_readme_examples.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8757 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_slovenian_pipeline.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1099 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_srl.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1284 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_tagger.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     2998 2024-04-10 10:01:35.000000 classla-2.1.1/tests_classla/test_tokenizer.py
```

### Comparing `classla-2.1/LICENSE` & `classla-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `classla-2.1/PKG-INFO` & `classla-2.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,20 @@
-Metadata-Version: 2.1
-Name: classla
-Version: 2.1
-Summary: Adapted Stanford NLP Python Library with improvements for specific languages.
-Home-page: https://github.com/clarinsi/classla-stanfordnlp.git
-Author: CLARIN.SI
-Author-email: info@clarin.si
-License: Apache License 2.0
-Keywords: natural-language-processing nlp natural-language-understanding stanford-nlp deep-learning clarinsi
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Text Processing :: Linguistic
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # A [CLASSLA](http://www.clarin.si/info/k-centre/) Fork of [Stanza](https://github.com/stanfordnlp/stanza) for Processing Slovenian, Croatian, Serbian, Macedonian and Bulgarian
 
 ## Description
 
 This pipeline allows for processing of standard Slovenian, Croatian, Serbian and Bulgarian on the levels of
 
 - tokenization and sentence splitting
 - part-of-speech tagging
 - lemmatization
 - dependency parsing
 - named entity recognition
 
-It also allows for (alpha) processing of standard Macedonian on the levels of 
+It also allows for processing of standard Macedonian on the levels of
 
 - tokenization and sentence splitting
 - part-of-speech tagging
 - lemmatization
 
 Finally, it allows for processing of non-standard (Internet) Slovenian, Croatian and Serbian on the same levels as standard language (all models are tailored to non-standard language except for dependency parsing where the standard module is used).
 
@@ -60,15 +30,45 @@
 - morphosyntactic tagging models based on larger quantities of training data than is available in UD (training data that are morphosyntactically tagged, but not UD-parsed)
 - lemmatization models based on larger quantities of training data than is available in UD (training data that are lemmatized, but not UD-parsed)
 - optional JOS-project-based parsing of Slovenian (usage documented [here](https://github.com/clarinsi/classla/blob/master/README.superuser.md#jos-dependency-parsing-system))
 - named entity recognition models for all languages except Macedonian (Stanza does not cover named entity recognition for any of the languages supported by classla)
 - Macedonian models (Macedonian is not available in UD yet)
 - non-standard models for Croatian, Slovenian, Serbian (there is no UD data for these varieties)
 
-The above modifications led to some important improvements in the tool’s performance in comparison to original Stanza. For standard Slovenian, for example, running the full classla pipeline increases sentence segmentation F1 scores to 99.52 (94.29% error reduction), lemmatization to 99.17 (68.8% error reduction), XPOS tagging  to 97.38 (46.75% error reduction), UPOS tagging to 98.69 (23.4% error reduction), and LAS to 92.05 (23.56% error reduction).  See official [Stanza performance](https://stanfordnlp.github.io/stanza/performance.html) (evaluated on different data splits) for comparison.
+The above modifications led to some important improvements in the tool's performance in comparison to original Stanza. For standard Slovenian, comparing the CLASSLA-Stanza tool with Stanza on the [SloBENCH benchmark](https://slobench.cjvt.si/leaderboard/view/11), shows relative error reduction (part of the error removed by moving from Stanza to CLASSLA-Stanza) on sentence segmentation to be 98%, on token segmentation 50%, on lemmatization 69%, on morphosyntactic XPOS tagging 65%, and on dependency parsing 34%.
+
+## Citing
+
+If you use this tool, please cite the following papers:
+
+```
+@inproceedings{ljubesic-dobrovoljc-2019-neural,
+    title = "What does Neural Bring? Analysing Improvements in Morphosyntactic Annotation and Lemmatisation of {S}lovenian, {C}roatian and {S}erbian",
+    author = "Ljube{\v{s}}i{\'c}, Nikola  and
+      Dobrovoljc, Kaja",
+    booktitle = "Proceedings of the 7th Workshop on Balto-Slavic Natural Language Processing",
+    month = aug,
+    year = "2019",
+    address = "Florence, Italy",
+    publisher = "Association for Computational Linguistics",
+    url = "https://www.aclweb.org/anthology/W19-3704",
+    doi = "10.18653/v1/W19-3704",
+    pages = "29--34"
+    }
+@misc{terčon2023classlastanza,
+      title={CLASSLA-Stanza: The Next Step for Linguistic Processing of South Slavic Languages},
+      author={Luka Terčon and Nikola Ljubešić},
+      year={2023},
+      eprint={2308.04255},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+
+```
+
 
 ## Installation
 ### pip
 We recommend that you install CLASSLA via pip, the Python package manager. To install, run:
 ```bash
 pip install classla
 ```
@@ -199,37 +199,17 @@
 
 The dependency parsing processor ```depparse``` performs syntactic dependency parsing of sentences following the [Universal Dependencies formalism](https://universaldependencies.org/introduction.html#:~:text=Universal%20Dependencies%20(UD)%20is%20a,from%20a%20language%20typology%20perspective.). It requires the ```tokenize``` and ```pos``` processors.
 
 ### Named entity recognition
 
 The named entity recognition processor ```ner``` identifies named entities in text following the [IOB2](https://en.wikipedia.org/wiki/Inside–outside–beginning_(tagging)) format. It requires only the ```tokenize``` processor.
 
-## Citing
-
-If you use this tool, please cite the following paper:
-
-```
-@inproceedings{ljubesic-dobrovoljc-2019-neural,
-    title = "What does Neural Bring? Analysing Improvements in Morphosyntactic Annotation and Lemmatisation of {S}lovenian, {C}roatian and {S}erbian",
-    author = "Ljube{\v{s}}i{\'c}, Nikola  and
-      Dobrovoljc, Kaja",
-    booktitle = "Proceedings of the 7th Workshop on Balto-Slavic Natural Language Processing",
-    month = aug,
-    year = "2019",
-    address = "Florence, Italy",
-    publisher = "Association for Computational Linguistics",
-    url = "https://www.aclweb.org/anthology/W19-3704",
-    doi = "10.18653/v1/W19-3704",
-    pages = "29--34"
-    }
-```
-
 ## Croatian examples
 
-### Example of standard Croatian 
+### Example of standard Croatian
 
 ```
 >>> import classla
 >>> nlp = classla.Pipeline('hr') # run classla.download('hr') beforehand if necessary
 >>> doc = nlp("Ante Starčević rođen je u Velikom Žitniku.")
 >>> print(doc.to_conll())
 # newpar id = 1
```

### Comparing `classla-2.1/README.md` & `classla-2.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,61 @@
+Metadata-Version: 2.1
+Name: classla
+Version: 2.1.1
+Summary: Adapted Stanford NLP Python Library with improvements for specific languages.
+Home-page: https://github.com/clarinsi/classla-stanfordnlp.git
+Author: CLARIN.SI
+Author-email: info@clarin.si
+License: Apache License 2.0
+Keywords: natural-language-processing nlp natural-language-understanding stanford-nlp deep-learning clarinsi
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy==1.23.0
+Requires-Dist: protobuf==4.21.2
+Requires-Dist: requests==2.28.0
+Requires-Dist: torch==1.12.0
+Requires-Dist: tqdm==4.62.3
+Requires-Dist: obeliks==1.1.6
+Requires-Dist: reldi-tokeniser==1.0.3
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+
 # A [CLASSLA](http://www.clarin.si/info/k-centre/) Fork of [Stanza](https://github.com/stanfordnlp/stanza) for Processing Slovenian, Croatian, Serbian, Macedonian and Bulgarian
 
 ## Description
 
 This pipeline allows for processing of standard Slovenian, Croatian, Serbian and Bulgarian on the levels of
 
 - tokenization and sentence splitting
 - part-of-speech tagging
 - lemmatization
 - dependency parsing
 - named entity recognition
 
-It also allows for (alpha) processing of standard Macedonian on the levels of 
+It also allows for processing of standard Macedonian on the levels of
 
 - tokenization and sentence splitting
 - part-of-speech tagging
 - lemmatization
 
 Finally, it allows for processing of non-standard (Internet) Slovenian, Croatian and Serbian on the same levels as standard language (all models are tailored to non-standard language except for dependency parsing where the standard module is used).
 
@@ -30,15 +71,45 @@
 - morphosyntactic tagging models based on larger quantities of training data than is available in UD (training data that are morphosyntactically tagged, but not UD-parsed)
 - lemmatization models based on larger quantities of training data than is available in UD (training data that are lemmatized, but not UD-parsed)
 - optional JOS-project-based parsing of Slovenian (usage documented [here](https://github.com/clarinsi/classla/blob/master/README.superuser.md#jos-dependency-parsing-system))
 - named entity recognition models for all languages except Macedonian (Stanza does not cover named entity recognition for any of the languages supported by classla)
 - Macedonian models (Macedonian is not available in UD yet)
 - non-standard models for Croatian, Slovenian, Serbian (there is no UD data for these varieties)
 
-The above modifications led to some important improvements in the tool’s performance in comparison to original Stanza. For standard Slovenian, for example, running the full classla pipeline increases sentence segmentation F1 scores to 99.52 (94.29% error reduction), lemmatization to 99.17 (68.8% error reduction), XPOS tagging  to 97.38 (46.75% error reduction), UPOS tagging to 98.69 (23.4% error reduction), and LAS to 92.05 (23.56% error reduction).  See official [Stanza performance](https://stanfordnlp.github.io/stanza/performance.html) (evaluated on different data splits) for comparison.
+The above modifications led to some important improvements in the tool's performance in comparison to original Stanza. For standard Slovenian, comparing the CLASSLA-Stanza tool with Stanza on the [SloBENCH benchmark](https://slobench.cjvt.si/leaderboard/view/11), shows relative error reduction (part of the error removed by moving from Stanza to CLASSLA-Stanza) on sentence segmentation to be 98%, on token segmentation 50%, on lemmatization 69%, on morphosyntactic XPOS tagging 65%, and on dependency parsing 34%.
+
+## Citing
+
+If you use this tool, please cite the following papers:
+
+```
+@inproceedings{ljubesic-dobrovoljc-2019-neural,
+    title = "What does Neural Bring? Analysing Improvements in Morphosyntactic Annotation and Lemmatisation of {S}lovenian, {C}roatian and {S}erbian",
+    author = "Ljube{\v{s}}i{\'c}, Nikola  and
+      Dobrovoljc, Kaja",
+    booktitle = "Proceedings of the 7th Workshop on Balto-Slavic Natural Language Processing",
+    month = aug,
+    year = "2019",
+    address = "Florence, Italy",
+    publisher = "Association for Computational Linguistics",
+    url = "https://www.aclweb.org/anthology/W19-3704",
+    doi = "10.18653/v1/W19-3704",
+    pages = "29--34"
+    }
+@misc{terčon2023classlastanza,
+      title={CLASSLA-Stanza: The Next Step for Linguistic Processing of South Slavic Languages},
+      author={Luka Terčon and Nikola Ljubešić},
+      year={2023},
+      eprint={2308.04255},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+
+```
+
 
 ## Installation
 ### pip
 We recommend that you install CLASSLA via pip, the Python package manager. To install, run:
 ```bash
 pip install classla
 ```
@@ -169,37 +240,17 @@
 
 The dependency parsing processor ```depparse``` performs syntactic dependency parsing of sentences following the [Universal Dependencies formalism](https://universaldependencies.org/introduction.html#:~:text=Universal%20Dependencies%20(UD)%20is%20a,from%20a%20language%20typology%20perspective.). It requires the ```tokenize``` and ```pos``` processors.
 
 ### Named entity recognition
 
 The named entity recognition processor ```ner``` identifies named entities in text following the [IOB2](https://en.wikipedia.org/wiki/Inside–outside–beginning_(tagging)) format. It requires only the ```tokenize``` processor.
 
-## Citing
-
-If you use this tool, please cite the following paper:
-
-```
-@inproceedings{ljubesic-dobrovoljc-2019-neural,
-    title = "What does Neural Bring? Analysing Improvements in Morphosyntactic Annotation and Lemmatisation of {S}lovenian, {C}roatian and {S}erbian",
-    author = "Ljube{\v{s}}i{\'c}, Nikola  and
-      Dobrovoljc, Kaja",
-    booktitle = "Proceedings of the 7th Workshop on Balto-Slavic Natural Language Processing",
-    month = aug,
-    year = "2019",
-    address = "Florence, Italy",
-    publisher = "Association for Computational Linguistics",
-    url = "https://www.aclweb.org/anthology/W19-3704",
-    doi = "10.18653/v1/W19-3704",
-    pages = "29--34"
-    }
-```
-
 ## Croatian examples
 
-### Example of standard Croatian 
+### Example of standard Croatian
 
 ```
 >>> import classla
 >>> nlp = classla.Pipeline('hr') # run classla.download('hr') beforehand if necessary
 >>> doc = nlp("Ante Starčević rođen je u Velikom Žitniku.")
 >>> print(doc.to_conll())
 # newpar id = 1
```

### Comparing `classla-2.1/classla/__init__.py` & `classla-2.1.1/classla/__init__.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/charlm.py` & `classla-2.1.1/classla/models/charlm.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/classifier.py` & `classla-2.1.1/classla/models/classifier.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/classifiers/classifier_args.py` & `classla-2.1.1/classla/models/classifiers/classifier_args.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/classifiers/cnn_classifier.py` & `classla-2.1.1/classla/models/classifiers/cnn_classifier.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/classifiers/iterate_test.py` & `classla-2.1.1/classla/models/classifiers/iterate_test.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/beam.py` & `classla-2.1.1/classla/models/common/beam.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/biaffine.py` & `classla-2.1.1/classla/models/common/biaffine.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/char_model.py` & `classla-2.1.1/classla/models/common/char_model.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/chuliu_edmonds.py` & `classla-2.1.1/classla/models/common/chuliu_edmonds.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/constant.py` & `classla-2.1.1/classla/models/common/constant.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/crf.py` & `classla-2.1.1/classla/models/common/crf.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/data.py` & `classla-2.1.1/classla/models/common/data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/doc.py` & `classla-2.1.1/classla/models/common/doc.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/dropout.py` & `classla-2.1.1/classla/models/common/dropout.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/hlstm.py` & `classla-2.1.1/classla/models/common/hlstm.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/loss.py` & `classla-2.1.1/classla/models/common/loss.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/packed_lstm.py` & `classla-2.1.1/classla/models/common/packed_lstm.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/pretrain.py` & `classla-2.1.1/classla/models/common/pretrain.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/seq2seq_model.py` & `classla-2.1.1/classla/models/common/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/seq2seq_modules.py` & `classla-2.1.1/classla/models/common/seq2seq_modules.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/seq2seq_utils.py` & `classla-2.1.1/classla/models/common/seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/trainer.py` & `classla-2.1.1/classla/models/common/trainer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/utils.py` & `classla-2.1.1/classla/models/common/utils.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/common/vocab.py` & `classla-2.1.1/classla/models/common/vocab.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/depparse/data.py` & `classla-2.1.1/classla/models/depparse/data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/depparse/model.py` & `classla-2.1.1/classla/models/depparse/model.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/depparse/scorer.py` & `classla-2.1.1/classla/models/depparse/scorer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/depparse/trainer.py` & `classla-2.1.1/classla/models/depparse/trainer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/identity_lemmatizer.py` & `classla-2.1.1/classla/models/identity_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/lemma/data.py` & `classla-2.1.1/classla/models/lemma/data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/lemma/edit.py` & `classla-2.1.1/classla/models/lemma/edit.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/lemma/trainer.py` & `classla-2.1.1/classla/models/lemma/trainer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/lemma/vocab.py` & `classla-2.1.1/classla/models/lemma/vocab.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/lemmatizer.py` & `classla-2.1.1/classla/models/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/mwt/data.py` & `classla-2.1.1/classla/models/mwt/data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/mwt/trainer.py` & `classla-2.1.1/classla/models/mwt/trainer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/mwt_expander.py` & `classla-2.1.1/classla/models/mwt_expander.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/ner/data.py` & `classla-2.1.1/classla/models/ner/data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/ner/model.py` & `classla-2.1.1/classla/models/ner/model.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/ner/scorer.py` & `classla-2.1.1/classla/models/ner/scorer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/ner/trainer.py` & `classla-2.1.1/classla/models/ner/trainer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/ner/utils.py` & `classla-2.1.1/classla/models/ner/utils.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/ner/vocab.py` & `classla-2.1.1/classla/models/ner/vocab.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/ner_tagger.py` & `classla-2.1.1/classla/models/ner_tagger.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/parser.py` & `classla-2.1.1/classla/models/parser.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/pos/build_xpos_vocab_factory.py` & `classla-2.1.1/classla/models/pos/build_xpos_vocab_factory.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/pos/data.py` & `classla-2.1.1/classla/models/pos/data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/pos/model.py` & `classla-2.1.1/classla/models/pos/model.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/pos/postprocessor.py` & `classla-2.1.1/classla/models/pos/postprocessor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/pos/scorer.py` & `classla-2.1.1/classla/models/pos/scorer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/pos/trainer.py` & `classla-2.1.1/classla/models/pos/trainer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/pos/vocab.py` & `classla-2.1.1/classla/models/pos/vocab.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/pos/xpos_vocab_factory.py` & `classla-2.1.1/classla/models/pos/xpos_vocab_factory.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/srl/data.py` & `classla-2.1.1/classla/models/srl/data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/srl/model.py` & `classla-2.1.1/classla/models/srl/model.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/srl/scorer.py` & `classla-2.1.1/classla/models/srl/scorer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/srl/trainer.py` & `classla-2.1.1/classla/models/srl/trainer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/srl/vocab.py` & `classla-2.1.1/classla/models/srl/vocab.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/srl_tagger.py` & `classla-2.1.1/classla/models/srl_tagger.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/models/tagger.py` & `classla-2.1.1/classla/models/tagger.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/core.py` & `classla-2.1.1/classla/pipeline/core.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/depparse_processor.py` & `classla-2.1.1/classla/pipeline/depparse_processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/external/jieba.py` & `classla-2.1.1/classla/pipeline/external/jieba.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/external/spacy.py` & `classla-2.1.1/classla/pipeline/external/spacy.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/external/sudachipy.py` & `classla-2.1.1/classla/pipeline/external/sudachipy.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/lemma_processor.py` & `classla-2.1.1/classla/pipeline/lemma_processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/mwt_processor.py` & `classla-2.1.1/classla/pipeline/mwt_processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/ner_processor.py` & `classla-2.1.1/classla/pipeline/ner_processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/pos_processor.py` & `classla-2.1.1/classla/pipeline/pos_processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/processor.py` & `classla-2.1.1/classla/pipeline/processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/sentiment_processor.py` & `classla-2.1.1/classla/pipeline/sentiment_processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/srl_processor.py` & `classla-2.1.1/classla/pipeline/srl_processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/pipeline/tokenize_processor.py` & `classla-2.1.1/classla/pipeline/tokenize_processor.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/protobuf/CoreNLP_pb2.py` & `classla-2.1.1/classla/protobuf/CoreNLP_pb2.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/protobuf/__init__.py` & `classla-2.1.1/classla/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/resources/common.py` & `classla-2.1.1/classla/resources/common.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/resources/installation.py` & `classla-2.1.1/classla/resources/installation.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/resources/prepare_resources.py` & `classla-2.1.1/classla/resources/prepare_resources.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/server/__init__.py` & `classla-2.1.1/classla/server/__init__.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/server/annotator.py` & `classla-2.1.1/classla/server/annotator.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/server/client.py` & `classla-2.1.1/classla/server/client.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/server/main.py` & `classla-2.1.1/classla/server/main.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/server/semgrex.py` & `classla-2.1.1/classla/server/semgrex.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/conll.py` & `classla-2.1.1/classla/utils/conll.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/conll18_ud_eval.py` & `classla-2.1.1/classla/utils/conll18_ud_eval.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/contract_mwt.py` & `classla-2.1.1/classla/utils/contract_mwt.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/helper_func.py` & `classla-2.1.1/classla/utils/helper_func.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/obeliks.py` & `classla-2.1.1/classla/utils/obeliks.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/postprocess_vietnamese_tokenizer_data.py` & `classla-2.1.1/classla/utils/postprocess_vietnamese_tokenizer_data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/prepare_ner_data.py` & `classla-2.1.1/classla/utils/prepare_ner_data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/prepare_tokenizer_data.py` & `classla-2.1.1/classla/utils/prepare_tokenizer_data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla/utils/reldi.py` & `classla-2.1.1/classla/utils/reldi.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/classla.egg-info/PKG-INFO` & `classla-2.1.1/classla.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classla
-Version: 2.1
+Version: 2.1.1
 Summary: Adapted Stanford NLP Python Library with improvements for specific languages.
 Home-page: https://github.com/clarinsi/classla-stanfordnlp.git
 Author: CLARIN.SI
 Author-email: info@clarin.si
 License: Apache License 2.0
 Keywords: natural-language-processing nlp natural-language-understanding stanford-nlp deep-learning clarinsi
 Classifier: Development Status :: 4 - Beta
@@ -18,33 +18,44 @@
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy==1.23.0
+Requires-Dist: protobuf==4.21.2
+Requires-Dist: requests==2.28.0
+Requires-Dist: torch==1.12.0
+Requires-Dist: tqdm==4.62.3
+Requires-Dist: obeliks==1.1.6
+Requires-Dist: reldi-tokeniser==1.0.3
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # A [CLASSLA](http://www.clarin.si/info/k-centre/) Fork of [Stanza](https://github.com/stanfordnlp/stanza) for Processing Slovenian, Croatian, Serbian, Macedonian and Bulgarian
 
 ## Description
 
 This pipeline allows for processing of standard Slovenian, Croatian, Serbian and Bulgarian on the levels of
 
 - tokenization and sentence splitting
 - part-of-speech tagging
 - lemmatization
 - dependency parsing
 - named entity recognition
 
-It also allows for (alpha) processing of standard Macedonian on the levels of 
+It also allows for processing of standard Macedonian on the levels of
 
 - tokenization and sentence splitting
 - part-of-speech tagging
 - lemmatization
 
 Finally, it allows for processing of non-standard (Internet) Slovenian, Croatian and Serbian on the same levels as standard language (all models are tailored to non-standard language except for dependency parsing where the standard module is used).
 
@@ -60,15 +71,45 @@
 - morphosyntactic tagging models based on larger quantities of training data than is available in UD (training data that are morphosyntactically tagged, but not UD-parsed)
 - lemmatization models based on larger quantities of training data than is available in UD (training data that are lemmatized, but not UD-parsed)
 - optional JOS-project-based parsing of Slovenian (usage documented [here](https://github.com/clarinsi/classla/blob/master/README.superuser.md#jos-dependency-parsing-system))
 - named entity recognition models for all languages except Macedonian (Stanza does not cover named entity recognition for any of the languages supported by classla)
 - Macedonian models (Macedonian is not available in UD yet)
 - non-standard models for Croatian, Slovenian, Serbian (there is no UD data for these varieties)
 
-The above modifications led to some important improvements in the tool’s performance in comparison to original Stanza. For standard Slovenian, for example, running the full classla pipeline increases sentence segmentation F1 scores to 99.52 (94.29% error reduction), lemmatization to 99.17 (68.8% error reduction), XPOS tagging  to 97.38 (46.75% error reduction), UPOS tagging to 98.69 (23.4% error reduction), and LAS to 92.05 (23.56% error reduction).  See official [Stanza performance](https://stanfordnlp.github.io/stanza/performance.html) (evaluated on different data splits) for comparison.
+The above modifications led to some important improvements in the tool's performance in comparison to original Stanza. For standard Slovenian, comparing the CLASSLA-Stanza tool with Stanza on the [SloBENCH benchmark](https://slobench.cjvt.si/leaderboard/view/11), shows relative error reduction (part of the error removed by moving from Stanza to CLASSLA-Stanza) on sentence segmentation to be 98%, on token segmentation 50%, on lemmatization 69%, on morphosyntactic XPOS tagging 65%, and on dependency parsing 34%.
+
+## Citing
+
+If you use this tool, please cite the following papers:
+
+```
+@inproceedings{ljubesic-dobrovoljc-2019-neural,
+    title = "What does Neural Bring? Analysing Improvements in Morphosyntactic Annotation and Lemmatisation of {S}lovenian, {C}roatian and {S}erbian",
+    author = "Ljube{\v{s}}i{\'c}, Nikola  and
+      Dobrovoljc, Kaja",
+    booktitle = "Proceedings of the 7th Workshop on Balto-Slavic Natural Language Processing",
+    month = aug,
+    year = "2019",
+    address = "Florence, Italy",
+    publisher = "Association for Computational Linguistics",
+    url = "https://www.aclweb.org/anthology/W19-3704",
+    doi = "10.18653/v1/W19-3704",
+    pages = "29--34"
+    }
+@misc{terčon2023classlastanza,
+      title={CLASSLA-Stanza: The Next Step for Linguistic Processing of South Slavic Languages},
+      author={Luka Terčon and Nikola Ljubešić},
+      year={2023},
+      eprint={2308.04255},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+
+```
+
 
 ## Installation
 ### pip
 We recommend that you install CLASSLA via pip, the Python package manager. To install, run:
 ```bash
 pip install classla
 ```
@@ -199,37 +240,17 @@
 
 The dependency parsing processor ```depparse``` performs syntactic dependency parsing of sentences following the [Universal Dependencies formalism](https://universaldependencies.org/introduction.html#:~:text=Universal%20Dependencies%20(UD)%20is%20a,from%20a%20language%20typology%20perspective.). It requires the ```tokenize``` and ```pos``` processors.
 
 ### Named entity recognition
 
 The named entity recognition processor ```ner``` identifies named entities in text following the [IOB2](https://en.wikipedia.org/wiki/Inside–outside–beginning_(tagging)) format. It requires only the ```tokenize``` processor.
 
-## Citing
-
-If you use this tool, please cite the following paper:
-
-```
-@inproceedings{ljubesic-dobrovoljc-2019-neural,
-    title = "What does Neural Bring? Analysing Improvements in Morphosyntactic Annotation and Lemmatisation of {S}lovenian, {C}roatian and {S}erbian",
-    author = "Ljube{\v{s}}i{\'c}, Nikola  and
-      Dobrovoljc, Kaja",
-    booktitle = "Proceedings of the 7th Workshop on Balto-Slavic Natural Language Processing",
-    month = aug,
-    year = "2019",
-    address = "Florence, Italy",
-    publisher = "Association for Computational Linguistics",
-    url = "https://www.aclweb.org/anthology/W19-3704",
-    doi = "10.18653/v1/W19-3704",
-    pages = "29--34"
-    }
-```
-
 ## Croatian examples
 
-### Example of standard Croatian 
+### Example of standard Croatian
 
 ```
 >>> import classla
 >>> nlp = classla.Pipeline('hr') # run classla.download('hr') beforehand if necessary
 >>> doc = nlp("Ante Starčević rođen je u Velikom Žitniku.")
 >>> print(doc.to_conll())
 # newpar id = 1
```

### Comparing `classla-2.1/classla.egg-info/SOURCES.txt` & `classla-2.1.1/classla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classla-2.1/setup.py` & `classla-2.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,28 +61,30 @@
         'Topic :: Software Development :: Libraries',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
 
     # What does your project relate to?
     keywords='natural-language-processing nlp natural-language-understanding stanford-nlp deep-learning clarinsi',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages=packages,
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['numpy==1.23.0', 'protobuf==4.21.2', 'requests==2.28.0', 'torch==1.12.0', 'tqdm==4.62.3', 'obeliks==1.1.6', 'reldi-tokeniser==1.0.2'],
+    install_requires=['numpy==1.23.0', 'protobuf==4.21.2', 'requests==2.28.0', 'torch==1.12.0', 'tqdm==4.62.3', 'obeliks==1.1.6', 'reldi-tokeniser==1.0.3'],
 
     # List required Python versions
     python_requires='>=3.6',
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
```

### Comparing `classla-2.1/tests/__init__.py` & `classla-2.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_client.py` & `classla-2.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_data_conversion.py` & `classla-2.1.1/tests/test_data_conversion.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_data_objects.py` & `classla-2.1.1/tests/test_data_objects.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_decorators.py` & `classla-2.1.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_depparse.py` & `classla-2.1.1/tests/test_depparse.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_depparse_data.py` & `classla-2.1.1/tests/test_depparse_data.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_doc.py` & `classla-2.1.1/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_english_pipeline.py` & `classla-2.1.1/tests/test_english_pipeline.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_installation.py` & `classla-2.1.1/tests/test_installation.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_lemmatizer.py` & `classla-2.1.1/tests/test_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_mwt_expander.py` & `classla-2.1.1/tests/test_mwt_expander.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_ner_tagger.py` & `classla-2.1.1/tests/test_ner_tagger.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_pretrain.py` & `classla-2.1.1/tests/test_pretrain.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_protobuf.py` & `classla-2.1.1/tests/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_requirements.py` & `classla-2.1.1/tests/test_requirements.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_semgrex.py` & `classla-2.1.1/tests/test_semgrex.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_server_misc.py` & `classla-2.1.1/tests/test_server_misc.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_server_request.py` & `classla-2.1.1/tests/test_server_request.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_server_start.py` & `classla-2.1.1/tests/test_server_start.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_tagger.py` & `classla-2.1.1/tests/test_tagger.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_tokenizer.py` & `classla-2.1.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests/test_utils.py` & `classla-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/__init__.py` & `classla-2.1.1/tests_classla/__init__.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_downloads.py` & `classla-2.1.1/tests_classla/test_downloads.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_lemmatizer.py` & `classla-2.1.1/tests_classla/test_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_ner.py` & `classla-2.1.1/tests_classla/test_ner.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_parser.py` & `classla-2.1.1/tests_classla/test_parser.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_readme_examples.py` & `classla-2.1.1/tests_classla/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_slovenian_pipeline.py` & `classla-2.1.1/tests_classla/test_slovenian_pipeline.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_srl.py` & `classla-2.1.1/tests_classla/test_srl.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_tagger.py` & `classla-2.1.1/tests_classla/test_tagger.py`

 * *Files identical despite different names*

### Comparing `classla-2.1/tests_classla/test_tokenizer.py` & `classla-2.1.1/tests_classla/test_tokenizer.py`

 * *Files identical despite different names*

