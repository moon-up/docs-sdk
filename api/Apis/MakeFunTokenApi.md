# MakeFunTokenApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**makeFunTokenGetCLFactory**](MakeFunTokenApi.md#makeFunTokenGetCLFactory) | **GET** /makefuntoken/{account}/CLFactory |  |
| [**makeFunTokenGetMaxTick**](MakeFunTokenApi.md#makeFunTokenGetMaxTick) | **GET** /makefuntoken/{account}/maxTick |  |
| [**makeFunTokenGetMinTick**](MakeFunTokenApi.md#makeFunTokenGetMinTick) | **GET** /makefuntoken/{account}/minTick |  |
| [**makeFunTokenMakeToken**](MakeFunTokenApi.md#makeFunTokenMakeToken) | **POST** /makefuntoken/{address}/makeToken |  |
| [**makeFunTokenSetSupplyLimits**](MakeFunTokenApi.md#makeFunTokenSetSupplyLimits) | **POST** /makefuntoken/{address}/setSupplyLimits |  |
| [**makeFunTokenSetTickLimits**](MakeFunTokenApi.md#makeFunTokenSetTickLimits) | **POST** /makefuntoken/{address}/setTickLimits |  |


<a name="makeFunTokenGetCLFactory"></a>
# **makeFunTokenGetCLFactory**
> MakeFunTokenHelperAPIResponse_string_ makeFunTokenGetCLFactory(account, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**MakeFunTokenHelperAPIResponse_string_**](../Models/MakeFunTokenHelperAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="makeFunTokenGetMaxTick"></a>
# **makeFunTokenGetMaxTick**
> MakeFunTokenHelperAPIResponse_number_ makeFunTokenGetMaxTick(account, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**MakeFunTokenHelperAPIResponse_number_**](../Models/MakeFunTokenHelperAPIResponse_number_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="makeFunTokenGetMinTick"></a>
# **makeFunTokenGetMinTick**
> MakeFunTokenHelperAPIResponse_number_ makeFunTokenGetMinTick(account, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**MakeFunTokenHelperAPIResponse_number_**](../Models/MakeFunTokenHelperAPIResponse_number_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="makeFunTokenMakeToken"></a>
# **makeFunTokenMakeToken**
> MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_ makeFunTokenMakeToken(address, Authorization, MakeFunTokenHelperInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **MakeFunTokenHelperInputBody** | [**MakeFunTokenHelperInputBody**](../Models/MakeFunTokenHelperInputBody.md)|  | |

### Return type

[**MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_**](../Models/MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="makeFunTokenSetSupplyLimits"></a>
# **makeFunTokenSetSupplyLimits**
> MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_ makeFunTokenSetSupplyLimits(address, Authorization, MakeFunTokenHelperInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **MakeFunTokenHelperInputBody** | [**MakeFunTokenHelperInputBody**](../Models/MakeFunTokenHelperInputBody.md)|  | |

### Return type

[**MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_**](../Models/MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="makeFunTokenSetTickLimits"></a>
# **makeFunTokenSetTickLimits**
> MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_ makeFunTokenSetTickLimits(address, Authorization, MakeFunTokenHelperInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **MakeFunTokenHelperInputBody** | [**MakeFunTokenHelperInputBody**](../Models/MakeFunTokenHelperInputBody.md)|  | |

### Return type

[**MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_**](../Models/MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

