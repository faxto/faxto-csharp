# IO.Swagger.Api.AccountApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BalanceGet**](AccountApi.md#balanceget) | **GET** /balance | 


<a name="balanceget"></a>
# **BalanceGet**
> void BalanceGet (string apiKey)



This API get users balance. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class BalanceGetExample
    {
        public void main()
        {
            var apiInstance = new AccountApi();
            var apiKey = apiKey_example;  // string | API Key

            try
            {
                apiInstance.BalanceGet(apiKey);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling AccountApi.BalanceGet: " + e.Message );
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

