# LitecoinApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listLitecoinAccounts**](LitecoinApi.md#listLitecoinAccounts) | **GET** /litecoin |  |
| [**litecoinCreateLitecoinAccount**](LitecoinApi.md#litecoinCreateLitecoinAccount) | **POST** /litecoin |  |
| [**litecoinDeleteLitecoinAccount**](LitecoinApi.md#litecoinDeleteLitecoinAccount) | **POST** /litecoin/{accountName}/delete |  |
| [**litecoinExportLitecoinAccount**](LitecoinApi.md#litecoinExportLitecoinAccount) | **POST** /litecoin/{accountName}/export |  |
| [**litecoinGetLitecoinAccount**](LitecoinApi.md#litecoinGetLitecoinAccount) | **GET** /litecoin/{accountName} |  |
| [**litecoinSignLitecoinTransaction**](LitecoinApi.md#litecoinSignLitecoinTransaction) | **POST** /litecoin/{accountName}/sign-tx |  |
| [**litecoinSignLitecoinTransactionWithMemo**](LitecoinApi.md#litecoinSignLitecoinTransactionWithMemo) | **POST** /litecoin/{accountName}/memo-sign-tx |  |


<a name="listLitecoinAccounts"></a>
# **listLitecoinAccounts**
> AccountAPIResponse listLitecoinAccounts(Authorization)



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

<a name="litecoinCreateLitecoinAccount"></a>
# **litecoinCreateLitecoinAccount**
> AccountAPIResponse litecoinCreateLitecoinAccount(Authorization, LitecoinInput)



    Creates a new Litecoin account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **LitecoinInput** | [**LitecoinInput**](../Models/LitecoinInput.md)| - The input data required to create a Litecoin account. | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="litecoinDeleteLitecoinAccount"></a>
# **litecoinDeleteLitecoinAccount**
> AccountAPIResponse litecoinDeleteLitecoinAccount(Authorization, accountName)



    Deletes a Litecoin account.

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

<a name="litecoinExportLitecoinAccount"></a>
# **litecoinExportLitecoinAccount**
> AccountAPIResponse litecoinExportLitecoinAccount(Authorization, accountName)



    Exports the account information for a given account name.

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

<a name="litecoinGetLitecoinAccount"></a>
# **litecoinGetLitecoinAccount**
> AccountAPIResponse litecoinGetLitecoinAccount(Authorization, accountName)



    Retrieves account information for a specified account name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token provided in the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to retrieve information for. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="litecoinSignLitecoinTransaction"></a>
# **litecoinSignLitecoinTransaction**
> LitecoinAPIResponse litecoinSignLitecoinTransaction(Authorization, accountName, LitecoinTransactionInput)



    Signs a Litecoin transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to sign the transaction for. | [default to null] |
| **LitecoinTransactionInput** | [**LitecoinTransactionInput**](../Models/LitecoinTransactionInput.md)| - The transaction input details. | |

### Return type

[**LitecoinAPIResponse**](../Models/LitecoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="litecoinSignLitecoinTransactionWithMemo"></a>
# **litecoinSignLitecoinTransactionWithMemo**
> LitecoinAPIResponse litecoinSignLitecoinTransactionWithMemo(Authorization, accountName, LitecoinTransactionInput)



    Signs a Litecoin transaction with a memo.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The account name from the request path. | [default to null] |
| **LitecoinTransactionInput** | [**LitecoinTransactionInput**](../Models/LitecoinTransactionInput.md)| - The transaction input details. | |

### Return type

[**LitecoinAPIResponse**](../Models/LitecoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

