# ENSApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**resolve**](ENSApi.md#resolve) | **POST** /ens/resolve |  |


<a name="resolve"></a>
# **resolve**
> EnsResolveAPIResponse resolve(Authorization, EnsResolveInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **EnsResolveInput** | [**EnsResolveInput**](../Models/EnsResolveInput.md)|  | |

### Return type

[**EnsResolveAPIResponse**](../Models/EnsResolveAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

