# Comparing `tmp/pbx_cloud_utils-1.2.0a6-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.2.0a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7160 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-May-10 08:55 cloud_utils/__init__.py
--rw-r--r--  2.0 unx    11956 b- defN 24-Apr-04 11:56 cloud_utils/aio_storage.py
--rw-r--r--  2.0 unx      284 b- defN 23-May-10 08:55 cloud_utils/exceptions.py
--rw-r--r--  2.0 unx     9825 b- defN 24-Apr-02 13:37 cloud_utils/storage.py
--rw-r--r--  2.0 unx     1258 b- defN 24-Apr-04 11:29 cloud_utils/types.py
--rw-r--r--  2.0 unx      346 b- defN 23-May-10 08:55 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-04 11:59 pbx_cloud_utils-1.2.0a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 11:59 pbx_cloud_utils-1.2.0a6.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-04 11:59 pbx_cloud_utils-1.2.0a6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      811 b- defN 24-Apr-04 11:59 pbx_cloud_utils-1.2.0a6.dist-info/RECORD
-10 files, 24908 bytes uncompressed, 5770 bytes compressed:  76.8%
+Zip file size: 7163 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 15:28 cloud_utils/__init__.py
+-rw-r--r--  2.0 unx    12017 b- defN 24-Apr-09 15:25 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx      284 b- defN 24-Apr-02 10:50 cloud_utils/exceptions.py
+-rw-r--r--  2.0 unx     9825 b- defN 24-Apr-08 11:05 cloud_utils/storage.py
+-rw-r--r--  2.0 unx     1258 b- defN 24-Apr-08 11:05 cloud_utils/types.py
+-rw-r--r--  2.0 unx      346 b- defN 24-Apr-02 10:50 cloud_utils/utils.py
+-rw-r--r--  2.0 unx      324 b- defN 24-Apr-09 15:28 pbx_cloud_utils-1.2.0a7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 15:28 pbx_cloud_utils-1.2.0a7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-09 15:28 pbx_cloud_utils-1.2.0a7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      811 b- defN 24-Apr-09 15:28 pbx_cloud_utils-1.2.0a7.dist-info/RECORD
+10 files, 24969 bytes uncompressed, 5773 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a6.dist-info/METADATA
+Filename: pbx_cloud_utils-1.2.0a7.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a6.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.2.0a7.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a6.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.2.0a7.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a6.dist-info/RECORD
+Filename: pbx_cloud_utils-1.2.0a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/aio_storage.py

```diff
@@ -58,30 +58,30 @@
     ) -> None:
         pass  # pragma: no cover
 
     @abstractmethod
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
-        pass
+        pass  # pragma: no cover
 
     @abstractmethod
     async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
-        pass
+        pass  # pragma: no cover
 
     @abstractmethod
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
     ):
-        pass
+        pass  # pragma: no cover
 
 
 class AsyncAmazonS3Storage(AsyncStorage):
     provider_storage_class_map: dict[str, str] = s3_storage_class_map
     provider_acl_map: dict[str, str] = s3_acl_map
 
     def __new__(cls, *args, **kwargs):
@@ -126,40 +126,40 @@
     async def change_storage_class(
         self,
         key: str,
         target_storage_class: PbxStorageClass,
         acl: PbxACL = PbxACL.PUBLIC_READ,
     ):
         session = aiobotocore.session.get_session()
-        async with session.create_client("s3", self.region_name) as client:
+        async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
                 MetadataDirective="COPY",
             )
 
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
         session = aiobotocore.session.get_session()
-        async with session.create_client("s3", self.region_name) as client:
+        async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=target_key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 MetadataDirective="COPY",
             )
 
     async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
         session = aiobotocore.session.get_session()
-        async with session.create_client("s3", self.region_name) as client:
+        async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             obj = await client.get_object(Bucket=self.bucket_name, Key=key)
             async with obj["Body"] as body_stream:
                 data = await body_stream.read()
             return BytesIO(data), {
                 "mimetype": obj.get("ContentType"),
                 "storage_class": obj.get("StorageClass", "STANDARD"),
             }
@@ -169,15 +169,15 @@
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
     ):
         session = aiobotocore.session.get_session()
-        async with session.create_client("s3", self.region_name) as client:
+        async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             return await client.put_object(
                 ACL=self.provider_acl_map[acl.name],
                 Body=content.getvalue(),
                 Bucket=self.bucket_name,
                 Key=key,
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
                 ContentType=mimetype,
@@ -242,15 +242,15 @@
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
     ):
         raise NotImplementedError()
 
 
-class AsyncGoogleCloudStorage(AsyncStorage):
+class HybridAsyncGoogleCloudStorage(AsyncStorage):
     provider_storage_class_map: dict[str, str] = gcs_storage_class_map
     provider_acl_map: dict[str, str] = gcs_acl_map
     bucket_client: gcs_storage.Bucket
     endpoint_url: str
 
     def __init__(self, endpoint_url: str, gcs_project_id: str = "", *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -303,35 +303,33 @@
         session = aiobotocore.session.get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
             obj = await client.get_object(Bucket=self.bucket_name, Key=key)
             async with obj["Body"] as body_stream:
                 data = await body_stream.read()
+            storage_class = obj["ResponseMetadata"]["HTTPHeaders"]["x-goog-storage-class"]
             return BytesIO(data), {
                 "mimetype": obj.get("ContentType"),
-                "storage_class": obj.get("StorageClass", "STANDARD"),
+                "storage_class": storage_class,
             }
 
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
     ):
         session = aiobotocore.session.get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
-            obj = await client.put_object(
+            return await client.put_object(
                 ACL=self.provider_acl_map[acl.name],
                 Body=content.getvalue(),
                 Bucket=self.bucket_name,
                 Key=key,
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
                 ContentType=mimetype,
             )
-        # aiobotocore doesn't support changing storage class on gcs
-        await self.change_storage_class(key, target_storage_class, acl)
-        return obj
```

