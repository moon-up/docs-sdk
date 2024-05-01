# DogeCoinApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createDogeCoinAccount**](DogeCoinApi.md#createDogeCoinAccount) | **POST** /dogecoin |  |
| [**getDogeCoinAccount**](DogeCoinApi.md#getDogeCoinAccount) | **GET** /dogecoin/{accountName} |  |
| [**listDogeCoinAccounts**](DogeCoinApi.md#listDogeCoinAccounts) | **GET** /dogecoin |  |
| [**signDogeCoinTransaction**](DogeCoinApi.md#signDogeCoinTransaction) | **POST** /dogecoin/{accountName}/sign-tx |  |


<a name="createDogeCoinAccount"></a>
# **createDogeCoinAccount**
> AccountAPIResponse createDogeCoinAccount(Authorization, DogeCoinInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **DogeCoinInput** | [**DogeCoinInput**](../Models/DogeCoinInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getDogeCoinAccount"></a>
# **getDogeCoinAccount**
> AccountAPIResponse getDogeCoinAccount(Authorization, accountName)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listDogeCoinAccounts"></a>
# **listDogeCoinAccounts**
> AccountAPIResponse listDogeCoinAccounts(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="signDogeCoinTransaction"></a>
# **signDogeCoinTransaction**
> DogeCoinAPIResponse signDogeCoinTransaction(Authorization, accountName, DogeCoinTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **DogeCoinTransactionInput** | [**DogeCoinTransactionInput**](../Models/DogeCoinTransactionInput.md)|  | |

### Return type

[**DogeCoinAPIResponse**](../Models/DogeCoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

