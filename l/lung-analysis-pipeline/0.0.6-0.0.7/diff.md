# Comparing `tmp/lung_analysis_pipeline-0.0.6.tar.gz` & `tmp/lung_analysis_pipeline-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lung_analysis_pipeline-0.0.6.tar", last modified: Sat Jun  3 20:24:48 2023, max compression
+gzip compressed data, was "dist/lung_analysis_pipeline-0.0.7.tar", last modified: Sun Jun  4 21:52:53 2023, max compression
```

## Comparing `lung_analysis_pipeline-0.0.6.tar` & `lung_analysis_pipeline-0.0.7.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/
--rw-r-----   0 root         (0) root         (0)     5399 2023-05-30 21:56:05.000000 lung_analysis_pipeline-0.0.6/README.md
--rw-r-----   0 root         (0) root         (0)        0 2023-06-01 18:50:05.000000 lung_analysis_pipeline-0.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/radiomics/
--rw-r-----   0 root         (0) root         (0)     6379 2023-06-03 20:19:42.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/radiomics/feature_extractor.py
--rw-r-----   0 root         (0) root         (0)        0 2023-05-30 23:16:38.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/radiomics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/HSCNN/
--rwxrwxrwx   0 root         (0) root         (0)     4877 2023-04-25 19:19:37.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/HSCNN/dataloader.py
--rwxrwxrwx   0 root         (0) root         (0)    23021 2023-04-25 19:23:54.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/HSCNN/train.py
--rwxrwxrwx   0 root         (0) root         (0)    13371 2023-06-01 17:45:50.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/HSCNN/model.py
--rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:33:34.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/HSCNN/__init__.py
--rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:32:08.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/
--rwxr-x---   0 root         (0) root         (0)      510 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluation_updt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/dataset/
--rwxr-x---   0 root         (0) root         (0)    17508 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader.py
--rwxr-x---   0 root         (0) root         (0)    19594 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader_UCLA.py
--rwxr-x---   0 root         (0) root         (0)      862 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/dataset/collate.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/dataset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/
--rwxr-x---   0 root         (0) root         (0)    27640 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/noduleCADEvaluationLUNA16.py
--rwxr-x---   0 root         (0) root         (0)      672 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/NoduleFinding.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/
--rwxr-x---   0 root         (0) root         (0)      791 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/csvTools.py
--rwxr-x---   0 root         (0) root         (0)      130 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/__init__.py
--rwxr-x---   0 root         (0) root         (0)     8924 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/test_normCnd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/utils/
--rwxr-x---   0 root         (0) root         (0)    17889 2023-05-30 03:19:49.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/utils/util.py
--rwxr-x---   0 root         (0) root         (0)     1474 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/utils/pybox.py
--rwxr-x---   0 root         (0) root         (0)     3777 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/utils/prepare_dataset_UCLA.py
--rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:34:25.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/utils/__init__.py
--rwxr-x---   0 root         (0) root         (0)    15175 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/
--rwxr-x---   0 root         (0) root         (0)     8483 2023-05-30 01:41:42.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/resnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/
--rwxr-x---   0 root         (0) root         (0)      799 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/build.py
--rwxr-x---   0 root         (0) root         (0)     1530 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/extension/
--rwxr-x---   0 root         (0) root         (0)      383 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/extension/__init__.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/__init__.py
--rwxr-x---   0 root         (0) root         (0)     1177 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/py_nms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/
--rwxr-x---   0 root         (0) root         (0)      819 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/build.py
--rwxr-x---   0 root         (0) root         (0)     1186 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/
--rwxr-x---   0 root         (0) root         (0)      383 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/__init__.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/__init__.py
--rwxr-x---   0 root         (0) root         (0)       83 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/__init__.py
--rwxr-x---   0 root         (0) root         (0)     9886 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/process.py
--rwxr-x---   0 root         (0) root         (0)     8351 2023-05-30 03:05:06.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/cgnl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/
--rwxr-x---   0 root         (0) root         (0)     7357 2023-05-30 01:47:56.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_target.py
--rwxr-x---   0 root         (0) root         (0)     7120 2023-05-30 01:47:31.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_target.py
--rwxr-x---   0 root         (0) root         (0)     2424 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/util.py
--rwxr-x---   0 root         (0) root         (0)     5208 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_loss.py
--rwxr-x---   0 root         (0) root         (0)     2051 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_loss.py
--rwxr-x---   0 root         (0) root         (0)     5526 2023-05-30 22:39:08.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_nms.py
--rwxr-x---   0 root         (0) root         (0)     3534 2023-05-30 01:37:59.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_nms.py
--rwxr-x---   0 root         (0) root         (0)      169 2023-05-30 01:28:27.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/__init__.py
--rwxr-x---   0 root         (0) root         (0)    20689 2023-06-01 00:01:31.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/sanet.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/__init__.py
--rw-r-----   0 root         (0) root         (0)      648 2023-06-01 17:47:29.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/__init__.py
--rwxr-x---   0 root         (0) root         (0)     5536 2023-05-30 04:31:32.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/test.py
--rwxr-x---   0 root         (0) root         (0)     3891 2023-05-30 20:36:19.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/options/
--rw-r-----   0 root         (0) root         (0)     5834 2023-06-01 17:43:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/options/opt.py
--rw-r-----   0 root         (0) root         (0)        0 2023-04-13 03:10:53.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/options/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/
--rwxrwxrwx   0 root         (0) root         (0)     8249 2023-05-02 00:42:08.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/niiDataset_with_label.py
--rwxrwxrwx   0 root         (0) root         (0)     2996 2023-05-02 00:42:33.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/h5Dataset_with_label.py
--rw-r-----   0 root         (0) root         (0)     2248 2023-05-02 00:42:21.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/DcmDataset.py
--rwxrwxrwx   0 root         (0) root         (0)    12951 2023-05-30 03:19:35.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/util.py
--rwxrwxrwx   0 root         (0) root         (0)     2299 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/dcmDataset.py
--rwxrwxrwx   0 root         (0) root         (0)     6704 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/h5Dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     5989 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/LRHR_dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     1777 2023-05-02 00:25:16.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8194 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/tmp_with_label.py
--rw-r-----   0 root         (0) root         (0)     5868 2023-06-01 05:17:54.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/nlstDataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/
--rwxrwxrwx   0 root         (0) root         (0)     4007 2023-05-23 21:08:59.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/bm3d_ht.py
--rwxrwxrwx   0 root         (0) root         (0)     3521 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/histogram_matching.py
--rw-r-----   0 root         (0) root         (0)        0 2023-04-21 04:31:56.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5268 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/compute_metrics.py
--rwxrwxrwx   0 root         (0) root         (0)     8024 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_ExternalFolder.py
--rwxrwxrwx   0 root         (0) root         (0)     3262 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_SingleVol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/options/
--rwxrwxrwx   0 root         (0) root         (0)     3917 2023-04-15 00:33:07.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/options/options.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/options/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/
--rwxrwxrwx   0 root         (0) root         (0)     8100 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm.py
--rwxrwxrwx   0 root         (0) root         (0)     9697 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_img_files.py
--rwxrwxrwx   0 root         (0) root         (0)      775 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/make_uids.py
--rwxrwxrwx   0 root         (0) root         (0)     1210 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_uids_for_cv.py
--rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/get_log_values.py
--rwxrwxrwx   0 root         (0) root         (0)    20002 2023-04-19 18:34:56.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/util.py
--rwxrwxrwx   0 root         (0) root         (0)     5395 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-RetinaNet.py
--rwxrwxrwx   0 root         (0) root         (0)     6686 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/batch_hr2Toh5.py
--rwxrwxrwx   0 root         (0) root         (0)      590 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/read_tensorboard.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3214 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_aapm.py
--rwxrwxrwx   0 root         (0) root         (0)     4344 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/segment_lungs.py
--rwxrwxrwx   0 root         (0) root         (0)     5201 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm_uids.py
--rwxrwxrwx   0 root         (0) root         (0)     2277 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/progress_bar.py
--rwxrwxrwx   0 root         (0) root         (0)    13690 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/train.py
--rwxrwxrwx   0 root         (0) root         (0)     2298 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/visualize_cases.py
--rw-r-----   0 root         (0) root         (0)        0 2023-05-02 03:43:26.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/
--rwxrwxrwx   0 root         (0) root         (0)    38696 2023-05-23 03:54:12.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_model.py
--rwxrwxrwx   0 root         (0) root         (0)     5731 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/lr_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/
--rwxrwxrwx   0 root         (0) root         (0)    29138 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/generators.py
--rwxrwxrwx   0 root         (0) root         (0)     7171 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/auxiliary_features.py
--rwxrwxrwx   0 root         (0) root         (0)     3367 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/loss.py
--rwxrwxrwx   0 root         (0) root         (0)     7002 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/block.py
--rwxrwxrwx   0 root         (0) root         (0)    16771 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/discriminators.py
--rwxrwxrwx   0 root         (0) root         (0)     2884 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/bam.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9406 2023-05-02 00:27:09.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/networks.py
--rwxrwxrwx   0 root         (0) root         (0)     3590 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/build_unet_model.py
--rwxrwxrwx   0 root         (0) root         (0)    12140 2023-05-23 03:54:04.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SR_model.py
--rwxrwxrwx   0 root         (0) root         (0)    22520 2023-05-23 03:54:07.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_exp.py
--rwxrwxrwx   0 root         (0) root         (0)     3892 2023-06-01 18:44:23.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11424 2023-05-22 22:39:50.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/
--rwxrwxrwx   0 root         (0) root         (0)      805 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/
--rwxrwxrwx   0 root         (0) root         (0)     2023 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/html.py
--rwxrwxrwx   0 root         (0) root         (0)    14226 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/util.py
--rwxrwxrwx   0 root         (0) root         (0)     8602 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1823 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists_dirs.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/
--rwxrwxrwx   0 root         (0) root         (0)     7544 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/pretrained_networks.py
--rwxrwxrwx   0 root         (0) root         (0)    14721 2023-04-14 19:07:07.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/dist_model.py
--rwxrwxrwx   0 root         (0) root         (0)      269 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/models.py
--rwxrwxrwx   0 root         (0) root         (0)    11713 2023-04-14 19:06:50.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/networks_basic.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1750 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/base_model.py
--rwxrwxrwx   0 root         (0) root         (0)     7630 2023-04-22 02:44:06.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/test.py
--rw-r-----   0 root         (0) root         (0)        0 2023-05-02 03:35:30.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/utils/
--rw-r-----   0 root         (0) root         (0)    28571 2023-06-01 04:23:01.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/utils/util.py
--rw-r-----   0 root         (0) root         (0)        0 2023-04-21 21:06:41.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/utils/__init__.py
--rw-r-----   0 root         (0) root         (0)    25935 2023-05-31 04:26:32.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/utils/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/
--rwxrwxrwx   0 root         (0) root         (0)    11011 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/train_unet_lidc.py
--rwxrwxrwx   0 root         (0) root         (0)     2301 2023-04-25 21:29:27.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_lidc.py
--rwxrwxrwx   0 root         (0) root         (0)     5448 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_resnet34_lidc.py
--rwxrwxrwx   0 root         (0) root         (0)     5823 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/train.py
--rwxrwxrwx   0 root         (0) root         (0)     3612 2023-04-28 20:34:39.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/setting.py
--rwxrwxrwx   0 root         (0) root         (0)     4368 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/model.py
--rwxrwxrwx   0 root         (0) root         (0)     6904 2023-06-01 17:45:20.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py
--rw-r-----   0 root         (0) root         (0)        0 2023-05-30 01:25:50.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3346 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/test.py
--rwxrwxrwx   0 root         (0) root         (0)     3482 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_norm.py
--rw-r-----   0 root         (0) root         (0)     3923 2023-06-01 17:44:25.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/model_pipeline.py
--rw-r-----   0 root         (0) root         (0)     1708 2023-05-30 04:43:18.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/__init__.py
--rw-r-----   0 root         (0) root         (0)      718 2023-06-03 20:24:38.000000 lung_analysis_pipeline-0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9190 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-03 20:24:48.000000 lung_analysis_pipeline-0.0.6/lung_analysis_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/
+-rw-r-----   0 root         (0) root         (0)     5399 2023-05-30 21:56:05.000000 lung_analysis_pipeline-0.0.7/README.md
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-01 18:50:05.000000 lung_analysis_pipeline-0.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/radiomics/
+-rw-r-----   0 root         (0) root         (0)     6763 2023-06-04 21:44:18.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/radiomics/feature_extractor.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-05-30 23:16:38.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/radiomics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/HSCNN/
+-rwxrwxrwx   0 root         (0) root         (0)     4877 2023-04-25 19:19:37.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/HSCNN/dataloader.py
+-rwxrwxrwx   0 root         (0) root         (0)    23021 2023-04-25 19:23:54.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/HSCNN/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    13467 2023-06-04 21:24:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/HSCNN/model.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:33:34.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/HSCNN/__init__.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:32:08.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/
+-rwxr-x---   0 root         (0) root         (0)      510 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluation_updt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/dataset/
+-rwxr-x---   0 root         (0) root         (0)    17508 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader.py
+-rwxr-x---   0 root         (0) root         (0)    19594 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader_UCLA.py
+-rwxr-x---   0 root         (0) root         (0)      862 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/dataset/collate.py
+-rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/dataset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/
+-rwxr-x---   0 root         (0) root         (0)    27640 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/noduleCADEvaluationLUNA16.py
+-rwxr-x---   0 root         (0) root         (0)      672 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/NoduleFinding.py
+-rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/
+-rwxr-x---   0 root         (0) root         (0)      791 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/csvTools.py
+-rwxr-x---   0 root         (0) root         (0)      130 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/__init__.py
+-rwxr-x---   0 root         (0) root         (0)     8924 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/test_normCnd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/utils/
+-rwxr-x---   0 root         (0) root         (0)    17889 2023-05-30 03:19:49.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/utils/util.py
+-rwxr-x---   0 root         (0) root         (0)     1474 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/utils/pybox.py
+-rwxr-x---   0 root         (0) root         (0)     3777 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/utils/prepare_dataset_UCLA.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:34:25.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/utils/__init__.py
+-rwxr-x---   0 root         (0) root         (0)    15175 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/
+-rwxr-x---   0 root         (0) root         (0)     8483 2023-05-30 01:41:42.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/resnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/
+-rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/
+-rwxr-x---   0 root         (0) root         (0)      799 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/build.py
+-rwxr-x---   0 root         (0) root         (0)     1530 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/extension/
+-rwxr-x---   0 root         (0) root         (0)      383 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/extension/__init__.py
+-rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/__init__.py
+-rwxr-x---   0 root         (0) root         (0)     1177 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/py_nms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/
+-rwxr-x---   0 root         (0) root         (0)      819 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/build.py
+-rwxr-x---   0 root         (0) root         (0)     1186 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/
+-rwxr-x---   0 root         (0) root         (0)      383 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/__init__.py
+-rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/__init__.py
+-rwxr-x---   0 root         (0) root         (0)       83 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/__init__.py
+-rwxr-x---   0 root         (0) root         (0)     9886 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/process.py
+-rwxr-x---   0 root         (0) root         (0)     8351 2023-05-30 03:05:06.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/cgnl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/
+-rwxr-x---   0 root         (0) root         (0)     7357 2023-05-30 01:47:56.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_target.py
+-rwxr-x---   0 root         (0) root         (0)     7120 2023-05-30 01:47:31.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_target.py
+-rwxr-x---   0 root         (0) root         (0)     2424 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/util.py
+-rwxr-x---   0 root         (0) root         (0)     5208 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_loss.py
+-rwxr-x---   0 root         (0) root         (0)     2051 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_loss.py
+-rwxr-x---   0 root         (0) root         (0)     5526 2023-05-30 22:39:08.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_nms.py
+-rwxr-x---   0 root         (0) root         (0)     3534 2023-05-30 01:37:59.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_nms.py
+-rwxr-x---   0 root         (0) root         (0)      169 2023-05-30 01:28:27.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/__init__.py
+-rwxr-x---   0 root         (0) root         (0)    20642 2023-06-03 22:05:06.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/sanet.py
+-rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/__init__.py
+-rw-r-----   0 root         (0) root         (0)      650 2023-06-03 22:47:27.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/__init__.py
+-rwxr-x---   0 root         (0) root         (0)     5536 2023-05-30 04:31:32.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/test.py
+-rwxr-x---   0 root         (0) root         (0)     3891 2023-05-30 20:36:19.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/options/
+-rw-r-----   0 root         (0) root         (0)     6803 2023-06-04 21:45:09.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/options/opt.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-04-13 03:10:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/options/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/
+-rwxrwxrwx   0 root         (0) root         (0)     8249 2023-05-02 00:42:08.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/niiDataset_with_label.py
+-rwxrwxrwx   0 root         (0) root         (0)     2996 2023-05-02 00:42:33.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/h5Dataset_with_label.py
+-rw-r-----   0 root         (0) root         (0)     3094 2023-06-04 20:45:17.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/DcmDataset.py
+-rwxrwxrwx   0 root         (0) root         (0)    12951 2023-05-30 03:19:35.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     2299 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/dcmDataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     6704 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/h5Dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     5989 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/LRHR_dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     1771 2023-06-04 20:29:39.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8194 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/tmp_with_label.py
+-rw-r-----   0 root         (0) root         (0)     5917 2023-06-04 20:58:54.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/nlstDataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/
+-rwxrwxrwx   0 root         (0) root         (0)     4126 2023-06-03 22:09:51.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/bm3d_ht.py
+-rwxrwxrwx   0 root         (0) root         (0)     3521 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/histogram_matching.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-04-21 04:31:56.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5268 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/compute_metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)     8024 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_ExternalFolder.py
+-rwxrwxrwx   0 root         (0) root         (0)     3262 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_SingleVol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/options/
+-rwxrwxrwx   0 root         (0) root         (0)     3917 2023-04-15 00:33:07.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/options/options.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/options/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/
+-rwxrwxrwx   0 root         (0) root         (0)     8100 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm.py
+-rwxrwxrwx   0 root         (0) root         (0)     9697 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_img_files.py
+-rwxrwxrwx   0 root         (0) root         (0)      775 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/make_uids.py
+-rwxrwxrwx   0 root         (0) root         (0)     1210 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_uids_for_cv.py
+-rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/get_log_values.py
+-rwxrwxrwx   0 root         (0) root         (0)    20002 2023-04-19 18:34:56.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     5395 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-RetinaNet.py
+-rwxrwxrwx   0 root         (0) root         (0)     6686 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/batch_hr2Toh5.py
+-rwxrwxrwx   0 root         (0) root         (0)      590 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/read_tensorboard.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3214 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_aapm.py
+-rwxrwxrwx   0 root         (0) root         (0)     4344 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/segment_lungs.py
+-rwxrwxrwx   0 root         (0) root         (0)     5201 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm_uids.py
+-rwxrwxrwx   0 root         (0) root         (0)     2277 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/progress_bar.py
+-rwxrwxrwx   0 root         (0) root         (0)    13690 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/train.py
+-rwxrwxrwx   0 root         (0) root         (0)     2298 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/visualize_cases.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-05-02 03:43:26.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/
+-rwxrwxrwx   0 root         (0) root         (0)    38696 2023-05-23 03:54:12.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     5731 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/lr_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/
+-rwxrwxrwx   0 root         (0) root         (0)    29138 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/generators.py
+-rwxrwxrwx   0 root         (0) root         (0)     7171 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/auxiliary_features.py
+-rwxrwxrwx   0 root         (0) root         (0)     3367 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)     7002 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/block.py
+-rwxrwxrwx   0 root         (0) root         (0)    16771 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/discriminators.py
+-rwxrwxrwx   0 root         (0) root         (0)     2884 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/bam.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9406 2023-05-02 00:27:09.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/networks.py
+-rwxrwxrwx   0 root         (0) root         (0)     3590 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/build_unet_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    12140 2023-05-23 03:54:04.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SR_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    22520 2023-05-23 03:54:07.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_exp.py
+-rwxrwxrwx   0 root         (0) root         (0)     3892 2023-06-01 18:44:23.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11424 2023-05-22 22:39:50.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/
+-rwxrwxrwx   0 root         (0) root         (0)      805 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/
+-rwxrwxrwx   0 root         (0) root         (0)     2023 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/html.py
+-rwxrwxrwx   0 root         (0) root         (0)    14226 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     8602 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1823 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists_dirs.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/
+-rwxrwxrwx   0 root         (0) root         (0)     7544 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/pretrained_networks.py
+-rwxrwxrwx   0 root         (0) root         (0)    14721 2023-04-14 19:07:07.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/dist_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      269 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/models.py
+-rwxrwxrwx   0 root         (0) root         (0)    11713 2023-04-14 19:06:50.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/networks_basic.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1750 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/base_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     7630 2023-04-22 02:44:06.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/test.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-05-02 03:35:30.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/utils/
+-rw-r-----   0 root         (0) root         (0)    29361 2023-06-04 21:17:38.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/utils/util.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-04-21 21:06:41.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/utils/__init__.py
+-rw-r-----   0 root         (0) root         (0)    25935 2023-05-31 04:26:32.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/utils/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/
+-rwxrwxrwx   0 root         (0) root         (0)    11011 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/train_unet_lidc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2301 2023-04-25 21:29:27.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_lidc.py
+-rwxrwxrwx   0 root         (0) root         (0)     5448 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_resnet34_lidc.py
+-rwxrwxrwx   0 root         (0) root         (0)     5823 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/train.py
+-rwxrwxrwx   0 root         (0) root         (0)     3612 2023-04-28 20:34:39.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/setting.py
+-rwxrwxrwx   0 root         (0) root         (0)     4368 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/model.py
+-rwxrwxrwx   0 root         (0) root         (0)     9258 2023-06-03 23:04:01.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-05-30 01:25:50.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3346 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/test.py
+-rwxrwxrwx   0 root         (0) root         (0)     3482 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_norm.py
+-rw-r-----   0 root         (0) root         (0)     3197 2023-06-04 21:41:39.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/model_pipeline.py
+-rw-r-----   0 root         (0) root         (0)     1708 2023-05-30 04:43:18.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/__init__.py
+-rw-r-----   0 root         (0) root         (0)      718 2023-06-04 21:52:39.000000 lung_analysis_pipeline-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9190 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-04 21:52:53.000000 lung_analysis_pipeline-0.0.7/lung_analysis_pipeline.egg-info/top_level.txt
```

### Comparing `lung_analysis_pipeline-0.0.6/README.md` & `lung_analysis_pipeline-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/radiomics/feature_extractor.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/radiomics/feature_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,16 +126,24 @@
             z, y, x = np.where(component_mask)
             start_z, end_z = np.min(z), np.max(z) + 1
             start_y, end_y = np.min(y), np.max(y) + 1
             start_x, end_x = np.min(x), np.max(x) + 1
 
             roi = image[start_z:end_z, start_y:end_y, start_x:end_x]
             roi_mask = mask[start_z:end_z, start_y:end_y, start_x:end_x]
