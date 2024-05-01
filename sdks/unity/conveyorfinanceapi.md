# ConveyorFinanceApi

## com.usemoon.MoonSDK.Api.ConveyorFinanceApi

All URIs are relative to _https://beta.usemoon.ai_

| Method   | HTTP request                          | Description |
| -------- | ------------------------------------- | ----------- |
| **Swap** | **POST** /conveyorfinance/{name}/swap |             |

## **Swap**

> ConveyorFinanceControllerResponse Swap (string authorization, string name, TokenSwapParams tokenSwapParams)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class SwapExample
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

            var apiInstance = new ConveyorFinanceApi(config);
            var authorization = "authorization_example";  // string | 
            var name = "name_example";  // string | 
            var tokenSwapParams = new TokenSwapParams(); // TokenSwapParams | 

            try
            {
                ConveyorFinanceControllerResponse result = apiInstance.Swap(authorization, name, tokenSwapParams);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ConveyorFinanceApi.Swap: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the SwapWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<ConveyorFinanceControllerResponse> response = apiInstance.SwapWithHttpInfo(authorization, name, tokenSwapParams);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ConveyorFinanceApi.SwapWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name                | Type                | Description | Notes |
| ------------------- | ------------------- | ----------- | ----- |
| **authorization**   | **string**          |             |       |
| **name**            | **string**          |             |       |
| **tokenSwapParams** | **TokenSwapParams** |             |       |

#### Return type

**ConveyorFinanceControllerResponse**

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
