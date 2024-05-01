# AaveApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**borrow**](AaveApi.md#borrow) | **POST** /aave/{name}/borrow |  |
| [**lend**](AaveApi.md#lend) | **POST** /aave/{name}/lend |  |
| [**repay**](AaveApi.md#repay) | **POST** /aave/{name}/repay |  |
| [**userReserveData**](AaveApi.md#userReserveData) | **POST** /aave/{name}/user-reserve-data |  |


<a name="borrow"></a>
# **borrow**
> TransactionAPIResponse borrow(Authorization, name, AaveInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **AaveInput** | [**AaveInput**](../Models/AaveInput.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="lend"></a>
# **lend**
> TransactionAPIResponse lend(Authorization, name, AaveInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **AaveInput** | [**AaveInput**](../Models/AaveInput.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="repay"></a>
# **repay**
> TransactionAPIResponse repay(Authorization, name, AaveInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **AaveInput** | [**AaveInput**](../Models/AaveInput.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="userReserveData"></a>
# **userReserveData**
> AaveReservesAPIResponse userReserveData(Authorization, name, AaveInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **AaveInput** | [**AaveInput**](../Models/AaveInput.md)|  | |

### Return type

[**AaveReservesAPIResponse**](../Models/AaveReservesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

