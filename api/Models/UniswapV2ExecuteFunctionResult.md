# UniswapV2ExecuteFunctionResult
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **simulation** | [**SimulateAssetChangesResponse**](SimulateAssetChangesResponse.md) |  | [optional] [default to null] |
| **broadcasted** | [**BroadCastRawTransactionResponse**](BroadCastRawTransactionResponse.md) |  | [optional] [default to null] |
| **message** | **String** | The broadcasted result of the transaction. | [optional] [default to null] |
| **success** | **Boolean** | The message returned by the API. | [optional] [default to null] |
| **user\_op** | **String** | Indicates whether the function was successful. | [optional] [default to null] |
| **data** | [**Transaction**](Transaction.md) |  | [optional] [default to null] |
| **params** | [**List**](AnyType.md) | The parameters passed to the function. | [default to null] |
| **function** | **String** | The name of the function executed. | [default to null] |
| **transaction** | [**UniswapV2Transaction**](UniswapV2Transaction.md) |  | [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

