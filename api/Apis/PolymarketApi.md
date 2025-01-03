# PolymarketApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**approveForPolymarket**](PolymarketApi.md#approveForPolymarket) | **POST** /polymarket/{account}/approveForPolymarket |  |
| [**cancelMarketOrders**](PolymarketApi.md#cancelMarketOrders) | **POST** /polymarket/{account}/cancelMarketOrders |  |
| [**cancelOrder**](PolymarketApi.md#cancelOrder) | **POST** /polymarket/{account}/cancelOrder |  |
| [**cancelOrders**](PolymarketApi.md#cancelOrders) | **POST** /polymarket/{account}/cancelOrders |  |
| [**createMarketBuyOrder**](PolymarketApi.md#createMarketBuyOrder) | **POST** /polymarket/{account}/createMarketBuyOrder |  |
| [**createOrder**](PolymarketApi.md#createOrder) | **POST** /polymarket/{account}/createOrder |  |
| [**dropNotifications**](PolymarketApi.md#dropNotifications) | **POST** /polymarket/{account}/dropNotifications |  |
| [**getBalanceAllowance**](PolymarketApi.md#getBalanceAllowance) | **GET** /polymarket/{account}/balanceAllowance |  |
| [**getMarket**](PolymarketApi.md#getMarket) | **GET** /polymarket/{account}/market/{conditionID} |  |
| [**getMarketTradeEvents**](PolymarketApi.md#getMarketTradeEvents) | **GET** /polymarket/{account}/marketTradeEvents/{conditionID} |  |
| [**getMarkets**](PolymarketApi.md#getMarkets) | **GET** /polymarket/{account}/markets |  |
| [**getNotifications**](PolymarketApi.md#getNotifications) | **GET** /polymarket/{account}/notifications |  |
| [**getOpenOrders**](PolymarketApi.md#getOpenOrders) | **GET** /polymarket/{account}/openOrders |  |
| [**getOrder**](PolymarketApi.md#getOrder) | **GET** /polymarket/{account}/order/{orderID} |  |
| [**getOrderBook**](PolymarketApi.md#getOrderBook) | **GET** /polymarket/{account}/orderBook |  |
| [**getPricesHistory**](PolymarketApi.md#getPricesHistory) | **GET** /polymarket/{account}/pricesHistory |  |
| [**getTrades**](PolymarketApi.md#getTrades) | **GET** /polymarket/{account}/trades |  |
| [**postOrder**](PolymarketApi.md#postOrder) | **POST** /polymarket/{account}/postOrder |  |
| [**updateBalanceAllowance**](PolymarketApi.md#updateBalanceAllowance) | **POST** /polymarket/{account}/updateBalanceAllowance |  |


<a name="approveForPolymarket"></a>
# **approveForPolymarket**
> PolymarketAPIResponse_any_ approveForPolymarket(account, Authorization, ApproveForPolymarketBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **ApproveForPolymarketBody** | [**ApproveForPolymarketBody**](../Models/ApproveForPolymarketBody.md)|  | |

### Return type

[**PolymarketAPIResponse_any_**](../Models/PolymarketAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="cancelMarketOrders"></a>
# **cancelMarketOrders**
> PolymarketAPIResponse_CancelMarketOrdersResponse_ cancelMarketOrders(account, Authorization, CancelMarketOrdersBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **CancelMarketOrdersBody** | [**CancelMarketOrdersBody**](../Models/CancelMarketOrdersBody.md)|  | |

### Return type

[**PolymarketAPIResponse_CancelMarketOrdersResponse_**](../Models/PolymarketAPIResponse_CancelMarketOrdersResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="cancelOrder"></a>
# **cancelOrder**
> PolymarketAPIResponse_CancelOrderResponse_ cancelOrder(account, Authorization, CancelOrderBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **CancelOrderBody** | [**CancelOrderBody**](../Models/CancelOrderBody.md)|  | |

### Return type

[**PolymarketAPIResponse_CancelOrderResponse_**](../Models/PolymarketAPIResponse_CancelOrderResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="cancelOrders"></a>
# **cancelOrders**
> PolymarketAPIResponse_CancelOrdersResponse_ cancelOrders(account, Authorization, CancelOrdersBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **CancelOrdersBody** | [**CancelOrdersBody**](../Models/CancelOrdersBody.md)|  | |

### Return type

[**PolymarketAPIResponse_CancelOrdersResponse_**](../Models/PolymarketAPIResponse_CancelOrdersResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createMarketBuyOrder"></a>
# **createMarketBuyOrder**
> PolymarketAPIResponse_CreateMarketBuyOrderResponse_ createMarketBuyOrder(account, Authorization, CreateMarketBuyOrderBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **CreateMarketBuyOrderBody** | [**CreateMarketBuyOrderBody**](../Models/CreateMarketBuyOrderBody.md)|  | |

### Return type

[**PolymarketAPIResponse_CreateMarketBuyOrderResponse_**](../Models/PolymarketAPIResponse_CreateMarketBuyOrderResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createOrder"></a>
# **createOrder**
> PolymarketAPIResponse_CreateOrderResponse_ createOrder(account, Authorization, CreateOrderBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **CreateOrderBody** | [**CreateOrderBody**](../Models/CreateOrderBody.md)|  | |

### Return type

[**PolymarketAPIResponse_CreateOrderResponse_**](../Models/PolymarketAPIResponse_CreateOrderResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="dropNotifications"></a>
# **dropNotifications**
> PolymarketAPIResponse_DropNotificationsResponse_ dropNotifications(account, Authorization, DropNotificationsBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **DropNotificationsBody** | [**DropNotificationsBody**](../Models/DropNotificationsBody.md)|  | |

### Return type

[**PolymarketAPIResponse_DropNotificationsResponse_**](../Models/PolymarketAPIResponse_DropNotificationsResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getBalanceAllowance"></a>
# **getBalanceAllowance**
> PolymarketAPIResponse_BalanceAllowanceResponse_ getBalanceAllowance(account, Authorization, chainId, asset\_type, token\_id)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **asset\_type** | **String**|  | [default to null] |
| **token\_id** | **String**|  | [optional] [default to null] |

### Return type

[**PolymarketAPIResponse_BalanceAllowanceResponse_**](../Models/PolymarketAPIResponse_BalanceAllowanceResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getMarket"></a>
# **getMarket**
> PolymarketAPIResponse_any_ getMarket(account, conditionID, Authorization, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **conditionID** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**PolymarketAPIResponse_any_**](../Models/PolymarketAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getMarketTradeEvents"></a>
# **getMarketTradeEvents**
> PolymarketAPIResponse_MarketTradeEvent-Array_ getMarketTradeEvents(account, conditionID, Authorization, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **conditionID** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**PolymarketAPIResponse_MarketTradeEvent-Array_**](../Models/PolymarketAPIResponse_MarketTradeEvent-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getMarkets"></a>
# **getMarkets**
> PolymarketAPIResponse_PaginationPayload_ getMarkets(account, Authorization, chainId, nextCursor)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **nextCursor** | **String**|  | [optional] [default to null] |

### Return type

[**PolymarketAPIResponse_PaginationPayload_**](../Models/PolymarketAPIResponse_PaginationPayload_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getNotifications"></a>
# **getNotifications**
> PolymarketAPIResponse_Notification-Array_ getNotifications(account, Authorization, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**PolymarketAPIResponse_Notification-Array_**](../Models/PolymarketAPIResponse_Notification-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getOpenOrders"></a>
# **getOpenOrders**
> PolymarketAPIResponse_OpenOrdersResponse_ getOpenOrders(account, Authorization, chainId, marketHash, outcomeId, assetId, nextCursor)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **marketHash** | **String**|  | [optional] [default to null] |
| **outcomeId** | **String**|  | [optional] [default to null] |
| **assetId** | **String**|  | [optional] [default to null] |
| **nextCursor** | **String**|  | [optional] [default to null] |

### Return type

[**PolymarketAPIResponse_OpenOrdersResponse_**](../Models/PolymarketAPIResponse_OpenOrdersResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getOrder"></a>
# **getOrder**
> PolymarketAPIResponse_OpenOrder_ getOrder(account, orderID, Authorization, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **orderID** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**PolymarketAPIResponse_OpenOrder_**](../Models/PolymarketAPIResponse_OpenOrder_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getOrderBook"></a>
# **getOrderBook**
> PolymarketAPIResponse_OrderBookSummary_ getOrderBook(account, Authorization, chainId, tokenID)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **tokenID** | **String**|  | [default to null] |

### Return type

[**PolymarketAPIResponse_OrderBookSummary_**](../Models/PolymarketAPIResponse_OrderBookSummary_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPricesHistory"></a>
# **getPricesHistory**
> PolymarketAPIResponse_MarketPrice-Array_ getPricesHistory(account, Authorization, chainId, market, startTs, endTs, fidelity, interval)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **market** | **String**|  | [optional] [default to null] |
| **startTs** | **Double**|  | [optional] [default to null] |
| **endTs** | **Double**|  | [optional] [default to null] |
| **fidelity** | **Double**|  | [optional] [default to null] |
| **interval** | **String**|  | [optional] [default to null] |

### Return type

[**PolymarketAPIResponse_MarketPrice-Array_**](../Models/PolymarketAPIResponse_MarketPrice-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTrades"></a>
# **getTrades**
> PolymarketAPIResponse_Trade-Array_ getTrades(account, Authorization, chainId, id, maker\_address, market, asset\_id, before, after, nextCursor)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **id** | **String**|  | [optional] [default to null] |
| **maker\_address** | **String**|  | [optional] [default to null] |
| **market** | **String**|  | [optional] [default to null] |
| **asset\_id** | **String**|  | [optional] [default to null] |
| **before** | **String**|  | [optional] [default to null] |
| **after** | **String**|  | [optional] [default to null] |
| **nextCursor** | **String**|  | [optional] [default to null] |

### Return type

[**PolymarketAPIResponse_Trade-Array_**](../Models/PolymarketAPIResponse_Trade-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="postOrder"></a>
# **postOrder**
> PolymarketAPIResponse_PostOrderResponse_ postOrder(account, Authorization, PostOrderBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **PostOrderBody** | [**PostOrderBody**](../Models/PostOrderBody.md)|  | |

### Return type

[**PolymarketAPIResponse_PostOrderResponse_**](../Models/PolymarketAPIResponse_PostOrderResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="updateBalanceAllowance"></a>
# **updateBalanceAllowance**
> PolymarketAPIResponse_UpdateBalanceAllowanceResponse_ updateBalanceAllowance(account, Authorization, UpdateBalanceAllowanceBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UpdateBalanceAllowanceBody** | [**UpdateBalanceAllowanceBody**](../Models/UpdateBalanceAllowanceBody.md)|  | |

### Return type

[**PolymarketAPIResponse_UpdateBalanceAllowanceResponse_**](../Models/PolymarketAPIResponse_UpdateBalanceAllowanceResponse_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

