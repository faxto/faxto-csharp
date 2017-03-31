# IO.Swagger.Api.FaxApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FaxDocumentIdCostsGet**](FaxApi.md#faxdocumentidcostsget) | **GET** /fax/{document_id}/costs | 
[**FaxHistoryGet**](FaxApi.md#faxhistoryget) | **GET** /fax-history | 
[**FaxJobIdStatusGet**](FaxApi.md#faxjobidstatusget) | **GET** /fax/{job_id}/status | 
[**FaxPost**](FaxApi.md#faxpost) | **POST** /fax | 


<a name="faxdocumentidcostsget"></a>
# **FaxDocumentIdCostsGet**
> void FaxDocumentIdCostsGet (string apiKey, string faxNumber, decimal? documentId)



This API get the cost of a sending fax. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FaxDocumentIdCostsGetExample
    {
        public void main()
        {
            
            var apiInstance = new FaxApi();
            var apiKey = apiKey_example;  // string | API Key
            var faxNumber = faxNumber_example;  // string | Fax Number
            var documentId = 3.4;  // decimal? | id of the file / document_id

            try
            {
                apiInstance.FaxDocumentIdCostsGet(apiKey, faxNumber, documentId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FaxApi.FaxDocumentIdCostsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **faxNumber** | **string**| Fax Number | 
 **documentId** | **decimal?**| id of the file / document_id | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="faxhistoryget"></a>
# **FaxHistoryGet**
> void FaxHistoryGet (string apiKey, string limit = null, string page = null)



This API get all fax history. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FaxHistoryGetExample
    {
        public void main()
        {
            
            var apiInstance = new FaxApi();
            var apiKey = apiKey_example;  // string | API Key
            var limit = limit_example;  // string | Number of records to return (optional) 
            var page = page_example;  // string | Page to display (optional) 

            try
            {
                apiInstance.FaxHistoryGet(apiKey, limit, page);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FaxApi.FaxHistoryGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **limit** | **string**| Number of records to return | [optional] 
 **page** | **string**| Page to display | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="faxjobidstatusget"></a>
# **FaxJobIdStatusGet**
> void FaxJobIdStatusGet (string apiKey, decimal? jobId)



This API get the status of the fax. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FaxJobIdStatusGetExample
    {
        public void main()
        {
            
            var apiInstance = new FaxApi();
            var apiKey = apiKey_example;  // string | API Key
            var jobId = 3.4;  // decimal? | id of the fax job

            try
            {
                apiInstance.FaxJobIdStatusGet(apiKey, jobId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FaxApi.FaxJobIdStatusGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **jobId** | **decimal?**| id of the fax job | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="faxpost"></a>
# **FaxPost**
> void FaxPost (string apiKey, string faxNumber, int? documentId = null, string tsiNumber = null, System.IO.Stream file = null, int? deleteFile = null)



This API send the fax. When we send fax using API, Fax.to send a POST to the Callback URL you specified in https://fax.to/member/api/live. Fax.to send POST data with the following information fax_job_id, status and message. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FaxPostExample
    {
        public void main()
        {
            
            var apiInstance = new FaxApi();
            var apiKey = apiKey_example;  // string | API Key
            var faxNumber = faxNumber_example;  // string | Fax Number
            var documentId = 56;  // int? | Document id. If you want to use existing document you need to specify the document_id (optional) 
            var tsiNumber = tsiNumber_example;  // string | If we want to to change the text or number that appear on 'from' or 'sender' of the fax (optional) 
            var file = new System.IO.Stream(); // System.IO.Stream | PDF file to upload (optional) 
            var deleteFile = 56;  // int? | Whether to delete file after fax transaction. (put 1 to delete) (optional) 

            try
            {
                apiInstance.FaxPost(apiKey, faxNumber, documentId, tsiNumber, file, deleteFile);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FaxApi.FaxPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **faxNumber** | **string**| Fax Number | 
 **documentId** | **int?**| Document id. If you want to use existing document you need to specify the document_id | [optional] 
 **tsiNumber** | **string**| If we want to to change the text or number that appear on &#39;from&#39; or &#39;sender&#39; of the fax | [optional] 
 **file** | **System.IO.Stream**| PDF file to upload | [optional] 
 **deleteFile** | **int?**| Whether to delete file after fax transaction. (put 1 to delete) | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

