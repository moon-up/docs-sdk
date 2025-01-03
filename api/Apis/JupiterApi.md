# JupiterApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**jUPITERCancelLimitOrders**](JupiterApi.md#jUPITERCancelLimitOrders) | **POST** /jupiter/{accountName}/cancelLimitOrders |  |
| [**jUPITERCreateLimitOrder**](JupiterApi.md#jUPITERCreateLimitOrder) | **POST** /jupiter/{accountName}/createLimitOrder |  |
| [**jUPITERGetIndexedRouteMap**](JupiterApi.md#jUPITERGetIndexedRouteMap) | **GET** /jupiter/indexedRouteMap |  |
| [**jUPITERGetOpenOrders**](JupiterApi.md#jUPITERGetOpenOrders) | **GET** /jupiter/openOrders |  |
| [**jUPITERGetOrderHistory**](JupiterApi.md#jUPITERGetOrderHistory) | **GET** /jupiter/orderHistory |  |
| [**jUPITERGetProgramIdToLabel**](JupiterApi.md#jUPITERGetProgramIdToLabel) | **GET** /jupiter/programIdToLabel |  |
| [**jUPITERGetQuote**](JupiterApi.md#jUPITERGetQuote) | **POST** /jupiter/{accountName}/quote |  |
| [**jUPITERGetSwapInstructions**](JupiterApi.md#jUPITERGetSwapInstructions) | **POST** /jupiter/{accountName}/swapInstructions |  |
| [**jUPITERGetTokens**](JupiterApi.md#jUPITERGetTokens) | **GET** /jupiter/tokens |  |
| [**jUPITERSwap**](JupiterApi.md#jUPITERSwap) | **POST** /jupiter/{accountName}/swap |  |


<a name="jUPITERCancelLimitOrders"></a>
# **jUPITERCancelLimitOrders**
> JupiterAPIResponse_JupiterExecuteFunctionResult_ jUPITERCancelLimitOrders(accountName, Authorization, JUPITER\_cancelLimitOrders\_request)



    Cancels limit orders for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to cancel limit orders for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **JUPITER\_cancelLimitOrders\_request** | [**JUPITER_cancelLimitOrders_request**](../Models/JUPITER_cancelLimitOrders_request.md)|  | |

### Return type

[**JupiterAPIResponse_JupiterExecuteFunctionResult_**](../Models/JupiterAPIResponse_JupiterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="jUPITERCreateLimitOrder"></a>
# **jUPITERCreateLimitOrder**
> JupiterAPIResponse_JupiterExecuteFunctionResult_ jUPITERCreateLimitOrder(accountName, Authorization, CreateLimitOrderBody)



    Creates a limit order for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to create the limit order for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **CreateLimitOrderBody** | [**CreateLimitOrderBody**](../Models/CreateLimitOrderBody.md)| - The input body for creating a limit order. | |

### Return type

[**JupiterAPIResponse_JupiterExecuteFunctionResult_**](../Models/JupiterAPIResponse_JupiterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="jUPITERGetIndexedRouteMap"></a>
# **jUPITERGetIndexedRouteMap**
> JupiterAPIResponse_any_ jUPITERGetIndexedRouteMap(Authorization, onlyDirectRoutes)



    Retrieves the indexed route map.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **onlyDirectRoutes** | **Boolean**| - A boolean value indicating whether to only include direct routes in the map. | [optional] [default to null] |

### Return type

[**JupiterAPIResponse_any_**](../Models/JupiterAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="jUPITERGetOpenOrders"></a>
# **jUPITERGetOpenOrders**
> JupiterAPIResponse_JupiterExecuteFunctionResult_ jUPITERGetOpenOrders(Authorization, wallet, inputMint, outputMint)



    Retrieves open orders for a given wallet address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **wallet** | **String**| - The wallet address to get open orders for. | [default to null] |
| **inputMint** | **String**| - Optional input mint address to filter orders. | [optional] [default to null] |
| **outputMint** | **String**| - Optional output mint address to filter orders. | [optional] [default to null] |

### Return type

[**JupiterAPIResponse_JupiterExecuteFunctionResult_**](../Models/JupiterAPIResponse_JupiterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="jUPITERGetOrderHistory"></a>
# **jUPITERGetOrderHistory**
> JupiterAPIResponse_JupiterExecuteFunctionResult_ jUPITERGetOrderHistory(Authorization, wallet, page)



    Retrieves order history for a given wallet address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **wallet** | **String**| - The wallet address to get order history for. | [default to null] |
| **page** | **Double**| - The page number for pagination. | [optional] [default to 1] |

### Return type

[**JupiterAPIResponse_JupiterExecuteFunctionResult_**](../Models/JupiterAPIResponse_JupiterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="jUPITERGetProgramIdToLabel"></a>
# **jUPITERGetProgramIdToLabel**
> JupiterAPIResponse_Record_string.string__ jUPITERGetProgramIdToLabel(Authorization)



    Retrieves the program ID to label mapping.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |

### Return type

[**JupiterAPIResponse_Record_string.string__**](../Models/JupiterAPIResponse_Record_string.string__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="jUPITERGetQuote"></a>
# **jUPITERGetQuote**
> JupiterAPIResponse_JupiterExecuteFunctionResult_ jUPITERGetQuote(accountName, Authorization, body)



    Retrieves the tokens available on the Jupiter platform.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to perform the swap for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **body** | **Pick_JupiterInputBody.Exclude_keyofJupiterInputBody.accountName__**| - The input body for the Jupiter swap operation, excluding the account name. | |

### Return type

[**JupiterAPIResponse_JupiterExecuteFunctionResult_**](../Models/JupiterAPIResponse_JupiterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="jUPITERGetSwapInstructions"></a>
# **jUPITERGetSwapInstructions**
> JupiterAPIResponse_JupiterExecuteFunctionResult_ jUPITERGetSwapInstructions(accountName, Authorization, body)



    Retrieves swap instructions for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account for which to retrieve swap instructions. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **body** | **Pick_JupiterInputBody.Exclude_keyofJupiterInputBody.accountName__**| - The body of the request, omitting the account name. | |

### Return type

[**JupiterAPIResponse_JupiterExecuteFunctionResult_**](../Models/JupiterAPIResponse_JupiterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="jUPITERGetTokens"></a>
# **jUPITERGetTokens**
> JupiterAPIResponse_string-Array_ jUPITERGetTokens(Authorization)



    Retrieves the tokens available on the Jupiter platform.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |

### Return type

[**JupiterAPIResponse_string-Array_**](../Models/JupiterAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="jUPITERSwap"></a>
# **jUPITERSwap**
> JupiterAPIResponse_JupiterExecuteFunctionResult_ jUPITERSwap(accountName, Authorization, body)



    Handles the swap operation for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to perform the swap for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **body** | **Pick_JupiterInputBody.Exclude_keyofJupiterInputBody.accountName__**| - The input body for the Jupiter swap operation, excluding the account name. | |

### Return type

[**JupiterAPIResponse_JupiterExecuteFunctionResult_**](../Models/JupiterAPIResponse_JupiterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

