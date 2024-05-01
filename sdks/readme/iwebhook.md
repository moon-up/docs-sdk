# openapi.model.IWebhook

## Load the model package

```dart
import 'package:openapi/api.dart';
```

## Properties

| Name                  | Type                                                          | Description | Notes |
| --------------------- | ------------------------------------------------------------- | ----------- | ----- |
| **block**             | [**Block**](block.md)                                         |             |       |
| **chainId**           | **String**                                                    |             |       |
| **logs**              | [**BuiltList\<Log>**](log.md)                                 |             |       |
| **txs**               | [**BuiltList\<Transaction>**](transaction.md)                 |             |       |
| **txsInternal**       | [**BuiltList\<InternalTransaction>**](internaltransaction.md) |             |       |
| **abi**               | [**BuiltList\<AbiItem>**](abiitem.md)                         |             |       |
| **retries**           | **double**                                                    |             |       |
| **confirmed**         | **bool**                                                      |             |       |
| **tag**               | **String**                                                    |             |       |
| **streamId**          | **String**                                                    |             |       |
| **erc20Transfers**    | [**BuiltList\<IERC20Transfer>**](ierc20transfer.md)           |             |       |
| **erc20Approvals**    | [**BuiltList\<IERC20Approval>**](ierc20approval.md)           |             |       |
| **nftTransfers**      | [**BuiltList\<INFTTransfer>**](infttransfer.md)               |             |       |
| **nativeBalances**    | [**BuiltList\<INativeBalance>**](inativebalance.md)           |             |       |
| **nftApprovals**      | [**IOldNFTApproval**](ioldnftapproval.md)                     |             |       |
| **nftTokenApprovals** | [**BuiltList\<INFTApproval>**](inftapproval.md)               |             |       |

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
