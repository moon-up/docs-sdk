# EosApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createEosAccount**](EosApi.md#createEosAccount) | **POST** /eos |  |
| [**deleteEosAccount**](EosApi.md#deleteEosAccount) | **POST** /eos/{accountName}/delete |  |
| [**exportEosAccount**](EosApi.md#exportEosAccount) | **POST** /eos/{accountName}/export |  |
| [**getEosAccount**](EosApi.md#getEosAccount) | **GET** /eos/{accountName} |  |
| [**listEosAccounts**](EosApi.md#listEosAccounts) | **GET** /eos |  |
| [**signEosTransaction**](EosApi.md#signEosTransaction) | **POST** /eos/{accountName}/sign-tx |  |


<a name="createEosAccount"></a>
# **createEosAccount**
> AccountAPIResponse createEosAccount(Authorization, EosInput)



    Creates a new EOS account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **EosInput** | [**EosInput**](../Models/EosInput.md)| - The input data required to create the EOS account. | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="deleteEosAccount"></a>
# **deleteEosAccount**
> AccountAPIResponse deleteEosAccount(Authorization, accountName)



    Deletes an EOS account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the EOS account to be deleted. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="exportEosAccount"></a>
# **exportEosAccount**
> AccountAPIResponse exportEosAccount(Authorization, accountName)



    Exports the account information for a given EOS account name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the EOS account to export. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getEosAccount"></a>
# **getEosAccount**
> AccountAPIResponse getEosAccount(Authorization, accountName)



    Retrieves account information from the EOS blockchain.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the EOS account to retrieve information for. | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listEosAccounts"></a>
# **listEosAccounts**
> AccountAPIResponse listEosAccounts(Authorization)



    Lists EOS accounts associated with the provided authorization token.

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

<a name="signEosTransaction"></a>
# **signEosTransaction**
> EosAPIResponse signEosTransaction(Authorization, accountName, EosTransactionInput)



    Signs an EOS transaction.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The EOS account name from the request path. | [default to null] |
| **EosTransactionInput** | [**EosTransactionInput**](../Models/EosTransactionInput.md)| - The transaction input data from the request body. | |

### Return type

[**EosAPIResponse**](../Models/EosAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

