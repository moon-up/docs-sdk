# AccountsApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**accountsBroadcastEthreeumTransaction**](AccountsApi.md#accountsBroadcastEthreeumTransaction) | **POST** /accounts/{accountName}/broadcast-tx |  |
| [**accountsCreateEthereumAccount**](AccountsApi.md#accountsCreateEthereumAccount) | **POST** /accounts |  |
| [**accountsDeleteEthereumAccount**](AccountsApi.md#accountsDeleteEthereumAccount) | **DELETE** /accounts/{accountName} |  |
| [**accountsDeployContract**](AccountsApi.md#accountsDeployContract) | **POST** /accounts/{accountName}/deploy |  |
| [**accountsEncodeAbiData**](AccountsApi.md#accountsEncodeAbiData) | **POST** /accounts/encode-data |  |
| [**accountsEstimateGas**](AccountsApi.md#accountsEstimateGas) | **POST** /accounts/{accountName}/estimate |  |
| [**accountsEthereumGetNativeBalance**](AccountsApi.md#accountsEthereumGetNativeBalance) | **GET** /accounts/{accountName}/balance |  |
| [**accountsEthereumGetNonce**](AccountsApi.md#accountsEthereumGetNonce) | **GET** /accounts/{accountName}/nonce |  |
| [**accountsExportEthreumAccount**](AccountsApi.md#accountsExportEthreumAccount) | **GET** /accounts/{accountName}/export |  |
| [**accountsGetEthreumAccount**](AccountsApi.md#accountsGetEthreumAccount) | **GET** /accounts/{accountName} |  |
| [**accountsListEthereumAccounts**](AccountsApi.md#accountsListEthereumAccounts) | **GET** /accounts |  |
| [**accountsSignEthereumTransaction**](AccountsApi.md#accountsSignEthereumTransaction) | **POST** /accounts/{accountName}/sign-transaction |  |
| [**accountsSignEthereumTypedData**](AccountsApi.md#accountsSignEthereumTypedData) | **POST** /accounts/{accountName}/sign-typed-data |  |
| [**accountsSignEthreumMessage**](AccountsApi.md#accountsSignEthreumMessage) | **POST** /accounts/{accountName}/sign-message |  |
| [**accountsSuggestGasPrice**](AccountsApi.md#accountsSuggestGasPrice) | **GET** /accounts/{accountName}/suggest-gas |  |
| [**accountsTransferEth**](AccountsApi.md#accountsTransferEth) | **POST** /accounts/{accountName}/transfer-eth |  |


<a name="accountsBroadcastEthreeumTransaction"></a>
# **accountsBroadcastEthreeumTransaction**
> BroadCastRawTransactionAPIResponse accountsBroadcastEthreeumTransaction(Authorization, accountName, BroadcastInput)



    Broadcasts a transaction using the provided account name and transaction details.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to broadcast the transaction from. | [default to null] |
| **BroadcastInput** | [**BroadcastInput**](../Models/BroadcastInput.md)| - The transaction details to be broadcasted. | |

### Return type

[**BroadCastRawTransactionAPIResponse**](../Models/BroadCastRawTransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="accountsCreateEthereumAccount"></a>
# **accountsCreateEthereumAccount**
> AccountAPIResponse accountsCreateEthereumAccount(Authorization, CreateAccountInput)



    Creates a new account using the provided authorization token and account input data.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **CreateAccountInput** | [**CreateAccountInput**](../Models/CreateAccountInput.md)| - The input data required to create a new account. | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="accountsDeleteEthereumAccount"></a>
# **accountsDeleteEthereumAccount**
> AccountAPIResponse accountsDeleteEthereumAccount(Authorization, accountName)



    Deletes an account based on the provided account name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to be deleted. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="accountsDeployContract"></a>
# **accountsDeployContract**
> TransactionAPIResponse accountsDeployContract(Authorization, accountName, DeployInput)



    Deploys a contract using the provided account name and deployment input.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to deploy the contract to. | [default to null] |
| **DeployInput** | [**DeployInput**](../Models/DeployInput.md)| - The deployment input data. | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="accountsEncodeAbiData"></a>
# **accountsEncodeAbiData**
> AbiEncodeOutput accountsEncodeAbiData(Authorization, AbiEncodeInput)



    Encodes data using the provided ABI and function parameters.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **AbiEncodeInput** | [**AbiEncodeInput**](../Models/AbiEncodeInput.md)| - The input object containing the ABI, function name, and parameters. | |

### Return type

[**AbiEncodeOutput**](../Models/AbiEncodeOutput.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="accountsEstimateGas"></a>
# **accountsEstimateGas**
> TransactionAPIResponse accountsEstimateGas(accountName, Authorization, InputBody)



    Estimates the gas required for a transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account for which to estimate gas. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing transaction details. | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="accountsEthereumGetNativeBalance"></a>
# **accountsEthereumGetNativeBalance**
> BalanceAPIResponse accountsEthereumGetNativeBalance(accountName, Authorization, chainId)



    Retrieves the balance of a specified account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to retrieve the balance for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |

### Return type

[**BalanceAPIResponse**](../Models/BalanceAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="accountsEthereumGetNonce"></a>
# **accountsEthereumGetNonce**
> NonceAPIResponse accountsEthereumGetNonce(accountName, Authorization, chainId)



    Retrieves the nonce for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to retrieve the nonce for. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |

### Return type

[**NonceAPIResponse**](../Models/NonceAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="accountsExportEthreumAccount"></a>
# **accountsExportEthreumAccount**
> ExportAccountAPIResponse accountsExportEthreumAccount(accountName, Authorization)



    Exports the account details including address, private key, and public key.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to be exported. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |

### Return type

[**ExportAccountAPIResponse**](../Models/ExportAccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="accountsGetEthreumAccount"></a>
# **accountsGetEthreumAccount**
> AccountAPIResponse accountsGetEthreumAccount(Authorization, accountName)



      Retrieves the account details for a given account name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to retrieve. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="accountsListEthereumAccounts"></a>
# **accountsListEthereumAccounts**
> AccountAPIResponse accountsListEthereumAccounts(Authorization)



    Lists accounts using the provided authorization token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="accountsSignEthereumTransaction"></a>
# **accountsSignEthereumTransaction**
> TransactionAPIResponse accountsSignEthereumTransaction(accountName, Authorization, InputBody)



    Signs a transaction for the specified account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account for which the transaction is to be signed. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing transaction details. | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="accountsSignEthereumTypedData"></a>
# **accountsSignEthereumTypedData**
> SignMessageAPIResponse accountsSignEthereumTypedData(accountName, Authorization, SignTypedData)



    Handles the signing of typed data for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account for which the data is to be signed. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **SignTypedData** | [**SignTypedData**](../Models/SignTypedData.md)| - The data to be signed. | |

### Return type

[**SignMessageAPIResponse**](../Models/SignMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="accountsSignEthreumMessage"></a>
# **accountsSignEthreumMessage**
> SignMessageAPIResponse accountsSignEthreumMessage(accountName, Authorization, SignMessage)



    Signs a message using the provided account name and authorization token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to sign the message with. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **SignMessage** | [**SignMessage**](../Models/SignMessage.md)| - The body of the request containing the message to be signed. | |

### Return type

[**SignMessageAPIResponse**](../Models/SignMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="accountsSuggestGasPrice"></a>
# **accountsSuggestGasPrice**
> TransactionAPIResponse accountsSuggestGasPrice(accountName, Authorization, chainId)



    Suggests the gas price for a given account and chain ID.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account for which to suggest the gas price. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The ID of the blockchain network. | [default to null] |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="accountsTransferEth"></a>
# **accountsTransferEth**
> TransactionAPIResponse accountsTransferEth(accountName, Authorization, InputBody)



    Transfers Ethereum from one account to another.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account from which Ethereum will be transferred. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)| - The input body containing transfer details. | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

