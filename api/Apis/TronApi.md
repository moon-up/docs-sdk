# TronApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**tronCreateTronAccount**](TronApi.md#tronCreateTronAccount) | **POST** /tron |  |
| [**tronDeleteTronAccount**](TronApi.md#tronDeleteTronAccount) | **POST** /tron/{accountName}/delete |  |
| [**tronExportTronAccount**](TronApi.md#tronExportTronAccount) | **POST** /tron/{accountName}/export |  |
| [**tronGetTronAccount**](TronApi.md#tronGetTronAccount) | **GET** /tron/{accountName} |  |
| [**tronListTronAccounts**](TronApi.md#tronListTronAccounts) | **GET** /tron |  |
| [**tronSignTronTransaction**](TronApi.md#tronSignTronTransaction) | **POST** /tron/{accountName}/sign-tx |  |


<a name="tronCreateTronAccount"></a>
# **tronCreateTronAccount**
> AccountAPIResponse tronCreateTronAccount(Authorization, TronInput)



    Creates a new account using the provided TronInput data.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **TronInput** | [**TronInput**](../Models/TronInput.md)| - The input data required to create a Tron account. | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="tronDeleteTronAccount"></a>
# **tronDeleteTronAccount**
> AccountAPIResponse tronDeleteTronAccount(Authorization, accountName)



    Deletes an account using the provided account name and authorization token.

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

<a name="tronExportTronAccount"></a>
# **tronExportTronAccount**
> AccountAPIResponse tronExportTronAccount(Authorization, accountName)



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

<a name="tronGetTronAccount"></a>
# **tronGetTronAccount**
> AccountAPIResponse tronGetTronAccount(Authorization, accountName)



    Retrieves account information from the Tron blockchain.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to retrieve information for. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="tronListTronAccounts"></a>
# **tronListTronAccounts**
> AccountAPIResponse tronListTronAccounts(Authorization)



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

<a name="tronSignTronTransaction"></a>
# **tronSignTronTransaction**
> TronAPIResponse tronSignTronTransaction(Authorization, accountName, TronTransactionInput)



    Signs a Tron transaction using the provided account name and transaction input.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to sign the transaction for. | [default to null] |
| **TronTransactionInput** | [**TronTransactionInput**](../Models/TronTransactionInput.md)| - The transaction input data. | |

### Return type

[**TronAPIResponse**](../Models/TronAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

