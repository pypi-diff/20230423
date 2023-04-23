# Comparing `tmp/aliyun-python-sdk-imm-2.1.11.tar.gz` & `tmp/aliyun-python-sdk-imm-2.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-imm-2.1.11.tar", last modified: Tue Apr  4 07:21:17 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-imm-2.1.12.tar", last modified: Sun Apr 23 08:10:07 2023, max compression
```

## Comparing `aliyun-python-sdk-imm-2.1.11.tar` & `aliyun-python-sdk-imm-2.1.12.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:21:17.000000 aliyun-python-sdk-imm-2.1.11/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1538 2023-04-04 07:21:17.000000 aliyun-python-sdk-imm-2.1.11/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:21:17.000000 aliyun-python-sdk-imm-2.1.11/aliyun_python_sdk_imm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyun_python_sdk_imm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6357 2023-04-04 07:21:17.000000 aliyun-python-sdk-imm-2.1.11/aliyun_python_sdk_imm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyun_python_sdk_imm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyun_python_sdk_imm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyun_python_sdk_imm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:21:17.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:21:17.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:21:17.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/
--rw-r--r--   0 root         (0) root         (0)     2643 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/AddImageMosaicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/AddStoryFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/AttachOSSBucketRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchDeleteFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchGetFigureClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchGetFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchIndexFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchUpdateFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CompareImageFacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateArchiveFileInspectionTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateCompressPointCloudTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateCustomizedStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2609 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFacesSearchingTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFigureClusteringTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFigureClustersMergingTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3141 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFileCompressionTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFileUncompressionTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateImageModerationTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     4105 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateImageSplicingTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2653 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateImageToPDFTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateLocationDateClusteringTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2655 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateMediaConvertTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateOfficeConversionTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateSimilarImageClusteringTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateVideoLabelClassificationTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateVideoModerationTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteLocationDateClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1837 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetachOSSBucketRequest.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageBodiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageCarsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageCodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageCroppingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py
--rw-r--r--   0 root         (0) root         (0)     2505 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GenerateDRMLicenseRequest.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GenerateVideoPlaylistRequest.py
--rw-r--r--   0 root         (0) root         (0)     4440 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetDRMLicenseRequest.py
--rw-r--r--   0 root         (0) root         (0)     1873 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetOSSBucketAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetVideoLabelClassificationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetVideoModerationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/IndexFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListBatchesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListBindingsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListDatasetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListProjectsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3158 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListTriggersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/LiveTranscodingRequest.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2583 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     4516 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/QueryStoriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ResumeBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ResumeBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ResumeTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SearchImageFigureClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SemanticQueryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SimpleQueryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/StopBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SuspendBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SuspendTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateFigureClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateLocationDateClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2582 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2346 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-04 07:21:17.000000 aliyun-python-sdk-imm-2.1.11/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-04-04 07:21:16.000000 aliyun-python-sdk-imm-2.1.11/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyun_python_sdk_imm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyun_python_sdk_imm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6357 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyun_python_sdk_imm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyun_python_sdk_imm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyun_python_sdk_imm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyun_python_sdk_imm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/AddImageMosaicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/AddStoryFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/AttachOSSBucketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchDeleteFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchGetFigureClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchGetFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchIndexFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchUpdateFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CompareImageFacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateArchiveFileInspectionTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateCompressPointCloudTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateCustomizedStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFacesSearchingTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFigureClusteringTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFigureClustersMergingTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFileCompressionTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFileUncompressionTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateImageModerationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateImageSplicingTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateImageToPDFTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateLocationDateClusteringTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateMediaConvertTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateOfficeConversionTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateSimilarImageClusteringTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateVideoLabelClassificationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateVideoModerationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteLocationDateClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetachOSSBucketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageBodiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageCarsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageCodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageCroppingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GenerateDRMLicenseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GenerateVideoPlaylistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetDRMLicenseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetOSSBucketAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetVideoLabelClassificationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetVideoModerationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/IndexFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListBatchesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListBindingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListDatasetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListProjectsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListTriggersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/LiveTranscodingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/QueryStoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ResumeBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ResumeBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ResumeTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SearchImageFigureClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SemanticQueryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SimpleQueryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/StopBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SuspendBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SuspendTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateFigureClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateLocationDateClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-04-23 08:10:07.000000 aliyun-python-sdk-imm-2.1.12/setup.py
```

### Comparing `aliyun-python-sdk-imm-2.1.11/LICENSE` & `aliyun-python-sdk-imm-2.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/PKG-INFO` & `aliyun-python-sdk-imm-2.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-imm
-Version: 2.1.11
+Version: 2.1.12
 Summary: The imm module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-imm
