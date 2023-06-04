# Comparing `tmp/autogluon.multimodal-0.7.1b20230602.tar.gz` & `tmp/autogluon.multimodal-0.7.1b20230603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.7.1b20230602.tar", last modified: Fri Jun  2 09:04:01 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.7.1b20230603.tar", last modified: Sat Jun  3 09:03:56 2023, max compression
```

## Comparing `autogluon.multimodal-0.7.1b20230602.tar` & `autogluon.multimodal-0.7.1b20230603.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.901665 autogluon.multimodal-0.7.1b20230602/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-02 09:04:01.901665 autogluon.multimodal-0.7.1b20230602/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:04:01.901665 autogluon.multimodal-0.7.1b20230602/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.885664 autogluon.multimodal-0.7.1b20230602/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.885664 autogluon.multimodal-0.7.1b20230602/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33147 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.893664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    82611 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.897664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.897664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.897664 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   118702 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.901665 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-02 09:03:27.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:04:01.889664 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:04:01.000000 autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.449062 autogluon.multimodal-0.7.1b20230603/
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-03 09:03:56.449062 autogluon.multimodal-0.7.1b20230603/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 09:03:56.449062 autogluon.multimodal-0.7.1b20230603/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.429062 autogluon.multimodal-0.7.1b20230603/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.429062 autogluon.multimodal-0.7.1b20230603/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.433062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.433062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.433062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.433062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.433062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.433062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.433062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.437062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.437062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.437062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.437062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.437062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35794 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.437062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82611 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.441062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.441062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.445062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118702 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.449062 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-03 09:03:22.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 09:03:56.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:56.433062 autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-03 09:03:56.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-03 09:03:56.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:56.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 09:03:56.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-03 09:03:56.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 09:03:56.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:56.000000 autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.7.1b20230602/PKG-INFO` & `autogluon.multimodal-0.7.1b20230603/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230602
+Version: 0.7.1b20230603
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -43,27 +43,27 @@
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
         
         | AutoGluon Task      |                                                                                Quickstart                                                                                |                                                                                API                                                                                |
         |:--------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#module-0)                 |
-        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.multimodal.MultiModalPredictor) |
-        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.timeseries.TimeSeriesPredictor) |
+        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.html)                 |
+        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.multimodal.MultiModalPredictor.html) |
+        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.timeseries.TimeSeriesPredictor.html) |
         
         ## Resources
         
-        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for [documentation](https://auto.gluon.ai/stable/api/index.html) and instructions on:
+        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for documentation and instructions on:
         - [Installing AutoGluon](https://auto.gluon.ai/stable/index.html#installation)
-        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html)
-          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
+        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html)
+          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular/tabular-essentials.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
         
