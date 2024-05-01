# \DefaultAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method         | HTTP request  | Description |
| -------------- | ------------- | ----------- |
| **GetMessage** | **Get** /ping |             |

## GetMessage

> PingResponse GetMessage(ctx).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultAPI.GetMessage(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultAPI.GetMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMessage`: PingResponse
	fmt.Fprintf(os.Stdout, "Response from `DefaultAPI.GetMessage`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetMessageRequest struct via the builder pattern

### Return type

**PingResponse**

### Authorization

No authorization required

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
