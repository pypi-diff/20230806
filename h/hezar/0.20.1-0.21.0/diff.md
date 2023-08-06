# Comparing `tmp/hezar-0.20.1.tar.gz` & `tmp/hezar-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.20.1.tar", max compression
+gzip compressed data, was "hezar-0.21.0.tar", max compression
```

## Comparing `hezar-0.20.1.tar` & `hezar-0.21.0.tar`

### file list

```diff
@@ -1,93 +1,95 @@
--rw-r--r--   0        0        0     1065 2023-08-05 10:51:49.803922 hezar-0.20.1/LICENSE
--rw-r--r--   0        0        0     4750 2023-08-05 10:51:49.803922 hezar-0.20.1/README.md
--rw-r--r--   0        0        0      260 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/__init__.py
--rw-r--r--   0        0        0     5336 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/builders.py
--rw-r--r--   0        0        0    11576 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/configs.py
--rw-r--r--   0        0        0     2072 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/__init__.py
--rw-r--r--   0        0        0     6365 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/data_collators.py
--rw-r--r--   0        0        0      320 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1758 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4545 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3653 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     3581 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0       26 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      273 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1614 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1686 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1644 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11719 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/model.py
--rw-r--r--   0        0        0     1434 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/model_outputs.py
--rw-r--r--   0        0        0      152 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3981 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     4142 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      877 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0       47 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text2text/__init__.py
--rw-r--r--   0        0        0       89 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text2text/t5/__init__.py
--rw-r--r--   0        0        0     3848 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text2text/t5/t5_text2text.py
--rw-r--r--   0        0        0      764 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text2text/t5/t5_text2text_config.py
--rw-r--r--   0        0        0      240 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3540 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3676 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3819 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0      155 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     4119 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     3633 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      324 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4965 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    19472 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8828 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2644 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2282 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    18229 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      164 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5615 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3660 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/logging.py
--rw-r--r--   0        0        0      936 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     1648 2023-08-05 10:51:49.811922 hezar-0.20.1/pyproject.toml
--rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 hezar-0.20.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-06 20:15:26.873012 hezar-0.21.0/LICENSE
+-rw-r--r--   0        0        0     4750 2023-08-06 20:15:26.873012 hezar-0.21.0/README.md
+-rw-r--r--   0        0        0      260 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5336 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/builders.py
+-rw-r--r--   0        0        0    11587 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/configs.py
+-rw-r--r--   0        0        0     2072 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6365 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      320 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1771 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4545 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3653 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     3581 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0       26 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4804 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3270 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3301 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      273 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1656 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1728 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1686 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11774 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/model.py
+-rw-r--r--   0        0        0     1434 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0      152 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     4076 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     4184 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/text2text/__init__.py
+-rw-r--r--   0        0        0       89 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/text2text/t5/__init__.py
+-rw-r--r--   0        0        0     3941 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/text2text/t5/t5_text2text.py
+-rw-r--r--   0        0        0      764 2023-08-06 20:15:26.873012 hezar-0.21.0/hezar/models/text2text/t5/t5_text2text_config.py
+-rw-r--r--   0        0        0      240 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3710 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     2939 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     4165 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0     1733 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_classification/text_classification.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     4494 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     3652 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      324 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4965 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    19486 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8828 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2644 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2282 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    18229 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      190 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5615 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0      531 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     3666 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0      936 2023-08-06 20:15:26.877012 hezar-0.21.0/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     1648 2023-08-06 20:15:26.877012 hezar-0.21.0/pyproject.toml
+-rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 hezar-0.21.0/PKG-INFO
```

### Comparing `hezar-0.20.1/LICENSE` & `hezar-0.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/README.md` & `hezar-0.21.0/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/builders.py` & `hezar-0.21.0/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/configs.py` & `hezar-0.21.0/hezar/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from omegaconf import DictConfig, OmegaConf
 
 from .constants import DEFAULT_MODEL_CONFIG_FILE, HEZAR_CACHE_DIR, ConfigType, TaskType
 from .utils import get_logger, get_module_config_class
 
