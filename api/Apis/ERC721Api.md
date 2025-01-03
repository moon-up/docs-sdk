# ERC721Api

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**erc721ApproveERC721**](ERC721Api.md#erc721ApproveERC721) | **POST** /erc721/{address}/approve |  |
| [**erc721GetERC721Approved**](ERC721Api.md#erc721GetERC721Approved) | **GET** /erc721/{tokenId}/getApproved |  |
| [**erc721GetERC721BalanceOf**](ERC721Api.md#erc721GetERC721BalanceOf) | **GET** /erc721/{account}/balanceOf |  |
| [**erc721GetERC721IsApprovedForAll**](ERC721Api.md#erc721GetERC721IsApprovedForAll) | **GET** /erc721/{owner}/{operator}/isApprovedForAll |  |
| [**erc721GetERC721Name**](ERC721Api.md#erc721GetERC721Name) | **GET** /erc721/name |  |
| [**erc721GetERC721OwnerOf**](ERC721Api.md#erc721GetERC721OwnerOf) | **GET** /erc721/{tokenId}/ownerOf |  |
| [**erc721GetERC721Symbol**](ERC721Api.md#erc721GetERC721Symbol) | **GET** /erc721/symbol |  |
| [**erc721GetERC721TokenURI**](ERC721Api.md#erc721GetERC721TokenURI) | **GET** /erc721/{tokenId}/tokenURI |  |
| [**erc721SafeTransferFromERC721**](ERC721Api.md#erc721SafeTransferFromERC721) | **POST** /erc721/{address}/safeTransferFrom |  |
| [**erc721SafeTransferFromWithDataERC721**](ERC721Api.md#erc721SafeTransferFromWithDataERC721) | **POST** /erc721/{address}/safeTransferFromWithData |  |
| [**erc721SetApprovalForAllERC721**](ERC721Api.md#erc721SetApprovalForAllERC721) | **POST** /erc721/{address}/setApprovalForAll |  |
| [**erc721TransferFromERC721**](ERC721Api.md#erc721TransferFromERC721) | **POST** /erc721/{address}/transferFrom |  |


<a name="erc721ApproveERC721"></a>
# **erc721ApproveERC721**
> ERC721APIResponse erc721ApproveERC721(address, Authorization, InputBody)



    Approves an ERC721 token for a given address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address to approve the token for. | [default to null] |
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The request body containing contract address and chain ID. | |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc721GetERC721Approved"></a>
# **erc721GetERC721Approved**
> ERC721APIResponse erc721GetERC721Approved(tokenId, Authorization, chainId, address)



    Retrieves the approved address for a specific ERC721 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**| - The ID of the token to check approval for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the ERC721 contract. | [default to null] |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc721GetERC721BalanceOf"></a>
# **erc721GetERC721BalanceOf**
> ERC721APIResponse erc721GetERC721BalanceOf(account, Authorization, chainId, address)



    Retrieves the balance of ERC721 tokens for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account address to query the balance for. | [default to null] |
| **Authorization** | **String**| - The authorization token for accessing the ERC721 instance. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The contract address of the ERC721 token. | [default to null] |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc721GetERC721IsApprovedForAll"></a>
# **erc721GetERC721IsApprovedForAll**
> ERC721APIResponse erc721GetERC721IsApprovedForAll(owner, operator, Authorization, chainId, address)



    Checks if an operator is approved to manage all assets of a given owner.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **owner** | **String**| - The address of the owner of the assets. | [default to null] |
| **operator** | **String**| - The address of the operator to check for approval. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the ERC721 contract. | [default to null] |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc721GetERC721Name"></a>
# **erc721GetERC721Name**
> ERC721APIResponse erc721GetERC721Name(Authorization, chainId, address)



    Retrieves the name of an ERC721 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the ERC721 contract. | [default to null] |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc721GetERC721OwnerOf"></a>
# **erc721GetERC721OwnerOf**
> ERC721APIResponse erc721GetERC721OwnerOf(tokenId, Authorization, chainId, address)



    Retrieves the owner of a specified ERC721 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**| - The ID of the token to query. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the ERC721 contract. | [default to null] |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc721GetERC721Symbol"></a>
# **erc721GetERC721Symbol**
> ERC721APIResponse erc721GetERC721Symbol(Authorization, chainId, address)



    Retrieves the symbol of an ERC721 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the ERC721 contract. | [default to null] |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc721GetERC721TokenURI"></a>
# **erc721GetERC721TokenURI**
> ERC721APIResponse erc721GetERC721TokenURI(tokenId, Authorization, chainId, address)



    Retrieves the token URI for a given ERC721 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**| - The ID of the token to retrieve the URI for. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the ERC721 contract. | [default to null] |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc721SafeTransferFromERC721"></a>
# **erc721SafeTransferFromERC721**
> ERC721APIResponse erc721SafeTransferFromERC721(address, Authorization, InputBody)



    Safely transfers an ERC721 token from one address to another.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address from which the token is being transferred. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The request body containing the contract address and chain ID. | |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc721SafeTransferFromWithDataERC721"></a>
# **erc721SafeTransferFromWithDataERC721**
> ERC721APIResponse erc721SafeTransferFromWithDataERC721(address, Authorization, InputBody)



    Safely transfers an ERC721 token from one address to another with additional data.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address to transfer the token to. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address and chain ID. | |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc721SetApprovalForAllERC721"></a>
# **erc721SetApprovalForAllERC721**
> ERC721APIResponse erc721SetApprovalForAllERC721(address, Authorization, InputBody)



    Sets approval for all ERC721 tokens for a given address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address to set approval for. | [default to null] |
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The request body containing contract address and chain ID. | |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc721TransferFromERC721"></a>
# **erc721TransferFromERC721**
> ERC721APIResponse erc721TransferFromERC721(address, Authorization, InputBody)



    Transfers an ERC721 token from one address to another.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address from which the token is being transferred. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address and chain ID. | |

### Return type

[**ERC721APIResponse**](../Models/ERC721APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

