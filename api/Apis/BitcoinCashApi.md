# BitcoinCashApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bitcoinCashBitcoinCashCreateAccount**](BitcoinCashApi.md#bitcoinCashBitcoinCashCreateAccount) | **POST** /bitcoincash/accounts |  |
| [**bitcoinCashBitcoinCashDeleteAccount**](BitcoinCashApi.md#bitcoinCashBitcoinCashDeleteAccount) | **POST** /bitcoincash/accounts/{accountName}/delete |  |
| [**bitcoinCashBitcoinCashExportAccount**](BitcoinCashApi.md#bitcoinCashBitcoinCashExportAccount) | **POST** /bitcoincash/accounts/{accountName}/export |  |
| [**bitcoinCashBitcoinCashGenerateUnsignedPSBTHex**](BitcoinCashApi.md#bitcoinCashBitcoinCashGenerateUnsignedPSBTHex) | **POST** /bitcoincash/accounts/{accountName}/generate-unsigned-psbt |  |
| [**bitcoinCashBitcoinCashGetAccount**](BitcoinCashApi.md#bitcoinCashBitcoinCashGetAccount) | **GET** /bitcoincash/accounts/{accountName} |  |
| [**bitcoinCashBitcoinCashSignBitcoinTransaction**](BitcoinCashApi.md#bitcoinCashBitcoinCashSignBitcoinTransaction) | **POST** /bitcoincash/accounts/{accountName}/sign-btc-tx |  |
| [**bitcoinCashBitcoinCashSignPSBTWithKeyPathAndScriptPath**](BitcoinCashApi.md#bitcoinCashBitcoinCashSignPSBTWithKeyPathAndScriptPath) | **POST** /bitcoincash/accounts/{accountName}/sign-psbt-with-key-path-and-script-path |  |
| [**bitcoinCashBitcoinCashSignTransaction**](BitcoinCashApi.md#bitcoinCashBitcoinCashSignTransaction) | **POST** /bitcoincash/accounts/{accountName}/sign-tx |  |
| [**bitcoinCashBitcoinCashSignTransactionWithMemo**](BitcoinCashApi.md#bitcoinCashBitcoinCashSignTransactionWithMemo) | **POST** /bitcoincash/accounts/{accountName}/memo-sign-tx |  |
| [**bitcoinCashListAccounts**](BitcoinCashApi.md#bitcoinCashListAccounts) | **GET** /bitcoincash/accounts |  |


<a name="bitcoinCashBitcoinCashCreateAccount"></a>
# **bitcoinCashBitcoinCashCreateAccount**
> BitcoinCashAPIResponse_AccountResponse_ bitcoinCashBitcoinCashCreateAccount(Authorization, BitcoinCashInput)



    Creates a new Bitcoin Cash account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **BitcoinCashInput** | [**BitcoinCashInput**](../Models/BitcoinCashInput.md)| - The input data required to create a Bitcoin Cash account. | |

### Return type

[**BitcoinCashAPIResponse_AccountResponse_**](../Models/BitcoinCashAPIResponse_AccountResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinCashBitcoinCashDeleteAccount"></a>
# **bitcoinCashBitcoinCashDeleteAccount**
> BitcoinCashAPIResponse_AccountResponse_ bitcoinCashBitcoinCashDeleteAccount(accountName, Authorization)



    Deletes a Bitcoin Cash account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to be deleted. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |

### Return type

[**BitcoinCashAPIResponse_AccountResponse_**](../Models/BitcoinCashAPIResponse_AccountResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="bitcoinCashBitcoinCashExportAccount"></a>
# **bitcoinCashBitcoinCashExportAccount**
> BitcoinCashAPIResponse_AccountResponse_ bitcoinCashBitcoinCashExportAccount(accountName, Authorization)



    Exports the account details for the specified account name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to export. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |

### Return type

[**BitcoinCashAPIResponse_AccountResponse_**](../Models/BitcoinCashAPIResponse_AccountResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="bitcoinCashBitcoinCashGenerateUnsignedPSBTHex"></a>
# **bitcoinCashBitcoinCashGenerateUnsignedPSBTHex**
> BitcoinCashAPIResponse__psbt_hex-string__ bitcoinCashBitcoinCashGenerateUnsignedPSBTHex(accountName, Authorization, UnsignedPSBTInput)



    Generates an unsigned PSBT (Partially Signed Bitcoin Transaction) hex string.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account for which to generate the PSBT. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **UnsignedPSBTInput** | [**UnsignedPSBTInput**](../Models/UnsignedPSBTInput.md)| - The input data required to generate the unsigned PSBT. | |

### Return type

[**BitcoinCashAPIResponse__psbt_hex-string__**](../Models/BitcoinCashAPIResponse__psbt_hex-string__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinCashBitcoinCashGetAccount"></a>
# **bitcoinCashBitcoinCashGetAccount**
> BitcoinCashAPIResponse_AccountResponse_ bitcoinCashBitcoinCashGetAccount(accountName, Authorization)



    Reads the account information for a given account name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to read. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |

### Return type

[**BitcoinCashAPIResponse_AccountResponse_**](../Models/BitcoinCashAPIResponse_AccountResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="bitcoinCashBitcoinCashSignBitcoinTransaction"></a>
# **bitcoinCashBitcoinCashSignBitcoinTransaction**
> BitcoinCashAPIResponse__signed_tx-string__ bitcoinCashBitcoinCashSignBitcoinTransaction(accountName, Authorization, BitcoinCash\_BitcoinCashSignBitcoinTransaction\_request)



    Signs a Bitcoin transaction for the specified account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to sign the transaction for. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **BitcoinCash\_BitcoinCashSignBitcoinTransaction\_request** | [**BitcoinCash_BitcoinCashSignBitcoinTransaction_request**](../Models/BitcoinCash_BitcoinCashSignBitcoinTransaction_request.md)| - The request body containing the network, inputs, and outputs. | |

### Return type

[**BitcoinCashAPIResponse__signed_tx-string__**](../Models/BitcoinCashAPIResponse__signed_tx-string__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinCashBitcoinCashSignPSBTWithKeyPathAndScriptPath"></a>
# **bitcoinCashBitcoinCashSignPSBTWithKeyPathAndScriptPath**
> BitcoinCashAPIResponse__signed_psbt_hex-string__ bitcoinCashBitcoinCashSignPSBTWithKeyPathAndScriptPath(accountName, Authorization, BitcoinCash\_BitcoinCashSignPSBTWithKeyPathAndScriptPath\_request)



    Signs a Partially Signed Bitcoin Transaction (PSBT) using a key path and script path.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to use for signing. | [default to null] |
| **Authorization** | **String**| - The authorization token for authentication. | [default to null] |
| **BitcoinCash\_BitcoinCashSignPSBTWithKeyPathAndScriptPath\_request** | [**BitcoinCash_BitcoinCashSignPSBTWithKeyPathAndScriptPath_request**](../Models/BitcoinCash_BitcoinCashSignPSBTWithKeyPathAndScriptPath_request.md)| - The request body containing the network and PSBT in hexadecimal format. | |

### Return type

[**BitcoinCashAPIResponse__signed_psbt_hex-string__**](../Models/BitcoinCashAPIResponse__signed_psbt_hex-string__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinCashBitcoinCashSignTransaction"></a>
# **bitcoinCashBitcoinCashSignTransaction**
> BitcoinCashAPIResponse_BitcoinCashTransactionOutput_ bitcoinCashBitcoinCashSignTransaction(accountName, Authorization, BitcoinCashTransactionInput)



    Signs a Bitcoin Cash transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to sign the transaction for. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **BitcoinCashTransactionInput** | [**BitcoinCashTransactionInput**](../Models/BitcoinCashTransactionInput.md)| - The transaction input data. | |

### Return type

[**BitcoinCashAPIResponse_BitcoinCashTransactionOutput_**](../Models/BitcoinCashAPIResponse_BitcoinCashTransactionOutput_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinCashBitcoinCashSignTransactionWithMemo"></a>
# **bitcoinCashBitcoinCashSignTransactionWithMemo**
> BitcoinCashAPIResponse_BitcoinCashTransactionOutput_ bitcoinCashBitcoinCashSignTransactionWithMemo(accountName, Authorization, BitcoinCashTransactionInput)



    Signs a Bitcoin Cash transaction with a memo.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to sign the transaction for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **BitcoinCashTransactionInput** | [**BitcoinCashTransactionInput**](../Models/BitcoinCashTransactionInput.md)| - The input data for the Bitcoin Cash transaction. | |

### Return type

[**BitcoinCashAPIResponse_BitcoinCashTransactionOutput_**](../Models/BitcoinCashAPIResponse_BitcoinCashTransactionOutput_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinCashListAccounts"></a>
# **bitcoinCashListAccounts**
> BitcoinCashAPIResponse_AccountResponse_ bitcoinCashListAccounts(Authorization)



    Lists Bitcoin Cash accounts associated with the provided authorization token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |

### Return type

[**BitcoinCashAPIResponse_AccountResponse_**](../Models/BitcoinCashAPIResponse_AccountResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

