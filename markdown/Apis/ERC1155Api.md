# ERC1155Api

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**balanceOf**](ERC1155Api.md#balanceOf) | **POST** /erc1155/{name}/balance-of |  |
| [**balanceOfBatch**](ERC1155Api.md#balanceOfBatch) | **POST** /erc1155/{name}/balance-of-batch |  |
| [**isApprovedForAll**](ERC1155Api.md#isApprovedForAll) | **POST** /erc1155/{name}/is-approved-for-all |  |
| [**safeBatchTransferFrom**](ERC1155Api.md#safeBatchTransferFrom) | **POST** /erc1155/{name}/safe-batch-transfer-from |  |
| [**safeTransferFrom**](ERC1155Api.md#safeTransferFrom) | **POST** /erc1155/{name}/safe-transfer-from |  |
| [**setApprovalForAll**](ERC1155Api.md#setApprovalForAll) | **POST** /erc1155/{name}/set-approval-for-all |  |


<a name="balanceOf"></a>
# **balanceOf**
> TransactionAPIResponse balanceOf(name, Authorization, Erc1155Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="balanceOfBatch"></a>
# **balanceOfBatch**
> TransactionAPIResponse balanceOfBatch(name, Authorization, Erc1155Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="isApprovedForAll"></a>
# **isApprovedForAll**
> TransactionAPIResponse isApprovedForAll(name, Authorization, Erc1155Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="safeBatchTransferFrom"></a>
# **safeBatchTransferFrom**
> TransactionAPIResponse safeBatchTransferFrom(name, Authorization, Erc1155Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="safeTransferFrom"></a>
# **safeTransferFrom**
> TransactionAPIResponse safeTransferFrom(name, Authorization, Erc1155Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="setApprovalForAll"></a>
# **setApprovalForAll**
> TransactionAPIResponse setApprovalForAll(name, Authorization, Erc1155Request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

