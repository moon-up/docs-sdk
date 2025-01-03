# ThorSwapApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getGasPrice**](ThorSwapApi.md#getGasPrice) | **GET** /thorswap/gasPrice |  |
| [**getQuote**](ThorSwapApi.md#getQuote) | **GET** /thorswap/quote |  |
| [**getSupportedChains**](ThorSwapApi.md#getSupportedChains) | **GET** /thorswap/supportedChains |  |
| [**getSupportedProviders**](ThorSwapApi.md#getSupportedProviders) | **GET** /thorswap/supportedProviders |  |
| [**swap**](ThorSwapApi.md#swap) | **POST** /thorswap/swap |  |


<a name="getGasPrice"></a>
# **getGasPrice**
> ThorSwapAPIResponse_GasPrice_ getGasPrice(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**ThorSwapAPIResponse_GasPrice_**](../Models/ThorSwapAPIResponse_GasPrice_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getQuote"></a>
# **getQuote**
> ThorSwapAPIResponse_Quote_ getQuote(Authorization, sellAsset, buyAsset, sellAmount, senderAddress, recipientAddress, chainId, slippage, limit, providers, preferredProvider, affiliateAddress, affiliateBasisPoints, allowSmartContractRecipient)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **sellAsset** | **String**|  | [default to null] |
| **buyAsset** | **String**|  | [default to null] |
| **sellAmount** | **Double**|  | [default to null] |
| **senderAddress** | **String**|  | [default to null] |
| **recipientAddress** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **slippage** | **Double**|  | [optional] [default to null] |
| **limit** | **Double**|  | [optional] [default to null] |
| **providers** | [**List**](../Models/String.md)|  | [optional] [default to null] |
| **preferredProvider** | **String**|  | [optional] [default to null] |
| **affiliateAddress** | **String**|  | [optional] [default to null] |
| **affiliateBasisPoints** | **Double**|  | [optional] [default to null] |
| **allowSmartContractRecipient** | **Boolean**|  | [optional] [default to null] |

### Return type

[**ThorSwapAPIResponse_Quote_**](../Models/ThorSwapAPIResponse_Quote_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getSupportedChains"></a>
# **getSupportedChains**
> ThorSwapAPIResponse_string-Array_ getSupportedChains(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**ThorSwapAPIResponse_string-Array_**](../Models/ThorSwapAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getSupportedProviders"></a>
# **getSupportedProviders**
> ThorSwapAPIResponse_string-Array_ getSupportedProviders(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**ThorSwapAPIResponse_string-Array_**](../Models/ThorSwapAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="swap"></a>
# **swap**
> ThorSwapAPIResponse_string_ swap(Authorization, Swap\_request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **Swap\_request** | [**Swap_request**](../Models/Swap_request.md)|  | |

### Return type

[**ThorSwapAPIResponse_string_**](../Models/ThorSwapAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