+            
+            roi_size = np.count_nonzero(roi_mask)
 
+            # Check the size of the ROI by the number of voxels and continue if it's less than the threshold
+            if roi_size < threshold_size:
+                continue
             # Extract features from the ROI
+            # print(roi.min())
+            # print(roi.max())
+            # print(f'{start_z}, {end_z}, {start_y}, {end_y}, {start_x}, {end_x}')
             feature = self.extractor.execute(sitk.GetImageFromArray(roi), sitk.GetImageFromArray(roi_mask))
             feature['NoduleFeatureID'] = f"{uid}-{i-1}"
             feature.move_to_end('NoduleFeatureID', last=False)
 
             features.append(util.convert_numpy_to_list(feature))
         
         input_data['radiomics'] = features
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/HSCNN/dataloader.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/HSCNN/dataloader.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/HSCNN/train.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/HSCNN/train.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Feature_Extractor/HSCNN/model.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Feature_Extractor/HSCNN/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,21 +187,18 @@
         feature = self.final_layer[0](final_layer_input) 
         return feature
 
     def run_test(self, input_data, roi, threshold_size=0): 
         
         with torch.no_grad():
             self.eval()
-            if roi == 'user' or roi == 'segmentation': 
-                if roi == 'segmentation': 
-                    mask = input_data['seg_mask'][0].cpu()
-                else: 
-                    mask = input_data['gt_mask'][0].cpu()
-                
+            if roi == 'segmentation': 
+                mask = input_data['seg_mask'][0].cpu()
                 image = input_data['volume'][0][0].cpu()
