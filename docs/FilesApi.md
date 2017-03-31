# IO.Swagger.Api.FilesApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FilesGet**](FilesApi.md#filesget) | **GET** /files | 
[**FilesIdDelete**](FilesApi.md#filesiddelete) | **DELETE** /files/{id} | 
[**FilesPost**](FilesApi.md#filespost) | **POST** /files | 


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
> System.IO.Stream FilesPost (string apiKey, System.IO.Stream file)



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

            try
            {
                System.IO.Stream result = apiInstance.FilesPost(apiKey, file);
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

### Return type

**System.IO.Stream**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

