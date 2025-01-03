# VeTheNFTApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**abstain**](VeTheNFTApi.md#abstain) | **POST** /thena/nft/{address}/abstain |  |
| [**approve**](VeTheNFTApi.md#approve) | **POST** /thena/nft/{address}/approve |  |
| [**attach**](VeTheNFTApi.md#attach) | **POST** /thena/nft/{address}/attach |  |
| [**checkpoint**](VeTheNFTApi.md#checkpoint) | **POST** /thena/nft/{address}/checkpoint |  |
| [**createLock**](VeTheNFTApi.md#createLock) | **POST** /thena/nft/{address}/createLock |  |
| [**createLockFor**](VeTheNFTApi.md#createLockFor) | **POST** /thena/nft/{address}/createLockFor |  |
| [**delegate**](VeTheNFTApi.md#delegate) | **POST** /thena/nft/{address}/delegate |  |
| [**delegateBySig**](VeTheNFTApi.md#delegateBySig) | **POST** /thena/nft/{address}/delegateBySig |  |
| [**depositFor**](VeTheNFTApi.md#depositFor) | **POST** /thena/nft/{address}/depositFor |  |
| [**detach**](VeTheNFTApi.md#detach) | **POST** /thena/nft/{address}/detach |  |
| [**getApproved**](VeTheNFTApi.md#getApproved) | **GET** /thena/nft/{tokenId}/getApproved |  |
| [**getBalanceOf**](VeTheNFTApi.md#getBalanceOf) | **GET** /thena/nft/{account}/balanceOf |  |
| [**getBalanceOfAtNFT**](VeTheNFTApi.md#getBalanceOfAtNFT) | **GET** /thena/nft/{tokenId}/balanceOfAtNFT |  |
| [**getBalanceOfNFT**](VeTheNFTApi.md#getBalanceOfNFT) | **GET** /thena/nft/{tokenId}/balanceOfNFT |  |
| [**getDelegates**](VeTheNFTApi.md#getDelegates) | **GET** /thena/nft/{delegator}/delegates |  |
| [**getLastUserSlope**](VeTheNFTApi.md#getLastUserSlope) | **GET** /thena/nft/{tokenId}/getLastUserSlope |  |
| [**getLocked**](VeTheNFTApi.md#getLocked) | **GET** /thena/nft/{tokenId}/locked |  |
| [**getLockedEnd**](VeTheNFTApi.md#getLockedEnd) | **GET** /thena/nft/{tokenId}/lockedEnd |  |
| [**getOwnerOf**](VeTheNFTApi.md#getOwnerOf) | **GET** /thena/nft/{tokenId}/ownerOf |  |
| [**getPastTotalSupply**](VeTheNFTApi.md#getPastTotalSupply) | **GET** /thena/nft/getPastTotalSupply |  |
| [**getPastVotes**](VeTheNFTApi.md#getPastVotes) | **GET** /thena/nft/{account}/getPastVotes |  |
| [**getTokenURI**](VeTheNFTApi.md#getTokenURI) | **GET** /thena/nft/{tokenId}/tokenURI |  |
| [**getTotalSupply**](VeTheNFTApi.md#getTotalSupply) | **GET** /thena/nft/totalSupply |  |
| [**getTotalSupplyAt**](VeTheNFTApi.md#getTotalSupplyAt) | **GET** /thena/nft/totalSupplyAt |  |
| [**getTotalSupplyAtT**](VeTheNFTApi.md#getTotalSupplyAtT) | **GET** /thena/nft/totalSupplyAtT |  |
| [**getUserPointHistory**](VeTheNFTApi.md#getUserPointHistory) | **GET** /thena/nft/{tokenId}/userPointHistory |  |
| [**getUserPointHistoryTS**](VeTheNFTApi.md#getUserPointHistoryTS) | **GET** /thena/nft/{tokenId}/userPointHistoryTS |  |
| [**getVotes**](VeTheNFTApi.md#getVotes) | **GET** /thena/nft/{account}/getVotes |  |
| [**increaseLockAmount**](VeTheNFTApi.md#increaseLockAmount) | **POST** /thena/nft/{address}/increaseLockAmount |  |
| [**increaseUnlockTime**](VeTheNFTApi.md#increaseUnlockTime) | **POST** /thena/nft/{address}/increaseUnlockTime |  |
| [**isApprovedForAll**](VeTheNFTApi.md#isApprovedForAll) | **GET** /thena/nft/{owner}/isApprovedForAll |  |
| [**merge**](VeTheNFTApi.md#merge) | **POST** /thena/nft/{address}/merge |  |
| [**safeTransferFrom**](VeTheNFTApi.md#safeTransferFrom) | **POST** /thena/nft/{address}/safeTransferFrom |  |
| [**setApprovalForAll**](VeTheNFTApi.md#setApprovalForAll) | **POST** /thena/nft/{address}/setApprovalForAll |  |
| [**split**](VeTheNFTApi.md#split) | **POST** /thena/nft/{address}/split |  |
| [**transferFrom**](VeTheNFTApi.md#transferFrom) | **POST** /thena/nft/{address}/transferFrom |  |
| [**voting**](VeTheNFTApi.md#voting) | **POST** /thena/nft/{address}/voting |  |
| [**withdraw**](VeTheNFTApi.md#withdraw) | **POST** /thena/nft/{address}/withdraw |  |


<a name="abstain"></a>
# **abstain**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ abstain(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="approve"></a>
# **approve**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ approve(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="attach"></a>
# **attach**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ attach(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="checkpoint"></a>
# **checkpoint**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ checkpoint(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createLock"></a>
# **createLock**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ createLock(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createLockFor"></a>
# **createLockFor**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ createLockFor(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="delegate"></a>
# **delegate**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ delegate(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="delegateBySig"></a>
# **delegateBySig**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ delegateBySig(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="depositFor"></a>
# **depositFor**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ depositFor(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="detach"></a>
# **detach**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ detach(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getApproved"></a>
# **getApproved**
> VeTheNFTAPIResponse_string_ getApproved(tokenId, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBalanceOf"></a>
# **getBalanceOf**
> VeTheNFTAPIResponse_string_ getBalanceOf(account, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBalanceOfAtNFT"></a>
# **getBalanceOfAtNFT**
> VeTheNFTAPIResponse_string_ getBalanceOfAtNFT(tokenId, Authorization, chainId, address, block)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **block** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBalanceOfNFT"></a>
# **getBalanceOfNFT**
> VeTheNFTAPIResponse_string_ getBalanceOfNFT(tokenId, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getDelegates"></a>
# **getDelegates**
> VeTheNFTAPIResponse_string_ getDelegates(delegator, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **delegator** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getLastUserSlope"></a>
# **getLastUserSlope**
> VeTheNFTAPIResponse_string_ getLastUserSlope(tokenId, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getLocked"></a>
# **getLocked**
> VeTheNFTAPIResponse_LockedData_ getLocked(tokenId, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_LockedData_**](../Models/VeTheNFTAPIResponse_LockedData_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getLockedEnd"></a>
# **getLockedEnd**
> VeTheNFTAPIResponse_string_ getLockedEnd(tokenId, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getOwnerOf"></a>
# **getOwnerOf**
> VeTheNFTAPIResponse_string_ getOwnerOf(tokenId, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPastTotalSupply"></a>
# **getPastTotalSupply**
> VeTheNFTAPIResponse_string_ getPastTotalSupply(Authorization, chainId, address, timestamp)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **timestamp** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPastVotes"></a>
# **getPastVotes**
> VeTheNFTAPIResponse_string_ getPastVotes(account, Authorization, chainId, address, timestamp)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **timestamp** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTokenURI"></a>
# **getTokenURI**
> VeTheNFTAPIResponse_string_ getTokenURI(tokenId, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalSupply"></a>
# **getTotalSupply**
> VeTheNFTAPIResponse_string_ getTotalSupply(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalSupplyAt"></a>
# **getTotalSupplyAt**
> VeTheNFTAPIResponse_string_ getTotalSupplyAt(Authorization, chainId, address, block)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **block** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTotalSupplyAtT"></a>
# **getTotalSupplyAtT**
> VeTheNFTAPIResponse_string_ getTotalSupplyAtT(Authorization, chainId, address, t)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **t** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getUserPointHistory"></a>
# **getUserPointHistory**
> VeTheNFTAPIResponse_UserPointHistoryData_ getUserPointHistory(tokenId, Authorization, chainId, address, loc)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **loc** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_UserPointHistoryData_**](../Models/VeTheNFTAPIResponse_UserPointHistoryData_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getUserPointHistoryTS"></a>
# **getUserPointHistoryTS**
> VeTheNFTAPIResponse_string_ getUserPointHistoryTS(tokenId, Authorization, chainId, address, idx)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **idx** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getVotes"></a>
# **getVotes**
> VeTheNFTAPIResponse_string_ getVotes(account, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_string_**](../Models/VeTheNFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="increaseLockAmount"></a>
# **increaseLockAmount**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ increaseLockAmount(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="increaseUnlockTime"></a>
# **increaseUnlockTime**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ increaseUnlockTime(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="isApprovedForAll"></a>
# **isApprovedForAll**
> VeTheNFTAPIResponse_boolean_ isApprovedForAll(owner, Authorization, chainId, address, operator)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **operator** | **String**|  | [default to null] |

### Return type

[**VeTheNFTAPIResponse_boolean_**](../Models/VeTheNFTAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="merge"></a>
# **merge**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ merge(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="safeTransferFrom"></a>
# **safeTransferFrom**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ safeTransferFrom(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="setApprovalForAll"></a>
# **setApprovalForAll**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ setApprovalForAll(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="split"></a>
# **split**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ split(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="transferFrom"></a>
# **transferFrom**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ transferFrom(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="voting"></a>
# **voting**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ voting(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="withdraw"></a>
# **withdraw**
> VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_ withdraw(address, Authorization, VeNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **VeNFTInputBody** | [**VeNFTInputBody**](../Models/VeNFTInputBody.md)|  | |

### Return type

[**VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_**](../Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