-
 __all__ = [
     "Config",
     "ModelConfig",
     "PreprocessorConfig",
     "TrainerConfig",
     "DatasetConfig",
     "EmbeddingConfig",
@@ -119,15 +118,15 @@
     def load(
         cls,
         hub_or_local_path: Union[str, os.PathLike],
         filename: Optional[str] = None,
         subfolder: Optional[str] = None,
         repo_type=None,
         **kwargs,
-    ):
+    ) -> "Config":
         """
         Load config from Hub or locally if it already exists on disk (handled by HfApi)
 
         Args:
             hub_or_local_path: Local or Hub path for the config
             filename: Configuration filename
             subfolder: Optional subfolder path where the config is in
```

### Comparing `hezar-0.20.1/hezar/constants.py` & `hezar-0.21.0/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/data/data_collators.py` & `hezar-0.21.0/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/data/datasets/dataset.py` & `hezar-0.21.0/hezar/data/datasets/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     @classmethod
     def load(
         cls,
         hub_path: Union[str, os.PathLike],
         config_filename: Optional[str] = None,
         split: Optional[Union[str, SplitType]] = None,
         **kwargs,
-    ):
+    ) -> "Dataset":
         """
         Load the dataset from hub.
 
         Args:
             hub_path: Path to dataset from hub or locally
             config_filename: Dataset config file name
             split: Dataset split, defaults to "train"
```

### Comparing `hezar-0.20.1/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.21.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.21.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.21.0/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/data/utils/data_utils.py` & `hezar-0.21.0/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/embeddings/embedding.py` & `hezar-0.21.0/hezar/embeddings/embedding.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from ..constants import (
     DEFAULT_EMBEDDING_CONFIG_FILE,
     DEFAULT_EMBEDDING_FILE,
     DEFAULT_EMBEDDING_SUBFOLDER,
 )
 from ..utils import get_logger
 
-
 logger = get_logger(__name__)
 
 
 class Embedding:
     """
     Base class for all embeddings.
     """
     filename = DEFAULT_EMBEDDING_FILE
+    vectors_filename = None
     config_filename = DEFAULT_EMBEDDING_CONFIG_FILE
     subfolder = DEFAULT_EMBEDDING_SUBFOLDER
 
     def __init__(self, config: EmbeddingConfig, **kwargs):
         self.config = config.update(kwargs)
         self.model = self.build()
 
@@ -55,84 +55,99 @@
     @classmethod
     def load(
         cls,
         hub_or_local_path,
         config_filename=None,
         subfolder=None,
         **kwargs,
-    ):
+    ) -> "Embedding":
         config_filename = config_filename or cls.config_filename
         subfolder = subfolder or cls.subfolder
 
         config = EmbeddingConfig.load(hub_or_local_path, filename=config_filename, subfolder=subfolder, **kwargs)
         config.pretrained_path = hub_or_local_path
 
         embedding = build_embedding(config.name, config, **kwargs)
 
         return embedding
 
     def save(
         self,
         path: Union[str, os.PathLike],
         filename: str = None,
+        subfolder: str = None,
         save_config: bool = True,
         config_filename: str = None,
     ):
         raise NotImplementedError
 
     def push_to_hub(
         self,
         repo_id,
         commit_message=None,
         subfolder=None,
         filename=None,
+        vectors_filename=None,
         config_filename=None,
         private=False,
     ):
         subfolder = subfolder or self.subfolder
         filename = filename or self.filename
+        vectors_filename = vectors_filename or self.vectors_filename
         config_filename = config_filename or self.config_filename
 
         api = HfApi()
         # create remote repo
         api.create_repo(repo_id, exist_ok=True)
         # save to tmp and prepare for push
         cache_path = tempfile.mkdtemp()
         # save embedding model file
-        embedding_save_dir = os.path.join(cache_path, subfolder)
+        embedding_save_dir = os.path.join(cache_path)
         os.makedirs(embedding_save_dir, exist_ok=True)
 
         if commit_message is None:
             commit_message = "Hezar: Upload embedding and config"
 
-        self.save(embedding_save_dir, filename, save_config=False)
+        self.save(embedding_save_dir, filename, subfolder=subfolder, save_config=False)
 
         self.config.push_to_hub(
             repo_id,
             config_filename,
             subfolder=subfolder,
             repo_type="model",
             private=private,
             commit_message=commit_message,
         )
 
         api.upload_file(
             repo_id=repo_id,
-            path_or_fileobj=os.path.join(embedding_save_dir, filename),
+            path_or_fileobj=os.path.join(embedding_save_dir, subfolder, filename),
             repo_type="model",
             path_in_repo=f"{subfolder}/{filename}",
             commit_message=commit_message,
         )
