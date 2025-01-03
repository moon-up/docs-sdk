# LynexNFTApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**approve**](LynexNFTApi.md#approve) | **POST** /lynex/nft/{address}/approve |  |
| [**burn**](LynexNFTApi.md#burn) | **POST** /lynex/nft/{address}/burn |  |
| [**checkpoint**](LynexNFTApi.md#checkpoint) | **POST** /lynex/nft/{address}/checkpoint |  |
| [**checkpointDelegatee**](LynexNFTApi.md#checkpointDelegatee) | **POST** /lynex/nft/{address}/checkpointDelegatee |  |
| [**claim**](LynexNFTApi.md#claim) | **POST** /lynex/nft/{address}/claim |  |
| [**createDelegatedLockFor**](LynexNFTApi.md#createDelegatedLockFor) | **POST** /lynex/nft/{address}/createDelegatedLockFor |  |
| [**createLock**](LynexNFTApi.md#createLock) | **POST** /lynex/nft/{address}/createLock |  |
| [**createLockFor**](LynexNFTApi.md#createLockFor) | **POST** /lynex/nft/{address}/createLockFor |  |
| [**delegate**](LynexNFTApi.md#delegate) | **POST** /lynex/nft/{address}/delegate |  |
| [**delegateBySig**](LynexNFTApi.md#delegateBySig) | **POST** /lynex/nft/{address}/delegateBySig |  |
| [**getApproved**](LynexNFTApi.md#getApproved) | **GET** /lynex/nft/getApproved |  |
| [**getBalanceOf**](LynexNFTApi.md#getBalanceOf) | **GET** /lynex/nft/balanceOf |  |
| [**getBalanceOfNFT**](LynexNFTApi.md#getBalanceOfNFT) | **GET** /lynex/nft/balanceOfNFT |  |
| [**getBalanceOfNFTAt**](LynexNFTApi.md#getBalanceOfNFTAt) | **GET** /lynex/nft/balanceOfNFTAt |  |
| [**getDelegates**](LynexNFTApi.md#getDelegates) | **GET** /lynex/nft/delegates |  |
| [**getLockDetails**](LynexNFTApi.md#getLockDetails) | **GET** /lynex/nft/lockDetails |  |
| [**getName**](LynexNFTApi.md#getName) | **GET** /lynex/nft/name |  |
| [**getOwnerOf**](LynexNFTApi.md#getOwnerOf) | **GET** /lynex/nft/ownerOf |  |
| [**getPastVotes**](LynexNFTApi.md#getPastVotes) | **GET** /lynex/nft/getPastVotes |  |
| [**getSymbol**](LynexNFTApi.md#getSymbol) | **GET** /lynex/nft/symbol |  |
| [**getTokenByIndex**](LynexNFTApi.md#getTokenByIndex) | **GET** /lynex/nft/tokenByIndex |  |
| [**getTokenOfOwnerByIndex**](LynexNFTApi.md#getTokenOfOwnerByIndex) | **GET** /lynex/nft/tokenOfOwnerByIndex |  |
| [**getTokenURI**](LynexNFTApi.md#getTokenURI) | **GET** /lynex/nft/tokenURI |  |
| [**getTotalNftsMinted**](LynexNFTApi.md#getTotalNftsMinted) | **GET** /lynex/nft/totalNftsMinted |  |
| [**getTotalSupply**](LynexNFTApi.md#getTotalSupply) | **GET** /lynex/nft/totalSupply |  |
| [**getVestedPayout**](LynexNFTApi.md#getVestedPayout) | **GET** /lynex/nft/vestedPayout |  |
| [**getVestedPayoutAtTime**](LynexNFTApi.md#getVestedPayoutAtTime) | **GET** /lynex/nft/vestedPayoutAtTime |  |
| [**getVestingPayout**](LynexNFTApi.md#getVestingPayout) | **GET** /lynex/nft/vestingPayout |  |
| [**getVestingPeriod**](LynexNFTApi.md#getVestingPeriod) | **GET** /lynex/nft/vestingPeriod |  |
| [**getVotes**](LynexNFTApi.md#getVotes) | **GET** /lynex/nft/getVotes |  |
| [**globalCheckpoint**](LynexNFTApi.md#globalCheckpoint) | **POST** /lynex/nft/{address}/globalCheckpoint |  |
| [**increaseLockAmount**](LynexNFTApi.md#increaseLockAmount) | **POST** /lynex/nft/{address}/increaseLockAmount |  |
| [**increaseUnlockTime**](LynexNFTApi.md#increaseUnlockTime) | **POST** /lynex/nft/{address}/increaseUnlockTime |  |
| [**isApprovedForAll**](LynexNFTApi.md#isApprovedForAll) | **GET** /lynex/nft/isApprovedForAll |  |
| [**merge**](LynexNFTApi.md#merge) | **POST** /lynex/nft/{address}/merge |  |
| [**safeTransferFrom**](LynexNFTApi.md#safeTransferFrom) | **POST** /lynex/nft/{address}/safeTransferFrom |  |
| [**setApprovalForAll**](LynexNFTApi.md#setApprovalForAll) | **POST** /lynex/nft/{address}/setApprovalForAll |  |
| [**setClaimApproval**](LynexNFTApi.md#setClaimApproval) | **POST** /lynex/nft/{address}/setClaimApproval |  |
| [**setClaimApprovalForAll**](LynexNFTApi.md#setClaimApprovalForAll) | **POST** /lynex/nft/{address}/setClaimApprovalForAll |  |
| [**split**](LynexNFTApi.md#split) | **POST** /lynex/nft/{address}/split |  |
| [**transferFrom**](LynexNFTApi.md#transferFrom) | **POST** /lynex/nft/{address}/transferFrom |  |
| [**unlockPermanent**](LynexNFTApi.md#unlockPermanent) | **POST** /lynex/nft/{address}/unlockPermanent |  |


<a name="approve"></a>
# **approve**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ approve(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="burn"></a>
# **burn**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ burn(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="checkpoint"></a>
# **checkpoint**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ checkpoint(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="checkpointDelegatee"></a>
# **checkpointDelegatee**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ checkpointDelegatee(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="claim"></a>
# **claim**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ claim(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createDelegatedLockFor"></a>
# **createDelegatedLockFor**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ createDelegatedLockFor(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createLock"></a>
# **createLock**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ createLock(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createLockFor"></a>
# **createLockFor**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ createLockFor(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="delegate"></a>
# **delegate**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ delegate(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="delegateBySig"></a>
# **delegateBySig**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ delegateBySig(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getApproved"></a>
# **getApproved**
> LynexNFTAPIResponse_string_ getApproved(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBalanceOf"></a>
# **getBalanceOf**
> LynexNFTAPIResponse_string_ getBalanceOf(Authorization, chainId, address, owner)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **owner** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBalanceOfNFT"></a>
# **getBalanceOfNFT**
> LynexNFTAPIResponse_string_ getBalanceOfNFT(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBalanceOfNFTAt"></a>
# **getBalanceOfNFTAt**
> LynexNFTAPIResponse_string_ getBalanceOfNFTAt(Authorization, chainId, address, tokenId, timestamp)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |
| **timestamp** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getDelegates"></a>
# **getDelegates**
> LynexNFTAPIResponse_string_ getDelegates(Authorization, chainId, address, tokenId, timestamp)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |
| **timestamp** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getLockDetails"></a>
# **getLockDetails**
> LynexNFTAPIResponse_any_ getLockDetails(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_any_**](../Models/LynexNFTAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getName"></a>
# **getName**
> LynexNFTAPIResponse_string_ getName(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getOwnerOf"></a>
# **getOwnerOf**
> LynexNFTAPIResponse_string_ getOwnerOf(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPastVotes"></a>
# **getPastVotes**
> LynexNFTAPIResponse_string_ getPastVotes(Authorization, chainId, address, account, timestamp)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **account** | **String**|  | [default to null] |
| **timestamp** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getSymbol"></a>
# **getSymbol**
> LynexNFTAPIResponse_string_ getSymbol(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTokenByIndex"></a>
# **getTokenByIndex**
> LynexNFTAPIResponse_string_ getTokenByIndex(Authorization, chainId, address, index)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **index** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTokenOfOwnerByIndex"></a>
# **getTokenOfOwnerByIndex**
> LynexNFTAPIResponse_string_ getTokenOfOwnerByIndex(Authorization, chainId, address, owner, index)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **owner** | **String**|  | [default to null] |
| **index** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTokenURI"></a>
# **getTokenURI**
> LynexNFTAPIResponse_string_ getTokenURI(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalNftsMinted"></a>
# **getTotalNftsMinted**
> LynexNFTAPIResponse_string_ getTotalNftsMinted(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalSupply"></a>
# **getTotalSupply**
> LynexNFTAPIResponse_string_ getTotalSupply(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getVestedPayout"></a>
# **getVestedPayout**
> LynexNFTAPIResponse_string_ getVestedPayout(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getVestedPayoutAtTime"></a>
# **getVestedPayoutAtTime**
> LynexNFTAPIResponse_string_ getVestedPayoutAtTime(Authorization, chainId, address, tokenId, timestamp)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |
| **timestamp** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getVestingPayout"></a>
# **getVestingPayout**
> LynexNFTAPIResponse_string_ getVestingPayout(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getVestingPeriod"></a>
# **getVestingPeriod**
> LynexNFTAPIResponse_VestingPeriodData_ getVestingPeriod(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_VestingPeriodData_**](../Models/LynexNFTAPIResponse_VestingPeriodData_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getVotes"></a>
# **getVotes**
> LynexNFTAPIResponse_string_ getVotes(Authorization, chainId, address, account)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **account** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_string_**](../Models/LynexNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="globalCheckpoint"></a>
# **globalCheckpoint**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ globalCheckpoint(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="increaseLockAmount"></a>
# **increaseLockAmount**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ increaseLockAmount(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="increaseUnlockTime"></a>
# **increaseUnlockTime**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ increaseUnlockTime(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="isApprovedForAll"></a>
# **isApprovedForAll**
> LynexNFTAPIResponse_boolean_ isApprovedForAll(Authorization, chainId, address, owner, operator)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **owner** | **String**|  | [default to null] |
| **operator** | **String**|  | [default to null] |

### Return type

[**LynexNFTAPIResponse_boolean_**](../Models/LynexNFTAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="merge"></a>
# **merge**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ merge(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="safeTransferFrom"></a>
# **safeTransferFrom**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ safeTransferFrom(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="setApprovalForAll"></a>
# **setApprovalForAll**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ setApprovalForAll(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="setClaimApproval"></a>
# **setClaimApproval**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ setClaimApproval(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="setClaimApprovalForAll"></a>
# **setClaimApprovalForAll**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ setClaimApprovalForAll(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="split"></a>
# **split**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ split(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="transferFrom"></a>
# **transferFrom**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ transferFrom(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="unlockPermanent"></a>
# **unlockPermanent**
> LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_ unlockPermanent(address, Authorization, LynexNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexNFTInputBody** | [**LynexNFTInputBody**](../Models/LynexNFTInputBody.md)|  | |

### Return type

[**LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_**](../Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

