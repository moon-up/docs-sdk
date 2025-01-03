# LynexApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**calculateOptimalVoteDistribution**](LynexApi.md#calculateOptimalVoteDistribution) | **GET** /lynex/data/vote-distribution |  |
| [**getAssetByAddress**](LynexApi.md#getAssetByAddress) | **GET** /lynex/data/assets/{address} |  |
| [**getAssets**](LynexApi.md#getAssets) | **GET** /lynex/data/assets |  |
| [**getPoolByAddress**](LynexApi.md#getPoolByAddress) | **GET** /lynex/data/pools/{address} |  |
| [**getPools**](LynexApi.md#getPools) | **GET** /lynex/data/pools |  |
| [**getPoolsByType**](LynexApi.md#getPoolsByType) | **GET** /lynex/data/pools/type/{type} |  |
| [**getTopAPRPools**](LynexApi.md#getTopAPRPools) | **GET** /lynex/data/pools/top-apr |  |
| [**getTotalValueLocked**](LynexApi.md#getTotalValueLocked) | **GET** /lynex/data/tvl |  |


<a name="calculateOptimalVoteDistribution"></a>
# **calculateOptimalVoteDistribution**
> LynexAPIResponse calculateOptimalVoteDistribution(Authorization, totalVotes, maxPools)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **totalVotes** | **Double**|  | [default to null] |
| **maxPools** | **Double**|  | [optional] [default to null] |

### Return type

[**LynexAPIResponse**](../Models/LynexAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getAssetByAddress"></a>
# **getAssetByAddress**
> LynexAPIResponse getAssetByAddress(address, Authorization)



    Retrieves an asset by its address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the asset to retrieve. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |

### Return type

[**LynexAPIResponse**](../Models/LynexAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getAssets"></a>
# **getAssets**
> LynexAPIResponse getAssets(Authorization)



    Retrieves the assets using the provided authorization token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |

### Return type

[**LynexAPIResponse**](../Models/LynexAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPoolByAddress"></a>
# **getPoolByAddress**
> LynexAPIResponse getPoolByAddress(address, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**LynexAPIResponse**](../Models/LynexAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPools"></a>
# **getPools**
> LynexAPIResponse getPools(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**LynexAPIResponse**](../Models/LynexAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPoolsByType"></a>
# **getPoolsByType**
> LynexAPIResponse getPoolsByType(type, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **type** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**LynexAPIResponse**](../Models/LynexAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTopAPRPools"></a>
# **getTopAPRPools**
> LynexAPIResponse getTopAPRPools(Authorization, limit)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **limit** | **Double**|  | [optional] [default to null] |

### Return type

[**LynexAPIResponse**](../Models/LynexAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalValueLocked"></a>
# **getTotalValueLocked**
> LynexAPIResponse getTotalValueLocked(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**LynexAPIResponse**](../Models/LynexAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

