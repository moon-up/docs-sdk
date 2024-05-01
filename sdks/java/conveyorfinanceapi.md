# ConveyorFinanceApi

## ConveyorFinanceApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                 | HTTP request                          | Description |
| -------------------------------------- | ------------------------------------- | ----------- |
| [**swap**](conveyorfinanceapi.md#swap) | **POST** /conveyorfinance/{name}/swap |             |

## **swap**

> ConveyorFinanceControllerResponse swap(authorization, name, tokenSwapParams)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.ConveyorFinanceApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app");
    
    // Configure API key authorization: ApiKeyAuth
    ApiKeyAuth ApiKeyAuth = (ApiKeyAuth) defaultClient.getAuthentication("ApiKeyAuth");
    ApiKeyAuth.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //ApiKeyAuth.setApiKeyPrefix("Token");

    // Configure API key authorization: BearerAuth
    ApiKeyAuth BearerAuth = (ApiKeyAuth) defaultClient.getAuthentication("BearerAuth");
    BearerAuth.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //BearerAuth.setApiKeyPrefix("Token");

    ConveyorFinanceApi apiInstance = new ConveyorFinanceApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    String name = "name_example"; // String | 
    TokenSwapParams tokenSwapParams = new TokenSwapParams(); // TokenSwapParams | 
    try {
      ConveyorFinanceControllerResponse result = apiInstance.swap(authorization, name, tokenSwapParams);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling ConveyorFinanceApi#swap");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name                | Type                                      | Description | Notes |
| ------------------- | ----------------------------------------- | ----------- | ----- |
| **authorization**   | **String**                                |             |       |
| **name**            | **String**                                |             |       |
| **tokenSwapParams** | [**TokenSwapParams**](tokenswapparams.md) |             |       |

#### Return type

[**ConveyorFinanceControllerResponse**](conveyorfinancecontrollerresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |
