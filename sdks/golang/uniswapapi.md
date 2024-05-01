# \UniSwapAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                       | HTTP request                                          | Description |
| ---------------------------- | ----------------------------------------------------- | ----------- |
| **AddLiquidity**             | **Post** /uniswap/{name}/add-liquidity                |             |
| **RemoveLiquidity**          | **Post** /uniswap/{name}/remove-liquidity             |             |
| **SwapExactETHForTokens**    | **Post** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| **SwapExactTokensForTokens** | **Post** /uniswap/{name}/swap-exact-tokens-for-tokens |             |

## AddLiquidity

> TransactionAPIResponse AddLiquidity(ctx, name).Authorization(authorization).UniswapInput(uniswapInput).Execute()

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
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	uniswapInput := *openapiclient.NewUniswapInput() // UniswapInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UniSwapAPI.AddLiquidity(context.Background(), name).Authorization(authorization).UniswapInput(uniswapInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UniSwapAPI.AddLiquidity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddLiquidity`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `UniSwapAPI.AddLiquidity`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiAddLiquidityRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**uniswapInput** | **UniswapInput** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## RemoveLiquidity

> TransactionAPIResponse RemoveLiquidity(ctx, name).Authorization(authorization).UniswapInput(uniswapInput).Execute()

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
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	uniswapInput := *openapiclient.NewUniswapInput() // UniswapInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UniSwapAPI.RemoveLiquidity(context.Background(), name).Authorization(authorization).UniswapInput(uniswapInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UniSwapAPI.RemoveLiquidity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RemoveLiquidity`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `UniSwapAPI.RemoveLiquidity`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveLiquidityRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**uniswapInput** | **UniswapInput** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## SwapExactETHForTokens

> TransactionAPIResponse SwapExactETHForTokens(ctx, name).Authorization(authorization).UniswapInput(uniswapInput).Execute()

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
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	uniswapInput := *openapiclient.NewUniswapInput() // UniswapInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UniSwapAPI.SwapExactETHForTokens(context.Background(), name).Authorization(authorization).UniswapInput(uniswapInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UniSwapAPI.SwapExactETHForTokens``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SwapExactETHForTokens`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `UniSwapAPI.SwapExactETHForTokens`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSwapExactETHForTokensRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**uniswapInput** | **UniswapInput** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## SwapExactTokensForTokens

> TransactionAPIResponse SwapExactTokensForTokens(ctx, name).Authorization(authorization).UniswapInput(uniswapInput).Execute()

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
	authorization := "authorization_example" // string | 
	name := "name_example" // string | 
	uniswapInput := *openapiclient.NewUniswapInput() // UniswapInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UniSwapAPI.SwapExactTokensForTokens(context.Background(), name).Authorization(authorization).UniswapInput(uniswapInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UniSwapAPI.SwapExactTokensForTokens``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SwapExactTokensForTokens`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `UniSwapAPI.SwapExactTokensForTokens`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSwapExactTokensForTokensRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**uniswapInput** | **UniswapInput** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
