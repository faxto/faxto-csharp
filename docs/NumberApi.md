# IO.Swagger.Api.NumberApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**NumbersGet**](NumberApi.md#numbersget) | **GET** /numbers | 


<a name="numbersget"></a>
# **NumbersGet**
> void NumbersGet (string apiKey, string page = null)



This API get users numbers. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class NumbersGetExample
    {
        public void main()
        {
            var apiInstance = new NumberApi();
            var apiKey = apiKey_example;  // string | API Key
            var page = page_example;  // string | Page to display (optional) 

            try
            {
                apiInstance.NumbersGet(apiKey, page);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling NumberApi.NumbersGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiKey** | **string**| API Key | 
 **page** | **string**| Page to display | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

