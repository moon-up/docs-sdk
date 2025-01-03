# ThenaApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**calculateOptimalVoteDistribution**](ThenaApi.md#calculateOptimalVoteDistribution) | **GET** /thena/data/vote-distribution |  |
| [**getFusionByAddress**](ThenaApi.md#getFusionByAddress) | **GET** /thena/data/fusions/{address} |  |
| [**getFusions**](ThenaApi.md#getFusions) | **GET** /thena/data/fusions |  |
| [**getFusionsByType**](ThenaApi.md#getFusionsByType) | **GET** /thena/data/fusions/type/{type} |  |
| [**getTopAPRFusions**](ThenaApi.md#getTopAPRFusions) | **GET** /thena/data/fusions/top-apr |  |
| [**getTopPairs**](ThenaApi.md#getTopPairs) | **GET** /thena/data/pairs/top |  |
| [**getTopTokens**](ThenaApi.md#getTopTokens) | **GET** /thena/data/tokens/top |  |
| [**getTotalValueLocked**](ThenaApi.md#getTotalValueLocked) | **GET** /thena/data/tvl |  |


<a name="calculateOptimalVoteDistribution"></a>
# **calculateOptimalVoteDistribution**
> ThenaAPIResponse calculateOptimalVoteDistribution(Authorization, totalVotes, maxFusions)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **totalVotes** | **Double**|  | [default to null] |
| **maxFusions** | **Double**|  | [optional] [default to null] |

### Return type

[**ThenaAPIResponse**](../Models/ThenaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getFusionByAddress"></a>
# **getFusionByAddress**
> ThenaAPIResponse getFusionByAddress(address, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**ThenaAPIResponse**](../Models/ThenaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getFusions"></a>
# **getFusions**
> ThenaAPIResponse getFusions(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**ThenaAPIResponse**](../Models/ThenaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getFusionsByType"></a>
# **getFusionsByType**
> ThenaAPIResponse getFusionsByType(type, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **type** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**ThenaAPIResponse**](../Models/ThenaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTopAPRFusions"></a>
# **getTopAPRFusions**
> ThenaAPIResponse getTopAPRFusions(Authorization, limit)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **limit** | **Double**|  | [optional] [default to null] |

### Return type

[**ThenaAPIResponse**](../Models/ThenaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTopPairs"></a>
# **getTopPairs**
> ThenaAPIResponse getTopPairs(Authorization, limit)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **limit** | **Double**|  | [optional] [default to null] |

### Return type

[**ThenaAPIResponse**](../Models/ThenaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTopTokens"></a>
# **getTopTokens**
> ThenaAPIResponse getTopTokens(Authorization, limit)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **limit** | **Double**|  | [optional] [default to null] |

### Return type

[**ThenaAPIResponse**](../Models/ThenaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalValueLocked"></a>
# **getTotalValueLocked**
> ThenaAPIResponse getTotalValueLocked(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**ThenaAPIResponse**](../Models/ThenaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