-
         logger.info(
             f"Uploaded: {self.__class__.__name__}(name={self.config.name})`"
             f" --> "
             f"{os.path.join(repo_id, subfolder, filename)}"
         )
 
+        api.upload_file(
+            repo_id=repo_id,
+            path_or_fileobj=os.path.join(embedding_save_dir, subfolder, vectors_filename),
+            repo_type="model",
+            path_in_repo=f"{subfolder}/{vectors_filename}",
+            commit_message=commit_message,
+        )
+        logger.info(
+            f"Uploaded: {self.__class__.__name__}(name={self.config.name})`"
+            f" --> "
+            f"{os.path.join(repo_id, subfolder, vectors_filename)}"
+        )
+
     def torch_embedding(self):
         import torch
         weights = torch.FloatTensor(self.vectors)
         embedding_layer = torch.nn.Embedding.from_pretrained(weights)
         return embedding_layer
 
     @property
```

### Comparing `hezar-0.20.1/hezar/embeddings/fasttext.py` & `hezar-0.21.0/hezar/embeddings/fasttext.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     cbow_mean = 1
     epochs = 5
     pretrained_path: str = None
 
 
 @register_embedding("fasttext", config_class=FastTextConfig)
 class FastText(Embedding):
-    filename = "embedding.model"
-    array_filename = "embedding.model.wv.vectors_ngrams.npy"
+    filename = "embedding.bin"
+    vectors_filename = "embedding.bin.wv.vectors.npy"
 
     def __init__(self, config: FastTextConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.model = self.build()
 
     def build(self):
         pretrained_path = self.config.get("pretrained_path")
@@ -80,24 +80,27 @@
             total_words=self.model.corpus_total_words,
         )
 
     def save(
         self,
         path: Union[str, os.PathLike],
         filename: str = None,
+        subfolder: str = None,
         save_config: bool = True,
         config_filename: str = None,
     ):
         filename = filename or self.filename
         config_filename = config_filename or self.config_filename
+        subfolder = subfolder or self.subfolder
 
-        os.makedirs(path, exist_ok=True)
-        self.config.save(path, config_filename)
+        save_dir = os.path.join(path, subfolder)
+        os.makedirs(save_dir, exist_ok=True)
+        self.config.save(path, config_filename, subfolder=subfolder)
 
-        self.model.save(os.path.join(path, filename))
+        self.model.save(os.path.join(save_dir, filename))
 
     @property
     def word_vectors(self):
         return self.model.wv
 
     @property
     def vectors(self):
```

### Comparing `hezar-0.20.1/hezar/embeddings/word2vec.py` & `hezar-0.21.0/hezar/embeddings/word2vec.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     train_algorithm: Literal["skipgram", "cbow"] = "skipgram"
     save_format: Literal["binary", "text"] = "binary"
     pretrained_path: str = None
 
 
 @register_embedding("word2vec", config_class=Word2VecConfig)
 class Word2Vec(Embedding):
+    vectors_filename = f"{Embedding.filename}.wv.vectors.npy"
+
     def __init__(self, config: Word2VecConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.model = self.build()
 
     def build(self):
         pretrained_path = self.config.get("pretrained_path")
         if pretrained_path:
@@ -78,24 +80,27 @@
             total_words=self.model.corpus_total_words,
         )
 
     def save(
         self,
         path: Union[str, os.PathLike],
         filename: str = None,
+        subfolder: str = None,
         save_config: bool = True,
         config_filename: str = None,
     ):
         filename = filename or self.filename
         config_filename = config_filename or self.config_filename
+        subfolder = subfolder or self.subfolder
 
-        os.makedirs(path, exist_ok=True)
-        self.config.save(path, config_filename)
+        save_dir = os.path.join(path, subfolder)
+        os.makedirs(save_dir, exist_ok=True)
+        self.config.save(path, config_filename, subfolder=subfolder)
 
