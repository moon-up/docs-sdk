# BitcoinApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bitcoinBitcoinCreateAccount**](BitcoinApi.md#bitcoinBitcoinCreateAccount) | **POST** /bitcoin |  |
| [**bitcoinBitcoinCreateBRC20Transaction**](BitcoinApi.md#bitcoinBitcoinCreateBRC20Transaction) | **POST** /bitcoin/{accountName}/brc20-tx |  |
| [**bitcoinBitcoinCreateSRC20Inscription**](BitcoinApi.md#bitcoinBitcoinCreateSRC20Inscription) | **POST** /bitcoin/{accountName}/src20-inscription |  |
| [**bitcoinBitcoinDeleteAccount**](BitcoinApi.md#bitcoinBitcoinDeleteAccount) | **POST** /bitcoin/{accountName}/delete |  |
| [**bitcoinBitcoinExportAccount**](BitcoinApi.md#bitcoinBitcoinExportAccount) | **POST** /bitcoin/{accountName}/export |  |
| [**bitcoinBitcoinGenerateUnsignedPSBTHex**](BitcoinApi.md#bitcoinBitcoinGenerateUnsignedPSBTHex) | **POST** /bitcoin/{accountName}/generate-unsigned-psbt |  |
| [**bitcoinBitcoinGetAccount**](BitcoinApi.md#bitcoinBitcoinGetAccount) | **GET** /bitcoin/{accountName} |  |
| [**bitcoinBitcoinSignTransaction**](BitcoinApi.md#bitcoinBitcoinSignTransaction) | **POST** /bitcoin/{accountName}/sign-tx |  |
| [**bitcoinListAccounts**](BitcoinApi.md#bitcoinListAccounts) | **GET** /bitcoin |  |


<a name="bitcoinBitcoinCreateAccount"></a>
# **bitcoinBitcoinCreateAccount**
> AccountAPIResponse bitcoinBitcoinCreateAccount(Authorization, BitcoinInput)



    Creates a new Bitcoin account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **BitcoinInput** | [**BitcoinInput**](../Models/BitcoinInput.md)| - The input data required to create a Bitcoin account. | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinBitcoinCreateBRC20Transaction"></a>
# **bitcoinBitcoinCreateBRC20Transaction**
> BitcoinAPIResponse bitcoinBitcoinCreateBRC20Transaction(Authorization, accountName, BRC20TransactionInput)



    Creates a BRC20 transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account for which the transaction is being created. | [default to null] |
| **BRC20TransactionInput** | [**BRC20TransactionInput**](../Models/BRC20TransactionInput.md)| - The input data for the BRC20 transaction. | |

### Return type

[**BitcoinAPIResponse**](../Models/BitcoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinBitcoinCreateSRC20Inscription"></a>
# **bitcoinBitcoinCreateSRC20Inscription**
> BitcoinAPIResponse bitcoinBitcoinCreateSRC20Inscription(Authorization, accountName, SRC20InscriptionInput)



    Creates an SRC20 inscription using the provided account name and inscription input.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account for which the inscription is being created. | [default to null] |
| **SRC20InscriptionInput** | [**SRC20InscriptionInput**](../Models/SRC20InscriptionInput.md)| - The input data for the SRC20 inscription. | |

### Return type

[**BitcoinAPIResponse**](../Models/BitcoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinBitcoinDeleteAccount"></a>
# **bitcoinBitcoinDeleteAccount**
> AccountAPIResponse bitcoinBitcoinDeleteAccount(Authorization, accountName)



    Deletes a Bitcoin account.

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

<a name="bitcoinBitcoinExportAccount"></a>
# **bitcoinBitcoinExportAccount**
> AccountAPIResponse bitcoinBitcoinExportAccount(Authorization, accountName)



    Exports the account details for the specified account name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to be exported. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="bitcoinBitcoinGenerateUnsignedPSBTHex"></a>
# **bitcoinBitcoinGenerateUnsignedPSBTHex**
> BitcoinAPIResponse bitcoinBitcoinGenerateUnsignedPSBTHex(Authorization, accountName, UnsignedPSBTInput)



    Generates an unsigned PSBT (Partially Signed Bitcoin Transaction) hex string.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account for which to generate the PSBT. | [default to null] |
| **UnsignedPSBTInput** | [**UnsignedPSBTInput**](../Models/UnsignedPSBTInput.md)| - The input data required to generate the unsigned PSBT. | |

### Return type

[**BitcoinAPIResponse**](../Models/BitcoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinBitcoinGetAccount"></a>
# **bitcoinBitcoinGetAccount**
> AccountAPIResponse bitcoinBitcoinGetAccount(Authorization, accountName)



    Retrieves the account information for a given account name.

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

<a name="bitcoinBitcoinSignTransaction"></a>
# **bitcoinBitcoinSignTransaction**
> BitcoinAPIResponse bitcoinBitcoinSignTransaction(Authorization, accountName, BitcoinTransactionInput)



    Signs a Bitcoin transaction using the provided account name and transaction input.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to sign the transaction for. | [default to null] |
| **BitcoinTransactionInput** | [**BitcoinTransactionInput**](../Models/BitcoinTransactionInput.md)| - The transaction input details. | |

### Return type

[**BitcoinAPIResponse**](../Models/BitcoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="bitcoinListAccounts"></a>
# **bitcoinListAccounts**
> AccountAPIResponse bitcoinListAccounts(Authorization)



    Lists the accounts associated with the provided authorization token.

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

