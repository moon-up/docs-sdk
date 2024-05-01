# \OneinchAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method              | HTTP request                         | Description |
| ------------------- | ------------------------------------ | ----------- |
| **ApproveCallData** | **Post** /oneinch/approve-call-data  |             |
| **ApproveSpender**  | **Post** /oneinch/approve-spender    |             |
| **Protocols**       | **Post** /oneinch/protocols          |             |
| **Quote**           | **Post** /oneinch/quote              |             |
| **Swap**            | **Post** /oneinch/{accountName}/swap |             |
| **Tokens**          | **Post** /oneinch/tokens             |             |

## ApproveCallData

> interface{} ApproveCallData(ctx).Body(body).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	body := interface{}(987) // interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OneinchAPI.ApproveCallData(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OneinchAPI.ApproveCallData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApproveCallData`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `OneinchAPI.ApproveCallData`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiApproveCallDataRequest struct via the builder pattern

| Name     | Type            | Description | Notes |
| -------- | --------------- | ----------- | ----- |
| **body** | **interface{}** |             |       |

### Return type

**interface{}**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## ApproveSpender

> interface{} ApproveSpender(ctx).Body(body).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	body := interface{}(987) // interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OneinchAPI.ApproveSpender(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OneinchAPI.ApproveSpender``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApproveSpender`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `OneinchAPI.ApproveSpender`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiApproveSpenderRequest struct via the builder pattern

| Name     | Type            | Description | Notes |
| -------- | --------------- | ----------- | ----- |
| **body** | **interface{}** |             |       |

### Return type

**interface{}**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## Protocols

> interface{} Protocols(ctx).Body(body).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	body := interface{}(987) // interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OneinchAPI.Protocols(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OneinchAPI.Protocols``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Protocols`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `OneinchAPI.Protocols`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiProtocolsRequest struct via the builder pattern

| Name     | Type            | Description | Notes |
| -------- | --------------- | ----------- | ----- |
| **body** | **interface{}** |             |       |

### Return type

**interface{}**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## Quote

> interface{} Quote(ctx).Body(body).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	body := interface{}(987) // interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OneinchAPI.Quote(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OneinchAPI.Quote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Quote`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `OneinchAPI.Quote`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiQuoteRequest struct via the builder pattern

| Name     | Type            | Description | Notes |
| -------- | --------------- | ----------- | ----- |
| **body** | **interface{}** |             |       |

### Return type

**interface{}**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## Swap

> interface{} Swap(ctx, accountName).Authorization(authorization).GetSwapDto(getSwapDto).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	accountName := "accountName_example" // string | 
	authorization := "authorization_example" // string | 
	getSwapDto := *openapiclient.NewGetSwapDto("Src_example", "Dst_example", "Amount_example", "From_example", float64(123)) // GetSwapDto | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OneinchAPI.Swap(context.Background(), accountName).Authorization(authorization).GetSwapDto(getSwapDto).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OneinchAPI.Swap``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Swap`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `OneinchAPI.Swap`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSwapRequest struct via the builder pattern

**authorization** | **string** | | **getSwapDto** | **GetSwapDto** | |

### Return type

**interface{}**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## Tokens

> interface{} Tokens(ctx).Body(body).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	body := interface{}(987) // interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OneinchAPI.Tokens(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OneinchAPI.Tokens``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Tokens`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `OneinchAPI.Tokens`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiTokensRequest struct via the builder pattern

| Name     | Type            | Description | Notes |
| -------- | --------------- | ----------- | ----- |
| **body** | **interface{}** |             |       |

### Return type

**interface{}**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