+
                 labeled_mask, num_components = measure.label(mask, return_num=True)
 
                 features = []
                 # Iterate over each labeled component
                 for i in range(1, num_components + 1):
                     # Extract the binary mask for the current component
                     component_mask = (labeled_mask == i)
@@ -243,24 +240,29 @@
                     # Resize ROI 
                     roi = util.resize_image(roi, size=(52,52,52))
                     roi = torch.from_numpy(roi)[None,None].cuda()
 
                     # Extract features from the ROI 
                     feature = self._extract_features(roi) 
                     features.append(feature)
-
-                # roi_centroids = detection_bboxes[:,1:4] # z, y, x
                 
-                # features = []
-                # for roi_centroid in roi_centroids:
-                #     roi = torch.from_numpy(util.extract_roi(image, roi_centroid)).cuda()
-                    
-                #     # Extract features from the ROI 
-                #     feature = self._extract_features(roi)
-                #     features.append(feature)
+                features = torch.cat(features, axis=0)
+                input_data['deep_feature'] = features
+                
+                return input_data 
+
+            elif roi == 'user': # user provided coordinates 
+                image = input_data['volume'][0][0].cpu()
+                centroids = input_data['feature_roi_centroids'][0] 
+                features = [] 
+                for roi_centroid in centroids:
+                    roi = torch.from_numpy(util.extract_roi(image, roi_centroid)).cuda()
+                    feature = self._extract_features(roi[None,None])
+                    # TODO: check if features are Nan
+                    features.append(feature)
                 features = torch.cat(features, axis=0)
                 input_data['deep_feature'] = features
                 return input_data
 
 def create_feat_extractor(opt): 
     # check if the specified model is supported 
     if opt['feature_extraction']['deep_feature']['model'] != 'hscnn':
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader_UCLA.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader_UCLA.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/dataset/collate.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/dataset/collate.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/noduleCADEvaluationLUNA16.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/noduleCADEvaluationLUNA16.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/NoduleFinding.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/NoduleFinding.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/csvTools.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/csvTools.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/test_normCnd.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/test_normCnd.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/utils/util.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/utils/util.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/utils/pybox.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/utils/pybox.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/utils/prepare_dataset_UCLA.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/utils/prepare_dataset_UCLA.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/train.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/train.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/resnet.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/resnet.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/build.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/build.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/__init__.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/__init__.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/py_nms.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/py_nms.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/build.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/build.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/__init__.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/__init__.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/process.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/process.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/cgnl.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/cgnl.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_target.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_target.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_target.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_target.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/util.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/util.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_loss.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_loss.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_loss.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_loss.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_nms.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_nms.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_nms.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_nms.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/net/sanet.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/net/sanet.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,15 +425,15 @@
         self.use_rcnn = True 
 
         # preprocess the volume 
         inputs = input_data['volume']
         inputs = inputs.cuda()
 
         inputs = pad2factor(inputs[0,0].cpu().numpy()) # padding is required for SANet 