-        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)
-        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)
+        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)
+        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)
         
         Refer to the [AutoGluon Roadmap](https://github.com/autogluon/autogluon/blob/master/ROADMAP.md) for details on upcoming features and releases.
         
         ### Scientific Publications
         - [AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data](https://arxiv.org/pdf/2003.06505.pdf) (*Arxiv*, 2020)
         - [Fast, Accurate, and Simple Models for Tabular Data via Augmented Distillation](https://proceedings.neurips.cc/paper/2020/hash/62d75fb2e3075506e8837d8f55021ab1-Abstract.html) (*NeurIPS*, 2020)
         - [Multimodal AutoML on Structured Tables with Text Fields](https://openreview.net/pdf?id=OHAIVOOl7Vl) (*ICML AutoML Workshop*, 2021)
```

### Comparing `autogluon.multimodal-0.7.1b20230602/setup.py` & `autogluon.multimodal-0.7.1b20230603/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,838 +13,827 @@
 from ..preprocess_dataframe import MultiModalFeaturePreprocessor
 from ..utils import apply_data_processor, apply_df_preprocessor, get_per_sample_features
 
 logger = logging.getLogger(__name__)
 
 try:
     import mmcv
-    from mmcv.utils import Config as MMCVConfig
-except:
-    MMCVConfig = None
-
-try:
     from mmcv.transforms import BaseTransform
     from mmcv.transforms.utils import cache_randomness
-except:
-    pass
-
-try:
+    from mmdet.structures.bbox import autocast_box_type
+    from mmdet.utils import log_img_scale
+    from mmengine.config import Config as MMConfig
     from mmengine.dataset import BaseDataset
-except:
-    pass
 
-try:
-    from mmdet.structures.bbox import autocast_box_type
-    from mmdet.utils import log_img_scale  # inline import to avoid mmdet uninstall error for other tasks
-except:
-    pass
-
-
-class MultiImageMixDataset(torch.utils.data.Dataset):
-    """
-    A Pytorch DataSet class to process a multimodal pd.DataFrame. It first uses a preprocessor to
-    produce model-agnostic features. Then, each processor prepares customized data for one modality
-    per model. For code simplicity, here we treat ground-truth label as one modality. This class is
-    independent of specific data modalities and models.
-    """
-
-    def __init__(
-        self,
-        data: pd.DataFrame,
-        preprocessor: List[MultiModalFeaturePreprocessor],
-        processors: List[dict],
-        model_config: MMCVConfig,
-        id_mappings: Optional[Union[Dict[str, Dict], Dict[str, pd.Series]]] = None,
-        is_training: bool = False,
-    ):
+    class MultiImageMixDataset(torch.utils.data.Dataset):
         """
-        Parameters
-        ----------
-        data
-            A pd.DataFrame containing multimodal features.
-        preprocessor
-            A list of multimodal feature preprocessors generating model-agnostic features.
-        processors
-            Data processors customizing data for each modality per model.
-        id_mappings
-             Id-to-content mappings. The contents can be text, image, etc.
-             This is used when the dataframe contains the query/response indexes instead of their contents.
-        is_training
-            Whether in training mode. Some data processing may be different between training
-            and validation/testing/prediction, e.g., image data augmentation is used only in
-            training.
-        model_config
-            Model config used to decided dataset type. e.g. if multi_image_mix_dataset is used in detection model,
-            MultiImageMixDataset will be used instead of BaseDataset
-        """
-        super().__init__()
-        self.processors = processors
-        self.is_training = is_training
-        self._consecutive_errors = 0
-
-        mix_config = model_config[MULTI_IMAGE_MIX_DATASET]
-        self.mix_data_key = "mmdet_image_image"  # the key of the data to mix, TODO: remove hardcoding
-        self.mix_result_key = "mix_results"  # the key of the mix result to store
-
-        self.mix_transforms = []
-        self.mix_transforms_types = []  # TODO: remove hardcode
-        if "mosaic" in mix_config:
-            self.mix_transforms.append(Mosaic(**mix_config["mosaic"]))
-            self.mix_transforms_types.append("mosaic")
-        if "mixup" in mix_config:
-            self.mix_transforms.append(MixUp(**mix_config["mixup"]))
-            self.mix_transforms_types.append("mixup")
-
-        self._skip_type_keys = None  # TODO: remove hardcode, we need to disable multi image mix in late epochs
-        self.max_refetch = 15  # TODO: remove hardcode (do we need refetch?)
-
-        self.lengths = []
-
-        for i, (per_preprocessor, per_processors_group) in enumerate(zip(preprocessor, processors)):
-            modality_features, modality_types, length = apply_df_preprocessor(
-                data=data,
-                df_preprocessor=per_preprocessor,
-                modalities=per_processors_group.keys(),
+        A Pytorch DataSet class to process a multimodal pd.DataFrame. It first uses a preprocessor to
+        produce model-agnostic features. Then, each processor prepares customized data for one modality
+        per model. For code simplicity, here we treat ground-truth label as one modality. This class is
+        independent of specific data modalities and models.
+        """
+
+        def __init__(
+            self,
+            data: pd.DataFrame,
+            preprocessor: List[MultiModalFeaturePreprocessor],
+            processors: List[dict],
+            model_config: MMConfig,
+            id_mappings: Optional[Union[Dict[str, Dict], Dict[str, pd.Series]]] = None,
+            is_training: bool = False,
+        ):
+            """
+            Parameters
+            ----------
+            data
+                A pd.DataFrame containing multimodal features.
+            preprocessor
+                A list of multimodal feature preprocessors generating model-agnostic features.
+            processors
+                Data processors customizing data for each modality per model.
+            id_mappings
+                Id-to-content mappings. The contents can be text, image, etc.
+                This is used when the dataframe contains the query/response indexes instead of their contents.
+            is_training
+                Whether in training mode. Some data processing may be different between training
+                and validation/testing/prediction, e.g., image data augmentation is used only in
+                training.
+            model_config
+                Model config used to decided dataset type. e.g. if multi_image_mix_dataset is used in detection model,
+                MultiImageMixDataset will be used instead of BaseDataset
+            """
+            super().__init__()
+            self.processors = processors
+            self.is_training = is_training
+            self._consecutive_errors = 0
+
+            mix_config = model_config[MULTI_IMAGE_MIX_DATASET]
+            self.mix_data_key = "mmdet_image_image"  # the key of the data to mix, TODO: remove hardcoding
+            self.mix_result_key = "mix_results"  # the key of the mix result to store
+
+            self.mix_transforms = []
+            self.mix_transforms_types = []  # TODO: remove hardcode
+            if "mosaic" in mix_config:
+                self.mix_transforms.append(Mosaic(**mix_config["mosaic"]))
+                self.mix_transforms_types.append("mosaic")
+            if "mixup" in mix_config:
+                self.mix_transforms.append(MixUp(**mix_config["mixup"]))
+                self.mix_transforms_types.append("mixup")
+
+            self._skip_type_keys = None  # TODO: remove hardcode, we need to disable multi image mix in late epochs
+            self.max_refetch = 15  # TODO: remove hardcode (do we need refetch?)
+
+            self.lengths = []
+
+            for i, (per_preprocessor, per_processors_group) in enumerate(zip(preprocessor, processors)):
+                modality_features, modality_types, length = apply_df_preprocessor(
+                    data=data,
+                    df_preprocessor=per_preprocessor,
+                    modalities=per_processors_group.keys(),
+                )
+                self.lengths.append(length)
+                setattr(self, f"modality_features_{i}", modality_features)
+                setattr(self, f"modality_types_{i}", modality_types)
+
+            assert len(set(self.lengths)) == 1
+
+            self.id_mappings = id_mappings
+
+        def __len__(self):
+            """
+            Assume that all modalities have the same sample number.
+
+            Returns
+            -------
+            Sample number in this dataset.
+            """
+            return self.lengths[0]
+
+        def _load_item(self, idx):
+            """
+            Get a single item without mix_results.
+            Iterate through all data processors to prepare model inputs. The data processors are
+            organized first by modalities and then by models.
+
+            Parameters
+            ----------
+            idx
+                Index of sample to process.
+
+            Returns
+            -------
+            Input data formatted as a dictionary.
+            """
+            ret = dict()
+            try:
+                for group_id, per_processors_group in enumerate(self.processors):
+                    per_sample_features = get_per_sample_features(
+                        modality_features=getattr(self, f"modality_features_{group_id}"),
+                        modality_types=getattr(self, f"modality_types_{group_id}"),
+                        idx=idx,
+                        id_mappings=self.id_mappings,
+                    )
+                    per_ret = apply_data_processor(
+                        per_sample_features=per_sample_features,
+                        data_processors=per_processors_group,
+                        feature_modalities=getattr(self, f"modality_types_{group_id}"),
+                        is_training=self.is_training,
+                        load_only=True,
+                    )
+                    ret.update(per_ret)
+            except Exception as e:
+                logger.debug(f"Skipping sample {idx} due to '{e}'")
+                self._consecutive_errors += 1
+                if self._consecutive_errors < GET_ITEM_ERROR_RETRY:
+                    return self.__getitem__((idx + 1) % self.__len__())
+                else:
+                    raise e
+            self._consecutive_errors = 0
+
+            return ret
+
+        def __getitem__(self, idx):
+            """
+            Iterate through all data processors to prepare model inputs. The data processors are
+            organized first by modalities and then by models.
+
+            Parameters
+            ----------
+            idx
+                Index of sample to process.
+
+            Returns
+            -------
+            Input data formatted as a dictionary.
+            """
+            results = copy.deepcopy(self._load_item(idx))
+
+            for (transform, transform_type) in zip(self.mix_transforms, self.mix_transforms_types):
+                assert hasattr(transform, "get_indexes")
+
+                if self._skip_type_keys is not None and transform_type in self._skip_type_keys:
+                    continue
+
+                for i in range(self.max_refetch):
+                    # Make sure the results passed the loading pipeline
+                    # of the original dataset is not None.
+                    indexes = transform.get_indexes(self)
+                    if not isinstance(indexes, collections.abc.Sequence):
+                        indexes = [indexes]
+                    mix_results = [copy.deepcopy(self._load_item(index)[self.mix_data_key]) for index in indexes]
+                    if None not in mix_results:
+                        results[self.mix_data_key][self.mix_result_key] = mix_results
+                        break
+                else:
+                    raise RuntimeError(
+                        "The loading pipeline of the original dataset"
+                        " always return None. Please check the correctness "
+                        "of the dataset and its pipeline."
+                    )
+
+                for i in range(self.max_refetch):
+                    # To confirm the results passed the training pipeline
+                    # of the wrapper is not None.
+                    updated_results = transform(copy.deepcopy(results[self.mix_data_key]))
+                    if updated_results is not None:
+                        results[self.mix_data_key] = updated_results
+                        break
+                else:
+                    raise RuntimeError(
+                        "The training pipeline of the dataset wrapper"
+                        " always return None.Please check the correctness "
+                        "of the dataset and its pipeline."
+                    )
+
+                if self.mix_result_key in results[self.mix_data_key]:
+                    results[self.mix_data_key].pop(self.mix_result_key)
+
+            rois_processor = self.processors[0][ROIS][0]  # TODO: remove hardcode
+            results.update(
+                rois_processor.process_one_loaded_sample(
+                    results,
+                    is_training=True,  # This dataset is used only in training
+                )
             )
-            self.lengths.append(length)
-            setattr(self, f"modality_features_{i}", modality_features)
-            setattr(self, f"modality_types_{i}", modality_types)
 
-        assert len(set(self.lengths)) == 1
+            return results
 
-        self.id_mappings = id_mappings
+    class Mosaic(BaseTransform):
+        """Mosaic augmentation.
 
-    def __len__(self):
-        """
-        Assume that all modalities have the same sample number.
-
-        Returns
-        -------
-        Sample number in this dataset.
-        """
-        return self.lengths[0]
+        Given 4 images, mosaic transform combines them into
+        one output image. The output image is composed of the parts from each sub-
+        image.
+
+        .. code:: text
+
+                            mosaic transform
+                            center_x
+                    +------------------------------+
+                    |       pad        |  pad      |
+                    |      +-----------+           |
+                    |      |           |           |
+                    |      |  image1   |--------+  |
+                    |      |           |        |  |
+                    |      |           | image2 |  |
+        center_y   |----+-------------+-----------|
+                    |    |   cropped   |           |
+                    |pad |   image3    |  image4   |
+                    |    |             |           |
+                    +----|-------------+-----------+
+                        |             |
+                        +-------------+
+
+        The mosaic transform steps are as follows:
+
+            1. Choose the mosaic center as the intersections of 4 images
+            2. Get the left top image according to the index, and randomly
+                sample another 3 images from the custom dataset.
+            3. Sub image will be cropped if image is larger than mosaic patch
+
+        Required Keys:
+
+        - img
+        - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+        - gt_bboxes_labels (np.int64) (optional)
+        - gt_ignore_flags (bool) (optional)
+        - mix_results (List[dict])
+
+        Modified Keys:
+
+        - img
+        - img_shape
+        - gt_bboxes (optional)
+        - gt_bboxes_labels (optional)
+        - gt_ignore_flags (optional)
 
-    def _load_item(self, idx):
-        """
-        Get a single item without mix_results.
-        Iterate through all data processors to prepare model inputs. The data processors are
-        organized first by modalities and then by models.
-
-        Parameters
-        ----------
-        idx
-            Index of sample to process.
-
-        Returns
-        -------
-        Input data formatted as a dictionary.
-        """
-        ret = dict()
-        try:
-            for group_id, per_processors_group in enumerate(self.processors):
-                per_sample_features = get_per_sample_features(
-                    modality_features=getattr(self, f"modality_features_{group_id}"),
-                    modality_types=getattr(self, f"modality_types_{group_id}"),
-                    idx=idx,
-                    id_mappings=self.id_mappings,
-                )
-                per_ret = apply_data_processor(
-                    per_sample_features=per_sample_features,
-                    data_processors=per_processors_group,
-                    feature_modalities=getattr(self, f"modality_types_{group_id}"),
-                    is_training=self.is_training,
-                    load_only=True,
+        Args:
+            img_scale (Sequence[int]): Image size after mosaic pipeline of single
+                image. The shape order should be (width, height).
+                Defaults to (640, 640).
+            center_ratio_range (Sequence[float]): Center ratio range of mosaic
+                output. Defaults to (0.5, 1.5).
+            bbox_clip_border (bool, optional): Whether to clip the objects outside
+                the border of the image. In some dataset like MOT17, the gt bboxes
+                are allowed to cross the border of images. Therefore, we don't
+                need to clip the gt bboxes in these cases. Defaults to True.
+            pad_val (int): Pad value. Defaults to 114.
+            prob (float): Probability of applying this transformation.
+                Defaults to 1.0.
+        """
+
+        def __init__(
+            self,
+            img_scale: Tuple[int, int] = (640, 640),
+            center_ratio_range: Tuple[float, float] = (0.5, 1.5),
+            bbox_clip_border: bool = True,
+            pad_val: float = 114.0,
+            prob: float = 1.0,
+        ) -> None:
+            assert isinstance(img_scale, tuple)
+            assert 0 <= prob <= 1.0, "The probability should be in range [0,1]. " f"got {prob}."
+
+            log_img_scale(img_scale, skip_square=True, shape_order="wh")
+            self.img_scale = img_scale
+            self.center_ratio_range = center_ratio_range
+            self.bbox_clip_border = bbox_clip_border
+            self.pad_val = pad_val
+            self.prob = prob
+
+        @cache_randomness
+        def get_indexes(self, dataset: BaseDataset) -> int:
+            """Call function to collect indexes.
+
+            Args:
+                dataset (:obj:`MultiImageMixDataset`): The dataset.
+
+            Returns:
+                list: indexes.
+            """
+
+            indexes = [random.randint(0, len(dataset)) for _ in range(3)]
+            return indexes
+
+        @autocast_box_type()
+        def transform(self, results: dict) -> dict:
+            """Mosaic transform function.
+
+            Args:
+                results (dict): Result dict.
+
+            Returns:
+                dict: Updated result dict.
+            """
+            if random.uniform(0, 1) > self.prob:
+                return results
+
+            assert "mix_results" in results
+            mosaic_bboxes = []
+            mosaic_bboxes_labels = []
+            mosaic_ignore_flags = []
+            if len(results["img"].shape) == 3:
+                mosaic_img = np.full(
+                    (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2), 3),
+                    self.pad_val,
+                    dtype=results["img"].dtype,
                 )
-                ret.update(per_ret)
-        except Exception as e:
-            logger.debug(f"Skipping sample {idx} due to '{e}'")
-            self._consecutive_errors += 1
-            if self._consecutive_errors < GET_ITEM_ERROR_RETRY:
-                return self.__getitem__((idx + 1) % self.__len__())
             else:
-                raise e
-        self._consecutive_errors = 0
-
-        return ret
+                mosaic_img = np.full(
+                    (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2)), self.pad_val, dtype=results["img"].dtype
+                )
 
-    def __getitem__(self, idx):
-        """
-        Iterate through all data processors to prepare model inputs. The data processors are
-        organized first by modalities and then by models.
+            # mosaic center x, y
+            center_x = int(random.uniform(*self.center_ratio_range) * self.img_scale[0])
+            center_y = int(random.uniform(*self.center_ratio_range) * self.img_scale[1])
+            center_position = (center_x, center_y)
+
+            loc_strs = ("top_left", "top_right", "bottom_left", "bottom_right")
+            for i, loc in enumerate(loc_strs):
+                if loc == "top_left":
+                    results_patch = copy.deepcopy(results)
+                else:
+                    results_patch = copy.deepcopy(results["mix_results"][i - 1])
+
+                img_i = results_patch["img"]
+                h_i, w_i = img_i.shape[:2]
+                # keep_ratio resize
+                scale_ratio_i = min(self.img_scale[1] / h_i, self.img_scale[0] / w_i)
+                img_i = mmcv.imresize(img_i, (int(w_i * scale_ratio_i), int(h_i * scale_ratio_i)))
+
+                # compute the combine parameters
+                paste_coord, crop_coord = self._mosaic_combine(loc, center_position, img_i.shape[:2][::-1])
+                x1_p, y1_p, x2_p, y2_p = paste_coord
+                x1_c, y1_c, x2_c, y2_c = crop_coord
+
+                # crop and paste image
+                mosaic_img[y1_p:y2_p, x1_p:x2_p] = img_i[y1_c:y2_c, x1_c:x2_c]
+
+                # adjust coordinate
+                gt_bboxes_i = results_patch["gt_bboxes"]
+                gt_bboxes_labels_i = results_patch["gt_bboxes_labels"]
+                gt_ignore_flags_i = results_patch["gt_ignore_flags"]
+
+                padw = x1_p - x1_c
+                padh = y1_p - y1_c
+                gt_bboxes_i.rescale_([scale_ratio_i, scale_ratio_i])
+                gt_bboxes_i.translate_([padw, padh])
+                mosaic_bboxes.append(gt_bboxes_i)
+                mosaic_bboxes_labels.append(gt_bboxes_labels_i)
+                mosaic_ignore_flags.append(gt_ignore_flags_i)
+
+            mosaic_bboxes = mosaic_bboxes[0].cat(mosaic_bboxes, 0)
+            mosaic_bboxes_labels = np.concatenate(mosaic_bboxes_labels, 0)
+            mosaic_ignore_flags = np.concatenate(mosaic_ignore_flags, 0)
 
-        Parameters
-        ----------
-        idx
-            Index of sample to process.
-
-        Returns
-        -------
-        Input data formatted as a dictionary.
-        """
-        results = copy.deepcopy(self._load_item(idx))
+            if self.bbox_clip_border:
+                mosaic_bboxes.clip_([2 * self.img_scale[1], 2 * self.img_scale[0]])
+            # remove outside bboxes
+            inside_inds = mosaic_bboxes.is_inside([2 * self.img_scale[1], 2 * self.img_scale[0]]).numpy()
+            mosaic_bboxes = mosaic_bboxes[inside_inds]
+            mosaic_bboxes_labels = mosaic_bboxes_labels[inside_inds]
+            mosaic_ignore_flags = mosaic_ignore_flags[inside_inds]
+
+            results["img"] = mosaic_img
+            results["img_shape"] = mosaic_img.shape[:2]
+            results["gt_bboxes"] = mosaic_bboxes
+            results["gt_bboxes_labels"] = mosaic_bboxes_labels
+            results["gt_ignore_flags"] = mosaic_ignore_flags
+            return results
 
-        for (transform, transform_type) in zip(self.mix_transforms, self.mix_transforms_types):
-            assert hasattr(transform, "get_indexes")
+        def _mosaic_combine(
+            self, loc: str, center_position_xy: Sequence[float], img_shape_wh: Sequence[int]
+        ) -> Tuple[Tuple[int], Tuple[int]]:
+            """Calculate global coordinate of mosaic image and local coordinate of
+            cropped sub-image.
+
+            Args:
+                loc (str): Index for the sub-image, loc in ('top_left',
+                'top_right', 'bottom_left', 'bottom_right').
+                center_position_xy (Sequence[float]): Mixing center for 4 images,
+                    (x, y).
+                img_shape_wh (Sequence[int]): Width and height of sub-image
+
+            Returns:
+                tuple[tuple[float]]: Corresponding coordinate of pasting and
+                    cropping
+                    - paste_coord (tuple): paste corner coordinate in mosaic image.
+                    - crop_coord (tuple): crop corner coordinate in mosaic image.
+            """
+            assert loc in ("top_left", "top_right", "bottom_left", "bottom_right")
+            if loc == "top_left":
+                # index0 to top left part of image
+                x1, y1, x2, y2 = (
+                    max(center_position_xy[0] - img_shape_wh[0], 0),
+                    max(center_position_xy[1] - img_shape_wh[1], 0),
+                    center_position_xy[0],
+                    center_position_xy[1],
+                )
+                crop_coord = img_shape_wh[0] - (x2 - x1), img_shape_wh[1] - (y2 - y1), img_shape_wh[0], img_shape_wh[1]
 
-            if self._skip_type_keys is not None and transform_type in self._skip_type_keys:
-                continue
+            elif loc == "top_right":
+                # index1 to top right part of image
+                x1, y1, x2, y2 = (
+                    center_position_xy[0],
+                    max(center_position_xy[1] - img_shape_wh[1], 0),
+                    min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
+                    center_position_xy[1],
+                )
+                crop_coord = 0, img_shape_wh[1] - (y2 - y1), min(img_shape_wh[0], x2 - x1), img_shape_wh[1]
 
-            for i in range(self.max_refetch):
-                # Make sure the results passed the loading pipeline
-                # of the original dataset is not None.
-                indexes = transform.get_indexes(self)
-                if not isinstance(indexes, collections.abc.Sequence):
-                    indexes = [indexes]
-                mix_results = [copy.deepcopy(self._load_item(index)[self.mix_data_key]) for index in indexes]
-                if None not in mix_results:
-                    results[self.mix_data_key][self.mix_result_key] = mix_results
-                    break
-            else:
-                raise RuntimeError(
-                    "The loading pipeline of the original dataset"
-                    " always return None. Please check the correctness "
-                    "of the dataset and its pipeline."
+            elif loc == "bottom_left":
+                # index2 to bottom left part of image
+                x1, y1, x2, y2 = (
+                    max(center_position_xy[0] - img_shape_wh[0], 0),
+                    center_position_xy[1],
+                    center_position_xy[0],
+                    min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
                 )
+                crop_coord = img_shape_wh[0] - (x2 - x1), 0, img_shape_wh[0], min(y2 - y1, img_shape_wh[1])
 
-            for i in range(self.max_refetch):
-                # To confirm the results passed the training pipeline
-                # of the wrapper is not None.
-                updated_results = transform(copy.deepcopy(results[self.mix_data_key]))
-                if updated_results is not None:
-                    results[self.mix_data_key] = updated_results
-                    break
             else:
-                raise RuntimeError(
-                    "The training pipeline of the dataset wrapper"
-                    " always return None.Please check the correctness "
-                    "of the dataset and its pipeline."
+                # index3 to bottom right part of image
+                x1, y1, x2, y2 = (
+                    center_position_xy[0],
+                    center_position_xy[1],
+                    min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
+                    min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
                 )
+                crop_coord = 0, 0, min(img_shape_wh[0], x2 - x1), min(y2 - y1, img_shape_wh[1])
 
-            if self.mix_result_key in results[self.mix_data_key]:
-                results[self.mix_data_key].pop(self.mix_result_key)
-
-        rois_processor = self.processors[0][ROIS][0]  # TODO: remove hardcode
-        results.update(
-            rois_processor.process_one_loaded_sample(
-                results,
-                is_training=True,  # This dataset is used only in training
-            )
-        )
-
-        return results
+            paste_coord = x1, y1, x2, y2
+            return paste_coord, crop_coord
 
+        def __repr__(self):
+            repr_str = self.__class__.__name__
+            repr_str += f"(img_scale={self.img_scale}, "
+            repr_str += f"center_ratio_range={self.center_ratio_range}, "
+            repr_str += f"pad_val={self.pad_val}, "
+            repr_str += f"prob={self.prob})"
+            return repr_str
+
+    class MixUp(BaseTransform):
+        """MixUp data augmentation.
+
+        .. code:: text
+
+                            mixup transform
+                    +------------------------------+
+                    | mixup image   |              |
+                    |      +--------|--------+     |
+                    |      |        |        |     |
+                    |---------------+        |     |
+                    |      |                 |     |
+                    |      |      image      |     |
+                    |      |                 |     |
+                    |      |                 |     |
+                    |      |-----------------+     |
+                    |             pad              |
+                    +------------------------------+
+
+        The mixup transform steps are as follows:
+
+            1. Another random image is picked by dataset and embedded in
+            the top left patch(after padding and resizing)
+            2. The target of mixup transform is the weighted average of mixup
+            image and origin image.
+
+        Required Keys:
+
+        - img
+        - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+        - gt_bboxes_labels (np.int64) (optional)
+        - gt_ignore_flags (bool) (optional)
+        - mix_results (List[dict])
+
+
+        Modified Keys:
+
+        - img
+        - img_shape
+        - gt_bboxes (optional)
+        - gt_bboxes_labels (optional)
+        - gt_ignore_flags (optional)
 
-class Mosaic(BaseTransform):
-    """Mosaic augmentation.
-
-    Given 4 images, mosaic transform combines them into
-    one output image. The output image is composed of the parts from each sub-
-    image.
-
-    .. code:: text
-
-                        mosaic transform
-                           center_x
-                +------------------------------+
-                |       pad        |  pad      |
-                |      +-----------+           |
-                |      |           |           |
-                |      |  image1   |--------+  |
-                |      |           |        |  |
-                |      |           | image2 |  |
-     center_y   |----+-------------+-----------|
-                |    |   cropped   |           |
-                |pad |   image3    |  image4   |
-                |    |             |           |
-                +----|-------------+-----------+
-                     |             |
-                     +-------------+
-
-     The mosaic transform steps are as follows:
-
-         1. Choose the mosaic center as the intersections of 4 images
-         2. Get the left top image according to the index, and randomly
-            sample another 3 images from the custom dataset.
-         3. Sub image will be cropped if image is larger than mosaic patch
-
-    Required Keys:
-
-    - img
-    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
-    - gt_bboxes_labels (np.int64) (optional)
-    - gt_ignore_flags (bool) (optional)
-    - mix_results (List[dict])
-
-    Modified Keys:
-
-    - img
-    - img_shape
-    - gt_bboxes (optional)
-    - gt_bboxes_labels (optional)
-    - gt_ignore_flags (optional)
-
-    Args:
-        img_scale (Sequence[int]): Image size after mosaic pipeline of single
-            image. The shape order should be (width, height).
-            Defaults to (640, 640).
-        center_ratio_range (Sequence[float]): Center ratio range of mosaic
-            output. Defaults to (0.5, 1.5).
-        bbox_clip_border (bool, optional): Whether to clip the objects outside
-            the border of the image. In some dataset like MOT17, the gt bboxes
-            are allowed to cross the border of images. Therefore, we don't
-            need to clip the gt bboxes in these cases. Defaults to True.
-        pad_val (int): Pad value. Defaults to 114.
-        prob (float): Probability of applying this transformation.
-            Defaults to 1.0.
-    """
-
-    def __init__(
-        self,
-        img_scale: Tuple[int, int] = (640, 640),
-        center_ratio_range: Tuple[float, float] = (0.5, 1.5),
-        bbox_clip_border: bool = True,
-        pad_val: float = 114.0,
-        prob: float = 1.0,
-    ) -> None:
-        assert isinstance(img_scale, tuple)
-        assert 0 <= prob <= 1.0, "The probability should be in range [0,1]. " f"got {prob}."
-
-        log_img_scale(img_scale, skip_square=True, shape_order="wh")
-        self.img_scale = img_scale
-        self.center_ratio_range = center_ratio_range
-        self.bbox_clip_border = bbox_clip_border
-        self.pad_val = pad_val
-        self.prob = prob
-
-    @cache_randomness
-    def get_indexes(self, dataset: BaseDataset) -> int:
-        """Call function to collect indexes.
 
         Args:
-            dataset (:obj:`MultiImageMixDataset`): The dataset.
-
-        Returns:
-            list: indexes.
-        """
-
-        indexes = [random.randint(0, len(dataset)) for _ in range(3)]
-        return indexes
-
-    @autocast_box_type()
-    def transform(self, results: dict) -> dict:
-        """Mosaic transform function.
-
-        Args:
-            results (dict): Result dict.
-
-        Returns:
-            dict: Updated result dict.
-        """
-        if random.uniform(0, 1) > self.prob:
-            return results
-
-        assert "mix_results" in results
-        mosaic_bboxes = []
-        mosaic_bboxes_labels = []
-        mosaic_ignore_flags = []
-        if len(results["img"].shape) == 3:
-            mosaic_img = np.full(
-                (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2), 3), self.pad_val, dtype=results["img"].dtype
-            )
-        else:
-            mosaic_img = np.full(
-                (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2)), self.pad_val, dtype=results["img"].dtype
-            )
-
-        # mosaic center x, y
-        center_x = int(random.uniform(*self.center_ratio_range) * self.img_scale[0])
-        center_y = int(random.uniform(*self.center_ratio_range) * self.img_scale[1])
-        center_position = (center_x, center_y)
-
-        loc_strs = ("top_left", "top_right", "bottom_left", "bottom_right")
-        for i, loc in enumerate(loc_strs):
-            if loc == "top_left":
-                results_patch = copy.deepcopy(results)
+            img_scale (Sequence[int]): Image output size after mixup pipeline.
+                The shape order should be (width, height). Defaults to (640, 640).
+            ratio_range (Sequence[float]): Scale ratio of mixup image.
+                Defaults to (0.5, 1.5).
+            flip_ratio (float): Horizontal flip ratio of mixup image.
+                Defaults to 0.5.
+            pad_val (int): Pad value. Defaults to 114.
+            max_iters (int): The maximum number of iterations. If the number of
+                iterations is greater than `max_iters`, but gt_bbox is still
+                empty, then the iteration is terminated. Defaults to 15.
+            bbox_clip_border (bool, optional): Whether to clip the objects outside
+                the border of the image. In some dataset like MOT17, the gt bboxes
+                are allowed to cross the border of images. Therefore, we don't
+                need to clip the gt bboxes in these cases. Defaults to True.
+        """
+
+        def __init__(
+            self,
+            img_scale: Tuple[int, int] = (640, 640),
+            ratio_range: Tuple[float, float] = (0.5, 1.5),
+            flip_ratio: float = 0.5,
+            pad_val: float = 114.0,
+            max_iters: int = 15,
+            bbox_clip_border: bool = True,
+        ) -> None:
+            assert isinstance(img_scale, tuple)
+            log_img_scale(img_scale, skip_square=True, shape_order="wh")
+            self.dynamic_scale = img_scale
+            self.ratio_range = ratio_range
+            self.flip_ratio = flip_ratio
+            self.pad_val = pad_val
+            self.max_iters = max_iters
+            self.bbox_clip_border = bbox_clip_border
+
+        @cache_randomness
+        def get_indexes(self, dataset: BaseDataset) -> int:
+            """Call function to collect indexes.
+
+            Args:
+                dataset (:obj:`MultiImageMixDataset`): The dataset.
+
+            Returns:
+                list: indexes.
+            """
+
+            index = [np.random.randint(0, len(dataset)) for _ in range(1)]
+
+            return index
+
+        @autocast_box_type()
+        def transform(self, results: dict) -> dict:
+            """MixUp transform function.
+
+            Args:
+                results (dict): Result dict.
+
+            Returns:
+                dict: Updated result dict.
+            """
+
+            assert "mix_results" in results
+            assert len(results["mix_results"]) == 1, "MixUp only support 2 images now !"
+
+            if results["mix_results"][0]["gt_bboxes"].shape[0] == 0:
+                # empty bbox
+                return results
+
+            retrieve_results = results["mix_results"][0]
+            retrieve_img = retrieve_results["img"]
+
+            jit_factor = random.uniform(*self.ratio_range)
+            is_filp = random.uniform(0, 1) > self.flip_ratio
+
+            if len(retrieve_img.shape) == 3:
+                out_img = (
+                    np.ones((self.dynamic_scale[1], self.dynamic_scale[0], 3), dtype=retrieve_img.dtype) * self.pad_val
+                )
             else:
-                results_patch = copy.deepcopy(results["mix_results"][i - 1])
-
-            img_i = results_patch["img"]
-            h_i, w_i = img_i.shape[:2]
-            # keep_ratio resize
-            scale_ratio_i = min(self.img_scale[1] / h_i, self.img_scale[0] / w_i)
-            img_i = mmcv.imresize(img_i, (int(w_i * scale_ratio_i), int(h_i * scale_ratio_i)))
-
-            # compute the combine parameters
-            paste_coord, crop_coord = self._mosaic_combine(loc, center_position, img_i.shape[:2][::-1])
-            x1_p, y1_p, x2_p, y2_p = paste_coord
-            x1_c, y1_c, x2_c, y2_c = crop_coord
-
-            # crop and paste image
-            mosaic_img[y1_p:y2_p, x1_p:x2_p] = img_i[y1_c:y2_c, x1_c:x2_c]
-
-            # adjust coordinate
-            gt_bboxes_i = results_patch["gt_bboxes"]
-            gt_bboxes_labels_i = results_patch["gt_bboxes_labels"]
-            gt_ignore_flags_i = results_patch["gt_ignore_flags"]
-
-            padw = x1_p - x1_c
-            padh = y1_p - y1_c
-            gt_bboxes_i.rescale_([scale_ratio_i, scale_ratio_i])
-            gt_bboxes_i.translate_([padw, padh])
-            mosaic_bboxes.append(gt_bboxes_i)
-            mosaic_bboxes_labels.append(gt_bboxes_labels_i)
-            mosaic_ignore_flags.append(gt_ignore_flags_i)
-
-        mosaic_bboxes = mosaic_bboxes[0].cat(mosaic_bboxes, 0)
-        mosaic_bboxes_labels = np.concatenate(mosaic_bboxes_labels, 0)
-        mosaic_ignore_flags = np.concatenate(mosaic_ignore_flags, 0)
-
-        if self.bbox_clip_border:
-            mosaic_bboxes.clip_([2 * self.img_scale[1], 2 * self.img_scale[0]])
-        # remove outside bboxes
-        inside_inds = mosaic_bboxes.is_inside([2 * self.img_scale[1], 2 * self.img_scale[0]]).numpy()
-        mosaic_bboxes = mosaic_bboxes[inside_inds]
-        mosaic_bboxes_labels = mosaic_bboxes_labels[inside_inds]
-        mosaic_ignore_flags = mosaic_ignore_flags[inside_inds]
-
-        results["img"] = mosaic_img
-        results["img_shape"] = mosaic_img.shape[:2]
-        results["gt_bboxes"] = mosaic_bboxes
-        results["gt_bboxes_labels"] = mosaic_bboxes_labels
-        results["gt_ignore_flags"] = mosaic_ignore_flags
-        return results
-
-    def _mosaic_combine(
-        self, loc: str, center_position_xy: Sequence[float], img_shape_wh: Sequence[int]
-    ) -> Tuple[Tuple[int], Tuple[int]]:
-        """Calculate global coordinate of mosaic image and local coordinate of
-        cropped sub-image.
-
-        Args:
-            loc (str): Index for the sub-image, loc in ('top_left',
-              'top_right', 'bottom_left', 'bottom_right').
-            center_position_xy (Sequence[float]): Mixing center for 4 images,
-                (x, y).
-            img_shape_wh (Sequence[int]): Width and height of sub-image
-
-        Returns:
-            tuple[tuple[float]]: Corresponding coordinate of pasting and
-                cropping
-                - paste_coord (tuple): paste corner coordinate in mosaic image.
-                - crop_coord (tuple): crop corner coordinate in mosaic image.
-        """
-        assert loc in ("top_left", "top_right", "bottom_left", "bottom_right")
-        if loc == "top_left":
-            # index0 to top left part of image
-            x1, y1, x2, y2 = (
-                max(center_position_xy[0] - img_shape_wh[0], 0),
-                max(center_position_xy[1] - img_shape_wh[1], 0),
-                center_position_xy[0],
-                center_position_xy[1],
-            )
-            crop_coord = img_shape_wh[0] - (x2 - x1), img_shape_wh[1] - (y2 - y1), img_shape_wh[0], img_shape_wh[1]
+                out_img = np.ones(self.dynamic_scale[::-1], dtype=retrieve_img.dtype) * self.pad_val
 
-        elif loc == "top_right":
-            # index1 to top right part of image
-            x1, y1, x2, y2 = (
-                center_position_xy[0],
-                max(center_position_xy[1] - img_shape_wh[1], 0),
-                min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
-                center_position_xy[1],
+            # 1. keep_ratio resize
+            scale_ratio = min(
+                self.dynamic_scale[1] / retrieve_img.shape[0], self.dynamic_scale[0] / retrieve_img.shape[1]
             )
-            crop_coord = 0, img_shape_wh[1] - (y2 - y1), min(img_shape_wh[0], x2 - x1), img_shape_wh[1]
-
-        elif loc == "bottom_left":
-            # index2 to bottom left part of image
-            x1, y1, x2, y2 = (
-                max(center_position_xy[0] - img_shape_wh[0], 0),
-                center_position_xy[1],
-                center_position_xy[0],
-                min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
+            retrieve_img = mmcv.imresize(
+                retrieve_img, (int(retrieve_img.shape[1] * scale_ratio), int(retrieve_img.shape[0] * scale_ratio))
             )
-            crop_coord = img_shape_wh[0] - (x2 - x1), 0, img_shape_wh[0], min(y2 - y1, img_shape_wh[1])
 
-        else:
-            # index3 to bottom right part of image
-            x1, y1, x2, y2 = (
-                center_position_xy[0],
-                center_position_xy[1],
-                min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
-                min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
-            )
-            crop_coord = 0, 0, min(img_shape_wh[0], x2 - x1), min(y2 - y1, img_shape_wh[1])
+            # 2. paste
+            out_img[: retrieve_img.shape[0], : retrieve_img.shape[1]] = retrieve_img
 
-        paste_coord = x1, y1, x2, y2
-        return paste_coord, crop_coord
+            # 3. scale jit
+            scale_ratio *= jit_factor
+            out_img = mmcv.imresize(out_img, (int(out_img.shape[1] * jit_factor), int(out_img.shape[0] * jit_factor)))
+
+            # 4. flip
+            if is_filp:
+                out_img = out_img[:, ::-1, :]
+
+            # 5. random crop
+            ori_img = results["img"]
+            origin_h, origin_w = out_img.shape[:2]
+            target_h, target_w = ori_img.shape[:2]
+            padded_img = np.ones((max(origin_h, target_h), max(origin_w, target_w), 3)) * self.pad_val
+            padded_img = padded_img.astype(np.uint8)
+            padded_img[:origin_h, :origin_w] = out_img
+
+            x_offset, y_offset = 0, 0
+            if padded_img.shape[0] > target_h:
+                y_offset = random.randint(0, padded_img.shape[0] - target_h)
+            if padded_img.shape[1] > target_w:
+                x_offset = random.randint(0, padded_img.shape[1] - target_w)
+            padded_cropped_img = padded_img[y_offset : y_offset + target_h, x_offset : x_offset + target_w]
+
+            # 6. adjust bbox
+            retrieve_gt_bboxes = retrieve_results["gt_bboxes"]
+            retrieve_gt_bboxes.rescale_([scale_ratio, scale_ratio])
+            if self.bbox_clip_border:
+                retrieve_gt_bboxes.clip_([origin_h, origin_w])
 
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += f"(img_scale={self.img_scale}, "
-        repr_str += f"center_ratio_range={self.center_ratio_range}, "
-        repr_str += f"pad_val={self.pad_val}, "
-        repr_str += f"prob={self.prob})"
-        return repr_str
-
-
-class MixUp(BaseTransform):
-    """MixUp data augmentation.
-
-    .. code:: text
-
-                         mixup transform
-                +------------------------------+
-                | mixup image   |              |
-                |      +--------|--------+     |
-                |      |        |        |     |
-                |---------------+        |     |
-                |      |                 |     |
-                |      |      image      |     |
-                |      |                 |     |
-                |      |                 |     |
-                |      |-----------------+     |
-                |             pad              |
-                +------------------------------+
-
-     The mixup transform steps are as follows:
-
-        1. Another random image is picked by dataset and embedded in
-           the top left patch(after padding and resizing)
-        2. The target of mixup transform is the weighted average of mixup
-           image and origin image.
-
-    Required Keys:
-
-    - img
-    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
-    - gt_bboxes_labels (np.int64) (optional)
-    - gt_ignore_flags (bool) (optional)
-    - mix_results (List[dict])
-
-
-    Modified Keys:
-
-    - img
-    - img_shape
-    - gt_bboxes (optional)
-    - gt_bboxes_labels (optional)
-    - gt_ignore_flags (optional)
-
-
-    Args:
-        img_scale (Sequence[int]): Image output size after mixup pipeline.
-            The shape order should be (width, height). Defaults to (640, 640).
-        ratio_range (Sequence[float]): Scale ratio of mixup image.
-            Defaults to (0.5, 1.5).
-        flip_ratio (float): Horizontal flip ratio of mixup image.
-            Defaults to 0.5.
-        pad_val (int): Pad value. Defaults to 114.
-        max_iters (int): The maximum number of iterations. If the number of
-            iterations is greater than `max_iters`, but gt_bbox is still
-            empty, then the iteration is terminated. Defaults to 15.
-        bbox_clip_border (bool, optional): Whether to clip the objects outside
-            the border of the image. In some dataset like MOT17, the gt bboxes
-            are allowed to cross the border of images. Therefore, we don't
-            need to clip the gt bboxes in these cases. Defaults to True.
-    """
-
-    def __init__(
-        self,
-        img_scale: Tuple[int, int] = (640, 640),
-        ratio_range: Tuple[float, float] = (0.5, 1.5),
-        flip_ratio: float = 0.5,
-        pad_val: float = 114.0,
-        max_iters: int = 15,
-        bbox_clip_border: bool = True,
-    ) -> None:
-        assert isinstance(img_scale, tuple)
-        log_img_scale(img_scale, skip_square=True, shape_order="wh")
-        self.dynamic_scale = img_scale
-        self.ratio_range = ratio_range
-        self.flip_ratio = flip_ratio
-        self.pad_val = pad_val
-        self.max_iters = max_iters
-        self.bbox_clip_border = bbox_clip_border
-
-    @cache_randomness
-    def get_indexes(self, dataset: BaseDataset) -> int:
-        """Call function to collect indexes.
+            if is_filp:
+                retrieve_gt_bboxes.flip_([origin_h, origin_w], direction="horizontal")
 
-        Args:
-            dataset (:obj:`MultiImageMixDataset`): The dataset.
+            # 7. filter
+            cp_retrieve_gt_bboxes = retrieve_gt_bboxes.clone()
+            cp_retrieve_gt_bboxes.translate_([-x_offset, -y_offset])
+            if self.bbox_clip_border:
+                cp_retrieve_gt_bboxes.clip_([target_h, target_w])
 
-        Returns:
-            list: indexes.
-        """
+            # 8. mix up
+            ori_img = ori_img.astype(np.float32)
+            mixup_img = 0.5 * ori_img + 0.5 * padded_cropped_img.astype(np.float32)
+
+            retrieve_gt_bboxes_labels = retrieve_results["gt_bboxes_labels"]
+            retrieve_gt_ignore_flags = retrieve_results["gt_ignore_flags"]
+
+            mixup_gt_bboxes = cp_retrieve_gt_bboxes.cat((results["gt_bboxes"], cp_retrieve_gt_bboxes), dim=0)
+            mixup_gt_bboxes_labels = np.concatenate((results["gt_bboxes_labels"], retrieve_gt_bboxes_labels), axis=0)
+            mixup_gt_ignore_flags = np.concatenate((results["gt_ignore_flags"], retrieve_gt_ignore_flags), axis=0)
 
-        index = [np.random.randint(0, len(dataset)) for _ in range(1)]
+            # remove outside bbox
+            inside_inds = mixup_gt_bboxes.is_inside([target_h, target_w]).numpy()
+            mixup_gt_bboxes = mixup_gt_bboxes[inside_inds]
+            mixup_gt_bboxes_labels = mixup_gt_bboxes_labels[inside_inds]
+            mixup_gt_ignore_flags = mixup_gt_ignore_flags[inside_inds]
+
+            results["img"] = mixup_img.astype(np.uint8)
+            results["img_shape"] = mixup_img.shape[:2]
+            results["gt_bboxes"] = mixup_gt_bboxes
+            results["gt_bboxes_labels"] = mixup_gt_bboxes_labels
+            results["gt_ignore_flags"] = mixup_gt_ignore_flags
 
-        return index
+            return results
 
-    @autocast_box_type()
-    def transform(self, results: dict) -> dict:
-        """MixUp transform function.
+        def __repr__(self):
+            repr_str = self.__class__.__name__
+            repr_str += f"(dynamic_scale={self.dynamic_scale}, "
+            repr_str += f"ratio_range={self.ratio_range}, "
+            repr_str += f"flip_ratio={self.flip_ratio}, "
+            repr_str += f"pad_val={self.pad_val}, "
+            repr_str += f"max_iters={self.max_iters}, "
+            repr_str += f"bbox_clip_border={self.bbox_clip_border})"
+            return repr_str
+
+    class RandomAffine(BaseTransform):
+        """Random affine transform data augmentation.
+
+        This operation randomly generates affine transform matrix which including
+        rotation, translation, shear and scaling transforms.
+
+        Required Keys:
+
+        - img
+        - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+        - gt_bboxes_labels (np.int64) (optional)
+        - gt_ignore_flags (bool) (optional)
+
+        Modified Keys:
+
+        - img
+        - img_shape
+        - gt_bboxes (optional)
+        - gt_bboxes_labels (optional)
+        - gt_ignore_flags (optional)
 
         Args:
-            results (dict): Result dict.
+            max_rotate_degree (float): Maximum degrees of rotation transform.
+                Defaults to 10.
+            max_translate_ratio (float): Maximum ratio of translation.
+                Defaults to 0.1.
+            scaling_ratio_range (tuple[float]): Min and max ratio of
+                scaling transform. Defaults to (0.5, 1.5).
+            max_shear_degree (float): Maximum degrees of shear
+                transform. Defaults to 2.
+            border (tuple[int]): Distance from width and height sides of input
+                image to adjust output shape. Only used in mosaic dataset.
+                Defaults to (0, 0).
+            border_val (tuple[int]): Border padding values of 3 channels.
+                Defaults to (114, 114, 114).
+            bbox_clip_border (bool, optional): Whether to clip the objects outside
+                the border of the image. In some dataset like MOT17, the gt bboxes
+                are allowed to cross the border of images. Therefore, we don't
+                need to clip the gt bboxes in these cases. Defaults to True.
+        """
+
+        def __init__(
+            self,
+            max_rotate_degree: float = 10.0,
+            max_translate_ratio: float = 0.1,
+            scaling_ratio_range: Tuple[float, float] = (0.5, 1.5),
+            max_shear_degree: float = 2.0,
+            border: Tuple[int, int] = (0, 0),
+            border_val: Tuple[int, int, int] = (114, 114, 114),
+            bbox_clip_border: bool = True,
+        ) -> None:
+            assert 0 <= max_translate_ratio <= 1
+            assert scaling_ratio_range[0] <= scaling_ratio_range[1]
+            assert scaling_ratio_range[0] > 0
+            self.max_rotate_degree = max_rotate_degree
+            self.max_translate_ratio = max_translate_ratio
+            self.scaling_ratio_range = scaling_ratio_range
+            self.max_shear_degree = max_shear_degree
+            self.border = border
+            self.border_val = border_val
+            self.bbox_clip_border = bbox_clip_border
+
+        @cache_randomness
+        def _get_random_homography_matrix(self, height, width):
+            # Rotation
+            rotation_degree = random.uniform(-self.max_rotate_degree, self.max_rotate_degree)
+            rotation_matrix = self._get_rotation_matrix(rotation_degree)
+
+            # Scaling
+            scaling_ratio = random.uniform(self.scaling_ratio_range[0], self.scaling_ratio_range[1])
+            scaling_matrix = self._get_scaling_matrix(scaling_ratio)
+
+            # Shear
+            x_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
+            y_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
+            shear_matrix = self._get_shear_matrix(x_degree, y_degree)
+
+            # Translation
+            trans_x = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * width
+            trans_y = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * height
+            translate_matrix = self._get_translation_matrix(trans_x, trans_y)
+
+            warp_matrix = translate_matrix @ shear_matrix @ rotation_matrix @ scaling_matrix
+            return warp_matrix
+
+        @autocast_box_type()
+        def transform(self, results: dict) -> dict:
+            import cv2  # TODO: support random affine requires cv2
+
+            img = results["img"]
+            height = img.shape[0] + self.border[1] * 2
+            width = img.shape[1] + self.border[0] * 2
+
+            warp_matrix = self._get_random_homography_matrix(height, width)
+
+            img = cv2.warpPerspective(img, warp_matrix, dsize=(width, height), borderValue=self.border_val)
+            results["img"] = img
+            results["img_shape"] = img.shape[:2]
+
+            bboxes = results["gt_bboxes"]
+            num_bboxes = len(bboxes)
+            if num_bboxes:
+                bboxes.project_(warp_matrix)
+                if self.bbox_clip_border:
+                    bboxes.clip_([height, width])
+                # remove outside bbox
+                valid_index = bboxes.is_inside([height, width]).numpy()
+                results["gt_bboxes"] = bboxes[valid_index]
+                results["gt_bboxes_labels"] = results["gt_bboxes_labels"][valid_index]
+                results["gt_ignore_flags"] = results["gt_ignore_flags"][valid_index]
 
-        Returns:
-            dict: Updated result dict.
-        """
-
-        assert "mix_results" in results
-        assert len(results["mix_results"]) == 1, "MixUp only support 2 images now !"
-
-        if results["mix_results"][0]["gt_bboxes"].shape[0] == 0:
-            # empty bbox
+                if "gt_masks" in results:
+                    raise NotImplementedError("RandomAffine only supports bbox.")
             return results
 
-        retrieve_results = results["mix_results"][0]
-        retrieve_img = retrieve_results["img"]
+        def __repr__(self):
+            repr_str = self.__class__.__name__
+            repr_str += f"(max_rotate_degree={self.max_rotate_degree}, "
+            repr_str += f"max_translate_ratio={self.max_translate_ratio}, "
+            repr_str += f"scaling_ratio_range={self.scaling_ratio_range}, "
+            repr_str += f"max_shear_degree={self.max_shear_degree}, "
+            repr_str += f"border={self.border}, "
+            repr_str += f"border_val={self.border_val}, "
+            repr_str += f"bbox_clip_border={self.bbox_clip_border})"
+            return repr_str
+
+        @staticmethod
+        def _get_rotation_matrix(rotate_degrees: float) -> np.ndarray:
+            radian = math.radians(rotate_degrees)
+            rotation_matrix = np.array(
+                [[np.cos(radian), -np.sin(radian), 0.0], [np.sin(radian), np.cos(radian), 0.0], [0.0, 0.0, 1.0]],
+                dtype=np.float32,
+            )
+            return rotation_matrix
 
-        jit_factor = random.uniform(*self.ratio_range)
-        is_filp = random.uniform(0, 1) > self.flip_ratio
+        @staticmethod
+        def _get_scaling_matrix(scale_ratio: float) -> np.ndarray:
+            scaling_matrix = np.array(
+                [[scale_ratio, 0.0, 0.0], [0.0, scale_ratio, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
+            )
+            return scaling_matrix
 
-        if len(retrieve_img.shape) == 3:
-            out_img = (
-                np.ones((self.dynamic_scale[1], self.dynamic_scale[0], 3), dtype=retrieve_img.dtype) * self.pad_val
+        @staticmethod
+        def _get_shear_matrix(x_shear_degrees: float, y_shear_degrees: float) -> np.ndarray:
+            x_radian = math.radians(x_shear_degrees)
+            y_radian = math.radians(y_shear_degrees)
+            shear_matrix = np.array(
+                [[1, np.tan(x_radian), 0.0], [np.tan(y_radian), 1, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
             )
-        else:
-            out_img = np.ones(self.dynamic_scale[::-1], dtype=retrieve_img.dtype) * self.pad_val
+            return shear_matrix
 
-        # 1. keep_ratio resize
-        scale_ratio = min(self.dynamic_scale[1] / retrieve_img.shape[0], self.dynamic_scale[0] / retrieve_img.shape[1])
-        retrieve_img = mmcv.imresize(
-            retrieve_img, (int(retrieve_img.shape[1] * scale_ratio), int(retrieve_img.shape[0] * scale_ratio))
-        )
-
-        # 2. paste
-        out_img[: retrieve_img.shape[0], : retrieve_img.shape[1]] = retrieve_img
-
-        # 3. scale jit
-        scale_ratio *= jit_factor
-        out_img = mmcv.imresize(out_img, (int(out_img.shape[1] * jit_factor), int(out_img.shape[0] * jit_factor)))
-
-        # 4. flip
-        if is_filp:
-            out_img = out_img[:, ::-1, :]
-
-        # 5. random crop
-        ori_img = results["img"]
-        origin_h, origin_w = out_img.shape[:2]
-        target_h, target_w = ori_img.shape[:2]
-        padded_img = np.ones((max(origin_h, target_h), max(origin_w, target_w), 3)) * self.pad_val
-        padded_img = padded_img.astype(np.uint8)
-        padded_img[:origin_h, :origin_w] = out_img
-
-        x_offset, y_offset = 0, 0
-        if padded_img.shape[0] > target_h:
-            y_offset = random.randint(0, padded_img.shape[0] - target_h)
-        if padded_img.shape[1] > target_w:
-            x_offset = random.randint(0, padded_img.shape[1] - target_w)
-        padded_cropped_img = padded_img[y_offset : y_offset + target_h, x_offset : x_offset + target_w]
-
-        # 6. adjust bbox
-        retrieve_gt_bboxes = retrieve_results["gt_bboxes"]
-        retrieve_gt_bboxes.rescale_([scale_ratio, scale_ratio])
-        if self.bbox_clip_border:
-            retrieve_gt_bboxes.clip_([origin_h, origin_w])
-
-        if is_filp:
-            retrieve_gt_bboxes.flip_([origin_h, origin_w], direction="horizontal")
-
-        # 7. filter
-        cp_retrieve_gt_bboxes = retrieve_gt_bboxes.clone()
-        cp_retrieve_gt_bboxes.translate_([-x_offset, -y_offset])
-        if self.bbox_clip_border:
-            cp_retrieve_gt_bboxes.clip_([target_h, target_w])
-
-        # 8. mix up
-        ori_img = ori_img.astype(np.float32)
-        mixup_img = 0.5 * ori_img + 0.5 * padded_cropped_img.astype(np.float32)
-
-        retrieve_gt_bboxes_labels = retrieve_results["gt_bboxes_labels"]
-        retrieve_gt_ignore_flags = retrieve_results["gt_ignore_flags"]
-
-        mixup_gt_bboxes = cp_retrieve_gt_bboxes.cat((results["gt_bboxes"], cp_retrieve_gt_bboxes), dim=0)
-        mixup_gt_bboxes_labels = np.concatenate((results["gt_bboxes_labels"], retrieve_gt_bboxes_labels), axis=0)
-        mixup_gt_ignore_flags = np.concatenate((results["gt_ignore_flags"], retrieve_gt_ignore_flags), axis=0)
-
-        # remove outside bbox
-        inside_inds = mixup_gt_bboxes.is_inside([target_h, target_w]).numpy()
-        mixup_gt_bboxes = mixup_gt_bboxes[inside_inds]
-        mixup_gt_bboxes_labels = mixup_gt_bboxes_labels[inside_inds]
-        mixup_gt_ignore_flags = mixup_gt_ignore_flags[inside_inds]
-
-        results["img"] = mixup_img.astype(np.uint8)
-        results["img_shape"] = mixup_img.shape[:2]
-        results["gt_bboxes"] = mixup_gt_bboxes
-        results["gt_bboxes_labels"] = mixup_gt_bboxes_labels
-        results["gt_ignore_flags"] = mixup_gt_ignore_flags
-
-        return results
-
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += f"(dynamic_scale={self.dynamic_scale}, "
-        repr_str += f"ratio_range={self.ratio_range}, "
-        repr_str += f"flip_ratio={self.flip_ratio}, "
-        repr_str += f"pad_val={self.pad_val}, "
-        repr_str += f"max_iters={self.max_iters}, "
-        repr_str += f"bbox_clip_border={self.bbox_clip_border})"
-        return repr_str
-
-
-class RandomAffine(BaseTransform):
-    """Random affine transform data augmentation.
-
-    This operation randomly generates affine transform matrix which including
-    rotation, translation, shear and scaling transforms.
-
-    Required Keys:
-
-    - img
-    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
-    - gt_bboxes_labels (np.int64) (optional)
-    - gt_ignore_flags (bool) (optional)
-
-    Modified Keys:
-
-    - img
-    - img_shape
-    - gt_bboxes (optional)
-    - gt_bboxes_labels (optional)
-    - gt_ignore_flags (optional)
-
-    Args:
-        max_rotate_degree (float): Maximum degrees of rotation transform.
-            Defaults to 10.
-        max_translate_ratio (float): Maximum ratio of translation.
-            Defaults to 0.1.
-        scaling_ratio_range (tuple[float]): Min and max ratio of
-            scaling transform. Defaults to (0.5, 1.5).
-        max_shear_degree (float): Maximum degrees of shear
-            transform. Defaults to 2.
-        border (tuple[int]): Distance from width and height sides of input
-            image to adjust output shape. Only used in mosaic dataset.
-            Defaults to (0, 0).
-        border_val (tuple[int]): Border padding values of 3 channels.
-            Defaults to (114, 114, 114).
-        bbox_clip_border (bool, optional): Whether to clip the objects outside
-            the border of the image. In some dataset like MOT17, the gt bboxes
-            are allowed to cross the border of images. Therefore, we don't
-            need to clip the gt bboxes in these cases. Defaults to True.
-    """
-
-    def __init__(
-        self,
-        max_rotate_degree: float = 10.0,
-        max_translate_ratio: float = 0.1,
-        scaling_ratio_range: Tuple[float, float] = (0.5, 1.5),
-        max_shear_degree: float = 2.0,
-        border: Tuple[int, int] = (0, 0),
-        border_val: Tuple[int, int, int] = (114, 114, 114),
-        bbox_clip_border: bool = True,
-    ) -> None:
-        assert 0 <= max_translate_ratio <= 1
-        assert scaling_ratio_range[0] <= scaling_ratio_range[1]
-        assert scaling_ratio_range[0] > 0
-        self.max_rotate_degree = max_rotate_degree
-        self.max_translate_ratio = max_translate_ratio
-        self.scaling_ratio_range = scaling_ratio_range
-        self.max_shear_degree = max_shear_degree
-        self.border = border
-        self.border_val = border_val
-        self.bbox_clip_border = bbox_clip_border
-
-    @cache_randomness
-    def _get_random_homography_matrix(self, height, width):
-        # Rotation
-        rotation_degree = random.uniform(-self.max_rotate_degree, self.max_rotate_degree)
-        rotation_matrix = self._get_rotation_matrix(rotation_degree)
-
-        # Scaling
-        scaling_ratio = random.uniform(self.scaling_ratio_range[0], self.scaling_ratio_range[1])
-        scaling_matrix = self._get_scaling_matrix(scaling_ratio)
-
-        # Shear
-        x_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
-        y_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
-        shear_matrix = self._get_shear_matrix(x_degree, y_degree)
-
-        # Translation
-        trans_x = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * width
-        trans_y = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * height
-        translate_matrix = self._get_translation_matrix(trans_x, trans_y)
-
-        warp_matrix = translate_matrix @ shear_matrix @ rotation_matrix @ scaling_matrix
-        return warp_matrix
-
-    @autocast_box_type()
-    def transform(self, results: dict) -> dict:
-        import cv2  # TODO: support random affine requires cv2
-
-        img = results["img"]
-        height = img.shape[0] + self.border[1] * 2
-        width = img.shape[1] + self.border[0] * 2
-
-        warp_matrix = self._get_random_homography_matrix(height, width)
-
-        img = cv2.warpPerspective(img, warp_matrix, dsize=(width, height), borderValue=self.border_val)
-        results["img"] = img
-        results["img_shape"] = img.shape[:2]
-
-        bboxes = results["gt_bboxes"]
-        num_bboxes = len(bboxes)
-        if num_bboxes:
-            bboxes.project_(warp_matrix)
-            if self.bbox_clip_border:
-                bboxes.clip_([height, width])
-            # remove outside bbox
-            valid_index = bboxes.is_inside([height, width]).numpy()
-            results["gt_bboxes"] = bboxes[valid_index]
-            results["gt_bboxes_labels"] = results["gt_bboxes_labels"][valid_index]
-            results["gt_ignore_flags"] = results["gt_ignore_flags"][valid_index]
-
-            if "gt_masks" in results:
-                raise NotImplementedError("RandomAffine only supports bbox.")
-        return results
-
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += f"(max_rotate_degree={self.max_rotate_degree}, "
-        repr_str += f"max_translate_ratio={self.max_translate_ratio}, "
-        repr_str += f"scaling_ratio_range={self.scaling_ratio_range}, "
-        repr_str += f"max_shear_degree={self.max_shear_degree}, "
-        repr_str += f"border={self.border}, "
-        repr_str += f"border_val={self.border_val}, "
-        repr_str += f"bbox_clip_border={self.bbox_clip_border})"
-        return repr_str
-
-    @staticmethod
-    def _get_rotation_matrix(rotate_degrees: float) -> np.ndarray:
-        radian = math.radians(rotate_degrees)
-        rotation_matrix = np.array(
-            [[np.cos(radian), -np.sin(radian), 0.0], [np.sin(radian), np.cos(radian), 0.0], [0.0, 0.0, 1.0]],
-            dtype=np.float32,
-        )
-        return rotation_matrix
-
-    @staticmethod
-    def _get_scaling_matrix(scale_ratio: float) -> np.ndarray:
-        scaling_matrix = np.array(
-            [[scale_ratio, 0.0, 0.0], [0.0, scale_ratio, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
-        )
-        return scaling_matrix
-
-    @staticmethod
-    def _get_shear_matrix(x_shear_degrees: float, y_shear_degrees: float) -> np.ndarray:
-        x_radian = math.radians(x_shear_degrees)
-        y_radian = math.radians(y_shear_degrees)
-        shear_matrix = np.array(
-            [[1, np.tan(x_radian), 0.0], [np.tan(y_radian), 1, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
-        )
-        return shear_matrix
-
-    @staticmethod
-    def _get_translation_matrix(x: float, y: float) -> np.ndarray:
-        translation_matrix = np.array([[1, 0.0, x], [0.0, 1, y], [0.0, 0.0, 1.0]], dtype=np.float32)
-        return translation_matrix
+        @staticmethod
+        def _get_translation_matrix(x: float, y: float) -> np.ndarray:
+            translation_matrix = np.array([[1, 0.0, x], [0.0, 1, y], [0.0, 0.0, 1.0]], dtype=np.float32)
+            return translation_matrix
+
+except Exception as e:
+    MultiImageMixDataset = None
```

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.7.1b20230603/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230602
+Version: 0.7.1b20230603
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -43,27 +43,27 @@
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
         
         | AutoGluon Task      |                                                                                Quickstart                                                                                |                                                                                API                                                                                |
         |:--------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#module-0)                 |
-        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.multimodal.MultiModalPredictor) |
-        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.timeseries.TimeSeriesPredictor) |
+        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.html)                 |
+        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.multimodal.MultiModalPredictor.html) |
+        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.timeseries.TimeSeriesPredictor.html) |
         
         ## Resources
         
-        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for [documentation](https://auto.gluon.ai/stable/api/index.html) and instructions on:
+        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for documentation and instructions on:
         - [Installing AutoGluon](https://auto.gluon.ai/stable/index.html#installation)
-        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html)
-          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
+        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html)
+          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular/tabular-essentials.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
         
-        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)
-        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)
+        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)
+        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)
         
         Refer to the [AutoGluon Roadmap](https://github.com/autogluon/autogluon/blob/master/ROADMAP.md) for details on upcoming features and releases.
         
         ### Scientific Publications
         - [AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data](https://arxiv.org/pdf/2003.06505.pdf) (*Arxiv*, 2020)
         - [Fast, Accurate, and Simple Models for Tabular Data via Augmented Distillation](https://proceedings.neurips.cc/paper/2020/hash/62d75fb2e3075506e8837d8f55021ab1-Abstract.html) (*NeurIPS*, 2020)
         - [Multimodal AutoML on Structured Tables with Text Fields](https://openreview.net/pdf?id=OHAIVOOl7Vl) (*ICML AutoML Workshop*, 2021)
```

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230602/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.7.1b20230603/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
 transformers<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
 sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.7.1b20230602
-autogluon.features==0.7.1b20230602
-autogluon.common==0.7.1b20230602
+autogluon.core[raytune]==0.7.1b20230603
+autogluon.features==0.7.1b20230603
+autogluon.common==0.7.1b20230603
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

