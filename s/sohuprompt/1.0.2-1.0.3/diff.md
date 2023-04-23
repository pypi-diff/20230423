# Comparing `tmp/sohuprompt-1.0.2.tar.gz` & `tmp/sohuprompt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sohuprompt-1.0.2.tar", last modified: Sat Apr 22 12:44:16 2023, max compression
+gzip compressed data, was "sohuprompt-1.0.3.tar", last modified: Sun Apr 23 03:00:06 2023, max compression
```

## Comparing `sohuprompt-1.0.2.tar` & `sohuprompt-1.0.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.270747 sohuprompt-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-22 12:44:16.270747 sohuprompt-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4942 2023-04-22 12:39:37.000000 sohuprompt-1.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 12:44:16.270747 sohuprompt-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      682 2023-04-22 12:41:22.000000 sohuprompt-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.263747 sohuprompt-1.0.2/sohuprompt/
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.265747 sohuprompt-1.0.2/sohuprompt/data_utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.266747 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/closed_QA.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/coreference.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/entity_typing.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/generation.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/nli.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/paraphrase.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/processor.py
--rw-r--r--   0 root         (0) root         (0)    16857 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/reading_comprehensation.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/relation.py
--rw-r--r--   0 root         (0) root         (0)    11478 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/sentiment.py
--rw-r--r--   0 root         (0) root         (0)     3604 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/summarization.py
--rw-r--r--   0 root         (0) root         (0)     5336 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/topic_classification.py
--rw-r--r--   0 root         (0) root         (0)     2884 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5039 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/conditional_generation_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5009 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/data_sampler.py
--rw-r--r--   0 root         (0) root         (0)    15671 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/fewglue_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10269 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/huggingface_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/lama_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/nli_dataset.py
--rw-r--r--   0 root         (0) root         (0)    14301 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/relation_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)    16683 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/text_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/typing_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11734 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/utils.py
--rw-r--r--   0 root         (0) root         (0)    15591 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/default_config.py
--rw-r--r--   0 root         (0) root         (0)     8986 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/lm_bff_trainer.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/pipeline_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.266747 sohuprompt-1.0.2/sohuprompt/plms/
--rw-r--r--   0 root         (0) root         (0)     7763 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.267747 sohuprompt-1.0.2/sohuprompt/plms/glm/
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4119 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/glm.py
--rw-r--r--   0 root         (0) root         (0)    56656 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    15054 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    17877 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/tokenization_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/lm.py
--rw-r--r--   0 root         (0) root         (0)     3820 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/mlm.py
--rw-r--r--   0 root         (0) root         (0)    17199 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/seq2seq.py
--rw-r--r--   0 root         (0) root         (0)     9699 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/utils.py
--rw-r--r--   0 root         (0) root         (0)    27881 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompt_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.269747 sohuprompt-1.0.2/sohuprompt/prompts/
--rw-r--r--   0 root         (0) root         (0)     3846 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11510 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/automatic_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8002 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/generation_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8815 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/knowledgeable_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/manual_template.py
--rw-r--r--   0 root         (0) root         (0)     9645 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/manual_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8620 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/mixed_template.py
--rw-r--r--   0 root         (0) root         (0)     8052 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/one2one_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)    12707 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/prefix_tuning_template.py
--rw-r--r--   0 root         (0) root         (0)    23406 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/prompt_generator.py
--rw-r--r--   0 root         (0) root         (0)    15008 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/prototypical_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/ptr_prompts.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/ptuning_prompts.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/soft_template.py
--rw-r--r--   0 root         (0) root         (0)     9069 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/soft_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/protoverb_trainer.py
--rw-r--r--   0 root         (0) root         (0)    31323 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.269747 sohuprompt-1.0.2/sohuprompt/utils/
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3866 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/calibrate.py
--rw-r--r--   0 root         (0) root         (0)    10852 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/crossfit_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/cuda.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/logging.py
--rw-r--r--   0 root         (0) root         (0)     5906 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/metrics.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/reproduciblity.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.264747 sohuprompt-1.0.2/sohuprompt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2614 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.985925 sohuprompt-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-04-23 03:00:06.984925 sohuprompt-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-04-23 02:57:04.000000 sohuprompt-1.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 03:00:06.985925 sohuprompt-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      682 2023-04-23 02:56:05.000000 sohuprompt-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.978925 sohuprompt-1.0.3/sohuprompt/
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-23 02:55:47.000000 sohuprompt-1.0.3/sohuprompt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.980925 sohuprompt-1.0.3/sohuprompt/data_utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.981925 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/closed_QA.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/coreference.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/entity_typing.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/generation.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/nli.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/paraphrase.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/processor.py
+-rw-r--r--   0 root         (0) root         (0)    16857 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/reading_comprehensation.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/relation.py
+-rw-r--r--   0 root         (0) root         (0)    11478 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/summarization.py
+-rw-r--r--   0 root         (0) root         (0)     5336 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/data_utils/ZH/topic_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/conditional_generation_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/data_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    15671 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/fewglue_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/huggingface_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/lama_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/nli_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14301 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/relation_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    16683 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/text_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/typing_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11734 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/data_utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15591 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/default_config.py
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/lm_bff_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    33757 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/pipeline_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.981925 sohuprompt-1.0.3/sohuprompt/plms/
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.982925 sohuprompt-1.0.3/sohuprompt/plms/glm/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4119 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/glm.py
+-rw-r--r--   0 root         (0) root         (0)    56656 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    15054 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    17877 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/plms/glm/tokenization_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/lm.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/mlm.py
+-rw-r--r--   0 root         (0) root         (0)    17199 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/seq2seq.py
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/plms/utils.py
+-rw-r--r--   0 root         (0) root         (0)    27881 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompt_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.983925 sohuprompt-1.0.3/sohuprompt/prompts/
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/automatic_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8002 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/generation_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/knowledgeable_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/manual_template.py
+-rw-r--r--   0 root         (0) root         (0)     9645 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/manual_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/mixed_template.py
+-rw-r--r--   0 root         (0) root         (0)     8052 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/one2one_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)    12707 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/prefix_tuning_template.py
+-rw-r--r--   0 root         (0) root         (0)    23406 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/prompt_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15008 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/prototypical_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/ptr_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/ptuning_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/soft_template.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/prompts/soft_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/protoverb_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    31323 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.984925 sohuprompt-1.0.3/sohuprompt/utils/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/calibrate.py
+-rw-r--r--   0 root         (0) root         (0)    10852 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/utils/crossfit_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/cuda.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-22 09:08:12.000000 sohuprompt-1.0.3/sohuprompt/utils/logging.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/reproduciblity.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-04-23 02:06:53.000000 sohuprompt-1.0.3/sohuprompt/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 03:00:06.979925 sohuprompt-1.0.3/sohuprompt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-23 03:00:06.000000 sohuprompt-1.0.3/sohuprompt.egg-info/top_level.txt
```

### Comparing `sohuprompt-1.0.2/README.md` & `sohuprompt-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   <a href="#预览">预览</a> •
   <a href="#安装">安装</a> •
   <a href="#如何使用">如何使用</a> 
 </p>
 
 </div>
 
