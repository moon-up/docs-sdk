# ERC1155Api

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**erc1155Erc1155BalanceOf**](ERC1155Api.md#erc1155Erc1155BalanceOf) | **POST** /erc1155/{name}/balance-of |  |
| [**erc1155Erc1155BalanceOfBatch**](ERC1155Api.md#erc1155Erc1155BalanceOfBatch) | **POST** /erc1155/{name}/balance-of-batch |  |
| [**erc1155Erc1155IsApprovedForAll**](ERC1155Api.md#erc1155Erc1155IsApprovedForAll) | **POST** /erc1155/{name}/is-approved-for-all |  |
| [**erc1155Erc1155SafeBatchTransferFrom**](ERC1155Api.md#erc1155Erc1155SafeBatchTransferFrom) | **POST** /erc1155/{name}/safe-batch-transfer-from |  |
| [**erc1155Erc1155SafeTransferFrom**](ERC1155Api.md#erc1155Erc1155SafeTransferFrom) | **POST** /erc1155/{name}/safe-transfer-from |  |
| [**erc1155Erc1155SetApprovalForAll**](ERC1155Api.md#erc1155Erc1155SetApprovalForAll) | **POST** /erc1155/{name}/set-approval-for-all |  |


<a name="erc1155Erc1155BalanceOf"></a>
# **erc1155Erc1155BalanceOf**
> TransactionAPIResponse erc1155Erc1155BalanceOf(name, Authorization, Erc1155Request)



    Retrieves the balance of an ERC1155 token for a specific account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| - The name identifier for the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)| - The request body containing ERC1155 parameters | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc1155Erc1155BalanceOfBatch"></a>
# **erc1155Erc1155BalanceOfBatch**
> TransactionAPIResponse erc1155Erc1155BalanceOfBatch(name, Authorization, Erc1155Request)



    Retrieves balances for multiple token IDs and accounts in a batch operation.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| - The name identifier for the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)| - The request body containing arrays of accounts and token IDs | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc1155Erc1155IsApprovedForAll"></a>
# **erc1155Erc1155IsApprovedForAll**
> TransactionAPIResponse erc1155Erc1155IsApprovedForAll(name, Authorization, Erc1155Request)



    Queries if an address is approved to manage all tokens of another address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| - The name identifier for the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)| - The request body containing owner and operator addresses | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc1155Erc1155SafeBatchTransferFrom"></a>
# **erc1155Erc1155SafeBatchTransferFrom**
> TransactionAPIResponse erc1155Erc1155SafeBatchTransferFrom(name, Authorization, Erc1155Request)



    Safely transfers multiple tokens between addresses in a batch operation.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| - The name identifier for the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)| - The request body containing batch transfer details | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc1155Erc1155SafeTransferFrom"></a>
# **erc1155Erc1155SafeTransferFrom**
> TransactionAPIResponse erc1155Erc1155SafeTransferFrom(name, Authorization, Erc1155Request)



    Safely transfers a single token between addresses.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| - The name identifier for the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)| - The request body containing transfer details | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc1155Erc1155SetApprovalForAll"></a>
# **erc1155Erc1155SetApprovalForAll**
> TransactionAPIResponse erc1155Erc1155SetApprovalForAll(name, Authorization, Erc1155Request)



    Enables or disables approval for a third party (\&quot;operator\&quot;) to manage all tokens.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| - The name identifier for the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **Erc1155Request** | [**Erc1155Request**](../Models/Erc1155Request.md)| - The request body containing operator address and approval status | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

