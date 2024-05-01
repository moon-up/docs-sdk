# ERC1155Api

## com.usemoon.MoonSDK.Api.ERC1155Api

All URIs are relative to _https://beta.usemoon.ai_

| Method                    | HTTP request                                      | Description |
| ------------------------- | ------------------------------------------------- | ----------- |
| **BalanceOf**             | **POST** /erc1155/{name}/balance-of               |             |
| **BalanceOfBatch**        | **POST** /erc1155/{name}/balance-of-batch         |             |
| **IsApprovedForAll**      | **POST** /erc1155/{name}/is-approved-for-all      |             |
| **SafeBatchTransferFrom** | **POST** /erc1155/{name}/safe-batch-transfer-from |             |
| **SafeTransferFrom**      | **POST** /erc1155/{name}/safe-transfer-from       |             |
| **SetApprovalForAll**     | **POST** /erc1155/{name}/set-approval-for-all     |             |

## **BalanceOf**

> TransactionAPIResponse BalanceOf (string name, string authorization, Erc1155Request erc1155Request)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class BalanceOfExample
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

            var apiInstance = new ERC1155Api(config);
            var name = "name_example";  // string | 
            var authorization = "authorization_example";  // string | 
            var erc1155Request = new Erc1155Request(); // Erc1155Request | 

            try
            {
                TransactionAPIResponse result = apiInstance.BalanceOf(name, authorization, erc1155Request);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ERC1155Api.BalanceOf: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the BalanceOfWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.BalanceOfWithHttpInfo(name, authorization, erc1155Request);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ERC1155Api.BalanceOfWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **string**         |             |       |
| **authorization**  | **string**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

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

## **BalanceOfBatch**

> TransactionAPIResponse BalanceOfBatch (string name, string authorization, Erc1155Request erc1155Request)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class BalanceOfBatchExample
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

            var apiInstance = new ERC1155Api(config);
            var name = "name_example";  // string | 
            var authorization = "authorization_example";  // string | 
            var erc1155Request = new Erc1155Request(); // Erc1155Request | 

            try
            {
                TransactionAPIResponse result = apiInstance.BalanceOfBatch(name, authorization, erc1155Request);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ERC1155Api.BalanceOfBatch: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the BalanceOfBatchWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.BalanceOfBatchWithHttpInfo(name, authorization, erc1155Request);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ERC1155Api.BalanceOfBatchWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **string**         |             |       |
| **authorization**  | **string**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

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

## **IsApprovedForAll**

> TransactionAPIResponse IsApprovedForAll (string name, string authorization, Erc1155Request erc1155Request)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class IsApprovedForAllExample
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

            var apiInstance = new ERC1155Api(config);
            var name = "name_example";  // string | 
            var authorization = "authorization_example";  // string | 
            var erc1155Request = new Erc1155Request(); // Erc1155Request | 

            try
            {
                TransactionAPIResponse result = apiInstance.IsApprovedForAll(name, authorization, erc1155Request);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ERC1155Api.IsApprovedForAll: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the IsApprovedForAllWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.IsApprovedForAllWithHttpInfo(name, authorization, erc1155Request);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ERC1155Api.IsApprovedForAllWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **string**         |             |       |
| **authorization**  | **string**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

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

## **SafeBatchTransferFrom**

> TransactionAPIResponse SafeBatchTransferFrom (string name, string authorization, Erc1155Request erc1155Request)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class SafeBatchTransferFromExample
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

            var apiInstance = new ERC1155Api(config);
            var name = "name_example";  // string | 
            var authorization = "authorization_example";  // string | 
            var erc1155Request = new Erc1155Request(); // Erc1155Request | 

            try
            {
                TransactionAPIResponse result = apiInstance.SafeBatchTransferFrom(name, authorization, erc1155Request);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ERC1155Api.SafeBatchTransferFrom: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the SafeBatchTransferFromWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.SafeBatchTransferFromWithHttpInfo(name, authorization, erc1155Request);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ERC1155Api.SafeBatchTransferFromWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **string**         |             |       |
| **authorization**  | **string**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

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

## **SafeTransferFrom**

> TransactionAPIResponse SafeTransferFrom (string name, string authorization, Erc1155Request erc1155Request)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class SafeTransferFromExample
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

            var apiInstance = new ERC1155Api(config);
            var name = "name_example";  // string | 
            var authorization = "authorization_example";  // string | 
            var erc1155Request = new Erc1155Request(); // Erc1155Request | 

            try
            {
                TransactionAPIResponse result = apiInstance.SafeTransferFrom(name, authorization, erc1155Request);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ERC1155Api.SafeTransferFrom: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the SafeTransferFromWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.SafeTransferFromWithHttpInfo(name, authorization, erc1155Request);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ERC1155Api.SafeTransferFromWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **string**         |             |       |
| **authorization**  | **string**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

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

## **SetApprovalForAll**

> TransactionAPIResponse SetApprovalForAll (string name, string authorization, Erc1155Request erc1155Request)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class SetApprovalForAllExample
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

            var apiInstance = new ERC1155Api(config);
            var name = "name_example";  // string | 
            var authorization = "authorization_example";  // string | 
            var erc1155Request = new Erc1155Request(); // Erc1155Request | 

            try
            {
                TransactionAPIResponse result = apiInstance.SetApprovalForAll(name, authorization, erc1155Request);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ERC1155Api.SetApprovalForAll: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the SetApprovalForAllWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.SetApprovalForAllWithHttpInfo(name, authorization, erc1155Request);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ERC1155Api.SetApprovalForAllWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **string**         |             |       |
| **authorization**  | **string**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

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
