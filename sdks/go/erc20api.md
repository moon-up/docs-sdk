# \Erc20API

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                 | HTTP request                         | Description |
| ------------------------------------------------------ | ------------------------------------ | ----------- |
| [**AllowanceErc20**](erc20api.md#AllowanceErc20)       | **Post** /erc20/{name}/allowance     |             |
| [**ApproveErc20**](erc20api.md#ApproveErc20)           | **Post** /erc20/{name}/approve       |             |
| [**BalanceOfErc20**](erc20api.md#BalanceOfErc20)       | **Post** /erc20/{name}/balance-of    |             |
| [**DecimalsErc20**](erc20api.md#DecimalsErc20)         | **Post** /erc20/{name}/decimals      |             |
| [**NameErc20**](erc20api.md#NameErc20)                 | **Post** /erc20/{name}/name          |             |
| [**SymbolErc20**](erc20api.md#SymbolErc20)             | **Post** /erc20/{name}/symbol        |             |
| [**TotalSupplyErc20**](erc20api.md#TotalSupplyErc20)   | **Post** /erc20/{name}/total-supply  |             |
| [**TransferErc20**](erc20api.md#TransferErc20)         | **Post** /erc20/{name}/transfer      |             |
| [**TransferFromErc20**](erc20api.md#TransferFromErc20) | **Post** /erc20/{name}/transfer-from |             |

## AllowanceErc20

> TransactionAPIResponse AllowanceErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.AllowanceErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.AllowanceErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AllowanceErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.AllowanceErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiAllowanceErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## ApproveErc20

> TransactionAPIResponse ApproveErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.ApproveErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.ApproveErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApproveErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.ApproveErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiApproveErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## BalanceOfErc20

> TransactionAPIResponse BalanceOfErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.BalanceOfErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.BalanceOfErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BalanceOfErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.BalanceOfErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiBalanceOfErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## DecimalsErc20

> TransactionAPIResponse DecimalsErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.DecimalsErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.DecimalsErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DecimalsErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.DecimalsErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiDecimalsErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## NameErc20

> TransactionAPIResponse NameErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.NameErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.NameErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NameErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.NameErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiNameErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## SymbolErc20

> TransactionAPIResponse SymbolErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.SymbolErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.SymbolErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SymbolErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.SymbolErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSymbolErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## TotalSupplyErc20

> TransactionAPIResponse TotalSupplyErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.TotalSupplyErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.TotalSupplyErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TotalSupplyErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.TotalSupplyErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiTotalSupplyErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## TransferErc20

> TransactionAPIResponse TransferErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.TransferErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.TransferErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TransferErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.TransferErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiTransferErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## TransferFromErc20

> TransactionAPIResponse TransferFromErc20(ctx, name).Authorization(authorization).InputBody(inputBody).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc20API.TransferFromErc20(context.Background(), name).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc20API.TransferFromErc20``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TransferFromErc20`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc20API.TransferFromErc20`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiTransferFromErc20Request struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc20api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
