# Erc4337Api

## com.usemoon.MoonSDK.Api.Erc4337Api

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                           | HTTP request                                             | Description |
| ---------------------------------------------------------------- | -------------------------------------------------------- | ----------- |
| [**GetAddress**](erc4337api.md#getaddress)                       | **POST** /erc4337/{accountName}/address                  |             |
| [**SignBroadcastUserOpTx**](erc4337api.md#signbroadcastuseroptx) | **POST** /erc4337/{accountName}/sign-broadcast-userop-tx |             |

## **GetAddress**

> AccountAPIResponse GetAddress (string authorization, string accountName, InputBody inputBody)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class GetAddressExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app";
            // Configure API key authorization: ApiKeyAuth
            config.AddApiKey("x-api-key", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("x-api-key", "Bearer");
            // Configure API key authorization: BearerAuth
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new Erc4337Api(config);
            var authorization = "authorization_example";  // string | 
            var accountName = "accountName_example";  // string | 
            var inputBody = new InputBody(); // InputBody | 

            try
            {
                AccountAPIResponse result = apiInstance.GetAddress(authorization, accountName, inputBody);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling Erc4337Api.GetAddress: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the GetAddressWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<AccountAPIResponse> response = apiInstance.GetAddressWithHttpInfo(authorization, accountName, inputBody);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling Erc4337Api.GetAddressWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **string**                    |             |       |
| **accountName**   | **string**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc4337api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **SignBroadcastUserOpTx**

> TransactionAPIResponse SignBroadcastUserOpTx (string authorization, string accountName, InputBody inputBody)

#### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace Example
{
    public class SignBroadcastUserOpTxExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app";
            // Configure API key authorization: ApiKeyAuth
            config.AddApiKey("x-api-key", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("x-api-key", "Bearer");
            // Configure API key authorization: BearerAuth
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new Erc4337Api(config);
            var authorization = "authorization_example";  // string | 
            var accountName = "accountName_example";  // string | 
            var inputBody = new InputBody(); // InputBody | 

            try
            {
                TransactionAPIResponse result = apiInstance.SignBroadcastUserOpTx(authorization, accountName, inputBody);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling Erc4337Api.SignBroadcastUserOpTx: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

**Using the SignBroadcastUserOpTxWithHttpInfo variant**

This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<TransactionAPIResponse> response = apiInstance.SignBroadcastUserOpTxWithHttpInfo(authorization, accountName, inputBody);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling Erc4337Api.SignBroadcastUserOpTxWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **string**                    |             |       |
| **accountName**   | **string**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc4337api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
