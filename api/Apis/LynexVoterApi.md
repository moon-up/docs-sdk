# LynexVoterApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**claimBribes**](LynexVoterApi.md#claimBribes) | **POST** /lynex/voter/{address}/claimBribes |  |
| [**claimFees**](LynexVoterApi.md#claimFees) | **POST** /lynex/voter/{address}/claimFees |  |
| [**claimRewards**](LynexVoterApi.md#claimRewards) | **POST** /lynex/voter/{address}/claimRewards |  |
| [**createGauge**](LynexVoterApi.md#createGauge) | **POST** /lynex/voter/{address}/createGauge |  |
| [**distribute**](LynexVoterApi.md#distribute) | **POST** /lynex/voter/{address}/distribute |  |
| [**getLastVoted**](LynexVoterApi.md#getLastVoted) | **GET** /lynex/voter/lastVoted |  |
| [**getPoolVoteLength**](LynexVoterApi.md#getPoolVoteLength) | **GET** /lynex/voter/poolVoteLength |  |
| [**getTotalWeight**](LynexVoterApi.md#getTotalWeight) | **GET** /lynex/voter/totalWeight |  |
| [**getWeights**](LynexVoterApi.md#getWeights) | **GET** /lynex/voter/weights |  |
| [**isGauge**](LynexVoterApi.md#isGauge) | **GET** /lynex/voter/isGauge |  |
| [**isWhitelisted**](LynexVoterApi.md#isWhitelisted) | **GET** /lynex/voter/isWhitelisted |  |
| [**killGauge**](LynexVoterApi.md#killGauge) | **POST** /lynex/voter/{address}/killGauge |  |
| [**notifyRewardAmount**](LynexVoterApi.md#notifyRewardAmount) | **POST** /lynex/voter/{address}/notifyRewardAmount |  |
| [**poke**](LynexVoterApi.md#poke) | **POST** /lynex/voter/{address}/poke |  |
| [**reset**](LynexVoterApi.md#reset) | **POST** /lynex/voter/{address}/reset |  |
| [**reviveGauge**](LynexVoterApi.md#reviveGauge) | **POST** /lynex/voter/{address}/reviveGauge |  |
| [**vote**](LynexVoterApi.md#vote) | **POST** /lynex/voter/{address}/vote |  |
| [**voteWithOptimalDistribution**](LynexVoterApi.md#voteWithOptimalDistribution) | **POST** /lynex/voter/{address}/voteWithOptimalDistribution |  |
| [**whitelist**](LynexVoterApi.md#whitelist) | **POST** /lynex/voter/{address}/whitelist |  |


<a name="claimBribes"></a>
# **claimBribes**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ claimBribes(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claimFees"></a>
# **claimFees**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ claimFees(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claimRewards"></a>
# **claimRewards**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ claimRewards(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createGauge"></a>
# **createGauge**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ createGauge(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="distribute"></a>
# **distribute**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ distribute(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getLastVoted"></a>
# **getLastVoted**
> LynexVoterAPIResponse_string_ getLastVoted(Authorization, chainId, address, voter)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **voter** | **String**|  | [default to null] |

### Return type

[**LynexVoterAPIResponse_string_**](../Models/LynexVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPoolVoteLength"></a>
# **getPoolVoteLength**
> LynexVoterAPIResponse_string_ getPoolVoteLength(Authorization, chainId, address, voter)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **voter** | **String**|  | [default to null] |

### Return type

[**LynexVoterAPIResponse_string_**](../Models/LynexVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalWeight"></a>
# **getTotalWeight**
> LynexVoterAPIResponse_string_ getTotalWeight(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**LynexVoterAPIResponse_string_**](../Models/LynexVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getWeights"></a>
# **getWeights**
> LynexVoterAPIResponse_string_ getWeights(Authorization, chainId, address, pool)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **pool** | **String**|  | [default to null] |

### Return type

[**LynexVoterAPIResponse_string_**](../Models/LynexVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="isGauge"></a>
# **isGauge**
> LynexVoterAPIResponse_boolean_ isGauge(Authorization, chainId, address, gauge)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **gauge** | **String**|  | [default to null] |

### Return type

[**LynexVoterAPIResponse_boolean_**](../Models/LynexVoterAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="isWhitelisted"></a>
# **isWhitelisted**
> LynexVoterAPIResponse_boolean_ isWhitelisted(Authorization, chainId, address, token)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **token** | **String**|  | [default to null] |

### Return type

[**LynexVoterAPIResponse_boolean_**](../Models/LynexVoterAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="killGauge"></a>
# **killGauge**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ killGauge(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="notifyRewardAmount"></a>
# **notifyRewardAmount**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ notifyRewardAmount(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="poke"></a>
# **poke**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ poke(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="reset"></a>
# **reset**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ reset(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="reviveGauge"></a>
# **reviveGauge**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ reviveGauge(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="vote"></a>
# **vote**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ vote(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="voteWithOptimalDistribution"></a>
# **voteWithOptimalDistribution**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ voteWithOptimalDistribution(address, Authorization, VoteWithOptimalDistribution\_request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VoteWithOptimalDistribution\_request** | [**VoteWithOptimalDistribution_request**](../Models/VoteWithOptimalDistribution_request.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="whitelist"></a>
# **whitelist**
> LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_ whitelist(address, Authorization, LynexVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexVoterInputBody** | [**LynexVoterInputBody**](../Models/LynexVoterInputBody.md)|  | |

### Return type

[**LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_**](../Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