```

### Comparing `aliyun-python-sdk-imm-2.1.11/README.rst` & `aliyun-python-sdk-imm-2.1.12/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyun_python_sdk_imm.egg-info/PKG-INFO` & `aliyun-python-sdk-imm-2.1.12/aliyun_python_sdk_imm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-imm
-Version: 2.1.11
+Version: 2.1.12
 Summary: The imm module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-imm
```

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyun_python_sdk_imm.egg-info/SOURCES.txt` & `aliyun-python-sdk-imm-2.1.12/aliyun_python_sdk_imm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/endpoint.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/AddImageMosaicRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/AddImageMosaicRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/AddStoryFilesRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/AddStoryFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/AttachOSSBucketRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/AttachOSSBucketRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchDeleteFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchDeleteFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchGetFigureClusterRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchGetFigureClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchGetFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchGetFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchIndexFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchIndexFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/BatchUpdateFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/BatchUpdateFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CompareImageFacesRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CompareImageFacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateArchiveFileInspectionTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateArchiveFileInspectionTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateBatchRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateBindingRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateCompressPointCloudTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateCompressPointCloudTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateCustomizedStoryRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateCustomizedStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateDatasetRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateDatasetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFacesSearchingTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFacesSearchingTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFigureClusteringTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFigureClusteringTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFigureClustersMergingTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFigureClustersMergingTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFileCompressionTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFileCompressionTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateFileUncompressionTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateFileUncompressionTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateImageModerationTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateImageModerationTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateImageSplicingTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateImageSplicingTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateImageToPDFTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateImageToPDFTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateLocationDateClusteringTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateLocationDateClusteringTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateMediaConvertTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateMediaConvertTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateOfficeConversionTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateOfficeConversionTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateProjectRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateSimilarImageClusteringTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateSimilarImageClusteringTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateStoryRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateVideoLabelClassificationTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateVideoLabelClassificationTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/CreateVideoModerationTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/CreateVideoModerationTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteBatchRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteBindingRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteDatasetRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteDatasetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteLocationDateClusterRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteLocationDateClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteProjectRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteStoryRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DeleteTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DeleteTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetachOSSBucketRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetachOSSBucketRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageBodiesRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageBodiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageCarsRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageCarsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageCodesRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageCodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageCroppingRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageCroppingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GenerateDRMLicenseRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GenerateDRMLicenseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GenerateVideoPlaylistRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GenerateVideoPlaylistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetBatchRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetBindingRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetDRMLicenseRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetDRMLicenseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetDatasetRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetDatasetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetOSSBucketAttachmentRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetOSSBucketAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetProjectRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetStoryRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetTaskRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetVideoLabelClassificationResultRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetVideoLabelClassificationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/GetVideoModerationResultRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/GetVideoModerationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/IndexFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/IndexFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListBatchesRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListBatchesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListBindingsRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListBindingsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListDatasetsRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListDatasetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListProjectsRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListProjectsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListRegionsRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListTasksRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ListTriggersRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ListTriggersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/LiveTranscodingRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/LiveTranscodingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/QueryStoriesRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/QueryStoriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ResumeBatchRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ResumeBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ResumeBindingRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ResumeBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/ResumeTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/ResumeTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SearchImageFigureClusterRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SearchImageFigureClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SemanticQueryRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SemanticQueryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SimpleQueryRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SimpleQueryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/StopBindingRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/StopBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SuspendBatchRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SuspendBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/SuspendTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/SuspendTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateBatchRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateDatasetRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateDatasetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateFigureClusterRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateFigureClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateLocationDateClusterRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateLocationDateClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateProjectRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateStoryRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/aliyunsdkimm/request/v20200930/UpdateTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.12/aliyunsdkimm/request/v20200930/UpdateTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.11/setup.py` & `aliyun-python-sdk-imm-2.1.12/setup.py`

 * *Files identical despite different names*

