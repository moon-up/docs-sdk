# DogeCoinApi

## DogeCoinApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                                | HTTP request                             | Description |
| --------------------------------------------------------------------- | ---------------------------------------- | ----------- |
| [**createDogeCoinAccount**](dogecoinapi.md#createDogeCoinAccount)     | **POST** /dogecoin                       |             |
| [**getDogeCoinAccount**](dogecoinapi.md#getDogeCoinAccount)           | **GET** /dogecoin/{accountName}          |             |
| [**listDogeCoinAccounts**](dogecoinapi.md#listDogeCoinAccounts)       | **GET** /dogecoin                        |             |
| [**signDogeCoinTransaction**](dogecoinapi.md#signDogeCoinTransaction) | **POST** /dogecoin/{accountName}/sign-tx |             |

## **createDogeCoinAccount**

> AccountAPIResponse createDogeCoinAccount(authorization, dogeCoinInput)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.DogeCoinApi;

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

    DogeCoinApi apiInstance = new DogeCoinApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    DogeCoinInput dogeCoinInput = new DogeCoinInput(); // DogeCoinInput | 
    try {
      AccountAPIResponse result = apiInstance.createDogeCoinAccount(authorization, dogeCoinInput);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DogeCoinApi#createDogeCoinAccount");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **dogeCoinInput** | [**DogeCoinInput**](dogecoininput.md) |             |       |

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

## **getDogeCoinAccount**

> AccountAPIResponse getDogeCoinAccount(authorization, accountName)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.DogeCoinApi;

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

    DogeCoinApi apiInstance = new DogeCoinApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    String accountName = "accountName_example"; // String | 
    try {
      AccountAPIResponse result = apiInstance.getDogeCoinAccount(authorization, accountName);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DogeCoinApi#getDogeCoinAccount");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **accountName**   | **String** |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

## **listDogeCoinAccounts**

> AccountAPIResponse listDogeCoinAccounts(authorization)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.DogeCoinApi;

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

    DogeCoinApi apiInstance = new DogeCoinApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    try {
      AccountAPIResponse result = apiInstance.listDogeCoinAccounts(authorization);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DogeCoinApi#listDogeCoinAccounts");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

## **signDogeCoinTransaction**

> DogeCoinAPIResponse signDogeCoinTransaction(authorization, accountName, dogeCoinTransactionInput)

#### Example

```java
// Import classes:
import org.usemoonai.moonsdk.client.ApiClient;
import org.usemoonai.moonsdk.client.ApiException;
import org.usemoonai.moonsdk.client.Configuration;
import org.usemoonai.moonsdk.client.auth.*;
import org.usemoonai.moonsdk.client.models.*;
import org.usemoonai.moonsdk.api.DogeCoinApi;

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

    DogeCoinApi apiInstance = new DogeCoinApi(defaultClient);
    String authorization = "authorization_example"; // String | 
    String accountName = "accountName_example"; // String | 
    DogeCoinTransactionInput dogeCoinTransactionInput = new DogeCoinTransactionInput(); // DogeCoinTransactionInput | 
    try {
      DogeCoinAPIResponse result = apiInstance.signDogeCoinTransaction(authorization, accountName, dogeCoinTransactionInput);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DogeCoinApi#signDogeCoinTransaction");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

#### Parameters

| Name                         | Type                                                        | Description | Notes |
| ---------------------------- | ----------------------------------------------------------- | ----------- | ----- |
| **authorization**            | **String**                                                  |             |       |
| **accountName**              | **String**                                                  |             |       |
| **dogeCoinTransactionInput** | [**DogeCoinTransactionInput**](dogecointransactioninput.md) |             |       |

#### Return type

[**DogeCoinAPIResponse**](dogecoinapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |
