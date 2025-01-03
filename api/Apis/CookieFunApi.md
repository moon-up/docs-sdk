# CookieFunApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**cookieFunGetKOLCommunity**](CookieFunApi.md#cookieFunGetKOLCommunity) | **GET** /cookiefun/kols/{username}/community |  |
| [**cookieFunGetKOLList**](CookieFunApi.md#cookieFunGetKOLList) | **GET** /cookiefun/kols |  |
| [**cookieFunGetKOLNetwork**](CookieFunApi.md#cookieFunGetKOLNetwork) | **GET** /cookiefun/kols/{username}/network |  |
| [**cookieFunGetPredictiveMetrics**](CookieFunApi.md#cookieFunGetPredictiveMetrics) | **GET** /cookiefun/predictive/{metric} |  |
| [**cookieFunGetTokenAnalytics**](CookieFunApi.md#cookieFunGetTokenAnalytics) | **GET** /cookiefun/tokens/{tokenId}/analytics |  |
| [**cookieFunGetTrendingNarratives**](CookieFunApi.md#cookieFunGetTrendingNarratives) | **GET** /cookiefun/narratives/trending |  |
| [**cookieFunGetTrendingTokens**](CookieFunApi.md#cookieFunGetTrendingTokens) | **GET** /cookiefun/tokens/trending |  |
| [**cookieFunGetTrendingTweets**](CookieFunApi.md#cookieFunGetTrendingTweets) | **GET** /cookiefun/tweets/trending |  |


<a name="cookieFunGetKOLCommunity"></a>
# **cookieFunGetKOLCommunity**
> CommunityMetricsAPIResponse cookieFunGetKOLCommunity(username, Authorization, period, metrics, filter)



    Retrieves community metrics for a specific KOL.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **username** | **String**| - The username of the KOL. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **period** | **String**| - The time period for the metrics. | [default to null] |
| **metrics** | [**List**](../Models/String.md)| - The specific metrics to retrieve. | [default to null] |
| **filter** | **String**| - The filter criteria for the community (optional). | [optional] [default to null] |

### Return type

[**CommunityMetricsAPIResponse**](../Models/CommunityMetricsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cookieFunGetKOLList"></a>
# **cookieFunGetKOLList**
> KOLListAPIResponse cookieFunGetKOLList(Authorization, limit, sort, filter, page)



    Retrieves a list of key opinion leaders (KOLs).

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **limit** | **Double**| - The number of results to return (optional). | [optional] [default to null] |
| **sort** | **String**| - The sorting criteria (optional). | [optional] [default to null] |
| **filter** | **String**| - The filter criteria (optional). | [optional] [default to null] |
| **page** | **Double**| - The page number for pagination (optional). | [optional] [default to null] |

### Return type

[**KOLListAPIResponse**](../Models/KOLListAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cookieFunGetKOLNetwork"></a>
# **cookieFunGetKOLNetwork**
> KOLNetworkAPIResponse cookieFunGetKOLNetwork(username, Authorization, depth, filter, metric)



    Retrieves the network information for a specific KOL.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **username** | **String**| - The username of the KOL. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **depth** | **Double**| - The depth of the network to retrieve (optional). | [optional] [default to null] |
| **filter** | **String**| - The filter criteria for the network (optional). | [optional] [default to null] |
| **metric** | **String**| - The metric to analyze the network (optional). | [optional] [default to null] |

### Return type

[**KOLNetworkAPIResponse**](../Models/KOLNetworkAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cookieFunGetPredictiveMetrics"></a>
# **cookieFunGetPredictiveMetrics**
> PredictiveMetricsAPIResponse cookieFunGetPredictiveMetrics(metric, Authorization, target, horizon, confidence)



    Retrieves predictive metrics.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **metric** | **String**| - The specific metric to predict. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **target** | **String**| - The target for the prediction. | [default to null] |
| **horizon** | **String**| - The time horizon for the prediction. | [default to null] |
| **confidence** | **Double**| - The minimum confidence level for the prediction (optional). | [optional] [default to null] |

### Return type

[**PredictiveMetricsAPIResponse**](../Models/PredictiveMetricsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cookieFunGetTokenAnalytics"></a>
# **cookieFunGetTokenAnalytics**
> TokenAnalyticsAPIResponse cookieFunGetTokenAnalytics(tokenId, Authorization, metrics, period, interval)



    Retrieves token analytics.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tokenId** | **String**| - The ID of the token. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **metrics** | [**List**](../Models/String.md)| - The metrics to retrieve for the token. | [default to null] |
| **period** | **String**| - The time period for the analytics. | [default to null] |
| **interval** | **String**| - The interval for the data points. | [default to null] |

### Return type

[**TokenAnalyticsAPIResponse**](../Models/TokenAnalyticsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cookieFunGetTrendingNarratives"></a>
# **cookieFunGetTrendingNarratives**
> NarrativeTrendsAPIResponse cookieFunGetTrendingNarratives(Authorization, timeframe, threshold, category)



    Retrieves trending narratives.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **timeframe** | **String**| - The timeframe for the trending narratives. | [default to null] |
| **threshold** | **Double**| - The minimum threshold for trend strength (optional). | [optional] [default to null] |
| **category** | **String**| - The category of narratives to retrieve (optional). | [optional] [default to null] |

### Return type

[**NarrativeTrendsAPIResponse**](../Models/NarrativeTrendsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cookieFunGetTrendingTokens"></a>
# **cookieFunGetTrendingTokens**
> TrendingTokensAPIResponse cookieFunGetTrendingTokens(Authorization, metrics, sort, filter, limit)



    Retrieves trending tokens.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **metrics** | [**List**](../Models/String.md)| - The metrics to include for each token. | [default to null] |
| **sort** | **String**| - The sorting criteria for the trending tokens. | [default to null] |
| **filter** | **String**| - The filter criteria for the trending tokens (optional). | [optional] [default to null] |
| **limit** | **Double**| - The number of trending tokens to retrieve (optional). | [optional] [default to null] |

### Return type

[**TrendingTokensAPIResponse**](../Models/TrendingTokensAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cookieFunGetTrendingTweets"></a>
# **cookieFunGetTrendingTweets**
> TrendingTweetsAPIResponse cookieFunGetTrendingTweets(Authorization, metrics, period, limit, category)



    Retrieves trending tweets.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **metrics** | [**List**](../Models/String.md)| - The metrics to include for each tweet. | [default to null] |
| **period** | **String**| - The time period for the trending tweets. | [default to null] |
| **limit** | **Double**| - The number of trending tweets to retrieve (optional). | [optional] [default to null] |
| **category** | **String**| - The category of tweets to retrieve (optional). | [optional] [default to null] |

### Return type

[**TrendingTweetsAPIResponse**](../Models/TrendingTweetsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

