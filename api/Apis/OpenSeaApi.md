# OpenSeaApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCollectionOffer**](OpenSeaApi.md#createCollectionOffer) | **POST** /opensea/{account}/createCollectionOffer |  |
| [**createOffer**](OpenSeaApi.md#createOffer) | **POST** /opensea/{account}/createOffer |  |
| [**getCollection**](OpenSeaApi.md#getCollection) | **GET** /opensea/{account}/collection/{slug} |  |
| [**getNFT**](OpenSeaApi.md#getNFT) | **GET** /opensea/{account}/nft/{address}/{tokenId} |  |
| [**unwrapWeth**](OpenSeaApi.md#unwrapWeth) | **POST** /opensea/{account}/unwrapWeth |  |
| [**wrapEth**](OpenSeaApi.md#wrapEth) | **POST** /opensea/{account}/wrapEth |  |


<a name="createCollectionOffer"></a>
# **createCollectionOffer**
> OpenSeaAPIResponse createCollectionOffer(account, Authorization, OpenSeaCollectionInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **OpenSeaCollectionInputBody** | [**OpenSeaCollectionInputBody**](../Models/OpenSeaCollectionInputBody.md)|  | |

### Return type

[**OpenSeaAPIResponse**](../Models/OpenSeaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createOffer"></a>
# **createOffer**
> OpenSeaAPIResponse createOffer(account, Authorization, OpenSeaNFTInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **OpenSeaNFTInputBody** | [**OpenSeaNFTInputBody**](../Models/OpenSeaNFTInputBody.md)|  | |

### Return type

[**OpenSeaAPIResponse**](../Models/OpenSeaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getCollection"></a>
# **getCollection**
> OpenSeaAPIResponse getCollection(account, slug, Authorization, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **slug** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [optional] [default to 1] |

### Return type

[**OpenSeaAPIResponse**](../Models/OpenSeaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getNFT"></a>
# **getNFT**
> OpenSeaAPIResponse getNFT(account, address, tokenId, Authorization, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [optional] [default to 1] |

### Return type

[**OpenSeaAPIResponse**](../Models/OpenSeaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="unwrapWeth"></a>
# **unwrapWeth**
> OpenSeaAPIResponse unwrapWeth(account, Authorization, WrapEth\_request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **WrapEth\_request** | [**WrapEth_request**](../Models/WrapEth_request.md)|  | |

### Return type

[**OpenSeaAPIResponse**](../Models/OpenSeaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="wrapEth"></a>
# **wrapEth**
> OpenSeaAPIResponse wrapEth(account, Authorization, WrapEth\_request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **WrapEth\_request** | [**WrapEth_request**](../Models/WrapEth_request.md)|  | |

### Return type

[**OpenSeaAPIResponse**](../Models/OpenSeaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

