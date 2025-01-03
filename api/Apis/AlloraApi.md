# AlloraApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPriceInference**](AlloraApi.md#getPriceInference) | **GET** /allora/inference |  |
| [**impliedFuturePrice**](AlloraApi.md#impliedFuturePrice) | **GET** /allora/implied-future-price |  |
| [**logReturnToPercentage**](AlloraApi.md#logReturnToPercentage) | **GET** /allora/log-return-to-percentage |  |


<a name="getPriceInference"></a>
# **getPriceInference**
> AlloraInferenceResponse getPriceInference(asset, timeframe, currentPrice, Authorization)



    Get price inference for a specific asset and timeframe

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **asset** | [**Asset**](../Models/.md)| - The asset to get inference for (ETH or BTC) | [default to null] [enum: ETH, BTC] |
| **timeframe** | [**TimeFrame**](../Models/.md)| - The timeframe for the inference (5m or 8h) | [default to null] [enum: 5m, 8h] |
| **currentPrice** | **Double**| - The current price of the asset | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |

### Return type

[**AlloraInferenceResponse**](../Models/AlloraInferenceResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="impliedFuturePrice"></a>
# **impliedFuturePrice**
> ImpliedFuturePrice_200_response impliedFuturePrice(currentPrice, logReturn, Authorization)



    Calculate implied future price

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **currentPrice** | **Double**| - The current price of the asset | [default to null] |
| **logReturn** | **Double**| - The log return | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |

### Return type

[**ImpliedFuturePrice_200_response**](../Models/ImpliedFuturePrice_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="logReturnToPercentage"></a>
# **logReturnToPercentage**
> LogReturnToPercentage_200_response logReturnToPercentage(logReturn, Authorization)



    Convert log return to percentage

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **logReturn** | **Double**| - The log return to convert | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |

### Return type

[**LogReturnToPercentage_200_response**](../Models/LogReturnToPercentage_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

