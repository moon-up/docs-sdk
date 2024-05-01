# IWebhook

## Properties

| Name                      | Type                                                                                                          | Description | Notes |
| ------------------------- | ------------------------------------------------------------------------------------------------------------- | ----------- | ----- |
| **block**                 | [**crate::models::Block**](Block.md)                                                                          |             |       |
| **chain\_id**             | **String**                                                                                                    |             |       |
| **logs**                  | [**Vec**](Log.md)[**crate::models::Log**](crate::models::Log)                                                 |             |       |
| **txs**                   | [**Vec**](Transaction.md)[**crate::models::Transaction**](crate::models::Transaction)                         |             |       |
| **txs\_internal**         | [**Vec**](InternalTransaction.md)[**crate::models::InternalTransaction**](crate::models::InternalTransaction) |             |       |
| **abi**                   | [**Vec**](AbiItem.md)[**crate::models::AbiItem**](crate::models::AbiItem)                                     |             |       |
| **retries**               | **f64**                                                                                                       |             |       |
| **confirmed**             | **bool**                                                                                                      |             |       |
| **tag**                   | **String**                                                                                                    |             |       |
| **stream\_id**            | **String**                                                                                                    |             |       |
| **erc20\_transfers**      | [**Vec**](docs/IERC20Transfer.md)[**crate::models::Ierc20Transfer**](crate::models::Ierc20Transfer)           |             |       |
| **erc20\_approvals**      | [**Vec**](docs/IERC20Approval.md)[**crate::models::Ierc20Approval**](crate::models::Ierc20Approval)           |             |       |
| **nft\_transfers**        | [**Vec**](docs/INFTTransfer.md)[**crate::models::InftTransfer**](crate::models::InftTransfer)                 |             |       |
| **native\_balances**      | [**Vec**](INativeBalance.md)[**crate::models::INativeBalance**](crate::models::INativeBalance)                |             |       |
| **nft\_approvals**        | [**crate::models::IOldNftApproval**](docs/IOldNFTApproval.md)                                                 |             |       |
| **nft\_token\_approvals** | [**Vec**](docs/INFTApproval.md)[**crate::models::InftApproval**](crate::models::InftApproval)                 |             |       |

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
