# Erc721Api

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**approve**](Erc721Api.md#approve) | **POST** /erc721/{name}/approve |  |
| [**balanceOf**](Erc721Api.md#balanceOf) | **POST** /erc721/{name}/balance-of |  |
| [**getApproved**](Erc721Api.md#getApproved) | **POST** /erc721/{name}/get-approved |  |
| [**isApprovedForAll**](Erc721Api.md#isApprovedForAll) | **POST** /erc721/{name}/is-approved-for-all |  |
| [**name**](Erc721Api.md#name) | **POST** /erc721/{name}/name |  |
| [**ownerOf**](Erc721Api.md#ownerOf) | **POST** /erc721/{name}/owner-of |  |
| [**safeTransferFrom**](Erc721Api.md#safeTransferFrom) | **POST** /erc721/{name}/safe-transfer-from |  |
| [**setApprovalForAll**](Erc721Api.md#setApprovalForAll) | **POST** /erc721/{name}/set-approval-for-all |  |
| [**symbol**](Erc721Api.md#symbol) | **POST** /erc721/{name}/symbol |  |
| [**tokenUri**](Erc721Api.md#tokenUri) | **POST** /erc721/{name}/token-uri |  |
| [**transfer**](Erc721Api.md#transfer) | **POST** /erc721/{name}/transfer |  |
| [**transferFrom**](Erc721Api.md#transferFrom) | **POST** /erc721/{name}/transfer-from |  |


<a name="approve"></a>
# **approve**
> TransactionAPIResponse approve(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="balanceOf"></a>
# **balanceOf**
> TransactionAPIResponse balanceOf(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getApproved"></a>
# **getApproved**
> TransactionAPIResponse getApproved(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="isApprovedForAll"></a>
# **isApprovedForAll**
> TransactionAPIResponse isApprovedForAll(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="name"></a>
# **name**
> TransactionAPIResponse name(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="ownerOf"></a>
# **ownerOf**
> TransactionAPIResponse ownerOf(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="safeTransferFrom"></a>
# **safeTransferFrom**
> TransactionAPIResponse safeTransferFrom(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="setApprovalForAll"></a>
# **setApprovalForAll**
> TransactionAPIResponse setApprovalForAll(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="symbol"></a>
# **symbol**
> TransactionAPIResponse symbol(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="tokenUri"></a>
# **tokenUri**
> TransactionAPIResponse tokenUri(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="transfer"></a>
# **transfer**
> TransactionAPIResponse transfer(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="transferFrom"></a>
# **transferFrom**
> TransactionAPIResponse transferFrom(Authorization, name, Erc721Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **Erc721Request** | [**Erc721Request**](../Models/Erc721Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

