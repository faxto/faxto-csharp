# IO.Swagger.Api.FaxApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FaxDocumentIdCostsGet**](FaxApi.md#faxdocumentidcostsget) | **GET** /fax/{document_id}/costs | 
[**FaxGet**](FaxApi.md#faxget) | **GET** /fax | 
[**FaxJobIdStatusGet**](FaxApi.md#faxjobidstatusget) | **GET** /fax/{job_id}/status | 
[**IncomingFaxesGet**](FaxApi.md#incomingfaxesget) | **GET** /incoming-faxes | 
[**IncomingFaxesNumberGet**](FaxApi.md#incomingfaxesnumberget) | **GET** /incoming-faxes/{number} | 
[**ProvisionNumbersGet**](FaxApi.md#provisionnumbersget) | **GET** /provision-numbers | 


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

<a name="faxget"></a>
# **FaxGet**
> void FaxGet (string apiKey, string limit = null, string page = null)



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
    public class FaxGetExample
    {
        public void main()
        {
            var apiInstance = new FaxApi();
            var apiKey = apiKey_example;  // string | API Key
            var limit = limit_example;  // string | Number of records to return (optional) 
            var page = page_example;  // string | Page to display (optional) 

            try
            {
                apiInstance.FaxGet(apiKey, limit, page);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FaxApi.FaxGet: " + e.Message );
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

<a name="incomingfaxesget"></a>
# **IncomingFaxesGet**
> void IncomingFaxesGet (string apiKey)



This API get faxes . 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class IncomingFaxesGetExample
    {
        public void main()
        {
            var apiInstance = new FaxApi();
            var apiKey = apiKey_example;  // string | API Key

            try
            {
                apiInstance.IncomingFaxesGet(apiKey);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FaxApi.IncomingFaxesGet: " + e.Message );
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

<a name="incomingfaxesnumberget"></a>
# **IncomingFaxesNumberGet**
> void IncomingFaxesNumberGet (string apiKey, string number)



This API get faxes  by number. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class IncomingFaxesNumberGetExample
    {
        public void main()
        {
            var apiInstance = new FaxApi();
            var apiKey = apiKey_example;  // string | API Key
            var number = number_example;  // string | Number in the fax

            try
            {
                apiInstance.IncomingFaxesNumberGet(apiKey, number);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FaxApi.IncomingFaxesNumberGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **number** | **string**| Number in the fax | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="provisionnumbersget"></a>
# **ProvisionNumbersGet**
> void ProvisionNumbersGet (string apiKey, string limit = null)



This API get Provision numbers. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ProvisionNumbersGetExample
    {
        public void main()
        {
            var apiInstance = new FaxApi();
            var apiKey = apiKey_example;  // string | API Key
            var limit = limit_example;  // string | Limit to display (optional) 

            try
            {
                apiInstance.ProvisionNumbersGet(apiKey, limit);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FaxApi.ProvisionNumbersGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **limit** | **string**| Limit to display | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

