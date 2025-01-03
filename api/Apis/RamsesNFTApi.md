# RamsesNFTApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**abstain**](RamsesNFTApi.md#abstain) | **POST** /ramses/nft/{address}/abstain |  |
| [**approve**](RamsesNFTApi.md#approve) | **POST** /ramses/nft/{address}/approve |  |
| [**attach**](RamsesNFTApi.md#attach) | **POST** /ramses/nft/{address}/attach |  |
| [**createLock**](RamsesNFTApi.md#createLock) | **POST** /ramses/nft/{address}/createLock |  |
| [**delegate**](RamsesNFTApi.md#delegate) | **POST** /ramses/nft/{address}/delegate |  |
| [**detach**](RamsesNFTApi.md#detach) | **POST** /ramses/nft/{address}/detach |  |
| [**getBalanceOf**](RamsesNFTApi.md#getBalanceOf) | **GET** /ramses/nft/balanceOf |  |
| [**getBalanceOfNFT**](RamsesNFTApi.md#getBalanceOfNFT) | **GET** /ramses/nft/balanceOfNFT |  |
| [**getDelegates**](RamsesNFTApi.md#getDelegates) | **GET** /ramses/nft/delegates |  |
| [**getLocked**](RamsesNFTApi.md#getLocked) | **GET** /ramses/nft/locked |  |
| [**getOwnerOf**](RamsesNFTApi.md#getOwnerOf) | **GET** /ramses/nft/ownerOf |  |
| [**getPastVotes**](RamsesNFTApi.md#getPastVotes) | **GET** /ramses/nft/getPastVotes |  |
| [**getTokenURI**](RamsesNFTApi.md#getTokenURI) | **GET** /ramses/nft/tokenURI |  |
| [**getTotalSupply**](RamsesNFTApi.md#getTotalSupply) | **GET** /ramses/nft/totalSupply |  |
| [**getVotes**](RamsesNFTApi.md#getVotes) | **GET** /ramses/nft/getVotes |  |
| [**increaseAmount**](RamsesNFTApi.md#increaseAmount) | **POST** /ramses/nft/{address}/increaseAmount |  |
| [**increaseUnlockTime**](RamsesNFTApi.md#increaseUnlockTime) | **POST** /ramses/nft/{address}/increaseUnlockTime |  |
| [**merge**](RamsesNFTApi.md#merge) | **POST** /ramses/nft/{address}/merge |  |
| [**split**](RamsesNFTApi.md#split) | **POST** /ramses/nft/{address}/split |  |
| [**transferFrom**](RamsesNFTApi.md#transferFrom) | **POST** /ramses/nft/{address}/transferFrom |  |
| [**withdraw**](RamsesNFTApi.md#withdraw) | **POST** /ramses/nft/{address}/withdraw |  |


<a name="abstain"></a>
# **abstain**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ abstain(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="approve"></a>
# **approve**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ approve(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="attach"></a>
# **attach**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ attach(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createLock"></a>
# **createLock**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ createLock(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="delegate"></a>
# **delegate**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ delegate(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="detach"></a>
# **detach**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ detach(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getBalanceOf"></a>
# **getBalanceOf**
> RamsesNFTAPIResponse_string_ getBalanceOf(Authorization, chainId, address, owner)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **owner** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_string_**](../Models/RamsesNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBalanceOfNFT"></a>
# **getBalanceOfNFT**
> RamsesNFTAPIResponse_string_ getBalanceOfNFT(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_string_**](../Models/RamsesNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getDelegates"></a>
# **getDelegates**
> RamsesNFTAPIResponse_string_ getDelegates(Authorization, chainId, address, account)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **account** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_string_**](../Models/RamsesNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getLocked"></a>
# **getLocked**
> RamsesNFTAPIResponse_LockedData_ getLocked(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_LockedData_**](../Models/RamsesNFTAPIResponse_LockedData_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getOwnerOf"></a>
# **getOwnerOf**
> RamsesNFTAPIResponse_string_ getOwnerOf(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_string_**](../Models/RamsesNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPastVotes"></a>
# **getPastVotes**
> RamsesNFTAPIResponse_string_ getPastVotes(Authorization, chainId, address, account, blockNumber)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **account** | **String**|  | [default to null] |
| **blockNumber** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_string_**](../Models/RamsesNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTokenURI"></a>
# **getTokenURI**
> RamsesNFTAPIResponse_string_ getTokenURI(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_string_**](../Models/RamsesNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalSupply"></a>
# **getTotalSupply**
> RamsesNFTAPIResponse_string_ getTotalSupply(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_string_**](../Models/RamsesNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getVotes"></a>
# **getVotes**
> RamsesNFTAPIResponse_string_ getVotes(Authorization, chainId, address, account)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **account** | **String**|  | [default to null] |

### Return type

[**RamsesNFTAPIResponse_string_**](../Models/RamsesNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="increaseAmount"></a>
# **increaseAmount**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ increaseAmount(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="increaseUnlockTime"></a>
# **increaseUnlockTime**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ increaseUnlockTime(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="merge"></a>
# **merge**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ merge(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="split"></a>
# **split**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ split(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="transferFrom"></a>
# **transferFrom**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ transferFrom(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="withdraw"></a>
# **withdraw**
> RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_ withdraw(address, Authorization, RamsesNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesNFTInputBody** | [**RamsesNFTInputBody**](../Models/RamsesNFTInputBody.md)|  | |

### Return type

[**RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_**](../Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

