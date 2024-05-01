# IWebhook

## Properties

| Name                  | Type                                                     | Description | Notes |
| --------------------- | -------------------------------------------------------- | ----------- | ----- |
| **block**             | [**Block**](block.md)                                    |             |       |
| **chainId**           | **String**                                               |             |       |
| **logs**              | [**List\<Log>**](log.md)                                 |             |       |
| **txs**               | [**List\<Transaction>**](transaction.md)                 |             |       |
| **txsInternal**       | [**List\<InternalTransaction>**](internaltransaction.md) |             |       |
| **abi**               | [**List\<AbiItem>**](abiitem.md)                         |             |       |
| **retries**           | **Double**                                               |             |       |
| **confirmed**         | **Boolean**                                              |             |       |
| **tag**               | **String**                                               |             |       |
| **streamId**          | **String**                                               |             |       |
| **erc20Transfers**    | [**List\<IERC20Transfer>**](ierc20transfer.md)           |             |       |
| **erc20Approvals**    | [**List\<IERC20Approval>**](ierc20approval.md)           |             |       |
| **nftTransfers**      | [**List\<INFTTransfer>**](infttransfer.md)               |             |       |
| **nativeBalances**    | [**List\<INativeBalance>**](inativebalance.md)           |             |       |
| **nftApprovals**      | [**IOldNFTApproval**](ioldnftapproval.md)                |             |       |
| **nftTokenApprovals** | [**List\<INFTApproval>**](inftapproval.md)               |             |       |
