# RamsesVoterApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**attachTokenToGauge**](RamsesVoterApi.md#attachTokenToGauge) | **POST** /ramses/voter/{address}/attachTokenToGauge |  |
| [**claimBribes**](RamsesVoterApi.md#claimBribes) | **POST** /ramses/voter/{address}/claimBribes |  |
| [**claimFees**](RamsesVoterApi.md#claimFees) | **POST** /ramses/voter/{address}/claimFees |  |
| [**claimRewards**](RamsesVoterApi.md#claimRewards) | **POST** /ramses/voter/{address}/claimRewards |  |
| [**createGauge**](RamsesVoterApi.md#createGauge) | **POST** /ramses/voter/{address}/createGauge |  |
| [**detachTokenFromGauge**](RamsesVoterApi.md#detachTokenFromGauge) | **POST** /ramses/voter/{address}/detachTokenFromGauge |  |
| [**distribute**](RamsesVoterApi.md#distribute) | **POST** /ramses/voter/{address}/distribute |  |
| [**getLastVoted**](RamsesVoterApi.md#getLastVoted) | **GET** /ramses/voter/lastVoted |  |
| [**getTotalWeight**](RamsesVoterApi.md#getTotalWeight) | **GET** /ramses/voter/totalWeight |  |
| [**getWeights**](RamsesVoterApi.md#getWeights) | **GET** /ramses/voter/weights |  |
| [**isGauge**](RamsesVoterApi.md#isGauge) | **GET** /ramses/voter/isGauge |  |
| [**isWhitelisted**](RamsesVoterApi.md#isWhitelisted) | **GET** /ramses/voter/isWhitelisted |  |
| [**killGauge**](RamsesVoterApi.md#killGauge) | **POST** /ramses/voter/{address}/killGauge |  |
| [**notifyRewardAmount**](RamsesVoterApi.md#notifyRewardAmount) | **POST** /ramses/voter/{address}/notifyRewardAmount |  |
| [**poke**](RamsesVoterApi.md#poke) | **POST** /ramses/voter/{address}/poke |  |
| [**reset**](RamsesVoterApi.md#reset) | **POST** /ramses/voter/{address}/reset |  |
| [**reviveGauge**](RamsesVoterApi.md#reviveGauge) | **POST** /ramses/voter/{address}/reviveGauge |  |
| [**vote**](RamsesVoterApi.md#vote) | **POST** /ramses/voter/{address}/vote |  |
| [**voteWithOptimalDistribution**](RamsesVoterApi.md#voteWithOptimalDistribution) | **POST** /ramses/voter/{address}/voteWithOptimalDistribution |  |
| [**whitelist**](RamsesVoterApi.md#whitelist) | **POST** /ramses/voter/{address}/whitelist |  |


<a name="attachTokenToGauge"></a>
# **attachTokenToGauge**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ attachTokenToGauge(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claimBribes"></a>
# **claimBribes**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ claimBribes(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claimFees"></a>
# **claimFees**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ claimFees(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claimRewards"></a>
# **claimRewards**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ claimRewards(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createGauge"></a>
# **createGauge**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ createGauge(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="detachTokenFromGauge"></a>
# **detachTokenFromGauge**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ detachTokenFromGauge(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="distribute"></a>
# **distribute**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ distribute(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getLastVoted"></a>
# **getLastVoted**
> RamsesVoterAPIResponse_string_ getLastVoted(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**RamsesVoterAPIResponse_string_**](../Models/RamsesVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalWeight"></a>
# **getTotalWeight**
> RamsesVoterAPIResponse_string_ getTotalWeight(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**RamsesVoterAPIResponse_string_**](../Models/RamsesVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getWeights"></a>
# **getWeights**
> RamsesVoterAPIResponse_string_ getWeights(Authorization, chainId, address, pool)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **pool** | **String**|  | [default to null] |

### Return type

[**RamsesVoterAPIResponse_string_**](../Models/RamsesVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="isGauge"></a>
# **isGauge**
> RamsesVoterAPIResponse_boolean_ isGauge(Authorization, chainId, address, gauge)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **gauge** | **String**|  | [default to null] |

### Return type

[**RamsesVoterAPIResponse_boolean_**](../Models/RamsesVoterAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="isWhitelisted"></a>
# **isWhitelisted**
> RamsesVoterAPIResponse_boolean_ isWhitelisted(Authorization, chainId, address, token)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **token** | **String**|  | [default to null] |

### Return type

[**RamsesVoterAPIResponse_boolean_**](../Models/RamsesVoterAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="killGauge"></a>
# **killGauge**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ killGauge(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="notifyRewardAmount"></a>
# **notifyRewardAmount**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ notifyRewardAmount(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="poke"></a>
# **poke**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ poke(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="reset"></a>
# **reset**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ reset(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="reviveGauge"></a>
# **reviveGauge**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ reviveGauge(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="vote"></a>
# **vote**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ vote(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="voteWithOptimalDistribution"></a>
# **voteWithOptimalDistribution**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ voteWithOptimalDistribution(address, Authorization, VoteWithOptimalDistribution\_request\_1)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VoteWithOptimalDistribution\_request\_1** | [**VoteWithOptimalDistribution_request_1**](../Models/VoteWithOptimalDistribution_request_1.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="whitelist"></a>
# **whitelist**
> RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_ whitelist(address, Authorization, RamsesVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesVoterInputBody** | [**RamsesVoterInputBody**](../Models/RamsesVoterInputBody.md)|  | |

### Return type

[**RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_**](../Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

