# AAVEV3UIIncentiveDataProviderApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**aAVEv3IncentiveDataProviderGetFullReservesData**](AAVEV3UIIncentiveDataProviderApi.md#aAVEv3IncentiveDataProviderGetFullReservesData) | **GET** /aave/v3/incentives/fullReservesIncentiveData |  |
| [**aAVEv3IncentiveDataProviderGetReservesData**](AAVEV3UIIncentiveDataProviderApi.md#aAVEv3IncentiveDataProviderGetReservesData) | **GET** /aave/v3/incentives/reservesIncentivesData |  |
| [**aAVEv3IncentiveDataProviderGetUserReservesData**](AAVEV3UIIncentiveDataProviderApi.md#aAVEv3IncentiveDataProviderGetUserReservesData) | **GET** /aave/v3/incentives/userReservesIncentivesData |  |


<a name="aAVEv3IncentiveDataProviderGetFullReservesData"></a>
# **aAVEv3IncentiveDataProviderGetFullReservesData**
> AAVEv3UiIncentiveDataProviderAPIResponse_FullReservesIncentiveData_ aAVEv3IncentiveDataProviderGetFullReservesData(Authorization, contract\_address, chain\_id, provider, user)



    Retrieves full incentive data for all reserves and user positions

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - Authorization token from request header | [default to null] |
| **contract\_address** | **String**| - Address of the incentive data provider contract | [default to null] |
| **chain\_id** | **String**| - Chain ID to target | [default to null] |
| **provider** | **String**| - Address of the pool address provider | [default to null] |
| **user** | **String**| - Address of the user to get incentive data for | [default to null] |

### Return type

[**AAVEv3UiIncentiveDataProviderAPIResponse_FullReservesIncentiveData_**](../Models/AAVEv3UiIncentiveDataProviderAPIResponse_FullReservesIncentiveData_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aAVEv3IncentiveDataProviderGetReservesData"></a>
# **aAVEv3IncentiveDataProviderGetReservesData**
> AAVEv3UiIncentiveDataProviderAPIResponse_AggregatedReserveIncentiveData-Array_ aAVEv3IncentiveDataProviderGetReservesData(Authorization, contract\_address, chain\_id, provider)



    Retrieves incentive data for all reserves in the pool

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - Authorization token from request header | [default to null] |
| **contract\_address** | **String**| - Address of the incentive data provider contract | [default to null] |
| **chain\_id** | **String**| - Chain ID to target | [default to null] |
| **provider** | **String**| - Address of the pool address provider | [default to null] |

### Return type

[**AAVEv3UiIncentiveDataProviderAPIResponse_AggregatedReserveIncentiveData-Array_**](../Models/AAVEv3UiIncentiveDataProviderAPIResponse_AggregatedReserveIncentiveData-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aAVEv3IncentiveDataProviderGetUserReservesData"></a>
# **aAVEv3IncentiveDataProviderGetUserReservesData**
> AAVEv3UiIncentiveDataProviderAPIResponse_UserReserveIncentiveData-Array_ aAVEv3IncentiveDataProviderGetUserReservesData(Authorization, contract\_address, chain\_id, provider, user)



    Retrieves incentive data for a user&#39;s positions in all reserves

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - Authorization token from request header | [default to null] |
| **contract\_address** | **String**| - Address of the incentive data provider contract | [default to null] |
| **chain\_id** | **String**| - Chain ID to target | [default to null] |
| **provider** | **String**| - Address of the pool address provider | [default to null] |
| **user** | **String**| - Address of the user to get incentive data for | [default to null] |

### Return type

[**AAVEv3UiIncentiveDataProviderAPIResponse_UserReserveIncentiveData-Array_**](../Models/AAVEv3UiIncentiveDataProviderAPIResponse_UserReserveIncentiveData-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