-        inputs = rescale_image(inputs, min_value=-1, max_value=1) # input image might be (0,1500) or (0,1). Need to rescale to (-1,1)
+        inputs = rescale_image(inputs, min_value=-1, max_value=1) #  rescale to [-1,1]
         inputs = torch.from_numpy(inputs)[None,None].cuda()
         
         # try: 
         with torch.no_grad(): 
             self.forward(inputs, None, None)
         detections = self.rpn_proposals.cpu().numpy() 
         if len(detections) == 0:
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/__init__.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def create_detect_model(opt): 
     # define config 
 
     # load pre-trained model 
     # path_to_weight = 'model.ckpt'
     # path_to_weight = pkg_resources.resource_filename(__name__, path_to_weight)
-    path_to_weight = opt['detection']['model']
+    path_to_weight = opt['detection']['weights']
     
     checkpoint = torch.load(path_to_weight)
     model = SANet(config)
     model.cuda()
     model.load_state_dict(checkpoint['state_dict'])
     logger.info('Nodule detection model {:s} is created.'.format(model.__class__.__name__))
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/test.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/test.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleDetect_SANet/config.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleDetect_SANet/config.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/options/opt.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/options/opt.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     opt = json.loads(json_str, object_pairs_hook=OrderedDict)
 
     check_order(opt)
 
     # results_root = opt['output']['output_location']
     # opt['output']['log'] = results_root
     # util.mkdir(results_root) 
-
+    if not 'output' in opt: 
+        raise ValueError('Need to specify an output location.')
     # For feature extraction, redirect to another file if the output path already exists 
     # for operation in ['feature_extraction', 'detection']:
     if 'feature_extraction' in opt: 
         for extractor in ['deep_feature', 'radiomics']:
             if extractor in opt['feature_extraction']:  
                 opt['feature_extraction'][extractor]['output_path'] and os.path.exists(opt['feature_extraction'][extractor]['output_path'])
                 filename = os.path.basename(opt['feature_extraction'][extractor]['output_path'])
@@ -68,15 +69,15 @@
     order = opt['order']
     for i, ops in enumerate(order): 
         if ops not in opt:
             raise ValueError('Please specify {} operation.'.format(ops))
         if ops == 'normalization': 
             if i != 0: 
                 raise ValueError('Normalization operation order not supported!')
-            if opt[ops]['model'] == 'bm3d' or "weights" not in opt[ops]: 
+            if opt[ops]['model'] != 'bm3d' and "weights" not in opt[ops]: 
                 raise ValueError('Need to specify path to normalization model weights.')
         elif ops == 'detection': 
             if "weights" not in opt[ops]: 
                 raise ValueError('Need to specify path to detection model weights.')
         elif ops == 'segmentation': 
             # there has to exist detection before seg or use detection is set to false 
             if opt[ops]['use_decetion_bbox'] and not 'detection' in order[:i]: 
@@ -89,20 +90,33 @@
             if 'weights' not in opt[ops]: 
                 raise ValueError('Need to specify path to segmentation model weights.')
         elif ops == 'feature_extraction': 
             if 'roi_source' not in opt[ops]:
                 raise ValueError('Segmentation operation order not supported! Need to specify source of ROI.')
             if opt[ops]['roi_source'] == 'segmentation' and not 'segmentation' in order[:i]: 
                 raise ValueError('Feature extraction order not supported. Need to specify a segmentation method.')
+            if opt[ops]['roi_source'] == 'segmentation' and opt['segmentation']['use_decetion_bbox']: 
+                raise NotImplementedError('Feature extraction with segmentation dependent on detection is not implemented.')
             if opt[ops]['roi_source'] == 'detection' and not 'detection' in order[:i]: 
                 raise ValueError('Feature extraction order not supported. Need to specify a detection method.')
-            if opt[ops]['roi_source'] == 'user' and 'feature_roi_centroid' not in opt['dataset']: 
-                raise ValueError('Feature extraction order not supported. Need to specify a ROI location.')
-            if opt[ops]['roi_source'] == 'user' and 'feature_mask' not in opt['dataset']: 
-                raise ValueError('Feature extraction order not supported. Need to specify a mask location.')
-            if opt[ops]['deep_feature']: 
+            # if opt[ops]['roi_source'] == 'user' and 'feature_roi_centroid' not in opt['dataset']: 
+            #     raise ValueError('Feature extraction order not supported. Need to specify a ROI location.')
+            # if opt[ops]['roi_source'] == 'user' and 'feature_mask' not in opt['dataset']: 
+            #     raise ValueError('Feature extraction order not supported. Need to specify a mask location.')
+            
+            if opt[ops]['roi_source'] == 'user': 
+                if 'deep_feature' in opt[ops] and 'feature_roi_centroid' not in opt['dataset']: 
+                    raise ValueError('Feature extraction not supported. Need to specify a ROI location.')
+                if 'radiomics' in opt[ops] and 'feature_mask' not in opt['dataset']: 
+                    raise ValueError('Feature extraction not supported. Need to specify a mask location.')
+
+            if not 'deep_feature' in opt[ops] and not 'radiomics' in opt[ops]: 
+                raise ValueError('Need to specify at least one feature extractor.')
+            if 'deep_feature' in opt[ops]: 
                 if 'model' not in opt[ops]['deep_feature']: 
                     raise ValueError('Need to specify a deep learning model for feature extraction.')
                 if opt[ops]['deep_feature']['model'] != 'hscnn': 
                     raise ValueError('Deep feature extraction model not supported.')
                 if 'weights' not in opt[ops]['deep_feature']: 
-                    raise ValueError('Need to specify path to deep feature extraction model weights.')
+                    raise ValueError('Need to specify path to deep feature extraction model weights.')
+
+
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/niiDataset_with_label.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/niiDataset_with_label.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/h5Dataset_with_label.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/h5Dataset_with_label.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/DcmDataset.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/DcmDataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,23 @@
         if self.opt['phase'] == 'train' or (self.opt['phase'] =='val' and self.opt['need_voxels']):
             self.ps = (self.opt['LR_slice_size'], self.opt['LR_size'], self.opt['LR_size'])
          
         self.paths = []
         for dirpath, dirnames, filenames in os.walk(self.in_folder):
             if any(f.endswith('.dcm') for f in filenames) and 'Contours' not in dirpath:
                 self.paths.append(dirpath)
+       
+        # feature extraction ROI 
+        if opt['feature_roi_centroid']:
+            with open(opt['feature_roi_centroid'], 'r') as json_file:
+                self.feature_roi = json.load(json_file)
+        if opt['feature_mask']:
+            with open(opt['feature_mask'], 'r') as json_file: 
+                self.img_to_mask_path = json.load(json_file)
+
 
         self.scale = self.opt['scale']
         self.ToTensor = util.ImgToTensor()
 
     def __len__(self):
         return len(self.paths)
 
@@ -37,20 +46,30 @@
         slices = [pydicom.dcmread(f) for f in dcm_files]
         volume = np.stack([slice.pixel_array for slice in slices], axis=0).astype(np.float16)
 
         # creates an extra dimension. e.g. 32x64x64 becomes 1x32x64x64
         volume = np.expand_dims(volume, axis=0)
 
         # convert to tensors and also within a certain range of values as defined in 'self.ToTensor()' class
