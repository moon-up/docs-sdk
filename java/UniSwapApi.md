# UniSwapApi

## UniSwapApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                                 | HTTP request                                          | Description |
| ---------------------------------------------------------------------- | ----------------------------------------------------- | ----------- |
| [**addLiquidity**](UniSwapApi.md#addLiquidity)                         | **POST** /uniswap/{name}/add-liquidity                |             |
| [**removeLiquidity**](UniSwapApi.md#removeLiquidity)                   | **POST** /uniswap/{name}/remove-liquidity             |             |
| [**swapExactETHForTokens**](UniSwapApi.md#swapExactETHForTokens)       | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| [**swapExactTokensForTokens**](UniSwapApi.md#swapExactTokensForTokens) | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |

## **addLiquidity**

> TransactionAPIResponse addLiquidity(authorization, name, uniswapInput)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.UniSwapApi;

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

    UniSwapApi apiInstance = new UniSwapApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    String name = "name_example"; // String | 
    UniswapInput uniswapInput = new UniswapInput(); // UniswapInput | 
    try {
      TransactionAPIResponse result = apiInstance.addLiquidity(authorization, name, uniswapInput);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UniSwapApi#addLiquidity");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **name**          | **String**                          |             |       |
| **uniswapInput**  | [**UniswapInput**](UniswapInput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](TransactionAPIResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

## **removeLiquidity**

> TransactionAPIResponse removeLiquidity(authorization, name, uniswapInput)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.UniSwapApi;

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

    UniSwapApi apiInstance = new UniSwapApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    String name = "name_example"; // String | 
    UniswapInput uniswapInput = new UniswapInput(); // UniswapInput | 
    try {
      TransactionAPIResponse result = apiInstance.removeLiquidity(authorization, name, uniswapInput);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UniSwapApi#removeLiquidity");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **name**          | **String**                          |             |       |
| **uniswapInput**  | [**UniswapInput**](UniswapInput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](TransactionAPIResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

## **swapExactETHForTokens**

> TransactionAPIResponse swapExactETHForTokens(authorization, name, uniswapInput)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.UniSwapApi;

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

    UniSwapApi apiInstance = new UniSwapApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    String name = "name_example"; // String | 
    UniswapInput uniswapInput = new UniswapInput(); // UniswapInput | 
    try {
      TransactionAPIResponse result = apiInstance.swapExactETHForTokens(authorization, name, uniswapInput);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UniSwapApi#swapExactETHForTokens");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **name**          | **String**                          |             |       |
| **uniswapInput**  | [**UniswapInput**](UniswapInput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](TransactionAPIResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

## **swapExactTokensForTokens**

> TransactionAPIResponse swapExactTokensForTokens(authorization, name, uniswapInput)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.UniSwapApi;

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

    UniSwapApi apiInstance = new UniSwapApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    String name = "name_example"; // String | 
    UniswapInput uniswapInput = new UniswapInput(); // UniswapInput | 
    try {
      TransactionAPIResponse result = apiInstance.swapExactTokensForTokens(authorization, name, uniswapInput);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UniSwapApi#swapExactTokensForTokens");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **name**          | **String**                          |             |       |
| **uniswapInput**  | [**UniswapInput**](UniswapInput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](TransactionAPIResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |
