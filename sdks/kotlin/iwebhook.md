# IWebhook

## Properties

| Name                  | Type                                                                        | Description | Notes |
| --------------------- | --------------------------------------------------------------------------- | ----------- | ----- |
| **block**             | [**Block**](block.md)                                                       |             |       |
| **chainId**           | **kotlin.String**                                                           |             |       |
| **logs**              | [**kotlin.collections.List\<Log>**](log.md)                                 |             |       |
| **txs**               | [**kotlin.collections.List\<Transaction>**](transaction.md)                 |             |       |
| **txsInternal**       | [**kotlin.collections.List\<InternalTransaction>**](internaltransaction.md) |             |       |
| **abi**               | [**kotlin.collections.List\<AbiItem>**](abiitem.md)                         |             |       |
| **retries**           | **kotlin.Double**                                                           |             |       |
| **confirmed**         | **kotlin.Boolean**                                                          |             |       |
| **tag**               | **kotlin.String**                                                           |             |       |
| **streamId**          | **kotlin.String**                                                           |             |       |
| **erc20Transfers**    | [**kotlin.collections.List\<IERC20Transfer>**](ierc20transfer.md)           |             |       |
| **erc20Approvals**    | [**kotlin.collections.List\<IERC20Approval>**](ierc20approval.md)           |             |       |
| **nftTransfers**      | [**kotlin.collections.List\<INFTTransfer>**](infttransfer.md)               |             |       |
| **nativeBalances**    | [**kotlin.collections.List\<INativeBalance>**](inativebalance.md)           |             |       |
| **nftApprovals**      | [**IOldNFTApproval**](ioldnftapproval.md)                                   |             |       |
| **nftTokenApprovals** | [**kotlin.collections.List\<INFTApproval>**](inftapproval.md)               |             |       |
