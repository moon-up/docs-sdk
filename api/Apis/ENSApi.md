# ENSApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**eNSResolve**](ENSApi.md#eNSResolve) | **POST** /ens/resolve |  |
| [**eNSReverseResolve**](ENSApi.md#eNSReverseResolve) | **POST** /ens/reverse |  |


<a name="eNSResolve"></a>
# **eNSResolve**
> EnsResolveAPIResponse eNSResolve(Authorization, EnsResolveInput)



    Resolves an ENS (Ethereum Name Service) name to its corresponding address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for accessing the ENS service. | [default to null] |
| **EnsResolveInput** | [**EnsResolveInput**](../Models/EnsResolveInput.md)| - The input data required for ENS resolution. | |

### Return type

[**EnsResolveAPIResponse**](../Models/EnsResolveAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="eNSReverseResolve"></a>
# **eNSReverseResolve**
> ENSReverseResolveAPIResponse eNSReverseResolve(Authorization, ENSReverseResolveInput)



    Resolves an ENS (Ethereum Name Service) address to its corresponding name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for accessing the ENS service. | [default to null] |
| **ENSReverseResolveInput** | [**ENSReverseResolveInput**](../Models/ENSReverseResolveInput.md)| - The input data required for ENS reverse resolution. | |

### Return type

[**ENSReverseResolveAPIResponse**](../Models/ENSReverseResolveAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

