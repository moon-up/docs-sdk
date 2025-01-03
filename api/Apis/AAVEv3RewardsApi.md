# AAVEv3RewardsApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**aAVEv3RewardsClaimAllRewards**](AAVEv3RewardsApi.md#aAVEv3RewardsClaimAllRewards) | **POST** /aave/v3/rewards/{address}/claimAllRewards |  |
| [**aAVEv3RewardsClaimAllRewardsOnBehalf**](AAVEv3RewardsApi.md#aAVEv3RewardsClaimAllRewardsOnBehalf) | **POST** /aave/v3/rewards/{address}/claimAllRewardsOnBehalf |  |
| [**aAVEv3RewardsClaimAllRewardsToSelf**](AAVEv3RewardsApi.md#aAVEv3RewardsClaimAllRewardsToSelf) | **POST** /aave/v3/rewards/{address}/claimAllRewardsToSelf |  |
| [**aAVEv3RewardsClaimRewards**](AAVEv3RewardsApi.md#aAVEv3RewardsClaimRewards) | **POST** /aave/v3/rewards/{address}/claimRewards |  |
| [**aAVEv3RewardsClaimRewardsOnBehalf**](AAVEv3RewardsApi.md#aAVEv3RewardsClaimRewardsOnBehalf) | **POST** /aave/v3/rewards/{address}/claimRewardsOnBehalf |  |
| [**aAVEv3RewardsClaimRewardsToSelf**](AAVEv3RewardsApi.md#aAVEv3RewardsClaimRewardsToSelf) | **POST** /aave/v3/rewards/{address}/claimRewardsToSelf |  |
| [**aAVEv3RewardsGetRewardsByAsset**](AAVEv3RewardsApi.md#aAVEv3RewardsGetRewardsByAsset) | **GET** /aave/v3/rewards/{account}/rewardsByAsset |  |
| [**aAVEv3RewardsGetRewardsData**](AAVEv3RewardsApi.md#aAVEv3RewardsGetRewardsData) | **GET** /aave/v3/rewards/{account}/rewardsData |  |
| [**aAVEv3RewardsGetUserRewards**](AAVEv3RewardsApi.md#aAVEv3RewardsGetUserRewards) | **GET** /aave/v3/rewards/{account}/userRewards |  |


<a name="aAVEv3RewardsClaimAllRewards"></a>
# **aAVEv3RewardsClaimAllRewards**
> AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_ aAVEv3RewardsClaimAllRewards(address, Authorization, AAVEv3RewardsInputBody)



    Claims all available rewards for the specified assets

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - Address claiming the rewards | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **AAVEv3RewardsInputBody** | [**AAVEv3RewardsInputBody**](../Models/AAVEv3RewardsInputBody.md)| - Input parameters for claiming all rewards | |

### Return type

[**AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_**](../Models/AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aAVEv3RewardsClaimAllRewardsOnBehalf"></a>
# **aAVEv3RewardsClaimAllRewardsOnBehalf**
> AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_ aAVEv3RewardsClaimAllRewardsOnBehalf(address, Authorization, AAVEv3RewardsInputBody)



    Claims all rewards on behalf of another address

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - Address claiming the rewards | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **AAVEv3RewardsInputBody** | [**AAVEv3RewardsInputBody**](../Models/AAVEv3RewardsInputBody.md)| - Input parameters for claiming all rewards | |

### Return type

[**AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_**](../Models/AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aAVEv3RewardsClaimAllRewardsToSelf"></a>
# **aAVEv3RewardsClaimAllRewardsToSelf**
> AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_ aAVEv3RewardsClaimAllRewardsToSelf(address, Authorization, AAVEv3RewardsInputBody)



    Claims all rewards to the calling address

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - Address claiming the rewards | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **AAVEv3RewardsInputBody** | [**AAVEv3RewardsInputBody**](../Models/AAVEv3RewardsInputBody.md)| - Input parameters for claiming all rewards | |

### Return type

[**AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_**](../Models/AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aAVEv3RewardsClaimRewards"></a>
# **aAVEv3RewardsClaimRewards**
> AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_ aAVEv3RewardsClaimRewards(address, Authorization, AAVEv3RewardsInputBody)



    Claims rewards for the specified assets and rewards

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - Address claiming the rewards | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **AAVEv3RewardsInputBody** | [**AAVEv3RewardsInputBody**](../Models/AAVEv3RewardsInputBody.md)| - Input parameters for claiming rewards | |

### Return type

[**AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_**](../Models/AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aAVEv3RewardsClaimRewardsOnBehalf"></a>
# **aAVEv3RewardsClaimRewardsOnBehalf**
> AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_ aAVEv3RewardsClaimRewardsOnBehalf(address, Authorization, AAVEv3RewardsInputBody)



    Claims rewards on behalf of another address

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - Address claiming the rewards | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **AAVEv3RewardsInputBody** | [**AAVEv3RewardsInputBody**](../Models/AAVEv3RewardsInputBody.md)| - Input parameters for claiming rewards | |

### Return type

[**AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_**](../Models/AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aAVEv3RewardsClaimRewardsToSelf"></a>
# **aAVEv3RewardsClaimRewardsToSelf**
> AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_ aAVEv3RewardsClaimRewardsToSelf(address, Authorization, AAVEv3RewardsInputBody)



    Claims rewards to the calling address

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - Address claiming the rewards | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **AAVEv3RewardsInputBody** | [**AAVEv3RewardsInputBody**](../Models/AAVEv3RewardsInputBody.md)| - Input parameters for claiming rewards | |

### Return type

[**AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_**](../Models/AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aAVEv3RewardsGetRewardsByAsset"></a>
# **aAVEv3RewardsGetRewardsByAsset**
> AAVEv3RewardsAPIResponse_string-Array_ aAVEv3RewardsGetRewardsByAsset(account, Authorization, chainId, address, asset)



    Retrieves all rewards for a specific asset

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - Account identifier for the request | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **chainId** | **String**| - Chain ID to target | [default to null] |
| **address** | **String**| - Contract address | [default to null] |
| **asset** | **String**| - Asset address to query rewards for | [default to null] |

### Return type

[**AAVEv3RewardsAPIResponse_string-Array_**](../Models/AAVEv3RewardsAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aAVEv3RewardsGetRewardsData"></a>
# **aAVEv3RewardsGetRewardsData**
> AAVEv3RewardsAPIResponse_string-Array_ aAVEv3RewardsGetRewardsData(account, Authorization, chainId, address, asset, reward)



    Retrieves rewards configuration data for an asset

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - Account identifier for the request | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **chainId** | **String**| - Chain ID to target | [default to null] |
| **address** | **String**| - Contract address | [default to null] |
| **asset** | **String**| - Asset address to get rewards data for | [default to null] |
| **reward** | **String**| - Reward token address | [default to null] |

### Return type

[**AAVEv3RewardsAPIResponse_string-Array_**](../Models/AAVEv3RewardsAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aAVEv3RewardsGetUserRewards"></a>
# **aAVEv3RewardsGetUserRewards**
> AAVEv3RewardsAPIResponse_string_ aAVEv3RewardsGetUserRewards(account, Authorization, chainId, address, assets, user, reward)



    Gets reward data for a specific user

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - Account identifier for the request | [default to null] |
| **Authorization** | **String**| - Authorization token from the request header | [default to null] |
| **chainId** | **String**| - Chain ID to target | [default to null] |
| **address** | **String**| - Contract address | [default to null] |
| **assets** | [**List**](../Models/String.md)| - Array of asset addresses to check rewards for | [default to null] |
| **user** | **String**| - User address to check rewards for | [default to null] |
| **reward** | **String**| - Reward token address | [default to null] |

### Return type

[**AAVEv3RewardsAPIResponse_string_**](../Models/AAVEv3RewardsAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

