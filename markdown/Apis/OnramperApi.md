# OnramperApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**onRamperCheckout**](OnramperApi.md#onRamperCheckout) | **POST** /onramper/fund/${accountName} |  |
| [**onRamperGetQuotesBuy**](OnramperApi.md#onRamperGetQuotesBuy) | **GET** /onramper/quotes/buy |  |
| [**onRamperGetQuotesSell**](OnramperApi.md#onRamperGetQuotesSell) | **GET** /onramper/quotes/sell |  |
| [**onRamperGetSupportedAssets**](OnramperApi.md#onRamperGetSupportedAssets) | **GET** /onramper/assets |  |
| [**onRamperGetSupportedCurrencies**](OnramperApi.md#onRamperGetSupportedCurrencies) | **GET** /onramper/currencies |  |
| [**onRamperGetSupportedDefaultsAll**](OnramperApi.md#onRamperGetSupportedDefaultsAll) | **GET** /onramper/defaults |  |
| [**onRamperGetSupportedOnRampsAll**](OnramperApi.md#onRamperGetSupportedOnRampsAll) | **GET** /onramper/onramps |  |
| [**onRamperGetSupportedPaymentTypes**](OnramperApi.md#onRamperGetSupportedPaymentTypes) | **GET** /onramper/payment-types |  |
| [**onRamperGetSupportedPaymentTypesFiat**](OnramperApi.md#onRamperGetSupportedPaymentTypesFiat) | **GET** /onramper/payment-types/fiat |  |


<a name="onRamperCheckout"></a>
# **onRamperCheckout**
> oas_any_type_not_mapped onRamperCheckout(Authorization, accountName, TransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **TransactionInput** | [**TransactionInput**](../Models/TransactionInput.md)|  | |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="onRamperGetQuotesBuy"></a>
# **onRamperGetQuotesBuy**
> List onRamperGetQuotesBuy(Authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **fiat** | **String**|  | [default to null] |
| **crypto** | **String**|  | [default to null] |
| **amount** | **Double**|  | [default to null] |
| **paymentMethod** | **String**|  | [optional] [default to creditcard] |
| **uuid** | **String**|  | [optional] [default to ] |
| **clientName** | **String**|  | [optional] [default to ] |
| **country** | **String**|  | [optional] [default to ] |

### Return type

[**List**](../Models/Quote.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="onRamperGetQuotesSell"></a>
# **onRamperGetQuotesSell**
> List onRamperGetQuotesSell(Authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **fiat** | **String**|  | [default to null] |
| **crypto** | **String**|  | [default to null] |
| **amount** | **Double**|  | [default to null] |
| **paymentMethod** | **String**|  | [optional] [default to creditcard] |
| **uuid** | **String**|  | [optional] [default to ] |
| **clientName** | **String**|  | [optional] [default to ] |
| **country** | **String**|  | [optional] [default to ] |

### Return type

[**List**](../Models/SellQuote.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="onRamperGetSupportedAssets"></a>
# **onRamperGetSupportedAssets**
> SupportedAssetResponse onRamperGetSupportedAssets(Authorization, source, country)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **source** | **String**|  | [default to null] |
| **country** | **String**|  | [default to null] |

### Return type

[**SupportedAssetResponse**](../Models/SupportedAssetResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="onRamperGetSupportedCurrencies"></a>
# **onRamperGetSupportedCurrencies**
> SupportedCurrenciesResponse onRamperGetSupportedCurrencies(Authorization, type)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **type** | **String**|  | [default to null] |

### Return type

[**SupportedCurrenciesResponse**](../Models/SupportedCurrenciesResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="onRamperGetSupportedDefaultsAll"></a>
# **onRamperGetSupportedDefaultsAll**
> SupportedDefaultResponse onRamperGetSupportedDefaultsAll(Authorization, country, type)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **country** | **String**|  | [default to null] |
| **type** | **String**|  | [default to null] |

### Return type

[**SupportedDefaultResponse**](../Models/SupportedDefaultResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="onRamperGetSupportedOnRampsAll"></a>
# **onRamperGetSupportedOnRampsAll**
> GetSupportedOnRampsResponse onRamperGetSupportedOnRampsAll(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**GetSupportedOnRampsResponse**](../Models/GetSupportedOnRampsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="onRamperGetSupportedPaymentTypes"></a>
# **onRamperGetSupportedPaymentTypes**
> SupportedPaymentTypesCurrencyResponse onRamperGetSupportedPaymentTypes(Authorization, fiat, country, type)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **fiat** | **String**|  | [default to null] |
| **country** | **String**|  | [default to null] |
| **type** | **String**|  | [default to null] |

### Return type

[**SupportedPaymentTypesCurrencyResponse**](../Models/SupportedPaymentTypesCurrencyResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="onRamperGetSupportedPaymentTypesFiat"></a>
# **onRamperGetSupportedPaymentTypesFiat**
> SupportedPaymentTypesCurrencyResponse onRamperGetSupportedPaymentTypesFiat(Authorization, fiat, country)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **fiat** | **String**|  | [default to null] |
| **country** | **String**|  | [default to null] |

### Return type

[**SupportedPaymentTypesCurrencyResponse**](../Models/SupportedPaymentTypesCurrencyResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

