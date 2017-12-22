# IO.Swagger.Api.FilesApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FileCleanGet**](FilesApi.md#filecleanget) | **GET** /file-clean | 
[**FileGeneratePreviewGet**](FilesApi.md#filegeneratepreviewget) | **GET** /file-generate-preview | 
[**FilesGet**](FilesApi.md#filesget) | **GET** /files | 
[**FilesIdDelete**](FilesApi.md#filesiddelete) | **DELETE** /files/{id} | 
[**FilesPost**](FilesApi.md#filespost) | **POST** /files | 


<a name="filecleanget"></a>
# **FileCleanGet**
> void FileCleanGet (string apiKey, string documentId)



This API get clean file from document id. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FileCleanGetExample
    {
        public void main()
        {
            var apiInstance = new FilesApi();
            var apiKey = apiKey_example;  // string | API Key
            var documentId = documentId_example;  // string | Document ID in the fax

            try
            {
                apiInstance.FileCleanGet(apiKey, documentId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FilesApi.FileCleanGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **documentId** | **string**| Document ID in the fax | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="filegeneratepreviewget"></a>
# **FileGeneratePreviewGet**
> void FileGeneratePreviewGet (string apiKey, string documentId)



This API get generated preview file from document id. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FileGeneratePreviewGetExample
    {
        public void main()
        {
            var apiInstance = new FilesApi();
            var apiKey = apiKey_example;  // string | API Key
            var documentId = documentId_example;  // string | Document ID in the fax

            try
            {
                apiInstance.FileGeneratePreviewGet(apiKey, documentId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FilesApi.FileGeneratePreviewGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **documentId** | **string**| Document ID in the fax | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="filesget"></a>
# **FilesGet**
> void FilesGet (string apiKey)



This API lists all the files 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FilesGetExample
    {
        public void main()
        {
            var apiInstance = new FilesApi();
            var apiKey = apiKey_example;  // string | API Key

            try
            {
                apiInstance.FilesGet(apiKey);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FilesApi.FilesGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="filesiddelete"></a>
# **FilesIdDelete**
> void FilesIdDelete (string apiKey, decimal? id)



This API deletes a single file. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FilesIdDeleteExample
    {
        public void main()
        {
            var apiInstance = new FilesApi();
            var apiKey = apiKey_example;  // string | API Key
            var id = 3.4;  // decimal? | id of the file / document

            try
            {
                apiInstance.FilesIdDelete(apiKey, id);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FilesApi.FilesIdDelete: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **id** | **decimal?**| id of the file / document | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="filespost"></a>
# **FilesPost**
> System.IO.Stream FilesPost (string apiKey, System.IO.Stream file, string addRemoteFile = null)



This API allows uploading of a single file. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FilesPostExample
    {
        public void main()
        {
            var apiInstance = new FilesApi();
            var apiKey = apiKey_example;  // string | API Key
            var file = new System.IO.Stream(); // System.IO.Stream | PDF file to upload
            var addRemoteFile = addRemoteFile_example;  // string | Given the remote file url (optional) 

            try
            {
                System.IO.Stream result = apiInstance.FilesPost(apiKey, file, addRemoteFile);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FilesApi.FilesPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **file** | **System.IO.Stream**| PDF file to upload | 
 **addRemoteFile** | **string**| Given the remote file url | [optional] 

### Return type

**System.IO.Stream**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

