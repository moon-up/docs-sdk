# ERC4626Api

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**erc4626ApproveERC4626**](ERC4626Api.md#erc4626ApproveERC4626) | **POST** /erc4626/{address}/approve |  |
| [**erc4626DepositToERC4626**](ERC4626Api.md#erc4626DepositToERC4626) | **POST** /erc4626/{address}/deposit |  |
| [**erc4626GetERC4626Allowance**](ERC4626Api.md#erc4626GetERC4626Allowance) | **GET** /erc4626/{account}/allowance |  |
| [**erc4626GetERC4626Asset**](ERC4626Api.md#erc4626GetERC4626Asset) | **GET** /erc4626/{account}/asset |  |
| [**erc4626GetERC4626BalanceOf**](ERC4626Api.md#erc4626GetERC4626BalanceOf) | **GET** /erc4626/{account}/balanceOf |  |
| [**erc4626GetERC4626ConvertToAssets**](ERC4626Api.md#erc4626GetERC4626ConvertToAssets) | **GET** /erc4626/{account}/convertToAssets |  |
| [**erc4626GetERC4626ConvertToShares**](ERC4626Api.md#erc4626GetERC4626ConvertToShares) | **GET** /erc4626/{account}/convertToShares |  |
| [**erc4626GetERC4626MaxDeposit**](ERC4626Api.md#erc4626GetERC4626MaxDeposit) | **GET** /erc4626/{account}/maxDeposit |  |
| [**erc4626GetERC4626MaxMint**](ERC4626Api.md#erc4626GetERC4626MaxMint) | **GET** /erc4626/{account}/maxMint |  |
| [**erc4626GetERC4626MaxRedeem**](ERC4626Api.md#erc4626GetERC4626MaxRedeem) | **GET** /erc4626/{account}/maxRedeem |  |
| [**erc4626GetERC4626MaxWithdraw**](ERC4626Api.md#erc4626GetERC4626MaxWithdraw) | **GET** /erc4626/{account}/maxWithdraw |  |
| [**erc4626GetERC4626PreviewDeposit**](ERC4626Api.md#erc4626GetERC4626PreviewDeposit) | **GET** /erc4626/{account}/previewDeposit |  |
| [**erc4626GetERC4626PreviewMint**](ERC4626Api.md#erc4626GetERC4626PreviewMint) | **GET** /erc4626/{account}/previewMint |  |
| [**erc4626GetERC4626PreviewRedeem**](ERC4626Api.md#erc4626GetERC4626PreviewRedeem) | **GET** /erc4626/{account}/previewRedeem |  |
| [**erc4626GetERC4626PreviewWithdraw**](ERC4626Api.md#erc4626GetERC4626PreviewWithdraw) | **GET** /erc4626/{account}/previewWithdraw |  |
| [**erc4626GetERC4626TotalAssets**](ERC4626Api.md#erc4626GetERC4626TotalAssets) | **GET** /erc4626/{account}/totalAssets |  |
| [**erc4626GetERC4626TotalSupply**](ERC4626Api.md#erc4626GetERC4626TotalSupply) | **GET** /erc4626/{account}/totalSupply |  |
| [**erc4626MintERC4626Shares**](ERC4626Api.md#erc4626MintERC4626Shares) | **POST** /erc4626/{address}/mint |  |
| [**erc4626RedeemERC4626Shares**](ERC4626Api.md#erc4626RedeemERC4626Shares) | **POST** /erc4626/{address}/redeem |  |
| [**erc4626TransferERC4626**](ERC4626Api.md#erc4626TransferERC4626) | **POST** /erc4626/{address}/transfer |  |
| [**erc4626TransferFromERC4626**](ERC4626Api.md#erc4626TransferFromERC4626) | **POST** /erc4626/{address}/transferFrom |  |
| [**erc4626WithdrawFromERC4626**](ERC4626Api.md#erc4626WithdrawFromERC4626) | **POST** /erc4626/{address}/withdraw |  |


<a name="erc4626ApproveERC4626"></a>
# **erc4626ApproveERC4626**
> ERC4626APIResponse erc4626ApproveERC4626(address, Authorization, InputBody)



    Approves a spender to transfer a specific amount of shares.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the spender | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address, chain ID, and amount | |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc4626DepositToERC4626"></a>
# **erc4626DepositToERC4626**
> ERC4626APIResponse erc4626DepositToERC4626(address, Authorization, InputBody)



    Deposits assets into the vault and mints shares to the receiver.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the receiver | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address, chain ID, and amount | |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc4626GetERC4626Allowance"></a>
# **erc4626GetERC4626Allowance**
> ERC4626APIResponse erc4626GetERC4626Allowance(account, Authorization, chainId, address, owner, spender)



    Gets the amount of shares that an owner has allowed a spender to use.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **owner** | **String**| - The address of the owner | [default to null] |
| **spender** | **String**| - The address of the spender | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626Asset"></a>
# **erc4626GetERC4626Asset**
> ERC4626APIResponse erc4626GetERC4626Asset(account, Authorization, chainId, address)



    Retrieves the underlying asset address of the ERC4626 vault.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626BalanceOf"></a>
# **erc4626GetERC4626BalanceOf**
> ERC4626APIResponse erc4626GetERC4626BalanceOf(account, Authorization, chainId, address)



    Gets the balance of shares for an account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626ConvertToAssets"></a>
# **erc4626GetERC4626ConvertToAssets**
> ERC4626APIResponse erc4626GetERC4626ConvertToAssets(account, Authorization, chainId, address, shares)



    Calculates the amount of assets that would be withdrawn for a given amount of shares.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **shares** | **String**| - The amount of shares to redeem | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626ConvertToShares"></a>
# **erc4626GetERC4626ConvertToShares**
> ERC4626APIResponse erc4626GetERC4626ConvertToShares(account, Authorization, chainId, address, assets)



    Calculates the amount of shares that would be minted for a given amount of assets.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **assets** | **String**| - The amount of assets to deposit | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626MaxDeposit"></a>
# **erc4626GetERC4626MaxDeposit**
> ERC4626APIResponse erc4626GetERC4626MaxDeposit(account, Authorization, chainId, address, receiver)



    Returns the maximum amount of assets that can be deposited in a single transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **receiver** | **String**| - The address of the receiver | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626MaxMint"></a>
# **erc4626GetERC4626MaxMint**
> ERC4626APIResponse erc4626GetERC4626MaxMint(account, Authorization, chainId, address, receiver)



    Returns the maximum amount of shares that can be minted in a single transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **receiver** | **String**| - The address of the receiver | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626MaxRedeem"></a>
# **erc4626GetERC4626MaxRedeem**
> ERC4626APIResponse erc4626GetERC4626MaxRedeem(account, Authorization, chainId, address, owner)



    Returns the maximum amount of shares that can be redeemed in a single transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **owner** | **String**| - The address of the owner | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626MaxWithdraw"></a>
# **erc4626GetERC4626MaxWithdraw**
> ERC4626APIResponse erc4626GetERC4626MaxWithdraw(account, Authorization, chainId, address, owner)



    Returns the maximum amount of assets that can be withdrawn in a single transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **owner** | **String**| - The address of the owner | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626PreviewDeposit"></a>
# **erc4626GetERC4626PreviewDeposit**
> ERC4626APIResponse erc4626GetERC4626PreviewDeposit(account, Authorization, chainId, address, assets)



    Simulates the amount of shares that would be received for a deposit of assets.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **assets** | **String**| - The amount of assets to deposit | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626PreviewMint"></a>
# **erc4626GetERC4626PreviewMint**
> ERC4626APIResponse erc4626GetERC4626PreviewMint(account, Authorization, chainId, address, shares)



    Simulates the amount of assets needed for minting a specific amount of shares.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **shares** | **String**| - The amount of shares to mint | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626PreviewRedeem"></a>
# **erc4626GetERC4626PreviewRedeem**
> ERC4626APIResponse erc4626GetERC4626PreviewRedeem(account, Authorization, chainId, address, shares)



    Simulates the amount of assets that would be received for redeeming shares.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **shares** | **String**| - The amount of shares to redeem | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626PreviewWithdraw"></a>
# **erc4626GetERC4626PreviewWithdraw**
> ERC4626APIResponse erc4626GetERC4626PreviewWithdraw(account, Authorization, chainId, address, assets)



    Simulates the amount of shares needed to withdraw a specific amount of assets.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |
| **assets** | **String**| - The amount of assets to withdraw | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626TotalAssets"></a>
# **erc4626GetERC4626TotalAssets**
> ERC4626APIResponse erc4626GetERC4626TotalAssets(account, Authorization, chainId, address)



    Gets the total amount of underlying assets held by the vault.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626GetERC4626TotalSupply"></a>
# **erc4626GetERC4626TotalSupply**
> ERC4626APIResponse erc4626GetERC4626TotalSupply(account, Authorization, chainId, address)



    Gets the total supply of shares.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account making the request | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **chainId** | **String**| - The blockchain network ID | [default to null] |
| **address** | **String**| - The ERC4626 vault contract address | [default to null] |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="erc4626MintERC4626Shares"></a>
# **erc4626MintERC4626Shares**
> ERC4626APIResponse erc4626MintERC4626Shares(address, Authorization, InputBody)



    Mints shares to the receiver by depositing exact amount of assets.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the receiver | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address, chain ID, and amount | |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc4626RedeemERC4626Shares"></a>
# **erc4626RedeemERC4626Shares**
> ERC4626APIResponse erc4626RedeemERC4626Shares(address, Authorization, InputBody)



    Redeems shares from owner and sends exact amount of assets to receiver.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the receiver | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address, chain ID, and amount | |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc4626TransferERC4626"></a>
# **erc4626TransferERC4626**
> ERC4626APIResponse erc4626TransferERC4626(address, Authorization, InputBody)



    Transfers shares to a specified address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the receiver | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address, chain ID, and amount | |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc4626TransferFromERC4626"></a>
# **erc4626TransferFromERC4626**
> ERC4626APIResponse erc4626TransferFromERC4626(address, Authorization, InputBody)



    Transfers shares from one address to another.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the receiver | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address, chain ID, and amount | |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="erc4626WithdrawFromERC4626"></a>
# **erc4626WithdrawFromERC4626**
> ERC4626APIResponse erc4626WithdrawFromERC4626(address, Authorization, InputBody)



    Withdraws assets from the vault to the receiver.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the receiver | [default to null] |
| **Authorization** | **String**| - The authorization token | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing the contract address, chain ID, and amount | |

### Return type

[**ERC4626APIResponse**](../Models/ERC4626APIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

