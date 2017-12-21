# IO.Swagger.Api.CountryApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AreacodesCountryCodeStateIdGet**](CountryApi.md#areacodescountrycodestateidget) | **GET** /areacodes/{countryCode}/{stateId} | 
[**CountriesCountryCodeDidgroupsGet**](CountryApi.md#countriescountrycodedidgroupsget) | **GET** /countries/{countryCode}/didgroups | 
[**CountriesDidgroupsDidGroupIdProvisionPost**](CountryApi.md#countriesdidgroupsdidgroupidprovisionpost) | **POST** /countries/didgroups/{didGroupId}/provision | 
[**CountriesGet**](CountryApi.md#countriesget) | **GET** /countries | 
[**StatesCountryCodeGet**](CountryApi.md#statescountrycodeget) | **GET** /states/{countryCode} | 


<a name="areacodescountrycodestateidget"></a>
# **AreacodesCountryCodeStateIdGet**
> void AreacodesCountryCodeStateIdGet (string countryCode, string stateId)



This API get areacodes . 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class AreacodesCountryCodeStateIdGetExample
    {
        public void main()
        {
            var apiInstance = new CountryApi();
            var countryCode = countryCode_example;  // string | countryCode in the Country
            var stateId = stateId_example;  // string | stateId in the Country

            try
            {
                apiInstance.AreacodesCountryCodeStateIdGet(countryCode, stateId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling CountryApi.AreacodesCountryCodeStateIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **countryCode** | **string**| countryCode in the Country | 
 **stateId** | **string**| stateId in the Country | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="countriescountrycodedidgroupsget"></a>
# **CountriesCountryCodeDidgroupsGet**
> void CountriesCountryCodeDidgroupsGet (string countryCode, string didGroupIds, string stateId, string cityNamePattern)



This API didgroups countryCode. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CountriesCountryCodeDidgroupsGetExample
    {
        public void main()
        {
            var apiInstance = new CountryApi();
            var countryCode = countryCode_example;  // string | countryCode in the Country
            var didGroupIds = didGroupIds_example;  // string | didGroupId in the Country
            var stateId = stateId_example;  // string | stateId in the Country
            var cityNamePattern = cityNamePattern_example;  // string | cityNamePattern in the Country

            try
            {
                apiInstance.CountriesCountryCodeDidgroupsGet(countryCode, didGroupIds, stateId, cityNamePattern);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling CountryApi.CountriesCountryCodeDidgroupsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **countryCode** | **string**| countryCode in the Country | 
 **didGroupIds** | **string**| didGroupId in the Country | 
 **stateId** | **string**| stateId in the Country | 
 **cityNamePattern** | **string**| cityNamePattern in the Country | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="countriesdidgroupsdidgroupidprovisionpost"></a>
# **CountriesDidgroupsDidGroupIdProvisionPost**
> void CountriesDidgroupsDidGroupIdProvisionPost (string didGroupId)



This API didgroups provision. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CountriesDidgroupsDidGroupIdProvisionPostExample
    {
        public void main()
        {
            var apiInstance = new CountryApi();
            var didGroupId = didGroupId_example;  // string | didGroupId in the Country

            try
            {
                apiInstance.CountriesDidgroupsDidGroupIdProvisionPost(didGroupId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling CountryApi.CountriesDidgroupsDidGroupIdProvisionPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **didGroupId** | **string**| didGroupId in the Country | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="countriesget"></a>
# **CountriesGet**
> void CountriesGet ()



This API get countries. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CountriesGetExample
    {
        public void main()
        {
            var apiInstance = new CountryApi();

            try
            {
                apiInstance.CountriesGet();
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling CountryApi.CountriesGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="statescountrycodeget"></a>
# **StatesCountryCodeGet**
> void StatesCountryCodeGet (string countryCode)



This API get States . 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class StatesCountryCodeGetExample
    {
        public void main()
        {
            var apiInstance = new CountryApi();
            var countryCode = countryCode_example;  // string | countryCode in the Country

            try
            {
                apiInstance.StatesCountryCodeGet(countryCode);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling CountryApi.StatesCountryCodeGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **countryCode** | **string**| countryCode in the Country | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

