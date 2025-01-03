# TransactionAPIResponse
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **success** | **Boolean** | The success status of the operation. | [default to null] |
| **message** | **String** | The message associated with the operation. | [default to null] |
| **body** | [**InputBody**](InputBody.md) |  | [optional] [default to null] |
| **address** | **String** | The address associated with the operation. | [optional] [default to null] |
| **transaction\_hash** | [**oas_any_type_not_mapped**](.md) | The hash of the transaction. | [optional] [default to null] |
| **signedTx** | [**oas_any_type_not_mapped**](.md) | The signed transaction data. | [optional] [default to null] |
| **data** | [**Transaction**](Transaction.md) |  | [optional] [default to null] |
| **broadcasted** | [**BroadCastRawTransactionResponse**](BroadCastRawTransactionResponse.md) |  | [optional] [default to null] |
| **transaction** | [**oas_any_type_not_mapped**](.md) | Additional transaction information. | [optional] [default to null] |
| **function** | **String** | The function name associated with the transaction. | [optional] [default to null] |
| **params** | [**List**](AnyType.md) | The parameters associated with the transaction function. | [optional] [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

