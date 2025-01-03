# AAVEV3WalletBalanceProviderApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**aaveV3WalletBalanceOf**](AAVEV3WalletBalanceProviderApi.md#aaveV3WalletBalanceOf) | **GET** /aave/v3/wallet-balance/balance-of |  |
| [**aaveV3WalletBatchBalanceOf**](AAVEV3WalletBalanceProviderApi.md#aaveV3WalletBatchBalanceOf) | **GET** /aave/v3/wallet-balance/batch-balance-of |  |
| [**aaveV3WalletUserWalletBalances**](AAVEV3WalletBalanceProviderApi.md#aaveV3WalletUserWalletBalances) | **GET** /aave/v3/wallet-balance/user-wallet-balances |  |


<a name="aaveV3WalletBalanceOf"></a>
# **aaveV3WalletBalanceOf**
> AAVEv3WalletBalanceProviderAPIResponse_string_ aaveV3WalletBalanceOf(Authorization, contract\_address, chain\_id, user, token\_address)



    Retrieves the balance of a specific token for a user from the AAVE v3 Wallet Balance Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **contract\_address** | **String**| - The address of the contract to query. | [default to null] |
| **chain\_id** | **String**| - The ID of the blockchain network. | [default to null] |
| **user** | **String**| - The address of the user whose balance is being queried. | [default to null] |
| **token\_address** | **String**| - The address of the token to query the balance for. | [default to null] |

### Return type

[**AAVEv3WalletBalanceProviderAPIResponse_string_**](../Models/AAVEv3WalletBalanceProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aaveV3WalletBatchBalanceOf"></a>
# **aaveV3WalletBatchBalanceOf**
> AAVEv3WalletBalanceProviderAPIResponse_string-Array_ aaveV3WalletBatchBalanceOf(Authorization, contract\_address, chain\_id, users, tokens)



    Retrieves the batch balance of multiple users for specified tokens.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **contract\_address** | **String**| - The address of the contract. | [default to null] |
| **chain\_id** | **String**| - The ID of the blockchain network. | [default to null] |
| **users** | [**List**](../Models/String.md)| - An array of user addresses to retrieve balances for. | [default to null] |
| **tokens** | [**List**](../Models/String.md)| - An array of token addresses to retrieve balances for. | [default to null] |

### Return type

[**AAVEv3WalletBalanceProviderAPIResponse_string-Array_**](../Models/AAVEv3WalletBalanceProviderAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aaveV3WalletUserWalletBalances"></a>
# **aaveV3WalletUserWalletBalances**
> AAVEv3WalletBalanceProviderAPIResponse__tokens-string-Array--balances-string-Array--__ aaveV3WalletUserWalletBalances(Authorization, contract\_address, chain\_id, provider, user)



    Retrieves the wallet balances for a user from the AAVE v3 Wallet Balance Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **contract\_address** | **String**| - The contract address to query. | [default to null] |
| **chain\_id** | **String**| - The chain ID to query. | [default to null] |
| **provider** | **String**| - The provider to use for querying balances. | [default to null] |
| **user** | **String**| - The user address to query balances for. | [default to null] |

### Return type

[**AAVEv3WalletBalanceProviderAPIResponse__tokens-string-Array--balances-string-Array--__**](../Models/AAVEv3WalletBalanceProviderAPIResponse__tokens-string-Array--balances-string-Array--__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

