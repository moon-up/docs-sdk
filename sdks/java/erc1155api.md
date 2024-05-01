# Erc1155Api

## Erc1155Api

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                           | HTTP request                                      | Description |
| ---------------------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**balanceOf**](erc1155api.md#balanceOf)                         | **POST** /erc1155/{name}/balance-of               |             |
| [**balanceOfBatch**](erc1155api.md#balanceOfBatch)               | **POST** /erc1155/{name}/balance-of-batch         |             |
| [**isApprovedForAll**](erc1155api.md#isApprovedForAll)           | **POST** /erc1155/{name}/is-approved-for-all      |             |
| [**safeBatchTransferFrom**](erc1155api.md#safeBatchTransferFrom) | **POST** /erc1155/{name}/safe-batch-transfer-from |             |
| [**safeTransferFrom**](erc1155api.md#safeTransferFrom)           | **POST** /erc1155/{name}/safe-transfer-from       |             |
| [**setApprovalForAll**](erc1155api.md#setApprovalForAll)         | **POST** /erc1155/{name}/set-approval-for-all     |             |

## **balanceOf**

> TransactionAPIResponse balanceOf(name, authorization, erc1155Request)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.Erc1155Api;

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

    Erc1155Api apiInstance = new Erc1155Api(defaultClient);
    String name = "name_example"; // String | 
    String authorization = "authorization_example"; // String | 
    Erc1155Request erc1155Request = new Erc1155Request(); // Erc1155Request | 
    try {
      TransactionAPIResponse result = apiInstance.balanceOf(name, authorization, erc1155Request);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling Erc1155Api#balanceOf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

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

## **balanceOfBatch**

> TransactionAPIResponse balanceOfBatch(name, authorization, erc1155Request)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.Erc1155Api;

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

    Erc1155Api apiInstance = new Erc1155Api(defaultClient);
    String name = "name_example"; // String | 
    String authorization = "authorization_example"; // String | 
    Erc1155Request erc1155Request = new Erc1155Request(); // Erc1155Request | 
    try {
      TransactionAPIResponse result = apiInstance.balanceOfBatch(name, authorization, erc1155Request);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling Erc1155Api#balanceOfBatch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

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

## **isApprovedForAll**

> TransactionAPIResponse isApprovedForAll(name, authorization, erc1155Request)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.Erc1155Api;

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

    Erc1155Api apiInstance = new Erc1155Api(defaultClient);
    String name = "name_example"; // String | 
    String authorization = "authorization_example"; // String | 
    Erc1155Request erc1155Request = new Erc1155Request(); // Erc1155Request | 
    try {
      TransactionAPIResponse result = apiInstance.isApprovedForAll(name, authorization, erc1155Request);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling Erc1155Api#isApprovedForAll");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

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

## **safeBatchTransferFrom**

> TransactionAPIResponse safeBatchTransferFrom(name, authorization, erc1155Request)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.Erc1155Api;

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

    Erc1155Api apiInstance = new Erc1155Api(defaultClient);
    String name = "name_example"; // String | 
    String authorization = "authorization_example"; // String | 
    Erc1155Request erc1155Request = new Erc1155Request(); // Erc1155Request | 
    try {
      TransactionAPIResponse result = apiInstance.safeBatchTransferFrom(name, authorization, erc1155Request);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling Erc1155Api#safeBatchTransferFrom");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

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

## **safeTransferFrom**

> TransactionAPIResponse safeTransferFrom(name, authorization, erc1155Request)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.Erc1155Api;

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

    Erc1155Api apiInstance = new Erc1155Api(defaultClient);
    String name = "name_example"; // String | 
    String authorization = "authorization_example"; // String | 
    Erc1155Request erc1155Request = new Erc1155Request(); // Erc1155Request | 
    try {
      TransactionAPIResponse result = apiInstance.safeTransferFrom(name, authorization, erc1155Request);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling Erc1155Api#safeTransferFrom");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

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

## **setApprovalForAll**

> TransactionAPIResponse setApprovalForAll(name, authorization, erc1155Request)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.Erc1155Api;

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

    Erc1155Api apiInstance = new Erc1155Api(defaultClient);
    String name = "name_example"; // String | 
    String authorization = "authorization_example"; // String | 
    Erc1155Request erc1155Request = new Erc1155Request(); // Erc1155Request | 
    try {
      TransactionAPIResponse result = apiInstance.setApprovalForAll(name, authorization, erc1155Request);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling Erc1155Api#setApprovalForAll");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

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
