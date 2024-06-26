# ENSApi

## com.usemoon.MoonSDK.Api.ENSApi

All URIs are relative to _https://beta.usemoon.ai_

| Method      | HTTP request          | Description |
| ----------- | --------------------- | ----------- |
| **Resolve** | **POST** /ens/resolve |             |

## **Resolve**

> EnsResolveAPIResponse Resolve (string authorization, EnsResolveInput ensResolveInput)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class ResolveExample
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

            var apiInstance = new ENSApi(config);
            var authorization = "authorization_example";  // string | 
            var ensResolveInput = new EnsResolveInput(); // EnsResolveInput | 

            try
            {
                EnsResolveAPIResponse result = apiInstance.Resolve(authorization, ensResolveInput);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ENSApi.Resolve: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the ResolveWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<EnsResolveAPIResponse> response = apiInstance.ResolveWithHttpInfo(authorization, ensResolveInput);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ENSApi.ResolveWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name                | Type                | Description | Notes |
| ------------------- | ------------------- | ----------- | ----- |
| **authorization**   | **string**          |             |       |
| **ensResolveInput** | **EnsResolveInput** |             |       |

#### Return type

**EnsResolveAPIResponse**

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
