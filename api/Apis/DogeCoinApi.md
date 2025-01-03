# DogeCoinApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**dogeCoinListAccounts**](DogeCoinApi.md#dogeCoinListAccounts) | **GET** /dogecoin |  |
| [**dogecoinDogeCoinCreateNewAccount**](DogeCoinApi.md#dogecoinDogeCoinCreateNewAccount) | **POST** /dogecoin |  |
| [**dogecoinDogeCoinDeleteAccount**](DogeCoinApi.md#dogecoinDogeCoinDeleteAccount) | **POST** /dogecoin/{accountName}/delete |  |
| [**dogecoinDogeCoinExportAccountDetails**](DogeCoinApi.md#dogecoinDogeCoinExportAccountDetails) | **POST** /dogecoin/{accountName}/export |  |
| [**dogecoinDogeCoinGetAccountDetails**](DogeCoinApi.md#dogecoinDogeCoinGetAccountDetails) | **GET** /dogecoin/{accountName} |  |
| [**dogecoinDogeCoinSignTransaction**](DogeCoinApi.md#dogecoinDogeCoinSignTransaction) | **POST** /dogecoin/{accountName}/sign-tx |  |
| [**dogecoinDogeCoinSignTransactionWithMemo**](DogeCoinApi.md#dogecoinDogeCoinSignTransactionWithMemo) | **POST** /dogecoin/{accountName}/memo-sign-tx |  |


<a name="dogeCoinListAccounts"></a>
# **dogeCoinListAccounts**
> AccountAPIResponse dogeCoinListAccounts(Authorization)



    Lists the accounts associated with the provided Dogecoin token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for accessing Dogecoin accounts. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dogecoinDogeCoinCreateNewAccount"></a>
# **dogecoinDogeCoinCreateNewAccount**
> AccountAPIResponse dogecoinDogeCoinCreateNewAccount(Authorization, DogeCoinInput)



    Creates a new Dogecoin account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **DogeCoinInput** | [**DogeCoinInput**](../Models/DogeCoinInput.md)| - The input data required to create a Dogecoin account. | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="dogecoinDogeCoinDeleteAccount"></a>
# **dogecoinDogeCoinDeleteAccount**
> AccountAPIResponse dogecoinDogeCoinDeleteAccount(Authorization, accountName)



    Deletes a Dogecoin account.

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

<a name="dogecoinDogeCoinExportAccountDetails"></a>
# **dogecoinDogeCoinExportAccountDetails**
> AccountAPIResponse dogecoinDogeCoinExportAccountDetails(Authorization, accountName)



    Exports the account details for a given account name.

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

<a name="dogecoinDogeCoinGetAccountDetails"></a>
# **dogecoinDogeCoinGetAccountDetails**
> AccountAPIResponse dogecoinDogeCoinGetAccountDetails(Authorization, accountName)



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

<a name="dogecoinDogeCoinSignTransaction"></a>
# **dogecoinDogeCoinSignTransaction**
> DogeCoinAPIResponse dogecoinDogeCoinSignTransaction(Authorization, accountName, DogeCoinTransactionInput)



    Signs a Dogecoin transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account for which the transaction is being signed. | [default to null] |
| **DogeCoinTransactionInput** | [**DogeCoinTransactionInput**](../Models/DogeCoinTransactionInput.md)| - The transaction input data. | |

### Return type

[**DogeCoinAPIResponse**](../Models/DogeCoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="dogecoinDogeCoinSignTransactionWithMemo"></a>
# **dogecoinDogeCoinSignTransactionWithMemo**
> DogeCoinAPIResponse dogecoinDogeCoinSignTransactionWithMemo(Authorization, accountName, DogeCoinTransactionInput)



    Signs a Dogecoin transaction with a memo.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to sign the transaction for. | [default to null] |
| **DogeCoinTransactionInput** | [**DogeCoinTransactionInput**](../Models/DogeCoinTransactionInput.md)| - The transaction input data. | |

### Return type

[**DogeCoinAPIResponse**](../Models/DogeCoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

