# FinancialDatasetsApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**financialDatasetsGetAllFinancials**](FinancialDatasetsApi.md#financialDatasetsGetAllFinancials) | **GET** /financial-datasets/all-financials/{ticker} |  |
| [**financialDatasetsGetAvailableTickers**](FinancialDatasetsApi.md#financialDatasetsGetAvailableTickers) | **GET** /financial-datasets/available-tickers |  |
| [**financialDatasetsGetBalanceSheets**](FinancialDatasetsApi.md#financialDatasetsGetBalanceSheets) | **GET** /financial-datasets/balance-sheets/{ticker} |  |
| [**financialDatasetsGetCashFlowStatements**](FinancialDatasetsApi.md#financialDatasetsGetCashFlowStatements) | **GET** /financial-datasets/cash-flow-statements/{ticker} |  |
| [**financialDatasetsGetCompanyFacts**](FinancialDatasetsApi.md#financialDatasetsGetCompanyFacts) | **GET** /financial-datasets/company-facts/{ticker} |  |
| [**financialDatasetsGetIncomeStatements**](FinancialDatasetsApi.md#financialDatasetsGetIncomeStatements) | **GET** /financial-datasets/income-statements/{ticker} |  |
| [**financialDatasetsGetInsiderTransactions**](FinancialDatasetsApi.md#financialDatasetsGetInsiderTransactions) | **GET** /financial-datasets/insider-transactions/{ticker} |  |
| [**financialDatasetsGetOptionsChain**](FinancialDatasetsApi.md#financialDatasetsGetOptionsChain) | **GET** /financial-datasets/options-chain/{ticker} |  |
| [**financialDatasetsGetPriceSnapshot**](FinancialDatasetsApi.md#financialDatasetsGetPriceSnapshot) | **GET** /financial-datasets/price-snapshot/{ticker} |  |
| [**financialDatasetsGetPrices**](FinancialDatasetsApi.md#financialDatasetsGetPrices) | **GET** /financial-datasets/prices/{ticker} |  |
| [**financialDatasetsGetSegmentedRevenues**](FinancialDatasetsApi.md#financialDatasetsGetSegmentedRevenues) | **GET** /financial-datasets/segmented-revenues/{ticker} |  |
| [**financialDatasetsSearchFinancials**](FinancialDatasetsApi.md#financialDatasetsSearchFinancials) | **POST** /financial-datasets/search-financials |  |
| [**financialDatasetsSearchFinancialsByLineItems**](FinancialDatasetsApi.md#financialDatasetsSearchFinancialsByLineItems) | **POST** /financial-datasets/search-line-items |  |


<a name="financialDatasetsGetAllFinancials"></a>
# **financialDatasetsGetAllFinancials**
> AllFinancialsAPIResponse financialDatasetsGetAllFinancials(ticker, Authorization, period, limit, cik)



    Retrieves all financials for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **period** | **String**| - The period type of the financials. | [default to null] [enum: annual, quarterly, ttm] |
| **limit** | **Double**| - The maximum number of financials to return. | [optional] [default to null] |
| **cik** | **String**| - The CIK number of the company. | [optional] [default to null] |

### Return type

[**AllFinancialsAPIResponse**](../Models/AllFinancialsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetAvailableTickers"></a>
# **financialDatasetsGetAvailableTickers**
> AvailableTickersAPIResponse financialDatasetsGetAvailableTickers(Authorization)



    Retrieves the available tickers.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |

### Return type

[**AvailableTickersAPIResponse**](../Models/AvailableTickersAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetBalanceSheets"></a>
# **financialDatasetsGetBalanceSheets**
> BalanceSheetsAPIResponse financialDatasetsGetBalanceSheets(ticker, Authorization, period, limit, cik)



    Retrieves the balance sheets for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **period** | **String**| - The period type of the balance sheets. | [default to null] [enum: annual, quarterly, ttm] |
| **limit** | **Double**| - The maximum number of balance sheets to return. | [optional] [default to null] |
| **cik** | **String**| - The CIK number of the company. | [optional] [default to null] |

### Return type

[**BalanceSheetsAPIResponse**](../Models/BalanceSheetsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetCashFlowStatements"></a>
# **financialDatasetsGetCashFlowStatements**
> CashFlowStatementsAPIResponse financialDatasetsGetCashFlowStatements(ticker, Authorization, period, limit, cik)



    Retrieves the cash flow statements for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **period** | **String**| - The period type of the cash flow statements. | [default to null] [enum: annual, quarterly, ttm] |
| **limit** | **Double**| - The maximum number of cash flow statements to return. | [optional] [default to null] |
| **cik** | **String**| - The CIK number of the company. | [optional] [default to null] |

### Return type

[**CashFlowStatementsAPIResponse**](../Models/CashFlowStatementsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetCompanyFacts"></a>
# **financialDatasetsGetCompanyFacts**
> CompanyFactsAPIResponse financialDatasetsGetCompanyFacts(ticker, Authorization)



    Retrieves the company facts for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |

### Return type

[**CompanyFactsAPIResponse**](../Models/CompanyFactsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetIncomeStatements"></a>
# **financialDatasetsGetIncomeStatements**
> IncomeStatementsAPIResponse financialDatasetsGetIncomeStatements(ticker, Authorization, period, limit, cik)



    Retrieves the income statements for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **period** | **String**| - The period type of the income statements. | [default to null] [enum: annual, quarterly, ttm] |
| **limit** | **Double**| - The maximum number of income statements to return. | [optional] [default to null] |
| **cik** | **String**| - The CIK number of the company. | [optional] [default to null] |

### Return type

[**IncomeStatementsAPIResponse**](../Models/IncomeStatementsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetInsiderTransactions"></a>
# **financialDatasetsGetInsiderTransactions**
> InsiderTransactionsAPIResponse financialDatasetsGetInsiderTransactions(ticker, Authorization, limit)



    Retrieves the insider transactions for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **limit** | **Double**| - The maximum number of insider transactions to return. | [optional] [default to null] |

### Return type

[**InsiderTransactionsAPIResponse**](../Models/InsiderTransactionsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetOptionsChain"></a>
# **financialDatasetsGetOptionsChain**
> OptionsChainAPIResponse financialDatasetsGetOptionsChain(ticker, Authorization, strike\_price, option\_type, expiration\_date)



    Retrieves the options chain for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **strike\_price** | **Double**| - The strike price of the options. | [optional] [default to null] |
| **option\_type** | **String**| - The type of option (call or put). | [optional] [default to null] [enum: call, put] |
| **expiration\_date** | **String**| - The expiration date of the options. | [optional] [default to null] |

### Return type

[**OptionsChainAPIResponse**](../Models/OptionsChainAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetPriceSnapshot"></a>
# **financialDatasetsGetPriceSnapshot**
> PriceSnapshotAPIResponse financialDatasetsGetPriceSnapshot(ticker, Authorization)



    Retrieves the price snapshot for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |

### Return type

[**PriceSnapshotAPIResponse**](../Models/PriceSnapshotAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetPrices"></a>
# **financialDatasetsGetPrices**
> PricesAPIResponse financialDatasetsGetPrices(ticker, Authorization, interval, interval\_multiplier, start\_date, end\_date, limit)



    Retrieves the price data for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **interval** | [**PriceInterval**](../Models/.md)| - The interval of the price data. | [default to null] [enum: second, minute, day, week, month, quarter, year] |
| **interval\_multiplier** | **Double**| - The interval multiplier of the price data. | [default to null] |
| **start\_date** | **String**| - The start date of the price data. | [default to null] |
| **end\_date** | **String**| - The end date of the price data. | [default to null] |
| **limit** | **Double**| - The maximum number of price data to return. | [optional] [default to null] |

### Return type

[**PricesAPIResponse**](../Models/PricesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsGetSegmentedRevenues"></a>
# **financialDatasetsGetSegmentedRevenues**
> SegmentedRevenuesAPIResponse financialDatasetsGetSegmentedRevenues(ticker, Authorization, period, limit, cik)



    Retrieves the segmented revenues for a given ticker symbol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **ticker** | **String**| - The ticker symbol of the company. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **period** | **String**| - The period type of the segmented revenues. | [default to null] [enum: annual, quarterly] |
| **limit** | **Double**| - The maximum number of segmented revenues to return. | [optional] [default to null] |
| **cik** | **String**| - The CIK number of the company. | [optional] [default to null] |

### Return type

[**SegmentedRevenuesAPIResponse**](../Models/SegmentedRevenuesAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="financialDatasetsSearchFinancials"></a>
# **financialDatasetsSearchFinancials**
> SearchFinancialsAPIResponse financialDatasetsSearchFinancials(Authorization, SearchRequest)



    Searches financials for a given search request.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **SearchRequest** | [**SearchRequest**](../Models/SearchRequest.md)| - The search request. | |

### Return type

[**SearchFinancialsAPIResponse**](../Models/SearchFinancialsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="financialDatasetsSearchFinancialsByLineItems"></a>
# **financialDatasetsSearchFinancialsByLineItems**
> LineItemsSearchAPIResponse financialDatasetsSearchFinancialsByLineItems(Authorization, FinancialDatasets\_SearchFinancialsByLineItems\_request)



    Searches financials by line items.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **FinancialDatasets\_SearchFinancialsByLineItems\_request** | [**FinancialDatasets_SearchFinancialsByLineItems_request**](../Models/FinancialDatasets_SearchFinancialsByLineItems_request.md)| - The search request. | |

### Return type

[**LineItemsSearchAPIResponse**](../Models/LineItemsSearchAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

