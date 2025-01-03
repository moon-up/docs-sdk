# TradingBotApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**activateBot**](TradingBotApi.md#activateBot) | **GET** /tradingBot/{botId}/activate |  |
| [**conversation**](TradingBotApi.md#conversation) | **GET** /tradingBot/{botId}/twitter/conversation/{tweetId} |  |
| [**createTweet**](TradingBotApi.md#createTweet) | **POST** /tradingBot/{botId}/twitter/createTweet |  |
| [**deactivateBot**](TradingBotApi.md#deactivateBot) | **GET** /tradingBot/{botId}/deactivate |  |
| [**followingTimeline**](TradingBotApi.md#followingTimeline) | **GET** /tradingBot/{botId}/twitter/followingTimeline |  |
| [**getBotLastRunResults**](TradingBotApi.md#getBotLastRunResults) | **GET** /tradingBot/{botId}/lastRunResults |  |
| [**getBotStatus**](TradingBotApi.md#getBotStatus) | **GET** /tradingBot/{botId}/status |  |
| [**getConfigs**](TradingBotApi.md#getConfigs) | **GET** /tradingBot/configs |  |
| [**restartBot**](TradingBotApi.md#restartBot) | **GET** /tradingBot/{botId}/restart |  |
| [**startBot**](TradingBotApi.md#startBot) | **GET** /tradingBot/{botId}/start |  |
| [**stopBot**](TradingBotApi.md#stopBot) | **GET** /tradingBot/{botId}/stop |  |
| [**triggerBot**](TradingBotApi.md#triggerBot) | **GET** /tradingBot/{botId}/trigger |  |
| [**tweetHistory**](TradingBotApi.md#tweetHistory) | **GET** /tradingBot/{botId}/twitter/tweet/history |  |
| [**tweetReplyTest**](TradingBotApi.md#tweetReplyTest) | **POST** /tradingBot/{botId}/tweetReplyTest |  |
| [**updatePersonality**](TradingBotApi.md#updatePersonality) | **PATCH** /tradingBot/{botId}/personality |  |


<a name="activateBot"></a>
# **activateBot**
> String activateBot(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="conversation"></a>
# **conversation**
> BotConfigType conversation(botId, tweetId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |
| **tweetId** | **String**|  | [default to null] |

### Return type

[**BotConfigType**](../Models/BotConfigType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="createTweet"></a>
# **createTweet**
> BotConfigType createTweet(botId, GeneratedTweet)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |
| **GeneratedTweet** | [**GeneratedTweet**](../Models/GeneratedTweet.md)|  | |

### Return type

[**BotConfigType**](../Models/BotConfigType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="deactivateBot"></a>
# **deactivateBot**
> String deactivateBot(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="followingTimeline"></a>
# **followingTimeline**
> BotConfigType followingTimeline(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

[**BotConfigType**](../Models/BotConfigType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBotLastRunResults"></a>
# **getBotLastRunResults**
> oas_any_type_not_mapped getBotLastRunResults(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getBotStatus"></a>
# **getBotStatus**
> String getBotStatus(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getConfigs"></a>
# **getConfigs**
> List getConfigs()



### Parameters
This endpoint does not need any parameter.

### Return type

[**List**](../Models/BotConfigType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="restartBot"></a>
# **restartBot**
> String restartBot(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="startBot"></a>
# **startBot**
> String startBot(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="stopBot"></a>
# **stopBot**
> String stopBot(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="triggerBot"></a>
# **triggerBot**
> String triggerBot(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="tweetHistory"></a>
# **tweetHistory**
> BotConfigType tweetHistory(botId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |

### Return type

[**BotConfigType**](../Models/BotConfigType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="tweetReplyTest"></a>
# **tweetReplyTest**
> String tweetReplyTest(botId, body)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |
| **body** | **String**|  | |

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="updatePersonality"></a>
# **updatePersonality**
> BotConfigType updatePersonality(botId, PersonalityInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **botId** | **String**|  | [default to null] |
| **PersonalityInput** | [**PersonalityInput**](../Models/PersonalityInput.md)|  | |

### Return type

[**BotConfigType**](../Models/BotConfigType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

