# LendingPoolApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**lendingPoolBorrow**](LendingPoolApi.md#lendingPoolBorrow) | **POST** /lending-pool/{accountName}/borrow |  |
| [**lendingPoolDeposit**](LendingPoolApi.md#lendingPoolDeposit) | **POST** /lending-pool/{accountName}/deposit |  |
| [**lendingPoolFlashLoan**](LendingPoolApi.md#lendingPoolFlashLoan) | **POST** /lending-pool/{accountName}/flash-loan |  |
| [**lendingPoolGetAddressesProvider**](LendingPoolApi.md#lendingPoolGetAddressesProvider) | **GET** /lending-pool/addresses-provider |  |
| [**lendingPoolGetFlashLoanPremiumTotal**](LendingPoolApi.md#lendingPoolGetFlashLoanPremiumTotal) | **GET** /lending-pool/flash-loan-premium |  |
| [**lendingPoolGetLendingPoolRevision**](LendingPoolApi.md#lendingPoolGetLendingPoolRevision) | **GET** /lending-pool/revision |  |
| [**lendingPoolGetMaxNumberReserves**](LendingPoolApi.md#lendingPoolGetMaxNumberReserves) | **GET** /lending-pool/max-reserves |  |
| [**lendingPoolGetMaxStableRateBorrowSizePercent**](LendingPoolApi.md#lendingPoolGetMaxStableRateBorrowSizePercent) | **GET** /lending-pool/max-stable-rate-borrow-size-percent |  |
| [**lendingPoolGetReserveData**](LendingPoolApi.md#lendingPoolGetReserveData) | **GET** /lending-pool/reserve-data |  |
| [**lendingPoolGetReservesList**](LendingPoolApi.md#lendingPoolGetReservesList) | **GET** /lending-pool/reserves-list |  |
| [**lendingPoolGetUserAccountData**](LendingPoolApi.md#lendingPoolGetUserAccountData) | **GET** /lending-pool/user-account-data |  |
| [**lendingPoolIsPaused**](LendingPoolApi.md#lendingPoolIsPaused) | **GET** /lending-pool/paused |  |
| [**lendingPoolLiquidationCall**](LendingPoolApi.md#lendingPoolLiquidationCall) | **POST** /lending-pool/{accountName}/liquidation-call |  |
| [**lendingPoolRepay**](LendingPoolApi.md#lendingPoolRepay) | **POST** /lending-pool/{accountName}/repay |  |
| [**lendingPoolSetUserUseReserveAsCollateral**](LendingPoolApi.md#lendingPoolSetUserUseReserveAsCollateral) | **POST** /lending-pool/{accountName}/set-user-use-reserve-as-collateral |  |
| [**lendingPoolSwapBorrowRateMode**](LendingPoolApi.md#lendingPoolSwapBorrowRateMode) | **POST** /lending-pool/{accountName}/swap-borrow-rate-mode |  |


<a name="lendingPoolBorrow"></a>
# **lendingPoolBorrow**
> LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_ lendingPoolBorrow(accountName, Authorization, LendingPoolInputBody)



    Handles the borrowing process from the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account requesting the borrow. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **LendingPoolInputBody** | [**LendingPoolInputBody**](../Models/LendingPoolInputBody.md)| - The body of the request containing lending pool input details. | |

### Return type

[**LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_**](../Models/LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="lendingPoolDeposit"></a>
# **lendingPoolDeposit**
> LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_ lendingPoolDeposit(accountName, Authorization, LendingPoolInputBody)



    Handles the deposit operation for a lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account making the deposit. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **LendingPoolInputBody** | [**LendingPoolInputBody**](../Models/LendingPoolInputBody.md)| - The body of the request containing deposit details. | |

### Return type

[**LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_**](../Models/LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="lendingPoolFlashLoan"></a>
# **lendingPoolFlashLoan**
> LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_ lendingPoolFlashLoan(accountName, Authorization, LendingPoolInputBody)



    Executes a flash loan operation on the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account requesting the flash loan. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **LendingPoolInputBody** | [**LendingPoolInputBody**](../Models/LendingPoolInputBody.md)| - The input body containing details for the flash loan. | |

### Return type

[**LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_**](../Models/LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="lendingPoolGetAddressesProvider"></a>
# **lendingPoolGetAddressesProvider**
> LendingPoolAPIResponse_string_ lendingPoolGetAddressesProvider(Authorization, address, chainId)



    Retrieves the addresses provider from the lending pool instance.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **address** | **String**| - The address query parameter. | [default to null] |
| **chainId** | **String**| - The chain ID query parameter. | [default to null] |

### Return type

[**LendingPoolAPIResponse_string_**](../Models/LendingPoolAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolGetFlashLoanPremiumTotal"></a>
# **lendingPoolGetFlashLoanPremiumTotal**
> LendingPoolAPIResponse_number_ lendingPoolGetFlashLoanPremiumTotal(Authorization, address, chainId)



    Retrieves the total flash loan premium for a given lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **address** | **String**| - The address of the lending pool. | [default to null] |
| **chainId** | **String**| - The chain ID of the blockchain network. | [default to null] |

### Return type

[**LendingPoolAPIResponse_number_**](../Models/LendingPoolAPIResponse_number_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolGetLendingPoolRevision"></a>
# **lendingPoolGetLendingPoolRevision**
> LendingPoolAPIResponse_number_ lendingPoolGetLendingPoolRevision(Authorization, address, chainId)



    Retrieves the revision number of a lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **address** | **String**| - The address of the lending pool. | [default to null] |
| **chainId** | **String**| - The chain ID where the lending pool is located. | [default to null] |

### Return type

[**LendingPoolAPIResponse_number_**](../Models/LendingPoolAPIResponse_number_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolGetMaxNumberReserves"></a>
# **lendingPoolGetMaxNumberReserves**
> LendingPoolAPIResponse_number_ lendingPoolGetMaxNumberReserves(Authorization, address, chainId)



    Retrieves the maximum number of reserves from the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **address** | **String**| - The address of the lending pool. | [default to null] |
| **chainId** | **String**| - The chain ID where the lending pool is located. | [default to null] |

### Return type

[**LendingPoolAPIResponse_number_**](../Models/LendingPoolAPIResponse_number_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolGetMaxStableRateBorrowSizePercent"></a>
# **lendingPoolGetMaxStableRateBorrowSizePercent**
> LendingPoolAPIResponse_number_ lendingPoolGetMaxStableRateBorrowSizePercent(Authorization, address, chainId)



    Retrieves the maximum stable rate borrow size percentage from the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **address** | **String**| - The address of the lending pool. | [default to null] |
| **chainId** | **String**| - The chain ID of the blockchain network. | [default to null] |

### Return type

[**LendingPoolAPIResponse_number_**](../Models/LendingPoolAPIResponse_number_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolGetReserveData"></a>
# **lendingPoolGetReserveData**
> LendingPoolAPIResponse_any_ lendingPoolGetReserveData(Authorization, address, chainId, asset)



    Retrieves reserve data for a specific asset from the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **address** | **String**| - The address of the lending pool. | [default to null] |
| **chainId** | **String**| - The chain ID of the blockchain network. | [default to null] |
| **asset** | **String**| - The asset for which to retrieve reserve data. | [default to null] |

### Return type

[**LendingPoolAPIResponse_any_**](../Models/LendingPoolAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolGetReservesList"></a>
# **lendingPoolGetReservesList**
> LendingPoolAPIResponse_string-Array_ lendingPoolGetReservesList(Authorization, address, chainId)



    Retrieves the list of reserves from the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **address** | **String**| - The address of the lending pool. | [default to null] |
| **chainId** | **String**| - The chain ID of the blockchain network. | [default to null] |

### Return type

[**LendingPoolAPIResponse_string-Array_**](../Models/LendingPoolAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolGetUserAccountData"></a>
# **lendingPoolGetUserAccountData**
> LendingPoolAPIResponse_any_ lendingPoolGetUserAccountData(Authorization, address, chainId, user)



    Retrieves user account data from the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **address** | **String**| - The address of the lending pool. | [default to null] |
| **chainId** | **String**| - The chain ID of the blockchain network. | [default to null] |
| **user** | **String**| - The user address for which to retrieve account data. | [default to null] |

### Return type

[**LendingPoolAPIResponse_any_**](../Models/LendingPoolAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolIsPaused"></a>
# **lendingPoolIsPaused**
> LendingPoolAPIResponse_boolean_ lendingPoolIsPaused(Authorization, address, chainId)



    Checks if the lending pool is paused.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **address** | **String**| - The address of the lending pool from the query parameters. | [default to null] |
| **chainId** | **String**| - The chain ID of the lending pool from the query parameters. | [default to null] |

### Return type

[**LendingPoolAPIResponse_boolean_**](../Models/LendingPoolAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lendingPoolLiquidationCall"></a>
# **lendingPoolLiquidationCall**
> LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_ lendingPoolLiquidationCall(accountName, Authorization, LendingPoolInputBody)



    Handles the liquidation call for a lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to be liquidated. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **LendingPoolInputBody** | [**LendingPoolInputBody**](../Models/LendingPoolInputBody.md)| - The body of the request containing necessary parameters. | |

### Return type

[**LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_**](../Models/LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="lendingPoolRepay"></a>
# **lendingPoolRepay**
> LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_ lendingPoolRepay(accountName, Authorization, LendingPoolInputBody)



    Repays a loan in the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to repay the loan for. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **LendingPoolInputBody** | [**LendingPoolInputBody**](../Models/LendingPoolInputBody.md)| - The body containing the lending pool input details. | |

### Return type

[**LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_**](../Models/LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="lendingPoolSetUserUseReserveAsCollateral"></a>
# **lendingPoolSetUserUseReserveAsCollateral**
> LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_ lendingPoolSetUserUseReserveAsCollateral(accountName, Authorization, LendingPoolInputBody)



    Sets the user&#39;s reserve as collateral.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the user&#39;s account. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **LendingPoolInputBody** | [**LendingPoolInputBody**](../Models/LendingPoolInputBody.md)| - The body containing lending pool input data. | |

### Return type

[**LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_**](../Models/LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="lendingPoolSwapBorrowRateMode"></a>
# **lendingPoolSwapBorrowRateMode**
> LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_ lendingPoolSwapBorrowRateMode(accountName, Authorization, LendingPoolInputBody)



    Swaps the borrow rate mode for a given account in the lending pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account for which the borrow rate mode is to be swapped. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **LendingPoolInputBody** | [**LendingPoolInputBody**](../Models/LendingPoolInputBody.md)| - The input body containing the contract address and chain ID. | |

### Return type

[**LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_**](../Models/LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

