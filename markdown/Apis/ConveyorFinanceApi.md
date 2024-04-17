# ConveyorFinanceApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**swap**](ConveyorFinanceApi.md#swap) | **POST** /conveyorfinance/{name}/swap |  |


<a name="swap"></a>
# **swap**
> ConveyorFinanceControllerResponse swap(Authorization, name, TokenSwapParams)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **TokenSwapParams** | [**TokenSwapParams**](../Models/TokenSwapParams.md)|  | |

### Return type

[**ConveyorFinanceControllerResponse**](../Models/ConveyorFinanceControllerResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

