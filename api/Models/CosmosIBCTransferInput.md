# CosmosIBCTransferInput
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **fromAddress** | **String** | The address from which the transfer is initiated. | [default to null] |
| **toAddress** | **String** | The address to which the transfer is sent. | [default to null] |
| **amount** | **String** | The amount of tokens to be transferred. | [default to null] |
| **denom** | **String** | The denomination of the tokens to be transferred. | [default to null] |
| **chainId** | **String** | The ID of the blockchain chain. | [default to null] |
| **sequence** | **Double** | The sequence number of the account initiating the transfer. | [default to null] |
| **accountNumber** | **Double** | The account number of the account initiating the transfer. | [default to null] |
| **feeDenom** | **String** | The denomination of the fee to be paid for the transfer. | [default to null] |
| **feeAmount** | **String** | The amount of the fee to be paid for the transfer. | [default to null] |
| **gasLimit** | **Double** | The gas limit for the transfer transaction. | [default to null] |
| **memo** | **String** | An optional memo to include with the transfer. | [default to null] |
| **timeoutHeight** | **Double** | The timeout height for the transfer transaction. | [default to null] |
| **sourcePort** | **String** | The source port for the IBC transfer. | [default to null] |
| **sourceChannel** | **String** | The source channel for the IBC transfer. | [default to null] |
| **timeoutTimestamp** | **Double** | The timeout timestamp for the IBC transfer, specified in nanoseconds. | [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

