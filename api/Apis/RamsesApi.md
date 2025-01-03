# RamsesApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**calculateOptimalVoteDistribution**](RamsesApi.md#calculateOptimalVoteDistribution) | **GET** /ramses/data/vote-distribution |  |
| [**getInfo**](RamsesApi.md#getInfo) | **GET** /ramses/data/info |  |
| [**getPoolByAddress**](RamsesApi.md#getPoolByAddress) | **GET** /ramses/data/pools/{address} |  |
| [**getPools**](RamsesApi.md#getPools) | **GET** /ramses/data/pools |  |
| [**getPoolsByType**](RamsesApi.md#getPoolsByType) | **GET** /ramses/data/pools/type/{type} |  |
| [**getTokens**](RamsesApi.md#getTokens) | **GET** /ramses/data/tokens |  |
| [**getTopAPRPools**](RamsesApi.md#getTopAPRPools) | **GET** /ramses/data/pools/top-apr |  |
| [**getTotalValueLocked**](RamsesApi.md#getTotalValueLocked) | **GET** /ramses/data/tvl |  |


<a name="calculateOptimalVoteDistribution"></a>
# **calculateOptimalVoteDistribution**
> RamsesAPIResponse calculateOptimalVoteDistribution(Authorization, totalVotes, maxPools)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **totalVotes** | **Double**|  | [default to null] |
| **maxPools** | **Double**|  | [optional] [default to null] |

### Return type

[**RamsesAPIResponse**](../Models/RamsesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getInfo"></a>
# **getInfo**
> RamsesAPIResponse getInfo(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**RamsesAPIResponse**](../Models/RamsesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPoolByAddress"></a>
# **getPoolByAddress**
> RamsesAPIResponse getPoolByAddress(address, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**RamsesAPIResponse**](../Models/RamsesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPools"></a>
# **getPools**
> RamsesAPIResponse getPools(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**RamsesAPIResponse**](../Models/RamsesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPoolsByType"></a>
# **getPoolsByType**
> RamsesAPIResponse getPoolsByType(type, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **type** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**RamsesAPIResponse**](../Models/RamsesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTokens"></a>
# **getTokens**
> RamsesAPIResponse getTokens(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**RamsesAPIResponse**](../Models/RamsesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTopAPRPools"></a>
# **getTopAPRPools**
> RamsesAPIResponse getTopAPRPools(Authorization, limit)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **limit** | **Double**|  | [optional] [default to null] |

### Return type

[**RamsesAPIResponse**](../Models/RamsesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalValueLocked"></a>
# **getTotalValueLocked**
> RamsesAPIResponse getTotalValueLocked(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**RamsesAPIResponse**](../Models/RamsesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

