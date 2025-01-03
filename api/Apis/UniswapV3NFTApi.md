# UniswapV3NFTApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**approve**](UniswapV3NFTApi.md#approve) | **POST** /uniswap/v3/nft/{address}/approve |  |
| [**balanceOf**](UniswapV3NFTApi.md#balanceOf) | **GET** /uniswap/v3/nft/balanceOf |  |
| [**baseURI**](UniswapV3NFTApi.md#baseURI) | **GET** /uniswap/v3/nft/baseURI |  |
| [**burn**](UniswapV3NFTApi.md#burn) | **POST** /uniswap/v3/nft/{address}/burn |  |
| [**collect**](UniswapV3NFTApi.md#collect) | **POST** /uniswap/v3/nft/{address}/collect |  |
| [**createAndInitializePoolIfNecessary**](UniswapV3NFTApi.md#createAndInitializePoolIfNecessary) | **POST** /uniswap/v3/nft/{address}/createAndInitializePoolIfNecessary |  |
| [**dOMAINSEPARATOR**](UniswapV3NFTApi.md#dOMAINSEPARATOR) | **GET** /uniswap/v3/nft/DOMAIN_SEPARATOR |  |
| [**decreaseLiquidity**](UniswapV3NFTApi.md#decreaseLiquidity) | **POST** /uniswap/v3/nft/{address}/decreaseLiquidity |  |
| [**factory**](UniswapV3NFTApi.md#factory) | **GET** /uniswap/v3/nft/factory |  |
| [**getApproved**](UniswapV3NFTApi.md#getApproved) | **GET** /uniswap/v3/nft/getApproved |  |
| [**increaseLiquidity**](UniswapV3NFTApi.md#increaseLiquidity) | **POST** /uniswap/v3/nft/{address}/increaseLiquidity |  |
| [**isApprovedForAll**](UniswapV3NFTApi.md#isApprovedForAll) | **GET** /uniswap/v3/nft/isApprovedForAll |  |
| [**mint**](UniswapV3NFTApi.md#mint) | **POST** /uniswap/v3/nft/{address}/mint |  |
| [**multicall**](UniswapV3NFTApi.md#multicall) | **POST** /uniswap/v3/nft/{address}/multicall |  |
| [**name**](UniswapV3NFTApi.md#name) | **GET** /uniswap/v3/nft/name |  |
| [**ownerOf**](UniswapV3NFTApi.md#ownerOf) | **GET** /uniswap/v3/nft/ownerOf |  |
| [**pERMITTYPEHASH**](UniswapV3NFTApi.md#pERMITTYPEHASH) | **GET** /uniswap/v3/nft/PERMIT_TYPEHASH |  |
| [**permit**](UniswapV3NFTApi.md#permit) | **POST** /uniswap/v3/nft/{address}/permit |  |
| [**positions**](UniswapV3NFTApi.md#positions) | **GET** /uniswap/v3/nft/positions |  |
| [**refundETH**](UniswapV3NFTApi.md#refundETH) | **POST** /uniswap/v3/nft/{address}/refundETH |  |
| [**setApprovalForAll**](UniswapV3NFTApi.md#setApprovalForAll) | **POST** /uniswap/v3/nft/{address}/setApprovalForAll |  |
| [**supportsInterface**](UniswapV3NFTApi.md#supportsInterface) | **GET** /uniswap/v3/nft/supportsInterface |  |
| [**sweepToken**](UniswapV3NFTApi.md#sweepToken) | **POST** /uniswap/v3/nft/{address}/sweepToken |  |
| [**symbol**](UniswapV3NFTApi.md#symbol) | **GET** /uniswap/v3/nft/symbol |  |
| [**tokenByIndex**](UniswapV3NFTApi.md#tokenByIndex) | **GET** /uniswap/v3/nft/tokenByIndex |  |
| [**tokenOfOwnerByIndex**](UniswapV3NFTApi.md#tokenOfOwnerByIndex) | **GET** /uniswap/v3/nft/tokenOfOwnerByIndex |  |
| [**tokenURI**](UniswapV3NFTApi.md#tokenURI) | **GET** /uniswap/v3/nft/tokenURI |  |
| [**totalSupply**](UniswapV3NFTApi.md#totalSupply) | **GET** /uniswap/v3/nft/totalSupply |  |
| [**transferFrom**](UniswapV3NFTApi.md#transferFrom) | **POST** /uniswap/v3/nft/{address}/transferFrom |  |
| [**unwrapWETH9**](UniswapV3NFTApi.md#unwrapWETH9) | **POST** /uniswap/v3/nft/{address}/unwrapWETH9 |  |
| [**wETH9**](UniswapV3NFTApi.md#wETH9) | **GET** /uniswap/v3/nft/WETH9 |  |


<a name="approve"></a>
# **approve**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ approve(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="balanceOf"></a>
# **balanceOf**
> UniswapV3NFTAPIResponse_string_ balanceOf(Authorization, chainId, address, owner)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **owner** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="baseURI"></a>
# **baseURI**
> UniswapV3NFTAPIResponse_string_ baseURI(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="burn"></a>
# **burn**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ burn(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="collect"></a>
# **collect**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ collect(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createAndInitializePoolIfNecessary"></a>
# **createAndInitializePoolIfNecessary**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ createAndInitializePoolIfNecessary(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="dOMAINSEPARATOR"></a>
# **dOMAINSEPARATOR**
> UniswapV3NFTAPIResponse_string_ dOMAINSEPARATOR(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="decreaseLiquidity"></a>
# **decreaseLiquidity**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ decreaseLiquidity(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="factory"></a>
# **factory**
> UniswapV3NFTAPIResponse_string_ factory(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getApproved"></a>
# **getApproved**
> UniswapV3NFTAPIResponse_string_ getApproved(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **Double**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="increaseLiquidity"></a>
# **increaseLiquidity**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ increaseLiquidity(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="isApprovedForAll"></a>
# **isApprovedForAll**
> UniswapV3NFTAPIResponse_boolean_ isApprovedForAll(Authorization, chainId, address, owner, operator)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **owner** | **String**|  | [default to null] |
| **operator** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_boolean_**](../Models/UniswapV3NFTAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="mint"></a>
# **mint**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ mint(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="multicall"></a>
# **multicall**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ multicall(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="name"></a>
# **name**
> UniswapV3NFTAPIResponse_string_ name(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="ownerOf"></a>
# **ownerOf**
> UniswapV3NFTAPIResponse_string_ ownerOf(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **Double**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="pERMITTYPEHASH"></a>
# **pERMITTYPEHASH**
> UniswapV3NFTAPIResponse_string_ pERMITTYPEHASH(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="permit"></a>
# **permit**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ permit(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="positions"></a>
# **positions**
> UniswapV3NFTAPIResponse_any_ positions(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **Double**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_any_**](../Models/UniswapV3NFTAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="refundETH"></a>
# **refundETH**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ refundETH(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="setApprovalForAll"></a>
# **setApprovalForAll**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ setApprovalForAll(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="supportsInterface"></a>
# **supportsInterface**
> UniswapV3NFTAPIResponse_boolean_ supportsInterface(Authorization, chainId, address, interfaceId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **interfaceId** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_boolean_**](../Models/UniswapV3NFTAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="sweepToken"></a>
# **sweepToken**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ sweepToken(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="symbol"></a>
# **symbol**
> UniswapV3NFTAPIResponse_string_ symbol(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="tokenByIndex"></a>
# **tokenByIndex**
> UniswapV3NFTAPIResponse_string_ tokenByIndex(Authorization, chainId, address, index)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **index** | **Double**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="tokenOfOwnerByIndex"></a>
# **tokenOfOwnerByIndex**
> UniswapV3NFTAPIResponse_string_ tokenOfOwnerByIndex(Authorization, chainId, address, owner, index)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **owner** | **String**|  | [default to null] |
| **index** | **Double**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="tokenURI"></a>
# **tokenURI**
> UniswapV3NFTAPIResponse_string_ tokenURI(Authorization, chainId, address, tokenId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **Double**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="totalSupply"></a>
# **totalSupply**
> UniswapV3NFTAPIResponse_string_ totalSupply(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="transferFrom"></a>
# **transferFrom**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ transferFrom(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="unwrapWETH9"></a>
# **unwrapWETH9**
> UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_ unwrapWETH9(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="wETH9"></a>
# **wETH9**
> UniswapV3NFTAPIResponse_string_ wETH9(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3NFTAPIResponse_string_**](../Models/UniswapV3NFTAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