-        self.model.save(os.path.join(path, filename))
+        self.model.save(os.path.join(save_dir, filename))
 
     @property
     def word_vectors(self):
         return self.model.wv
 
     @property
     def vectors(self):
```

### Comparing `hezar-0.20.1/hezar/metrics/f1.py` & `hezar-0.21.0/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/metrics/metric.py` & `hezar-0.21.0/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/metrics/recall.py` & `hezar-0.21.0/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/metrics/seqeval.py` & `hezar-0.21.0/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.21.0/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from ....models import Model
 from ....registry import register_model
 from .bert_lm_config import BertLMConfig
 
 
 @register_model("bert_lm", config_class=BertLMConfig)
 class BertLM(Model):
+    tokenizer_name = "wordpiece_tokenizer"
+
     def __init__(self, config, **kwargs):
         super().__init__(config=config, **kwargs)
         self.bert = BertModel(BertConfig(**self.config))
 
     def forward(self, inputs, **kwargs):
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
@@ -28,15 +30,15 @@
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
         if "text_normalizer" in self.preprocessor:
             normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
-        tokenizer = self.preprocessor["wordpiece_tokenizer"]
+        tokenizer = self.preprocessor[self.tokenizer_name]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         hidden_states = inputs.get("hidden_states", None)
         attentions = inputs.get("attentions", None)
         outputs = {
```

### Comparing `hezar-0.20.1/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.21.0/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.21.0/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from ....models import Model
 from ....registry import register_model
 from .distilbert_lm_config import DistilBertLMConfig
 
 
 @register_model("distilbert_lm", config_class=DistilBertLMConfig)
 class DistilBertLM(Model):
+    tokenizer_name = "wordpiece_tokenizer"
+
     def __init__(self, config, **kwargs):
         super().__init__(config=config, **kwargs)
         self.distilbert = DistilBertModel(DistilBertConfig(**self.config))
 
     def forward(self, inputs, **kwargs):
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
@@ -28,15 +30,15 @@
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
         if "text_normalizer" in self.preprocessor:
             normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
-        tokenizer = self.preprocessor["wordpiece_tokenizer"]
+        tokenizer = self.preprocessor[self.tokenizer_name]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         hidden_states = inputs.get("hidden_states", None)
         attentions = inputs.get("attentions", None)
         outputs = {
```

### Comparing `hezar-0.20.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.21.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.21.0/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from ....models import Model
 from ....registry import register_model
 from .roberta_lm_config import RobertaLMConfig
 
 
 @register_model("roberta_lm", config_class=RobertaLMConfig)
 class RobertaLM(Model):
+    tokenizer_name = "bpe_tokenizer"
+
     def __init__(self, config, **kwargs):
         super().__init__(config=config, **kwargs)
         self.roberta = RobertaModel(RobertaConfig(**self.config))
 
     def forward(self, inputs, **kwargs):
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
@@ -28,15 +30,15 @@
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
         if "text_normalizer" in self.preprocessor:
             normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
-        tokenizer = self.preprocessor["bpe_tokenizer"]
+        tokenizer = self.preprocessor[self.tokenizer_name]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         hidden_states = inputs.get("hidden_states", None)
         attentions = inputs.get("attentions", None)
         outputs = {
```

### Comparing `hezar-0.20.1/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.21.0/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/model.py` & `hezar-0.21.0/hezar/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 Examples:
     >>> # Load from hub
     >>> from hezar import Model
     >>> model = Model.load("hezarai/bert-base-fa")
 """
 import os
 import tempfile
-from abc import abstractmethod
 from collections import OrderedDict
-from typing import Any, Dict, Mapping, Optional, Union
+from typing import Any, Dict, Mapping, Optional, Union, List
 
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from torch import nn
 
 from ..builders import build_model
 from ..configs import ModelConfig
 from ..constants import DEFAULT_MODEL_CONFIG_FILE, DEFAULT_MODEL_FILE, HEZAR_CACHE_DIR
 from ..preprocessors import Preprocessor, PreprocessorsContainer
 from ..utils import get_logger
 
-
 __all__ = [
     "Model",
     "ModelConfig",
 ]
 
 logger = get_logger(__name__)
 
@@ -54,15 +52,15 @@
         hub_or_local_path: Union[str, os.PathLike],
         load_locally: Optional[bool] = False,
         load_preprocessor: Optional[bool] = True,
         model_filename: Optional[str] = None,
         config_filename: Optional[str] = None,
         save_path: Optional[Union[str, os.PathLike]] = None,
         **kwargs,
-    ):
+    ) -> "Model":
         """
         Load the model from local path or hub.
 
         It's recommended to actually use this method with :class:`hezar.Model` rather than any other model class
         unless you actually know that the class is the same as the one on the Hub, because the output will always be
         the one specified on the Hub!
 
@@ -236,15 +234,14 @@
         logger.info(
             f"Uploaded: "
             f"`{self.__class__.__name__}(name={self.config.name})`"
             f" --> "
             f"`{os.path.join(repo_id, filename)}`"
         )
 
-    @abstractmethod
     def forward(self, inputs, **kwargs) -> Dict:
         """
         Forward inputs through the model and return logits, etc.
 
         Args:
             inputs: The required inputs for the model forward
 
@@ -276,15 +273,15 @@
 
         Returns:
             Processed model output values and converted to human-readable results
         """
         return inputs
 
     @torch.inference_mode()
-    def predict(self, inputs, **kwargs) -> Dict:
+    def predict(self, inputs, **kwargs) -> Union[Dict, List[Dict]]:
         """
         Perform an end-to-end prediction on raw inputs.
 
         Args:
             inputs: Raw inputs e.g, a list of texts, path to images, etc.
 
         Returns:
@@ -302,19 +299,19 @@
         return processed_outputs
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     @property
-    def preprocessor(self):
+    def preprocessor(self) -> PreprocessorsContainer:
         return self._preprocessor
 
     @preprocessor.setter
-    def preprocessor(self, value):
+    def preprocessor(self, value: Union[Preprocessor, PreprocessorsContainer]):
         if isinstance(value, Preprocessor):
             preprocessor = PreprocessorsContainer()
             preprocessor[value.config.name] = value
         elif isinstance(value, Mapping):
             preprocessor = PreprocessorsContainer(**value)
         elif value is None:
             preprocessor = None
```

### Comparing `hezar-0.20.1/hezar/models/model_outputs.py` & `hezar-0.21.0/hezar/models/model_outputs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.21.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from ....models import Model
 from ....registry import register_model
 from .bert_sequence_labeling_config import BertSequenceLabelingConfig
 
 
 @register_model("bert_sequence_labeling", BertSequenceLabelingConfig)
 class BertSequenceLabeling(Model):
+    """
+    BERT model for sequence labeling
+    """
+    tokenizer_name = "wordpiece_tokenizer"
+
     def __init__(self, config: BertSequenceLabelingConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.bert = BertModel(self._build_inner_config())
         classifier_dropout = (
             config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
         )
         self.dropout = nn.Dropout(classifier_dropout)
@@ -66,15 +71,15 @@
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
         if "text_normalizer" in self.preprocessor:
             normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
-        tokenizer = self.preprocessor["wordpiece_tokenizer"]
+        tokenizer = self.preprocessor[self.tokenizer_name]
         inputs = tokenizer(
             inputs,
             return_word_ids=True,
             return_tokens=True,
             padding=True,
             truncation=True,
             return_tensors="pt",
```

### Comparing `hezar-0.20.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.21.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.21.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from ....models import Model
 from ....registry import register_model
 from .distilbert_sequence_labeling_config import DistilBertSequenceLabelingConfig
 
 
 @register_model("distilbert_sequence_labeling", DistilBertSequenceLabelingConfig)
 class DistilBertSequenceLabeling(Model):
+    tokenizer_name = "wordpiece_tokenizer"
+
     def __init__(self, config: DistilBertSequenceLabelingConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.distilbert = DistilBertModel(self._build_inner_config())
         classifier_dropout = (
             config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
         )
         self.dropout = nn.Dropout(classifier_dropout)
@@ -67,15 +69,15 @@
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
         if "text_normalizer" in self.preprocessor:
             normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
-        tokenizer = self.preprocessor["wordpiece_tokenizer"]
+        tokenizer = self.preprocessor[self.tokenizer_name]
         inputs = tokenizer(
             inputs,
             return_word_ids=True,
             return_tokens=True,
             padding=True,
             truncation=True,
             return_tensors="pt",
```

### Comparing `hezar-0.20.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.21.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/text2text/t5/t5_text2text.py` & `hezar-0.21.0/hezar/models/text2text/t5/t5_text2text.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from ....models import Model
 from ....registry import register_model
 from .t5_text2text_config import T5Text2TextConfig
 
 
 @register_model("t5_text2text", config_class=T5Text2TextConfig)
 class T5Text2Text(Model):
+    """
+    T5 for text to text generation
+    """
+    tokenizer_name = "sentencepiece_unigram_tokenizer"
+
     def __init__(self, config: T5Text2TextConfig, **kwargs):
         super().__init__(config=config, **kwargs)
 
         self.t5 = T5ForConditionalGeneration(T5Config(**self.config))
 
     def forward(self, inputs, **kwargs) -> Dict:
         input_ids = inputs.get("token_ids")
@@ -63,15 +68,15 @@
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
         if "text_normalizer" in self.preprocessor:
             normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
-        tokenizer = self.preprocessor["sentencepiece_unigram_tokenizer"]
+        tokenizer = self.preprocessor[self.tokenizer_name]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         records = []
         tokenizer = self.preprocessor["sentencepiece_unigram_tokenizer"]
         for output_ids in inputs["output_ids"][0]:
```

### Comparing `hezar-0.20.1/hezar/models/text2text/t5/t5_text2text_config.py` & `hezar-0.21.0/hezar/models/text2text/t5/t5_text2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.21.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 A BERT model for text classification built using HuggingFace Transformers
 """
 from typing import Dict, List, Union
 
 from torch import nn
 from transformers import BertConfig, BertModel
 
-from ....models import Model
+from ..text_classification import TextClassificationModel
 from ....registry import register_model
 from .bert_text_classification_config import BertTextClassificationConfig
 
 
 @register_model(model_name="bert_text_classification", config_class=BertTextClassificationConfig)
-class BertTextClassification(Model):
+class BertTextClassification(TextClassificationModel):
     """
     A standard 🤗Transformers Bert model for text classification
 
     Args:
         config: The whole model config including arguments needed for the inner 🤗Transformers model.
     """
+    tokenizer_name = "wordpiece_tokenizer"
+
     def __init__(self, config: BertTextClassificationConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.bert = BertModel(self._build_inner_config())
         classifier_dropout = (
             self.config.classifier_dropout if self.config.classifier_dropout is not None
             else self.config.hidden_dropout_prob
         )
@@ -36,51 +38,43 @@
             self.config.num_labels = len(self.config.id2label)
         bert_config = BertConfig(**self.config)
         return bert_config
 
     def forward(self, inputs, **kwargs) -> Dict:
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
+        token_types_ids = inputs.get("token_type_ids", None) or kwargs.get("token_type_ids", None)
+        position_ids = inputs.get("position_ids", None) or kwargs.get("position_ids", None)
         head_mask = inputs.get("head_mask", None)
         inputs_embeds = inputs.get("inputs_embeds", None)
+        encoder_hidden_states = inputs.get("encoder_hidden_states", None) or kwargs.get("encoder_hidden_states", None)
+        encoder_attention_mask = inputs.get("encoder_attention_mask", None) or kwargs.get("encoder_attention_mask", None)
+        past_key_values = inputs.get("past_key_values", None) or kwargs.get("past_key_values", None)
+        use_cache = inputs.get("use_cache", None) or kwargs.get("use_cache", None)
         output_attentions = inputs.get("output_attentions", None)
         output_hidden_states = inputs.get("output_hidden_states", None)
+        return_dict = inputs.get("return_dict", None) or kwargs.get("return_dict", None)
 
         lm_outputs = self.bert(
             input_ids,
             attention_mask=attention_mask,
+            token_type_ids=token_types_ids,
+            position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
+            encoder_hidden_states=encoder_hidden_states,
+            encoder_attention_mask=encoder_attention_mask,
+            past_key_values=past_key_values,
+            use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
-            **kwargs,
+            return_dict=return_dict,
         )
         pooled_output = lm_outputs[1]
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
         outputs = {
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
         }
         return outputs
-
-    def preprocess(self, inputs: Union[str, List[str]], **kwargs):
-        if isinstance(inputs, str):
-            inputs = [inputs]
-        if "text_normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["text_normalizer"]
-            inputs = normalizer(inputs)
-        tokenizer = self.preprocessor["wordpiece_tokenizer"]
-        inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
-        return inputs
-
-    def post_process(self, inputs, **kwargs) -> Dict:
-        logits = inputs["logits"]
-        predictions = logits.argmax(1)
-        predictions_probs = logits.softmax(1).max(1)
-        outputs = {"labels": [], "probs": []}
-        for prediction, prob in zip(predictions, predictions_probs):
-            label = self.config.id2label[prediction.item()]
-            outputs["labels"].append(label)
-            outputs["probs"].append(prob.item())
-        return outputs
```

### Comparing `hezar-0.20.1/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.21.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.21.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 A DistilBERT model for text classification built using HuggingFace Transformers
 """
-from typing import Dict, List, Union
+from typing import Dict
 
 from torch import nn
 from transformers import DistilBertConfig, DistilBertModel
 
-from ....models import Model
-from ....registry import register_model
 from .distilbert_text_classification_config import DistilBertTextClassificationConfig
+from ..text_classification import TextClassificationModel
+from ....registry import register_model
 
 
 @register_model(model_name="distilbert_text_classification", config_class=DistilBertTextClassificationConfig)
-class DistilBertTextClassification(Model):
+class DistilBertTextClassification(TextClassificationModel):
     """
     A standard 🤗Transformers DistilBert model for text classification
 
     Args:
         config: The whole model config including arguments needed for the inner 🤗Transformers model.
     """
+    tokenizer_name = "wordpiece_tokenizer"
 
     def __init__(self, config: DistilBertTextClassificationConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.distilbert = DistilBertModel(self._build_inner_config())
         self.pre_classifier = nn.Linear(self.config.dim, self.config.dim)
         self.classifier = nn.Linear(self.config.dim, self.config.num_labels)
         self.dropout = nn.Dropout(self.config.seq_classif_dropout)
@@ -38,51 +39,31 @@
     def forward(self, inputs, **kwargs) -> Dict:
         input_ids = inputs.get("token_ids")
         attention_mask = inputs.get("attention_mask", None)
         head_mask = inputs.get("head_mask", None)
         inputs_embeds = inputs.get("inputs_embeds", None)
         output_attentions = inputs.get("output_attentions", None)
         output_hidden_states = inputs.get("output_hidden_states", None)
+        return_dict = inputs.get("return_dict", None) or kwargs.get("return_dict", None)
 
         lm_outputs = self.distilbert(
             input_ids,
             attention_mask=attention_mask,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
-            **kwargs,
+            return_dict=return_dict,
         )
         hidden_state = lm_outputs[0]
         pooled_output = hidden_state[:, 0]
         pooled_output = self.pre_classifier(pooled_output)
         pooled_output = nn.ReLU()(pooled_output)
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
 
         outputs = {
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
         }
         return outputs
-
-    def preprocess(self, inputs: Union[str, List[str]], **kwargs):
-        if isinstance(inputs, str):
-            inputs = [inputs]
-        if "text_normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["text_normalizer"]
-            inputs = normalizer(inputs)
-        tokenizer = self.preprocessor["wordpiece_tokenizer"]
-        inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
-        return inputs
-
-    def post_process(self, inputs, **kwargs) -> Dict:
-        logits = inputs["logits"]
-        predictions = logits.argmax(1)
-        predictions_probs = logits.softmax(1).max(1)
-        outputs = {"labels": [], "probs": []}
-        for prediction, prob in zip(predictions, predictions_probs):
-            label = self.config.id2label[prediction.item()]
-            outputs["labels"].append(label)
-            outputs["probs"].append(prob.item())
-        return outputs
```

### Comparing `hezar-0.20.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.21.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.21.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/preprocessors/preprocessor.py` & `hezar-0.21.0/hezar/preprocessors/preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,26 @@
         return preprocessors
 
 
 class PreprocessorsContainer(OrderedDict):
     """
     A class to hold the preprocessors by their name
     """
+    def __getattr__(self, item):
+        """
+        Override this method to be able to access preprocessors as attributes
+
+        Examples:
+            >>> preprocessor["text_normalizer"] is preprocessor.text_normalizer  # noqa
+            ... True
+        """
+        if item in self:
+            return self[item]
+        else:
+            super().__getattribute__(item)
 
     def save(self, path):
         """
         Save every preprocessor item in the container
         """
         for name, preprocessor in self.items():
             preprocessor.save(path)
```

### Comparing `hezar-0.20.1/hezar/preprocessors/text_normalizer.py` & `hezar-0.21.0/hezar/preprocessors/text_normalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
 from dataclasses import dataclass, field
 from typing import List, Union
 
 from huggingface_hub import create_repo
 from tokenizers import normalizers
 
+from .preprocessor import Preprocessor
 from ..builders import build_preprocessor
 from ..configs import PreprocessorConfig
 from ..constants import DEFAULT_NORMALIZER_CONFIG_FILE, DEFAULT_PREPROCESSOR_SUBFOLDER
 from ..registry import register_preprocessor
 from ..utils import get_logger
-from .preprocessor import Preprocessor
-
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class TextNormalizerConfig(PreprocessorConfig):
     name: str = field(default="text_normalizer")
@@ -61,15 +60,15 @@
     @classmethod
     def load(
         cls,
         hub_or_local_path,
         subfolder=None,
         config_filename=None,
         **kwargs
-    ):
+    ) -> "TextNormalizer":
         config_filename = config_filename or cls.normalizer_config_file
         subfolder = subfolder or cls.preprocessor_subfolder
         config = TextNormalizerConfig.load(
             hub_or_local_path,
             filename=config_filename,
             subfolder=subfolder,
         )
```

### Comparing `hezar-0.20.1/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.21.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.21.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.21.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.21.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 
 import torch
 from huggingface_hub import create_repo, upload_file
 from tokenizers import Tokenizer as HFTokenizer
 from tokenizers.decoders import Decoder
 from tokenizers.models import Model
 
+from ..preprocessor import Preprocessor
 from ...builders import build_preprocessor
 from ...configs import PreprocessorConfig
 from ...constants import DEFAULT_TOKENIZER_CONFIG_FILE, DEFAULT_TOKENIZER_FILE
 from ...data.utils import convert_batch_dict_dtype
 from ...utils import get_logger
-from ..preprocessor import Preprocessor
-
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class TokenizerConfig(PreprocessorConfig):
     name: str = "tokenizer"
@@ -397,15 +396,15 @@
     @classmethod
     def load(
         cls,
         hub_or_local_path,
         config_filename=None,
         subfolder=None,
         **kwargs,
-    ):
+    ) -> "Tokenizer":
         config_filename = config_filename or cls.tokenizer_config_filename
         subfolder = subfolder or cls.preprocessor_subfolder
         config = TokenizerConfig.load(
             hub_or_local_path,
             filename=config_filename,
             subfolder=subfolder,
         )
```

### Comparing `hezar-0.20.1/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.21.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/registry.py` & `hezar-0.21.0/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.21.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.21.0/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/trainers/trainer.py` & `hezar-0.21.0/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/trainers/trainer_utils.py` & `hezar-0.21.0/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/utils/common_utils.py` & `hezar-0.21.0/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/utils/core_utils.py` & `hezar-0.21.0/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/hezar/utils/hub_utils.py` & `hezar-0.21.0/hezar/utils/hub_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,13 +116,13 @@
         for r, d, f in files_itr:
             if r == hub_or_local_path:
                 files.append(f)
             else:
                 for x in f:
                     files.append(f"{r.replace(f'{hub_or_local_path}/', '')}/{x}")
     else:
-        files = HfApi().list_repo_files(hub_or_local_path, repo_type=RepoType.MODEL)
+        files = HfApi().list_repo_files(hub_or_local_path, repo_type=RepoType.MODEL.value)
 
     if subfolder is not None:
         files = [x.replace(f"{subfolder}/", "") for x in files if subfolder in x]
 
     return files
```

### Comparing `hezar-0.20.1/hezar/utils/registry_utils.py` & `hezar-0.21.0/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.1/pyproject.toml` & `hezar-0.21.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.20.1"
+version = "0.21.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.20.1/PKG-INFO` & `hezar-0.21.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.20.1
+Version: 0.21.0
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