-![version](https://img.shields.io/badge/version-v1.0.2-green)
+![version](https://img.shields.io/badge/version-v1.0.3-green)
 
 
 
 
 ## 新闻
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
  #
                                   SohuPrompt
                       é¢è§ â¢ å®è£ â¢ å¦ä½ä½¿ç¨
-![version](https://img.shields.io/badge/version-v1.0.2-green) ## æ°é» -
+![version](https://img.shields.io/badge/version-v1.0.3-green) ## æ°é» -
 âï¸ 2023å¹´4æï¼çæ¬æ´æ°ï¼æ¯æ[ChatGLM](https://github.com/THUDM/
 ChatGLM-6B), å¯ä»¥ä½¿ç¨SohuPromptå·¥å·å¯¹ChatGLMè¿è¡å¾®è°. -
 2023å¹´4æï¼SohuPrompt
 v1.0.1çæ¬åå¸ï¼æ¬¢è¿å¤§å®¶ä¸ºSohuPromptè´¡ç®ä»£ç ã ## é¢è§ Prompt-
 learningæ¯ææ°çè®­ç»èå¼ï¼å®å¯ä»¥å°é¢è®­ç»è¯­è¨æ¨¡åï¼PLMsï¼æ´å¥½çééä¸æ¸¸NLPä»»å¡ãSohuPromptåºæä¾äºä¸ä¸ªæ åãçµæ´»åå¯æ©å±çæ¡æ¶ï¼ç¨äºé¨ç½²prompt-
 learningæµæ°´çº¿ï¼å®æ¯æç´æ¥ä»[huggingface transformers](https://
 github.com/huggingface/transformers)å è½½PLMsãå¨æªæ¥ï¼æä»¬å°æ¯æ
```

### Comparing `sohuprompt-1.0.2/setup.py` & `sohuprompt-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(name='sohuprompt',
-        version='1.0.2',
+        version='1.0.3',
         packages=find_packages(),  # 查找包的路径
         # package_dir={'': 'src'},  # 包的root路径映射到的实际路径
         # include_package_data=False,
         # package_data={'data': []},
         description='A python lib for sohuprompt',
         # long_description='',
         author='senhaowang,chencheng',
```

### Comparing `sohuprompt-1.0.2/sohuprompt/config.py` & `sohuprompt-1.0.3/sohuprompt/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 try:
     from typing import OrderedDict
 except ImportError:
     from collections import OrderedDict
 import argparse
 from yacs.config import CfgNode
 import sys
-from SohuPrompt.utils.utils import check_config_conflicts
+from sohuprompt.utils.utils import check_config_conflicts
 from .default_config import get_default_config
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 import os
 
 
 def get_config_from_file(path):
     cfg = CfgNode(new_allowed=True)
     cfg.merge_from_file(path)
     return cfg
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/closed_QA.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/closed_QA.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/coreference.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/coreference.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/entity_typing.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/entity_typing.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/generation.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/generation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/nli.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/nli.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/paraphrase.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/paraphrase.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/reading_comprehensation.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/reading_comprehensation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/relation.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/relation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/sentiment.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/sentiment.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/summarization.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/summarization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/topic_classification.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/ZH/topic_classification.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/__init__.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from .lama_dataset import PROCESSORS as LAMA_PROCESSORS
 from .conditional_generation_dataset import PROCESSORS as CG_PROCESSORS
 from .utils import InputExample, InputFeatures
 from .data_sampler import FewShotSampler
 # support loading transformers datasets from https://huggingface.co/docs/datasets/
 from .nli_dataset import PROCESSORS as NLI_PROCESSORS
 
-from SohuPrompt.utils.logging import logger
-from SohuPrompt.data_utils.huggingface_dataset import PROCESSORS as HF_PROCESSORS
+from sohuprompt.utils.logging import logger
+from sohuprompt.data_utils.huggingface_dataset import PROCESSORS as HF_PROCESSORS
 
 PROCESSORS = {
     **TYPING_PROCESSORS,
     **TC_PROCESSORS,
     **SUPERGLUE_PROCESSORS,
     **RC_PROCESSORS,
     **LAMA_PROCESSORS,
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/conditional_generation_dataset.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/conditional_generation_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 This file contains the logic for loading data for all Conditional Generation tasks.
 """
 
-from SohuPrompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.utils import InputExample
 import os
 import json, csv
 from abc import ABC, abstractmethod
 from collections import defaultdict, Counter
 from typing import List, Dict, Callable
 
-from SohuPrompt.utils.logging import logger
-from SohuPrompt.data_utils.data_processor import DataProcessor
+from sohuprompt.utils.logging import logger
+from sohuprompt.data_utils.data_processor import DataProcessor
 
 class GCProcessor(DataProcessor):
     def __init__(self):
         super().__init__()
         self.labels = None
 
     def get_examples(self, data_dir: str, split: str) -> List[InputExample]:
@@ -47,15 +47,15 @@
     """
     # TODO citation
 
     Examples:
 
     .. code-block:: python
 
-        from SohuPrompt.data_utils.conditional_generation_dataset import PROCESSORS
+        from sohuprompt.data_utils.conditional_generation_dataset import PROCESSORS
 
         base_path = "datasets/CondGen"
 
         dataset_name = "webnlg_2017"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         train_dataset = processor.get_train_examples(dataset_path)
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/data_processor.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/data_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from typing import *
 from abc import abstractmethod
-from SohuPrompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.utils import InputExample
 
 class DataProcessor:
     """
     labels of the dataset is optional
 
     here's the examples of loading the labels:
 
@@ -91,39 +91,39 @@
         """
         return len(self.labels)
 
     def get_train_examples(self, data_dir: Optional[str] = None) -> InputExample:
         """
         get train examples from the training file under :obj:`data_dir`
 
-        call ``get_examples(data_dir, "train")``, see :py:meth:`~SohuPrompt.data_utils.data_processor.DataProcessor.get_examples`
+        call ``get_examples(data_dir, "train")``, see :py:meth:`~sohuprompt.data_utils.data_processor.DataProcessor.get_examples`
         """
         return self.get_examples(data_dir, "train")
 
     def get_dev_examples(self, data_dir: Optional[str] = None) -> List[InputExample]:
         """
         get dev examples from the development file under :obj:`data_dir`
 
-        call ``get_examples(data_dir, "dev")``, see :py:meth:`~SohuPrompt.data_utils.data_processor.DataProcessor.get_examples`
+        call ``get_examples(data_dir, "dev")``, see :py:meth:`~sohuprompt.data_utils.data_processor.DataProcessor.get_examples`
         """
         return self.get_examples(data_dir, "dev")
 
     def get_test_examples(self, data_dir: Optional[str] = None) -> List[InputExample]:
         """
         get test examples from the test file under :obj:`data_dir`
 
-        call ``get_examples(data_dir, "test")``, see :py:meth:`~SohuPrompt.data_utils.data_processor.DataProcessor.get_examples`
+        call ``get_examples(data_dir, "test")``, see :py:meth:`~sohuprompt.data_utils.data_processor.DataProcessor.get_examples`
         """
         return self.get_examples(data_dir, "test")
 
     def get_unlabeled_examples(self, data_dir: Optional[str] = None) -> List[InputExample]:
         """
         get unlabeled examples from the unlabeled file under :obj:`data_dir`
 
-        call ``get_examples(data_dir, "unlabeled")``, see :py:meth:`~SohuPrompt.data_utils.data_processor.DataProcessor.get_examples`
+        call ``get_examples(data_dir, "unlabeled")``, see :py:meth:`~sohuprompt.data_utils.data_processor.DataProcessor.get_examples`
         """
         return self.get_examples(data_dir, "unlabeled")
 
     @abstractmethod
     def get_examples(self, data_dir: Optional[str] = None, split: Optional[str] = None) -> List[InputExample]:
         """get the :obj:`split` of dataset under :obj:`data_dir`
 
@@ -132,10 +132,10 @@
         training file could be located in ``data_dir/train.txt``
 
         Args:
             data_dir (str): the base path of the dataset
             split (str): ``train`` / ``dev`` / ``test`` / ``unlabeled``
 
         Returns:
-            List[InputExample]: return a list of :py:class:`~SohuPrompt.data_utils.data_utils.InputExample`
+            List[InputExample]: return a list of :py:class:`~sohuprompt.data_utils.data_utils.InputExample`
         """
         raise NotImplementedError
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/data_sampler.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/data_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict, namedtuple
 from typing import *
 
 import numpy as np
 from torch.utils.data import Dataset
 from torch.utils.data.dataset import Subset
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 from typing import Union
 
 
 
 
 class FewShotSampler(object):
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/fewglue_dataset.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/fewglue_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 import random
 from abc import ABC, abstractmethod
 from collections import defaultdict, Counter
 from typing import List, Dict, Callable, Sequence
 
 from torch.utils.data import dataset
 
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
-from SohuPrompt.data_utils.utils import InputExample
-from SohuPrompt.data_utils.data_processor import DataProcessor
+from sohuprompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.data_processor import DataProcessor
 
 
 
 
 
 class FewGLUEDataProcessor(DataProcessor):
     """Processor for FewGLUE
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/huggingface_dataset.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/huggingface_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # limitations under the License.
 
 """
 This file contains the logic for loading data for all FewGLUE tasks.
 """
 
 
-from SohuPrompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.utils import InputExample
 
-from SohuPrompt.data_utils.data_processor import DataProcessor
+from sohuprompt.data_utils.data_processor import DataProcessor
 from datasets import load_dataset
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 from datasets import load_from_disk
 import os
 
 HUGGING_FACE_SCRIPTS = 'super_glue' # if you can not connect huggingface in your machine, you can download the scripts manually and change this line.
 HUGGING_FACE_SCRIPTS = '../../huggingface_datasets/super_glue'
 class SuperglueMultiRCProcessor(DataProcessor):
     def __init__(self):
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/lama_dataset.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/lama_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from collections import defaultdict, Counter
 from typing import *
 import tokenizers
 import sys
 
 from transformers.tokenization_utils import PreTrainedTokenizer
 
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
-from SohuPrompt.data_utils.utils import InputExample
-from SohuPrompt.data_utils.data_processor import DataProcessor
+from sohuprompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.data_processor import DataProcessor
 
 
 
 class LAMAProcessor(DataProcessor):
     """This dataset is a variant of the original `LAMA <https://github.com/facebookresearch/LAMA>`_ dataset, which adds train and dev split, and was created by `AutoPrompt <https://github.com/ucinlp/autoprompt>`_ .
 
     The code of this Processor refers to `the data processing phase in P-tuning <https://github.com/THUDM/P-tuning/tree/main/LAMA>`_
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/nli_dataset.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/nli_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from typing import List
-from SohuPrompt.data_utils import InputExample
-from SohuPrompt.data_utils.data_processor import DataProcessor
+from sohuprompt.data_utils import InputExample
+from sohuprompt.data_utils.data_processor import DataProcessor
 
 # logger = log.get_logger(__name__)
 
 
 
 class SNLIProcessor(DataProcessor):
     """
@@ -25,15 +25,15 @@
 
     We use the data released in `Making Pre-trained Language Models Better Few-shot Learners (Gao et al. 2020) <https://arxiv.org/pdf/2012.15723.pdf>`_
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.lmbff_dataset import PROCESSORS
+        from sohuprompt.data_utils.lmbff_dataset import PROCESSORS
 
         base_path = "datasets"
 
         dataset_name = "SNLI"
         dataset_path = os.path.join(base_path, dataset_name, '16-13')
         processor = PROCESSORS[dataset_name.lower()]()
         train_dataset = processor.get_train_examples(dataset_path)
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/relation_classification_dataset.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/relation_classification_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 
 import os
 import json, csv
 from abc import ABC, abstractmethod
 from collections import defaultdict, Counter
 from typing import *
 
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
-from SohuPrompt.data_utils.utils import InputExample
-from SohuPrompt.data_utils.data_processor import DataProcessor
+from sohuprompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.data_processor import DataProcessor
 
 
 
 
 class TACREDProcessor(DataProcessor):
     """
     `TAC Relation Extraction Dataset (TACRED) <https://nlp.stanford.edu/projects/tacred/>`_ is one of the largest and most widely used datasets for relation classification.
     It was released together with the paper `Position-aware Attention and Supervised Data Improve Slot Filling (Zhang et al. 2017) <https://nlp.stanford.edu/pubs/zhang2017tacred.pdf>`_
     This processor is also inherited by :py:class:`TACREVProcessor` and :py:class:`ReTACREDProcessor`.
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.relation_classification_dataset import PROCESSORS
+        from sohuprompt.data_utils.relation_classification_dataset import PROCESSORS
 
         base_path = "datasets/RelationClassification"
 
         dataset_name = "TACRED"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         train_dataset = processor.get_train_examples(dataset_path)
@@ -80,15 +80,15 @@
 
     This processor inherit :py:class:`TACREDProcessor` and can be used similarly
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.relation_classification_dataset import PROCESSORS
+        from sohuprompt.data_utils.relation_classification_dataset import PROCESSORS
 
         base_path = "datasets/RelationClassification"
 
         dataset_name = "TACREV"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         train_dataset = processor.get_train_examples(dataset_path)
@@ -114,15 +114,15 @@
 
     This processor inherit :py:class:`TACREDProcessor` and can be used similarly
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.relation_classification_dataset import PROCESSORS
+        from sohuprompt.data_utils.relation_classification_dataset import PROCESSORS
 
         base_path = "datasets/RelationClassification"
 
         dataset_name = "ReTACRED"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         train_dataset = processor.get_train_examples(dataset_path)
@@ -146,15 +146,15 @@
 
     It was released together with the paper `SemEval-2010 Task 8: Multi-Way Classification of Semantic Relations Between Pairs of Nominals (Hendrickx et al. 2010) <https://aclanthology.org/S10-1006.pdf>`_
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.relation_classification_dataset import PROCESSORS
+        from sohuprompt.data_utils.relation_classification_dataset import PROCESSORS
 
         base_path = "datasets/RelationClassification"
 
         dataset_name = "SemEval"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         train_dataset = processor.get_train_examples(dataset_path)
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/text_classification_dataset.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/text_classification_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 import os
 import json, csv
 from abc import ABC, abstractmethod
 from collections import defaultdict, Counter
 from typing import List, Dict, Callable
 import pandas as pd
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
-from SohuPrompt.data_utils.utils import InputExample
-from SohuPrompt.data_utils.data_processor import DataProcessor
+from sohuprompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.data_processor import DataProcessor
 
 
 class ReProcessor(DataProcessor):
     def __init__(self):
         super().__init__()
         self.labels = [0,1]
 
@@ -115,15 +115,15 @@
 
     we use dataset provided by `LOTClass <https://github.com/yumeng5/LOTClass>`_
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.text_classification_dataset import PROCESSORS
+        from sohuprompt.data_utils.text_classification_dataset import PROCESSORS
 
         base_path = "datasets/TextClassification"
 
         dataset_name = "agnews"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         trainvalid_dataset = processor.get_train_examples(dataset_path)
@@ -161,15 +161,15 @@
 
     we use dataset provided by `LOTClass <https://github.com/yumeng5/LOTClass>`_
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.text_classification_dataset import PROCESSORS
+        from sohuprompt.data_utils.text_classification_dataset import PROCESSORS
 
         base_path = "datasets/TextClassification"
 
         dataset_name = "dbpedia"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         trainvalid_dataset = processor.get_train_examples(dataset_path)
@@ -205,15 +205,15 @@
 
     we use dataset provided by `LOTClass <https://github.com/yumeng5/LOTClass>`_
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.text_classification_dataset import PROCESSORS
+        from sohuprompt.data_utils.text_classification_dataset import PROCESSORS
 
         base_path = "datasets/TextClassification"
 
         dataset_name = "imdb"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         trainvalid_dataset = processor.get_train_examples(dataset_path)
@@ -312,15 +312,15 @@
     """
     Yahoo! Answers Topic Classification Dataset
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.text_classification_dataset import PROCESSORS
+        from sohuprompt.data_utils.text_classification_dataset import PROCESSORS
 
         base_path = "datasets/TextClassification"
     """
 
     def __init__(self):
         super().__init__()
         self.labels = ["Society & Culture", "Science & Mathematics", "Health", "Education & Reference", "Computers & Internet", "Sports", "Business & Finance", "Entertainment & Music"
@@ -366,15 +366,15 @@
 
     We use the data released in `Making Pre-trained Language Models Better Few-shot Learners (Gao et al. 2020) <https://arxiv.org/pdf/2012.15723.pdf>`_
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.lmbff_dataset import PROCESSORS
+        from sohuprompt.data_utils.lmbff_dataset import PROCESSORS
 
         base_path = "datasets/TextClassification"
 
         dataset_name = "SST-2"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         train_dataset = processor.get_train_examples(dataset_path)
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/typing_dataset.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/typing_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 import json, csv
 from abc import ABC, abstractmethod
 from collections import defaultdict, Counter
 from typing import *
 
 from transformers.tokenization_utils import SPECIAL_TOKENS_MAP_FILE
 
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
-from SohuPrompt.data_utils.utils import InputExample
-from SohuPrompt.data_utils.data_processor import DataProcessor
+from sohuprompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.data_processor import DataProcessor
 
 
 
 class FewNERDProcessor(DataProcessor):
     """
     `Few-NERD <https://ningding97.github.io/fewnerd/>`_ a large-scale, fine-grained manually annotated named entity recognition dataset
 
     It was released together with `Few-NERD: Not Only a Few-shot NER Dataset (Ning Ding et al. 2021) <https://arxiv.org/pdf/2105.07464.pdf>`_
 
     Examples:
 
     ..  code-block:: python
 
-        from SohuPrompt.data_utils.typing_dataset import PROCESSORS
+        from sohuprompt.data_utils.typing_dataset import PROCESSORS
 
         base_path = "datasets/Typing"
 
         dataset_name = "FewNERD"
         dataset_path = os.path.join(base_path, dataset_name)
         processor = PROCESSORS[dataset_name.lower()]()
         train_dataset = processor.get_train_examples(dataset_path)
```

### Comparing `sohuprompt-1.0.2/sohuprompt/data_utils/utils.py` & `sohuprompt-1.0.3/sohuprompt/data_utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import json
 import pickle
 from typing import *
 
 import torch
 from torch.utils.data._utils.collate import default_collate
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 from typing import Union
 
 
 class InputExample(object):
     """A raw input example consisting of segments of text,
     a label for classification task or a target sequence of generation task.
@@ -278,15 +278,15 @@
         r'''
         This function is used to collate the input_features.
 
         Args:
             batch (:obj:`List[Union[Dict, InputFeatures]]`): A batch of the current data.
 
         Returns:
-            :obj:`InputFeatures`: Return the :py:class:`~SohuPrompt.data_utils.data_utils.InputFeatures of the current batch of data.
+            :obj:`InputFeatures`: Return the :py:class:`~sohuprompt.data_utils.data_utils.InputFeatures of the current batch of data.
         '''
 
 
         elem = batch[0]
         return_dict = {}
         for key in elem:
             if key == "encoded_tgt_text":
```

### Comparing `sohuprompt-1.0.2/sohuprompt/default_config.py` & `sohuprompt-1.0.3/sohuprompt/default_config.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/lm_bff_trainer.py` & `sohuprompt-1.0.3/sohuprompt/lm_bff_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from transformers.data.processors.utils import InputExample, InputFeatures
 
 
-from SohuPrompt import PromptDataLoader, PromptForClassification
-from SohuPrompt.pipeline_base import PromptModel
+from sohuprompt import PromptDataLoader, PromptForClassification
+from sohuprompt.pipeline_base import PromptModel
 
-from SohuPrompt.prompts import ManualVerbalizer, ManualTemplate
+from sohuprompt.prompts import ManualVerbalizer, ManualTemplate
 from typing import List, Optional, Dict, Union
 from . import Verbalizer, PromptDataLoader
 import copy
 import warnings
 from .trainer import ClassificationRunner
 from yacs.config import CfgNode
-from SohuPrompt.utils.logging import logger
-from SohuPrompt.utils.cuda import model_to_device
-from SohuPrompt.prompts import load_template_generator, load_verbalizer_generator
-from SohuPrompt.plms import load_plm_from_config
+from sohuprompt.utils.logging import logger
+from sohuprompt.utils.cuda import model_to_device
+from sohuprompt.prompts import load_template_generator, load_verbalizer_generator
+from sohuprompt.plms import load_plm_from_config
 
 
 
 
 def build_dataloader(dataset, template, tokenizer,tokenizer_wrapper_class, config, split):
     dataloader = PromptDataLoader(
         dataset = dataset,
```

### Comparing `sohuprompt-1.0.2/sohuprompt/pipeline_base.py` & `sohuprompt-1.0.3/sohuprompt/pipeline_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from torch.utils.data.sampler import RandomSampler
 from transformers.configuration_utils import PretrainedConfig
 from transformers import GenerationMixin
 import torch
 import torch.nn as nn
 from torch.utils.data import Dataset
 from typing import *
-from SohuPrompt.data_utils import InputExample, InputFeatures
+from sohuprompt.data_utils import InputExample, InputFeatures
 from torch.utils.data._utils.collate import default_collate
 from tqdm.std import tqdm
 from transformers.tokenization_utils import PreTrainedTokenizer
 from transformers.utils.dummy_pt_objects import PreTrainedModel
-from SohuPrompt.plms.utils import TokenizerWrapper
-from SohuPrompt.prompt_base import Template, Verbalizer
-from SohuPrompt.plms.glm import ChatGLMForConditionalGeneration
+from sohuprompt.plms.utils import TokenizerWrapper
+from sohuprompt.prompt_base import Template, Verbalizer
+from sohuprompt.plms.glm import ChatGLMForConditionalGeneration
 from collections import defaultdict
-from SohuPrompt.utils import round_list, signature
+from sohuprompt.utils import round_list, signature
 import numpy as np
 from torch.utils.data import DataLoader
 from yacs.config import CfgNode
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 from transformers import AdamW, get_linear_schedule_with_warmup
 
 
 class PromptDataLoader(object):
     r"""
     PromptDataLoader wraps the original dataset. The input data is firstly wrapped with the
     prompt's template, and then is tokenized by a wrapperd-tokenizer.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/__init__.py` & `sohuprompt-1.0.3/sohuprompt/plms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ChatGLMForConditionalGeneration,
     ChatGLMTokenizer,
     GLMTokenizerWrapper,
 )
 from collections import namedtuple
 from yacs.config import CfgNode
 
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 ModelClass = namedtuple("ModelClass", ("config", "tokenizer", "model", "wrapper"))
 
 _MODEL_CLASSES = {
     "bert": ModelClass(
         **{
```

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/glm/configuration_chatglm.py` & `sohuprompt-1.0.3/sohuprompt/plms/glm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/glm/glm.py` & `sohuprompt-1.0.3/sohuprompt/plms/glm/glm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt.plms.utils import TokenizerWrapper
+from sohuprompt.plms.utils import TokenizerWrapper
 from typing import List, Dict, Optional
 from collections import defaultdict
 import numpy as np
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 class GLMTokenizerWrapper(TokenizerWrapper):
     r"""
     GLMTokenizer is a general language model from THUDM. GLM is a new model structure similar to GPT .
     Therefore it can only predict <mask> position
     at the end of the sentence. A prefix-style template like: 'A <mask> news : <text_a> <text_b> ' is
```

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/glm/modeling_chatglm.py` & `sohuprompt-1.0.3/sohuprompt/plms/glm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/glm/quantization.py` & `sohuprompt-1.0.3/sohuprompt/plms/glm/quantization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/glm/tokenization_chatglm.py` & `sohuprompt-1.0.3/sohuprompt/plms/glm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/lm.py` & `sohuprompt-1.0.3/sohuprompt/plms/lm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt.plms.utils import TokenizerWrapper
+from sohuprompt.plms.utils import TokenizerWrapper
 from typing import List, Dict, Optional
 from collections import defaultdict
 import numpy as np
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 class LMTokenizerWrapper(TokenizerWrapper):
     r"""
     LMTokenizer is a causual language model. Therefore it can only predict <mask> position
     at the end of the sentence. A prefix-style template like: 'A <mask> news : <text_a> <text_b> ' is
     not applicable in this situation.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/mlm.py` & `sohuprompt-1.0.3/sohuprompt/plms/mlm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from transformers.models.auto.tokenization_auto import tokenizer_class_from_name
 
-from SohuPrompt.plms.utils import TokenizerWrapper
+from sohuprompt.plms.utils import TokenizerWrapper
 from typing import List, Dict
 from collections import defaultdict
 
 class MLMTokenizerWrapper(TokenizerWrapper):
     add_input_keys = ['input_ids', 'attention_mask', 'token_type_ids']
 
     @property
```

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/seq2seq.py` & `sohuprompt-1.0.3/sohuprompt/plms/seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from json import decoder
 
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt.plms.utils import TokenizerWrapper
+from sohuprompt.plms.utils import TokenizerWrapper
 from typing import List, Dict, Optional
 from collections import defaultdict
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 class T5TokenizerWrapper(TokenizerWrapper):
     r"""
     Given wrapped example, e.g. A fun movie ! it is <mask> and <mask> .
     The input tokens is:  A fun movie ! it is <extra_id_0> and <extra_id_1> . </s>
     The decoder tokens is: <pad> <extra_id_0> <extra_id_1> </s>
     The expected output is <extra_id_0> good interesting </s>
```

### Comparing `sohuprompt-1.0.2/sohuprompt/plms/utils.py` & `sohuprompt-1.0.3/sohuprompt/plms/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 import torch.nn as nn
 from torch.utils.data import Dataset
 from typing import Union, List, Tuple, Dict, Optional
 from transformers.data.processors.utils import InputExample, InputFeatures
 from transformers.tokenization_utils import PreTrainedTokenizer
 from collections import defaultdict
-from SohuPrompt.utils import round_list
+from sohuprompt.utils import round_list
 import numpy as np
 
 
 class TokenizerWrapper:
     def __init__(
         self,
         max_seq_length: int,
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompt_base.py` & `sohuprompt-1.0.3/sohuprompt/prompt_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from abc import abstractmethod
 import json
 
 from transformers.file_utils import ModelOutput
-from SohuPrompt.config import convert_cfg_to_dict
+from sohuprompt.config import convert_cfg_to_dict
 
 from transformers.utils.dummy_pt_objects import PreTrainedModel
-from SohuPrompt.utils.utils import signature
+from sohuprompt.utils.utils import signature
 
 from yacs.config import CfgNode
-from SohuPrompt.data_utils import InputFeatures, InputExample
+from sohuprompt.data_utils import InputFeatures, InputExample
 import torch
 import torch.nn as nn
 from typing import *
 from transformers.tokenization_utils import PreTrainedTokenizer
 
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 import numpy as np
 import torch.nn.functional as F
 
 
 class Template(nn.Module):
     r'''
     Base class for all the templates.
@@ -190,15 +190,15 @@
         This function process the example into a list of dict,
         Each dict functions as a group, which has the sample properties, such as
         whether it's shortenable, whether it's the masked position, whether it's soft token, etc.
         Since a text will be tokenized in the subsequent processing procedure,
         these attributes are broadcasted along the tokenized sentence.
 
         Args:
-            example (:obj:`InputExample`): An :py:class:`~SohuPrompt.data_utils.data_utils.InputExample` object, which should have attributes that are able to be filled in the template.
+            example (:obj:`InputExample`): An :py:class:`~sohuprompt.data_utils.data_utils.InputExample` object, which should have attributes that are able to be filled in the template.
 
         Returns:
             :obj:`List[Dict]`: A list of dict of the same length as self.text. e.g. ``[{"loss_ids": 0, "text": "It was"}, {"loss_ids": 1, "text": "<mask>"}, ]``
         '''
 
         if self.text is None:
             raise ValueError("template text has not been initialized")
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/__init__.py` & `sohuprompt-1.0.3/sohuprompt/prompts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from yacs.config import CfgNode
-from SohuPrompt.utils.utils import signature
+from sohuprompt.utils.utils import signature
 from typing import Optional
 from transformers.tokenization_utils import PreTrainedTokenizer
 
 from transformers.utils.dummy_pt_objects import PreTrainedModel
 from .manual_template import ManualTemplate
 from .manual_verbalizer import ManualVerbalizer
 from .mixed_template import MixedTemplate
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/automatic_verbalizer.py` & `sohuprompt-1.0.3/sohuprompt/prompts/automatic_verbalizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt.data_utils import InputFeatures
-from SohuPrompt import Verbalizer
+from sohuprompt.data_utils import InputFeatures
+from sohuprompt import Verbalizer
 from typing import List, Optional, Dict
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 
 class AutomaticVerbalizer(Verbalizer):
     r"""
     This implementation is slightly different from the original code in that
     1). we allow re-selecting the verbalizer after a fixed training steps.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/generation_verbalizer.py` & `sohuprompt-1.0.3/sohuprompt/prompts/generation_verbalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from functools import partial
 import json
-from SohuPrompt.data_utils.utils import InputExample
+from sohuprompt.data_utils.utils import InputExample
 from transformers.tokenization_utils import PreTrainedTokenizer
 from yacs.config import CfgNode
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import re
-from SohuPrompt import Verbalizer
+from sohuprompt import Verbalizer
 from typing import *
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SohuPrompt.utils.logging import logger
-from SohuPrompt.utils.crossfit_metrics import *
+from sohuprompt.utils.logging import logger
+from sohuprompt.utils.crossfit_metrics import *
 import re
 
 
 class GenerationVerbalizer(Verbalizer):
     r"""
     This verbalizer is useful when the label prediction is better defined by a piece of input.
     For example, in correference resolution, the tgt_text is a proper noun mentioned in the text.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/knowledgeable_verbalizer.py` & `sohuprompt-1.0.3/sohuprompt/prompts/knowledgeable_verbalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
-from SohuPrompt.prompts.manual_template import ManualTemplate
+from sohuprompt.prompts.manual_template import ManualTemplate
 from transformers.tokenization_utils import PreTrainedTokenizer
 from transformers.utils.dummy_pt_objects import PreTrainedModel
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import re
-from SohuPrompt.prompts.manual_verbalizer import ManualVerbalizer
+from sohuprompt.prompts.manual_verbalizer import ManualVerbalizer
 from typing import *
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 
 class KnowledgeableVerbalizer(ManualVerbalizer):
     r"""
     This is the implementation of knowledeagble verbalizer, which uses external knowledge to expand the set of label words.
     This class inherit the ``ManualVerbalizer`` class.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/manual_verbalizer.py` & `sohuprompt-1.0.3/sohuprompt/prompts/manual_verbalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from transformers.tokenization_utils import PreTrainedTokenizer
 from yacs.config import CfgNode
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import re
-from SohuPrompt import Verbalizer
+from sohuprompt import Verbalizer
 from typing import *
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 
 class ManualVerbalizer(Verbalizer):
     r"""
     The basic manually defined verbalizer class, this class is inherited from the :obj:`Verbalizer` class.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/mixed_template.py` & `sohuprompt-1.0.3/sohuprompt/prompts/mixed_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 import os
 import string
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
-from SohuPrompt.data_utils.utils import InputExample, InputFeatures
+from sohuprompt.data_utils.utils import InputExample, InputFeatures
 from typing import *
 
 from transformers import PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt import Template
+from sohuprompt import Template
 
 import torch
 from torch import nn
 
 class MixedTemplate(Template):
     r"""The Mixed Template class defined by a string of `text`. See more examples in the `tutorial <https://github.com/thunlp/OpenPrompt/blob/ca27491101df0108a8dd753e5b1e79bf591f65d3/tutorial/1.1_mixed_template.py>`_.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/one2one_verbalizer.py` & `sohuprompt-1.0.3/sohuprompt/prompts/one2one_verbalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from transformers.tokenization_utils import PreTrainedTokenizer
 from yacs.config import CfgNode
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import re
-from SohuPrompt import Verbalizer
+from sohuprompt import Verbalizer
 from typing import *
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 
 class One2oneVerbalizer(Verbalizer):
     r"""
     The basic manually defined verbalizer class, this class is inherited from the :obj:`Verbalizer` class.
     This class restrict the use of label words to one words per label. For a verbalzer with less constraints,
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/prefix_tuning_template.py` & `sohuprompt-1.0.3/sohuprompt/prompts/prefix_tuning_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 from functools import partial
 from transformers.configuration_utils import PretrainedConfig
 from transformers.models.gpt2.configuration_gpt2 import GPT2Config
-from SohuPrompt.plms import ChatGLMConfig, ChatGLMForConditionalGeneration
+from sohuprompt.plms import ChatGLMConfig, ChatGLMForConditionalGeneration
 from transformers.models.t5.configuration_t5 import T5Config
 from transformers.models.t5.modeling_t5 import T5ForConditionalGeneration
 from transformers.models.gpt2.modeling_gpt2 import GPT2LMHeadModel
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import os
 import torch
 from torch import nn
 from typing import *
 from transformers import PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt import Template
-from SohuPrompt.utils.logging import logger
+from sohuprompt import Template
+from sohuprompt.utils.logging import logger
 
 
 class PrefixTuningTemplate(Template):
     r"""This is the implementation which support T5 and other Encoder-Decoder model,
     as soon as their blocks allows the ``past_key_values`` to be injected to the model.
     This implementation modifies the huggingface's T5 forward without touching the code-base.
     However, it may fail to work when used in DataParallel model. Please use it using
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/prompt_generator.py` & `sohuprompt-1.0.3/sohuprompt/prompts/prompt_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from builtins import ValueError
 from typing import List, Optional, Dict, Union
 from tokenizers import Tokenizer
 import json
 import torch
 import torch.nn.functional as F
 from yacs.config import CfgNode
-from SohuPrompt.data_utils.utils import InputExample, InputFeatures
-from SohuPrompt.pipeline_base import PromptDataLoader, PromptModel
+from sohuprompt.data_utils.utils import InputExample, InputFeatures
+from sohuprompt.pipeline_base import PromptDataLoader, PromptModel
 
-from SohuPrompt.prompt_base import Template, Verbalizer
-from SohuPrompt.prompts import ManualTemplate, ManualVerbalizer
+from sohuprompt.prompt_base import Template, Verbalizer
+from sohuprompt.prompts import ManualTemplate, ManualVerbalizer
 from ..utils import logger
 from transformers import T5Tokenizer, T5ForConditionalGeneration, BertForMaskedLM, RobertaForMaskedLM, RobertaTokenizer, PreTrainedModel, PreTrainedTokenizer
 from tqdm import tqdm
 from typing import List, Optional, Dict
 import itertools
 import numpy as np
 from ..utils import signature
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/prototypical_verbalizer.py` & `sohuprompt-1.0.3/sohuprompt/prompts/prototypical_verbalizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from inspect import Parameter
 import json
 from os import stat
 from transformers.file_utils import ModelOutput
 from transformers.tokenization_utils import PreTrainedTokenizer
 from transformers.utils.dummy_pt_objects import PreTrainedModel
 from yacs.config import CfgNode
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import re
-from SohuPrompt import Verbalizer
+from sohuprompt import Verbalizer
 from typing import *
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 import copy
 from transformers.modeling_outputs import CausalLMOutputWithCrossAttentions, Seq2SeqLMOutput, MaskedLMOutput
 
 from transformers.models.t5 import  T5ForConditionalGeneration
 
 class ProtoVerbalizer(Verbalizer):
     r"""
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/ptr_prompts.py` & `sohuprompt-1.0.3/sohuprompt/prompts/ptr_prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 import json
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import os
 import torch
 from torch import nn
 from typing import *
 from transformers import PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt import Verbalizer
-from SohuPrompt.prompts import One2oneVerbalizer, PtuningTemplate
+from sohuprompt import Verbalizer
+from sohuprompt.prompts import One2oneVerbalizer, PtuningTemplate
 
 class PTRTemplate(PtuningTemplate):
     """
     Args:
         model (:obj:`PreTrainedModel`): The pre-trained language model for the current prompt-learning task.
         tokenizer (:obj:`PreTrainedTokenizer`): A tokenizer to appoint the vocabulary and the tokenization strategy.
         text (:obj:`Optional[List[str]]`, optional): manual template format. Defaults to None.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/ptuning_prompts.py` & `sohuprompt-1.0.3/sohuprompt/prompts/ptuning_prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import os
 import torch
 from torch import nn
 from typing import *
 from transformers import PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt.prompts import MixedTemplate
+from sohuprompt.prompts import MixedTemplate
 
 class PtuningTemplate(MixedTemplate):
     """
     Args:
         model (:obj:`PreTrainedModel`): The pre-trained language model for the current prompt-learning task.
         tokenizer (:obj:`PreTrainedTokenizer`): A tokenizer to appoint the vocabulary and the tokenization strategy.
         prompt_encoder_type (:obj:`str`): head above the embedding layer of new tokens. Can be ``lstm`` or ``mlp``.
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/soft_template.py` & `sohuprompt-1.0.3/sohuprompt/prompts/soft_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 import os
 
 from torch.nn.parameter import Parameter
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 
-from SohuPrompt.data_utils import InputExample, InputFeatures
+from sohuprompt.data_utils import InputExample, InputFeatures
 from typing import *
 
 from transformers import PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizer
-from SohuPrompt import Template
-from SohuPrompt.prompts import ManualTemplate, ManualVerbalizer
+from sohuprompt import Template
+from sohuprompt.prompts import ManualTemplate, ManualVerbalizer
 
 import torch
 from torch import nn
 
 class SoftTemplate(Template):
     r"""This is the implementation of `The Power of Scale for Parameter-Efficient
     Prompt Tuning <https://arxiv.org/pdf/2104.08691v1.pdf>`_ . Similar to :obj:`PrefixTuningTemplate`,
```

### Comparing `sohuprompt-1.0.2/sohuprompt/prompts/soft_verbalizer.py` & `sohuprompt-1.0.3/sohuprompt/prompts/soft_verbalizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from inspect import Parameter
 import json
 from os import stat
 from transformers.file_utils import ModelOutput
 from transformers.tokenization_utils import PreTrainedTokenizer
 from transformers.utils.dummy_pt_objects import PreTrainedModel
 from yacs.config import CfgNode
-from SohuPrompt.data_utils import InputFeatures
+from sohuprompt.data_utils import InputFeatures
 import re
-from SohuPrompt import Verbalizer
+from sohuprompt import Verbalizer
 from typing import *
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 import copy
 from transformers.modeling_outputs import CausalLMOutputWithCrossAttentions, Seq2SeqLMOutput, MaskedLMOutput
 
 from transformers.models.t5 import  T5ForConditionalGeneration
 
 class SoftVerbalizer(Verbalizer):
     r"""
```

### Comparing `sohuprompt-1.0.2/sohuprompt/protoverb_trainer.py` & `sohuprompt-1.0.3/sohuprompt/protoverb_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os, shutil
 import sys
 sys.path.append(".")
 
 import torch
 from torch import nn
 from torch.nn.parallel.data_parallel import DataParallel
-from SohuPrompt.utils.cuda import model_to_device
+from sohuprompt.utils.cuda import model_to_device
 from tensorboardX import SummaryWriter
 
 from tqdm import tqdm
 import dill
 import warnings
 
 from typing import Callable, Union, Dict
 try:
     from typing import OrderedDict
 except ImportError:
     from collections import OrderedDict
 
-from SohuPrompt.pipeline_base import PromptForClassification, PromptForGeneration
-from SohuPrompt.trainer import BaseRunner, ClassificationRunner
-from SohuPrompt import PromptDataLoader
-from SohuPrompt.prompts import *
-from SohuPrompt.utils.logging import logger
-from SohuPrompt.utils.metrics import classification_metrics, generation_metric
+from sohuprompt.pipeline_base import PromptForClassification, PromptForGeneration
+from sohuprompt.trainer import BaseRunner, ClassificationRunner
+from sohuprompt import PromptDataLoader
+from sohuprompt.prompts import *
+from sohuprompt.utils.logging import logger
+from sohuprompt.utils.metrics import classification_metrics, generation_metric
 from transformers import  AdamW, get_linear_schedule_with_warmup
 from transformers.optimization import  Adafactor, AdafactorSchedule
 
 
 
 
 class ProtoVerbClassificationRunner(BaseRunner):
```

### Comparing `sohuprompt-1.0.2/sohuprompt/trainer.py` & `sohuprompt-1.0.3/sohuprompt/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 import sys
 
 sys.path.append(".")
 
 import torch
 from torch import nn
 from torch.nn.parallel.data_parallel import DataParallel
-from SohuPrompt.utils.cuda import model_to_device
+from sohuprompt.utils.cuda import model_to_device
 from tensorboardX import SummaryWriter
 
 from tqdm import tqdm
 import dill
 import warnings
 
 from typing import Callable, Union, Dict
 
 try:
     from typing import OrderedDict
 except ImportError:
     from collections import OrderedDict
 
-from SohuPrompt.pipeline_base import PromptForClassification, PromptForGeneration
-from SohuPrompt.plms import ChatGLMForConditionalGeneration
-from SohuPrompt import PromptDataLoader
-from SohuPrompt.prompts import *
-from SohuPrompt.utils.logging import logger
-from SohuPrompt.utils.metrics import classification_metrics, generation_metric
+from sohuprompt.pipeline_base import PromptForClassification, PromptForGeneration
+from sohuprompt.plms import ChatGLMForConditionalGeneration
+from sohuprompt import PromptDataLoader
+from sohuprompt.prompts import *
+from sohuprompt.utils.logging import logger
+from sohuprompt.utils.metrics import classification_metrics, generation_metric
 from transformers import AdamW, get_linear_schedule_with_warmup
 from transformers.optimization import Adafactor, AdafactorSchedule
 from transformers.trainer_pt_utils import LabelSmoother
 from packaging import version
 import time
 
 parsed_torch_version_base = version.parse(version.parse(torch.__version__).base_version)
```

### Comparing `sohuprompt-1.0.2/sohuprompt/utils/calibrate.py` & `sohuprompt-1.0.3/sohuprompt/utils/calibrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from yacs.config import CfgNode
-from SohuPrompt.data_utils import FewShotSampler
+from sohuprompt.data_utils import FewShotSampler
 from torch.utils.data.dataset import Dataset
 from transformers.data.processors.utils import InputExample
-from SohuPrompt.pipeline_base import PromptDataLoader, PromptModel, PromptForClassification
+from sohuprompt.pipeline_base import PromptDataLoader, PromptModel, PromptForClassification
 from typing import *
 import torch
 from tqdm import tqdm
 
 # def pmi_calibrate(prompt_model: PromptModel,context_dataloader, max_seq_length: int) -> torch.Tensor:
 #     r"""Pmi calibrate. See `Paper <https://arxiv.org/pdf/2104.08315.pdf>`_
```

### Comparing `sohuprompt-1.0.2/sohuprompt/utils/crossfit_metrics.py` & `sohuprompt-1.0.3/sohuprompt/utils/crossfit_metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/utils/cuda.py` & `sohuprompt-1.0.3/sohuprompt/utils/cuda.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 def model_to_device(model, config):
     r"""
     model: the model to be wrapped
     config: the environment subconfig.
     """
     import os
```

### Comparing `sohuprompt-1.0.2/sohuprompt/utils/logging.py` & `sohuprompt-1.0.3/sohuprompt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.2/sohuprompt/utils/metrics.py` & `sohuprompt-1.0.3/sohuprompt/utils/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.metrics import f1_score, precision_score, recall_score, accuracy_score
 from typing import *
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 def f1(p, r):
     if p == 0. or r == 0.:
         return 0.
     return 2*p*r/(p+r)
 
 def label_path(label, label_path_sep):
```

### Comparing `sohuprompt-1.0.2/sohuprompt/utils/utils.py` & `sohuprompt-1.0.3/sohuprompt/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import shutil
 from typing import List
 import inspect
 from collections import namedtuple
 
 import torch
 from yacs.config import CfgNode
-from SohuPrompt.utils.logging import logger
+from sohuprompt.utils.logging import logger
 
 
 
 def round_list(l: List[float], max_sum:int):
     r"""round a list of float e.g. [0.2,1.5, 4.5]
     to [1,2,4] # ceil and restrict the sum to `max_sum`
     used into balanced truncate.
```

### Comparing `sohuprompt-1.0.2/sohuprompt.egg-info/SOURCES.txt` & `sohuprompt-1.0.3/sohuprompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