-        volume = self.ToTensor(volume, clip=True, raw_data_range=1500.)
+        transformed_vol = self.ToTensor(volume, clip=True, raw_data_range=1500.)
 
         # generate a volume id 
         patient_id = slices[0].PatientID.replace("_", "-")
         timepoint = slices[0].StudyDate
         series_instance_uid = slices[0].SeriesInstanceUID
         modality = slices[0].Modality 
         volume_id = f"{patient_id}_{timepoint}_{series_instance_uid}_{modality}"
 
         # HR and mask are not allowed to be None. Passing vol_in. 
-        out_dict = {'LR': volume, 'HR': volume, 'mask': volume, 'spacings': [], 'uid': volume_id, 'input_info': {}}
+        out_dict = {'original_vol_in': torch.from_numpy(original_vol_in), 'LR': transformed_vol, 'spacings': [], 'uid': volume_id}
+
+        # load ROI centroids for feature extraction if provided 
+        feature_rois = []
+        if hasattr(self, 'feature_roi'): 
+            feature_rois = self.feature_roi[data_dir_path]
+            feature_rois = torch.tensor(feature_rois)
+            out_dict['feature_roi_centroids'] = feature_rois
+        # if hasattr(self, 'img_to_mask_path'): 
+        #     gt_mask = self.load_masks(mask_dir_path)
+        #     out_dict['gt_mask'] = gt_mask 
 
         return out_dict
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/util.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/util.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/dcmDataset.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/dcmDataset.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/h5Dataset.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/h5Dataset.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/LRHR_dataset.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/LRHR_dataset.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/__init__.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 Create Dataset object for dataloader
 """
 def create_dataset(dataset_opt):
     # import dataset class depending on 'data_type'
     if dataset_opt['image_type'] == 'h5':
         from .h5Dataset_with_label import h5Dataset as D
     elif dataset_opt['image_type'] == 'dicom':
-        # from .DcmDataset import dcmDataset as D
-        from .nlstDataset import dcmDataset as D
-    elif dataset_opt['image_type'] == 'nii':
-        from .niiDataset_with_label import NIIDataset as D
+        from .DcmDataset import dcmDataset as D
+        # from .nlst Dataset import dcmDataset as D
+    elif dataset_opt['image_type'] == 'nifti':
+        from .nlstDataset import nlstDataset as D
 
     # # load uids in this phase    
     # with open(dataset_opt['uids_path'], 'r') as f:
     #     lines = f.readlines() # ['1d7425c7412df778d26c027dc5f46a38\n', ....]
     #     # remove \n from each element in 'lines' list
     #     dataset_opt['uids'] = [l.rstrip() for l in lines]
     dataset = D(dataset_opt) # create dataobject
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/tmp_with_label.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/tmp_with_label.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/dataset/nlstDataset.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/dataset/nlstDataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import numpy as np 
 import nibabel as nib
 import nrrd
 import nibabel
 import pydicom
 from lung_analysis_pipeline.utils import util
 
-class dcmDataset(data.Dataset):
+class nlstDataset(data.Dataset):
     def __init__(self, opt): 
-        super(dcmDataset, self).__init__()
+        super(nlstDataset, self).__init__()
         self.FILL_RATIO_THRESHOLD = 0.8
         self.opt = opt
         self.in_folder = opt['dataroot_LR']
 
         # feature extraction ROI 
         if opt['feature_roi_centroid']:
             with open(opt['feature_roi_centroid'], 'r') as json_file:
@@ -48,32 +48,27 @@
         # dcm_files.sort(key=lambda x: int(pydicom.dcmread(x).InstanceNumber))
         # slices = [pydicom.dcmread(f) for f in dcm_files]
         # vol_in = np.stack([slice.pixel_array for slice in slices], axis=0).astype(np.float16)
 
         ## load NIFTI 
         data_dir_path = self.paths[index]
         data_file_path = os.path.join(data_dir_path, 'Contours', 'NIFTI', 'image.nii.gz')
-        # mask_dir_path = os.path.join(data_dir_path, 'Contours', 'NIFTI')
-        mask_dir_path = self.img_to_mask_path[data_dir_path]
         image_data = nib.load(data_file_path)
         vol_in = image_data.get_fdata()
         vol_in = np.transpose(vol_in, (2,1,0)) # onvert from WHD format to DHW format
         # Optional: Print the image shape and data type
         # print('Image Shape:', vol_in.shape)
         # print('Data Type:', vol_in.dtype)
-        gt_mask = self.load_masks(mask_dir_path)
-        # gt_mask = np.expand_dims(gt_mask, axis=0)
-        # print('gt_mask Shape:', gt_mask.shape)
-        # print('gt_mask Type:', gt_mask.dtype)
-
+        
+      
         # creates an extra dimension. e.g. (156, 512, 512) becomes (1, 156, 512, 512)
         vol_in = np.expand_dims(vol_in, axis=0)
 
         # convert to tensors and also within a certain range of values as defined in 'self.ToTensor()' class
-        vol_in = self.ToTensor(vol_in, clip=True, raw_data_range=1500.)
+        transformed_vol_in = self.ToTensor(vol_in, clip=True, raw_data_range=1500.)
         # vol_in = torch.from_numpy(np.array(vol_in, np.float32, copy=False))
 
         # generate a volume id 
         # patient_id = slices[0].PatientID.replace("_", "-")
         # timepoint = slices[0].StudyDate
         # series_instance_uid = slices[0].SeriesInstanceUID
         # modality = slices[0].Modality 
@@ -81,21 +76,30 @@
 
         # # some info needed when saving results 
         # spacings = [slices[0].PixelSpacing[0], slices[0].PixelSpacing[1], abs(slices[1].SliceLocation - slices[0].SliceLocation)]
         # input_info = {'patient_id': splits[3], 'time': splits[4], 'name': splits[5]}
         # input_info['spacings'] = spacings
         # input_info['image_position'] = slices[0].ImagePositionPatient
 
+        
+        # out_dict = {'LR': vol_in, 'spacings': [], 'uid': volume_id, 'feature_roi_centroids': feature_rois}
+        out_dict = {'original_vol_in': torch.from_numpy(vol_in), 'LR': transformed_vol_in, 'spacings': [], 'uid': self.uids[index]}
+        # 'feature_roi_centroids': feature_rois, 'gt_mask': gt_mask
+        
         # load ROI centroids for feature extraction if provided 
         feature_rois = []
         if hasattr(self, 'feature_roi'): 
             feature_rois = self.feature_roi[data_dir_path]
             feature_rois = torch.tensor(feature_rois)
-        # out_dict = {'LR': vol_in, 'spacings': [], 'uid': volume_id, 'feature_roi_centroids': feature_rois}
-        out_dict = {'LR': vol_in, 'spacings': [], 'uid': self.uids[index], 'feature_roi_centroids': feature_rois, 'gt_mask': gt_mask}
+            out_dict['feature_roi_centroids'] = feature_rois
+        if hasattr(self, 'img_to_mask_path'): 
+            mask_dir_path = self.img_to_mask_path[data_dir_path]
+            gt_mask = self.load_masks(mask_dir_path)
+            out_dict['gt_mask'] = gt_mask 
+
         return out_dict
     
     def load_masks(self, mask_root): 
         combined_mask = None 
         for filename in os.listdir(mask_root): 
             if filename.startswith("Lesion"):
                 file_path = os.path.join(mask_root, filename)
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/bm3d_ht.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/bm3d_ht.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,30 +68,31 @@
         nrrd.write(volume_save_path, lr_bm3d_norm_clipped, spacing_info, index_order='C')
 
 """
 Apply bm3d denoising to data['LR'] of shape 3D(D,H,W) and value [0,1]
 data: dictionary from dataloader 
 """
 def calculate_scan_bm3d(data):
-    lr_scan = data['LR'][0,0].numpy()
+    lr_scan = data['original_vol_in'][0,0].numpy()
+    lr_scan = lr_scan - lr_scan.min() # +1024.0
     lr_bm3d_norm = np.empty(lr_scan.shape)
     for index, slice_ in enumerate(lr_scan):
         img_slice = rescale_img(slice_, clip=None, max_val=255.0)
         sigma_est = np.mean(estimate_sigma(img_slice, multichannel=False))
         BM3D_denoised_image = bm3d.bm3d(img_slice, sigma_psd=sigma_est, stage_arg=bm3d.BM3DStages.ALL_STAGES) # bm3d.BM3DStages.HARD_THRESHOLDING
         # bm3d_clipped = rescale_img(BM3D_denoised_image, clip=(0.0, 255.0), max_val=slice_.max())
         bm3d_clipped = rescale_img(BM3D_denoised_image, clip=(0.0, 255.0), max_val=1500)
         lr_bm3d_norm[index] = bm3d_clipped
     
     # lr_bm3d_norm = lr_bm3d_norm.astype(np.int16)
     lr_bm3d_norm_clipped = np.clip(lr_bm3d_norm, 0, 1500)
     lr_bm3d_norm_clipped = lr_bm3d_norm_clipped.round()
+    lr_bm3d_norm_clipped = rescale_intensity(lr_bm3d_norm_clipped) # [0,1]
     # lr_bm3d_norm_clipped = lr_bm3d_norm_clipped.astype(np.int16)
-    data['volume'] = torch.from_numpy(lr_bm3d_norm_clipped)
-    print(lr_bm3d_norm[10])
+    data['volume'] = torch.from_numpy(lr_bm3d_norm_clipped)[None,None]
     return data
 
 if __name__ == '__main__':
     dataroot_LR = '/datasets/data_st1.0_merged'
     UID = '/datasets/uids/70-30_split/ucla_testUID_70_30_split.txt'
     save_path = '../../results/BM3D-70-30-Split_tileStitch-32x64x64_Ref-k2d100/merged_cases/test_st1.0_norm'
     calculate_bm3d(dataroot_LR, UID, save_path)
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/histogram_matching.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/compute_metrics.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/compute_metrics.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_ExternalFolder.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_ExternalFolder.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_SingleVol.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_SingleVol.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/options/options.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/options/options.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_img_files.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_img_files.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/make_uids.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/make_uids.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_uids_for_cv.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_uids_for_cv.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/get_log_values.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/get_log_values.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/util.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/util.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-RetinaNet.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-RetinaNet.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/batch_hr2Toh5.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/batch_hr2Toh5.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/read_tensorboard.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/read_tensorboard.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_aapm.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_aapm.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/segment_lungs.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/segment_lungs.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm_uids.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm_uids.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/progress_bar.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/train.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/train.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/visualize_cases.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/visualize_cases.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_model.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_model.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/lr_scheduler.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/generators.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/generators.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/auxiliary_features.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/auxiliary_features.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/loss.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/loss.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/block.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/block.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/discriminators.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/discriminators.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/bam.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/bam.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/networks.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/networks.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/build_unet_model.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/build_unet_model.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SR_model.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SR_model.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_exp.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_exp.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/__init__.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/models/base_model.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/models/base_model.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/html.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/html.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/util.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/util.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/visualizer.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists_dirs.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists_dirs.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/pretrained_networks.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/dist_model.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/dist_model.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/networks_basic.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/networks_basic.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/base_model.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/base_model.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/Normalization_Pipeline/codes/test.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/Normalization_Pipeline/codes/test.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/utils/util.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/utils/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,43 +187,56 @@
         volume = np.transpose(volume, (2, 1, 0))
         volume_img = nib.Nifti1Image(volume, np.eye(4))
         # Save the image to a file
         nib.save(volume_img, volume_path)
     else: 
         raise NotImplementedError('Output dtype not supported.')
 
-def save_mask(opt, input_info, results_dir, seg_result_dtype, patient_id, mask):
-    
-    mask = mask.astype(np.uint8) # to unsigned char 
-    if seg_result_dtype == 'nrrd': 
-        volume_path = os.path.join(results_dir, patient_id+'.nrrd')
-
-        header = {
-            'units': ['mm', 'mm', 'mm'], 
-            'Segment0_LabelValue': 1, 
-        } 
-
-        # save header in dict format 
-        # spacings = input_info['spacings']
-        # space_directions = ((spacings[0], 0, 0), (0, spacings[1], 0), (0, 0, spacings[2]))
-        # header['space directions'] = space_directions
-        # header['space origin'] = input_info['image_position']
-
-        nrrd.write(volume_path, mask, header, index_order='C')
-    elif seg_result_dtype == 'nifti': 
-        volume_path = os.path.join(results_dir, patient_id+'.nii.gz')
-        # print('mask shape before: {}'.format(mask.shape))
-        mask = np.transpose(mask, (2, 1, 0))
-        # print('mask shape after: {}'.format(mask.shape))
-        mask_img = nib.Nifti1Image(mask, np.eye(4))
+def save_nifti(path, data): 
+    data = np.transpose(data, (2, 1, 0))
+    # print('mask shape after: {}'.format(mask.shape))
+    data_img = nib.Nifti1Image(data, np.eye(4))
+
+    # Save the image to a file
+    nib.save(data_img, path)
+
+def save_mask(opt,data):
+    results_dir = opt['segmentation']['output_path']
+    seg_result_dtype = opt['segmentation']['output_dtype']
+    instance_id = data['uid'][0]
+    if 'seg_mask' in data:
+        mask = tensor2mask(data['seg_mask'][0], out_type=np.uint16)
+        # print(mask.shape)
+        if seg_result_dtype == 'nrrd': 
+            volume_path = os.path.join(results_dir, instance_id+'.nrrd')
+            header = {'units': ['mm', 'mm', 'mm'],  'Segment0_LabelValue': 1} 
+
+            nrrd.write(volume_path, mask, header, index_order='C')
+        elif seg_result_dtype == 'nifti': 
+            volume_path = os.path.join(results_dir, instance_id+'.nii.gz')
+            save_nifti(volume_path, mask)
+        else: 
+            raise NotImplementedError('Segmentation output dtype not supported.')
+    elif 'seg_masks' in data: # detection bboxes -> seg masks 
+        masks = data['seg_masks']
+        for i, mask in enumerate(masks): 
+            mask = tensor2mask(mask, out_type=np.uint16) # to unsigned char 
+            # print(mask.shape) 
+            if seg_result_dtype == 'nrrd': 
+                volume_path = os.path.join(results_dir, instance_id + f'-{i}' + '.nrrd')
+                # print(volume_path)
+                header = {'units': ['mm', 'mm', 'mm'],  'Segment0_LabelValue': 1} 
+
+                nrrd.write(volume_path, mask, header, index_order='C')
+            elif seg_result_dtype == 'nifti': 
+                volume_path = os.path.join(results_dir, instance_id + f'-{i}' + '.nii.gz')
+                save_nifti(volume_path, mask)
+            else: 
+                raise NotImplementedError('Segmentation output dtype not supported.')
 
-        # Save the image to a file
-        nib.save(mask_img, volume_path)
-    else: 
-        raise NotImplementedError('Segmentation output dtype not supported.')
 
 def save_vol_nested(opt, spacings, results_dir, input_info, volume):
     patient_id = input_info['patient_id'][0]
     time = input_info['time'][0]
     name = input_info['name'][0]
     # create nested directories if not exist 
     patient_dir = os.path.join(results_dir, patient_id)
@@ -714,17 +727,17 @@
     current_max = np.max(image)
 
     # Rescale the image to the desired range
     rescaled_image = (image - current_min) * (max_value - min_value) / (current_max - current_min) + min_value
 
     return rescaled_image
 
-def resize_image(data, size=(52,52,52)):
+def resize_image(data, size):
     """
