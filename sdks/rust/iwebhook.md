# IWebhook

## Properties

| Name                      | Type                                                                                                           | Description | Notes |
| ------------------------- | -------------------------------------------------------------------------------------------------------------- | ----------- | ----- |
| **block**                 | [**crate::models::Block**](block.md)                                                                           |             |       |
| **chain\_id**             | **String**                                                                                                     |             |       |
| **logs**                  | [**Vec**](log.md)[**crate::models::Log**](crate::models::Log)                                                  |             |       |
| **txs**                   | [**Vec**](transaction.md)[**crate::models::Transaction**](crate::models::Transaction)                          |             |       |
| **txs\_internal**         | [**Vec**](internaltransaction.md)[**crate::models::InternalTransaction**](crate::models::InternalTransaction)  |             |       |
| **abi**                   | [**Vec**](abiitem.md)[**crate::models::AbiItem**](crate::models::AbiItem)                                      |             |       |
| **retries**               | **f64**                                                                                                        |             |       |
| **confirmed**             | **bool**                                                                                                       |             |       |
| **tag**                   | **String**                                                                                                     |             |       |
| **stream\_id**            | **String**                                                                                                     |             |       |
| **erc20\_transfers**      | [**Vec**](../../rust/docs/IERC20Transfer.md)[**crate::models::Ierc20Transfer**](crate::models::Ierc20Transfer) |             |       |
| **erc20\_approvals**      | [**Vec**](../../rust/docs/IERC20Approval.md)[**crate::models::Ierc20Approval**](crate::models::Ierc20Approval) |             |       |
| **nft\_transfers**        | [**Vec**](../../rust/docs/INFTTransfer.md)[**crate::models::InftTransfer**](crate::models::InftTransfer)       |             |       |
| **native\_balances**      | [**Vec**](inativebalance.md)[**crate::models::INativeBalance**](crate::models::INativeBalance)                 |             |       |
| **nft\_approvals**        | [**crate::models::IOldNftApproval**](../../rust/docs/IOldNFTApproval.md)                                       |             |       |
| **nft\_token\_approvals** | [**Vec**](../../rust/docs/INFTApproval.md)[**crate::models::InftApproval**](crate::models::InftApproval)       |             |       |

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
