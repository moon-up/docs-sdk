# EvmWalletHistoryTransactionJSON
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **hash** | **String** |  | [default to null] |
| **nonce** | **String** |  | [default to null] |
| **transaction\_index** | **String** |  | [default to null] |
| **from\_address\_entity** | **String** |  | [optional] [default to null] |
| **from\_address\_entity\_logo** | **String** |  | [optional] [default to null] |
| **from\_address** | **String** |  | [default to null] |
| **from\_address\_label** | **String** |  | [optional] [default to null] |
| **to\_address\_entity** | **String** |  | [optional] [default to null] |
| **to\_address\_entity\_logo** | **String** |  | [optional] [default to null] |
| **to\_address** | **String** |  | [optional] [default to null] |
| **to\_address\_label** | **String** |  | [optional] [default to null] |
| **value** | **String** |  | [default to null] |
| **gas** | **String** |  | [optional] [default to null] |
| **gas\_price** | **String** |  | [default to null] |
| **input** | **String** |  | [optional] [default to null] |
| **receipt\_cumulative\_gas\_used** | **String** |  | [default to null] |
| **receipt\_gas\_used** | **String** |  | [default to null] |
| **receipt\_contract\_address** | **String** |  | [optional] [default to null] |
| **receipt\_status** | **String** |  | [default to null] |
| **transaction\_fee** | **String** |  | [optional] [default to null] |
| **block\_timestamp** | **String** |  | [default to null] |
| **block\_number** | **String** |  | [default to null] |
| **block\_hash** | **String** |  | [default to null] |
| **internal\_transactions** | [**List**](EvmInternalTransactionJSON.md) |  | [optional] [default to null] |
| **category** | [**EvmETransactionCategoryJSON**](EvmETransactionCategoryJSON.md) |  | [default to null] |
| **contract\_interactions** | [**EvmResolveContractInteractionResponseJSON**](EvmResolveContractInteractionResponseJSON.md) |  | [optional] [default to null] |
| **possible\_spam** | **Boolean** |  | [optional] [default to null] |
| **method\_label** | **String** |  | [optional] [default to null] |
| **summary** | **String** |  | [default to null] |
| **nft\_transfers** | [**List**](EvmWalletHistoryNftTransferJSON.md) |  | [default to null] |
| **erc20\_transfers** | [**List**](EvmWalletHistoryErc20TransferJSON.md) |  | [default to null] |
| **native\_transfers** | [**List**](EvmNativeTransferJSON.md) |  | [default to null] |
| **logs** | [**List**](EvmLogVerboseJSON.md) |  | [optional] [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

