# ERC20Api

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**erc20ApproveERC20TokenSpending**](ERC20Api.md#erc20ApproveERC20TokenSpending) | **POST** /erc20/{address}/approve |  |
| [**erc20GetERC20TokenAllowance**](ERC20Api.md#erc20GetERC20TokenAllowance) | **GET** /erc20/{account}/allowance |  |
| [**erc20GetERC20TokenBalance**](ERC20Api.md#erc20GetERC20TokenBalance) | **GET** /erc20/{account}/balanceOf |  |
| [**erc20GetERC20TokenDecimals**](ERC20Api.md#erc20GetERC20TokenDecimals) | **GET** /erc20/{account}/decimals |  |
| [**erc20GetERC20TokenName**](ERC20Api.md#erc20GetERC20TokenName) | **GET** /erc20/{account}/name |  |
| [**erc20GetERC20TokenSymbol**](ERC20Api.md#erc20GetERC20TokenSymbol) | **GET** /erc20/{account}/symbol |  |
| [**erc20GetERC20TokenTotalSupply**](ERC20Api.md#erc20GetERC20TokenTotalSupply) | **GET** /erc20/{account}/totalSupply |  |
| [**erc20TransferERC20Token**](ERC20Api.md#erc20TransferERC20Token) | **POST** /erc20/{address}/transfer |  |
| [**erc20TransferFromERC20Token**](ERC20Api.md#erc20TransferFromERC20Token) | **POST** /erc20/{address}/transferFrom |  |


<a name="erc20ApproveERC20TokenSpending"></a>
# **erc20ApproveERC20TokenSpending**
> ERC20APIResponse_ERC20ExecuteFunctionResult_ erc20ApproveERC20TokenSpending(address, Authorization, ERC20InputBody)



    Approves a specified address to spend tokens on behalf of the user.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address to be approved. | [default to null] |
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **ERC20InputBody** | [**ERC20InputBody**](../Models/ERC20InputBody.md)| - The body of the request containing contract address and chain ID. | |

### Return type

[**ERC20APIResponse_ERC20ExecuteFunctionResult_**](../Models/ERC20APIResponse_ERC20ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc20GetERC20TokenAllowance"></a>
# **erc20GetERC20TokenAllowance**
> ERC20APIResponse_string_ erc20GetERC20TokenAllowance(account, Authorization, chainId, address, owner, spender)



    Retrieves the allowance of a specified ERC20 token for a given owner and spender.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account address making the request. | [default to null] |
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The contract address of the ERC20 token. | [default to null] |
| **owner** | **String**| - The address of the token owner. | [default to null] |
| **spender** | **String**| - The address of the spender. | [default to null] |

### Return type

[**ERC20APIResponse_string_**](../Models/ERC20APIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc20GetERC20TokenBalance"></a>
# **erc20GetERC20TokenBalance**
> ERC20APIResponse_string_ erc20GetERC20TokenBalance(account, Authorization, chainId, address)



    Retrieves the balance of a specified ERC20 token for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The address of the account to retrieve the balance for. | [default to null] |
| **Authorization** | **String**| - The authorization token for accessing the ERC20 instance. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the ERC20 token contract. | [default to null] |

### Return type

[**ERC20APIResponse_string_**](../Models/ERC20APIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc20GetERC20TokenDecimals"></a>
# **erc20GetERC20TokenDecimals**
> ERC20APIResponse_number_ erc20GetERC20TokenDecimals(account, Authorization, chainId, address)



    Retrieves the number of decimals for the provided ERC20 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account address for the ERC20 token. | [default to null] |
| **Authorization** | **String**| - The authorization token for accessing the ERC20 token. | [default to null] |
| **chainId** | **String**| - The chain ID for the ERC20 token. | [default to null] |
| **address** | **String**| - The contract address for the ERC20 token. | [default to null] |

### Return type

[**ERC20APIResponse_number_**](../Models/ERC20APIResponse_number_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc20GetERC20TokenName"></a>
# **erc20GetERC20TokenName**
> ERC20APIResponse_string_ erc20GetERC20TokenName(account, Authorization, chainId, address)



    Retrieves the name of an ERC20 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account address. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The blockchain chain ID. | [default to null] |
| **address** | **String**| - The ERC20 token contract address. | [default to null] |

### Return type

[**ERC20APIResponse_string_**](../Models/ERC20APIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc20GetERC20TokenSymbol"></a>
# **erc20GetERC20TokenSymbol**
> ERC20APIResponse_string_ erc20GetERC20TokenSymbol(account, Authorization, chainId, address)



    Retrieves the symbol of an ERC20 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account address. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the ERC20 token contract. | [default to null] |

### Return type

[**ERC20APIResponse_string_**](../Models/ERC20APIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc20GetERC20TokenTotalSupply"></a>
# **erc20GetERC20TokenTotalSupply**
> ERC20APIResponse_string_ erc20GetERC20TokenTotalSupply(account, Authorization, chainId, address)



    Retrieves the total supply of an ERC20 token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account address. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The blockchain chain ID. | [default to null] |
| **address** | **String**| - The ERC20 token contract address. | [default to null] |

### Return type

[**ERC20APIResponse_string_**](../Models/ERC20APIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc20TransferERC20Token"></a>
# **erc20TransferERC20Token**
> ERC20APIResponse_ERC20ExecuteFunctionResult_ erc20TransferERC20Token(address, Authorization, ERC20InputBody)



    Transfers ERC20 tokens to a specified address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address to transfer tokens to. | [default to null] |
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **ERC20InputBody** | [**ERC20InputBody**](../Models/ERC20InputBody.md)| - The body of the request containing transfer details. | |

### Return type

[**ERC20APIResponse_ERC20ExecuteFunctionResult_**](../Models/ERC20APIResponse_ERC20ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc20TransferFromERC20Token"></a>
# **erc20TransferFromERC20Token**
> ERC20APIResponse_ERC20ExecuteFunctionResult_ erc20TransferFromERC20Token(address, Authorization, ERC20InputBody)



    Transfers tokens from one address to another.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address from which the tokens will be transferred. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **ERC20InputBody** | [**ERC20InputBody**](../Models/ERC20InputBody.md)| - The body containing the contract address and chain ID. | |

### Return type

[**ERC20APIResponse_ERC20ExecuteFunctionResult_**](../Models/ERC20APIResponse_ERC20ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