-    Resize the data to the input size
+    Resize the data to the input size. Data and size in DxHxW format.
     """ 
     # [height, width, depth] = data.shape
     [depth, height, width] = data.shape 
     # scale = [self.input_D*1.0/depth, self.input_H*1.0/height, self.input_W*1.0/width] 
     target_depth, target_height, target_width = size 
     scale = [target_depth*1.0/depth, target_height*1.0/height, target_width*1.0/width] 
     data = ndimage.interpolation.zoom(data, scale, order=0)
@@ -748,14 +761,16 @@
     y_min, y_max = max(0, y - 26), min(image.shape[1], y + 26)
     x_min, x_max = max(0, x - 26), min(image.shape[2], x + 26)
     # add zero padding if expected ROI lies partially out of the image                 
     roi = image[z_min:z_max, y_min:y_max, x_min:x_max]
     # pad_dims = [0, 52-(x_max-x_min), 0, 52-(y_max-y_min), 0, 52-(z_max-z_min)]
     # roi = F.pad(roi, pad_dims, mode='constant', value=0)
     pad_dims = ((0, 52-(z_max-z_min)), (0, 52-(y_max-y_min)), (0, 52-(x_max-x_min)))
+    if any(x > 50 for _,x in pad_dims ):
+        print(pad_dims)
     roi = np.pad(roi, pad_width=pad_dims, mode='constant', constant_values=0)
     
     return roi 
 
 def extract_roi_with_diameter(image, centroid, diameter):
     z, y, x = centroid
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/utils/patch.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/utils/patch.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/train_unet_lidc.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/train_unet_lidc.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_lidc.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_lidc.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_resnet34_lidc.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_resnet34_lidc.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/train.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/train.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/setting.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/setting.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/model.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/model.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/test.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/test.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_norm.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_norm.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/model_pipeline.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/model_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,53 +27,41 @@
                 self.feature_extractions['deep_feature'] = create_feat_extractor(opt)
             if 'radiomics' in opt['feature_extraction']:
                 self.feature_extractions['radiomics'] = radiomic_feature_extractor(opt)
     def test(self, input_data): 
         
         if hasattr(self, 'norm_model'):
             input_data = self.norm_model.run_test(input_data)
-
             # save norm output 
             if self.opt['normalization']['output_path']:
-                # print('saving norm')
                 norm_results_dir = self.opt['normalization']['output_path']
                 util.mkdir(norm_results_dir)
-
-                sr_vol = util.tensor2img(input_data['volume'], out_type=np.uint16)
+                sr_vol = util.tensor2img(input_data['volume'][0][0], out_type=np.uint16)
                 util.save_vol(self.opt, [], norm_results_dir, input_data['uid'][0], sr_vol, dtype=self.opt['normalization']['output_dtype'])
         else: 
             input_data['volume'] = input_data['LR']
         
         if hasattr(self, 'detect_model'):
             detect_output = self.detect_model.run_test(input_data)
-            # print(detect_output['detection_bboxes'])
             if self.opt['detection']['output_path']:
                 util.save_detect_bbox(self.opt, detect_output)
 
         if hasattr(self, 'seg_model'): 
-            if self.opt['segmentation']['use_decetion_bbox']: 
-                seg_output = self.seg_model.run_test(detect_output) 
-            else: 
-                seg_output = self.seg_model.run_test(input_data) 
+            seg_output = self.seg_model.run_test(input_data, self.opt) 
             if self.opt['segmentation']['output_path']:
-                # seg_ressult_dir = os.path.join(results_dir, 'segmentation')
                 seg_ressult_dir = self.opt['segmentation']['output_path']
-                seg_result_dtype = self.opt['segmentation']['output_dtype']
                 util.mkdir(seg_ressult_dir)
-
-                seg_mask = util.tensor2mask(seg_output['seg_mask'][0][0], out_type=np.uint16)
-                util.save_mask(self.opt, seg_output['input_info'], seg_ressult_dir, seg_result_dtype, seg_output['uid'][0], seg_mask)
+                util.save_mask(self.opt, seg_output)
+        
         if hasattr(self, 'feature_extractions'): 
             for key, extractor in self.feature_extractions.items(): 
                 # extract feature 
-                feat_output = extractor.run_test(input_data, roi=self.opt['feature_extraction']['roi_source'], threshold_size=0)
+                feat_output = extractor.run_test(input_data, roi=self.opt['feature_extraction']['roi_source'], threshold_size=10)
                 
                 # only save results if output location is provided 
                 if self.opt['feature_extraction'][key]['output_path']:
-                    # save features 
-                    
-                    # util.save_feature_csv(feat_file, feat_dtype, feat_output['uid'][0], feat_output[key].cpu().numpy())
                     util.save_features(key, self.opt, feat_output)
+        
         if self.opt['gpu_ids']: 
             torch.cuda.synchronize()
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline/__init__.py` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.6/setup.py` & `lung_analysis_pipeline-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A lung analysis pipeline'
 LONG_DESCRIPTION = 'A lung analysis pipeline for normalization, detection, segmentation, and feature extraction'
 
 # Setting up
 setup(
     name="lung_analysis_pipeline",
     version=VERSION,
```

### Comparing `lung_analysis_pipeline-0.0.6/lung_analysis_pipeline.egg-info/SOURCES.txt` & `lung_analysis_pipeline-0.0.7/lung_analysis_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

