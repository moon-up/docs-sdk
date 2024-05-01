# UniSwapApi

## com.usemoon.MoonSDK.Api.UniSwapApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                       | HTTP request                                          | Description |
| ---------------------------- | ----------------------------------------------------- | ----------- |
| **AddLiquidity**             | **POST** /uniswap/{name}/add-liquidity                |             |
| **RemoveLiquidity**          | **POST** /uniswap/{name}/remove-liquidity             |             |
| **SwapExactETHForTokens**    | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| **SwapExactTokensForTokens** | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |

## **AddLiquidity**

> TransactionAPIResponse AddLiquidity (string authorization, string name, UniswapInput uniswapInput)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class AddLiquidityExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://beta.usemoon.ai";
            // Configure API key authorization: ApiKeyAuth
            config.AddApiKey("x-api-key", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("x-api-key", "Bearer");
            // Configure API key authorization: BearerAuth
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new UniSwapApi(config);
            var authorization = "authorization_example";  // string | 
            var name = "name_example";  // string | 
            var uniswapInput = new UniswapInput(); // UniswapInput | 

            try
            {
                TransactionAPIResponse result = apiInstance.AddLiquidity(authorization, name, uniswapInput);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UniSwapApi.AddLiquidity: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the AddLiquidityWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.AddLiquidityWithHttpInfo(authorization, name, uniswapInput);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UniSwapApi.AddLiquidityWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **string**       |             |       |
| **name**          | **string**       |             |       |
| **uniswapInput**  | **UniswapInput** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **RemoveLiquidity**

> TransactionAPIResponse RemoveLiquidity (string authorization, string name, UniswapInput uniswapInput)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class RemoveLiquidityExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://beta.usemoon.ai";
            // Configure API key authorization: ApiKeyAuth
            config.AddApiKey("x-api-key", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("x-api-key", "Bearer");
            // Configure API key authorization: BearerAuth
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new UniSwapApi(config);
            var authorization = "authorization_example";  // string | 
            var name = "name_example";  // string | 
            var uniswapInput = new UniswapInput(); // UniswapInput | 

            try
            {
                TransactionAPIResponse result = apiInstance.RemoveLiquidity(authorization, name, uniswapInput);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UniSwapApi.RemoveLiquidity: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the RemoveLiquidityWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.RemoveLiquidityWithHttpInfo(authorization, name, uniswapInput);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UniSwapApi.RemoveLiquidityWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **string**       |             |       |
| **name**          | **string**       |             |       |
| **uniswapInput**  | **UniswapInput** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **SwapExactETHForTokens**

> TransactionAPIResponse SwapExactETHForTokens (string authorization, string name, UniswapInput uniswapInput)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class SwapExactETHForTokensExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://beta.usemoon.ai";
            // Configure API key authorization: ApiKeyAuth
            config.AddApiKey("x-api-key", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("x-api-key", "Bearer");
            // Configure API key authorization: BearerAuth
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new UniSwapApi(config);
            var authorization = "authorization_example";  // string | 
            var name = "name_example";  // string | 
            var uniswapInput = new UniswapInput(); // UniswapInput | 

            try
            {
                TransactionAPIResponse result = apiInstance.SwapExactETHForTokens(authorization, name, uniswapInput);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UniSwapApi.SwapExactETHForTokens: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the SwapExactETHForTokensWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.SwapExactETHForTokensWithHttpInfo(authorization, name, uniswapInput);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UniSwapApi.SwapExactETHForTokensWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **string**       |             |       |
| **name**          | **string**       |             |       |
| **uniswapInput**  | **UniswapInput** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **SwapExactTokensForTokens**

> TransactionAPIResponse SwapExactTokensForTokens (string authorization, string name, UniswapInput uniswapInput)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class SwapExactTokensForTokensExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://beta.usemoon.ai";
            // Configure API key authorization: ApiKeyAuth
            config.AddApiKey("x-api-key", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("x-api-key", "Bearer");
            // Configure API key authorization: BearerAuth
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new UniSwapApi(config);
            var authorization = "authorization_example";  // string | 
            var name = "name_example";  // string | 
            var uniswapInput = new UniswapInput(); // UniswapInput | 

            try
            {
                TransactionAPIResponse result = apiInstance.SwapExactTokensForTokens(authorization, name, uniswapInput);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling UniSwapApi.SwapExactTokensForTokens: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the SwapExactTokensForTokensWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.SwapExactTokensForTokensWithHttpInfo(authorization, name, uniswapInput);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling UniSwapApi.SwapExactTokensForTokensWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **string**       |             |       |
| **name**          | **string**       |             |       |
| **uniswapInput**  | **UniswapInput** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
