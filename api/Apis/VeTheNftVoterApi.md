# VeTheNftVoterApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**attachTokenToGauge**](VeTheNftVoterApi.md#attachTokenToGauge) | **POST** /thena/voter/{address}/attachTokenToGauge |  |
| [**claimBribes**](VeTheNftVoterApi.md#claimBribes) | **POST** /thena/voter/{address}/claimBribes |  |
| [**claimFees**](VeTheNftVoterApi.md#claimFees) | **POST** /thena/voter/{address}/claimFees |  |
| [**claimRewards**](VeTheNftVoterApi.md#claimRewards) | **POST** /thena/voter/{address}/claimRewards |  |
| [**createGauge**](VeTheNftVoterApi.md#createGauge) | **POST** /thena/voter/{address}/createGauge |  |
| [**detachTokenFromGauge**](VeTheNftVoterApi.md#detachTokenFromGauge) | **POST** /thena/voter/{address}/detachTokenFromGauge |  |
| [**distribute**](VeTheNftVoterApi.md#distribute) | **POST** /thena/voter/{address}/distribute |  |
| [**getTotalWeight**](VeTheNftVoterApi.md#getTotalWeight) | **GET** /thena/voter/totalWeight |  |
| [**getWeights**](VeTheNftVoterApi.md#getWeights) | **GET** /thena/voter/weights |  |
| [**isGauge**](VeTheNftVoterApi.md#isGauge) | **GET** /thena/voter/isGauge |  |
| [**isWhitelisted**](VeTheNftVoterApi.md#isWhitelisted) | **GET** /thena/voter/isWhitelisted |  |
| [**killGauge**](VeTheNftVoterApi.md#killGauge) | **POST** /thena/voter/{address}/killGauge |  |
| [**lastVoted**](VeTheNftVoterApi.md#lastVoted) | **GET** /thena/voter/lastVoted |  |
| [**notifyRewardAmount**](VeTheNftVoterApi.md#notifyRewardAmount) | **POST** /thena/voter/{address}/notifyRewardAmount |  |
| [**poke**](VeTheNftVoterApi.md#poke) | **POST** /thena/voter/{address}/poke |  |
| [**poolVoteLength**](VeTheNftVoterApi.md#poolVoteLength) | **GET** /thena/voter/poolVoteLength |  |
| [**reset**](VeTheNftVoterApi.md#reset) | **POST** /thena/voter/{address}/reset |  |
| [**reviveGauge**](VeTheNftVoterApi.md#reviveGauge) | **POST** /thena/voter/{address}/reviveGauge |  |
| [**vote**](VeTheNftVoterApi.md#vote) | **POST** /thena/voter/{address}/vote |  |
| [**voteWithOptimalDistribution**](VeTheNftVoterApi.md#voteWithOptimalDistribution) | **POST** /thena/voter/{address}/voteWithOptimalDistribution |  |
| [**whitelist**](VeTheNftVoterApi.md#whitelist) | **POST** /thena/voter/{address}/whitelist |  |


<a name="attachTokenToGauge"></a>
# **attachTokenToGauge**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ attachTokenToGauge(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claimBribes"></a>
# **claimBribes**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ claimBribes(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claimFees"></a>
# **claimFees**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ claimFees(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claimRewards"></a>
# **claimRewards**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ claimRewards(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createGauge"></a>
# **createGauge**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ createGauge(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="detachTokenFromGauge"></a>
# **detachTokenFromGauge**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ detachTokenFromGauge(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="distribute"></a>
# **distribute**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ distribute(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getTotalWeight"></a>
# **getTotalWeight**
> VeTheNftVoterAPIResponse_string_ getTotalWeight(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNftVoterAPIResponse_string_**](../Models/VeTheNftVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getWeights"></a>
# **getWeights**
> VeTheNftVoterAPIResponse_string_ getWeights(Authorization, chainId, address, pool)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **pool** | **String**|  | [default to null] |

### Return type

[**VeTheNftVoterAPIResponse_string_**](../Models/VeTheNftVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="isGauge"></a>
# **isGauge**
> VeTheNftVoterAPIResponse_boolean_ isGauge(Authorization, chainId, address, gauge)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **gauge** | **String**|  | [default to null] |

### Return type

[**VeTheNftVoterAPIResponse_boolean_**](../Models/VeTheNftVoterAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="isWhitelisted"></a>
# **isWhitelisted**
> VeTheNftVoterAPIResponse_boolean_ isWhitelisted(Authorization, chainId, address, tokenAddress)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenAddress** | **String**|  | [default to null] |

### Return type

[**VeTheNftVoterAPIResponse_boolean_**](../Models/VeTheNftVoterAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="killGauge"></a>
# **killGauge**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ killGauge(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="lastVoted"></a>
# **lastVoted**
> VeTheNftVoterAPIResponse_string_ lastVoted(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**VeTheNftVoterAPIResponse_string_**](../Models/VeTheNftVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="notifyRewardAmount"></a>
# **notifyRewardAmount**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ notifyRewardAmount(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="poke"></a>
# **poke**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ poke(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="poolVoteLength"></a>
# **poolVoteLength**
> VeTheNftVoterAPIResponse_string_ poolVoteLength(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**VeTheNftVoterAPIResponse_string_**](../Models/VeTheNftVoterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="reset"></a>
# **reset**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ reset(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="reviveGauge"></a>
# **reviveGauge**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ reviveGauge(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="vote"></a>
# **vote**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ vote(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="voteWithOptimalDistribution"></a>
# **voteWithOptimalDistribution**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ voteWithOptimalDistribution(address, Authorization, VoteWithOptimalDistribution\_request\_2)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VoteWithOptimalDistribution\_request\_2** | [**VoteWithOptimalDistribution_request_2**](../Models/VoteWithOptimalDistribution_request_2.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="whitelist"></a>
# **whitelist**
> VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_ whitelist(address, Authorization, VeTheNftVoterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeTheNftVoterInputBody** | [**VeTheNftVoterInputBody**](../Models/VeTheNftVoterInputBody.md)|  | |

### Return type

[**VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_**](../Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

