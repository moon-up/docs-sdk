# IWebhook

## Properties

| Name                      | Type                                                      | Description | Notes |
| ------------------------- | --------------------------------------------------------- | ----------- | ----- |
| **block**                 | [**Block**](Block.md)                                     |             |       |
| **chain\_id**             | **str**                                                   |             |       |
| **logs**                  | [**List\[Log\]**](Log.md)                                 |             |       |
| **txs**                   | [**List\[Transaction\]**](Transaction.md)                 |             |       |
| **txs\_internal**         | [**List\[InternalTransaction\]**](InternalTransaction.md) |             |       |
| **abi**                   | [**List\[AbiItem\]**](AbiItem.md)                         |             |       |
| **retries**               | **float**                                                 |             |       |
| **confirmed**             | **bool**                                                  |             |       |
| **tag**                   | **str**                                                   |             |       |
| **stream\_id**            | **str**                                                   |             |       |
| **erc20\_transfers**      | [**List\[IERC20Transfer\]**](IERC20Transfer.md)           |             |       |
| **erc20\_approvals**      | [**List\[IERC20Approval\]**](IERC20Approval.md)           |             |       |
| **nft\_transfers**        | [**List\[INFTTransfer\]**](INFTTransfer.md)               |             |       |
| **native\_balances**      | [**List\[INativeBalance\]**](INativeBalance.md)           |             |       |
| **nft\_approvals**        | [**IOldNFTApproval**](IOldNFTApproval.md)                 |             |       |
| **nft\_token\_approvals** | [**List\[INFTApproval\]**](INFTApproval.md)               |             |       |

## Example

```python
from moonsdk.models.i_webhook import IWebhook

# TODO update the JSON string below
json = "{}"
# create an instance of IWebhook from a JSON string
i_webhook_instance = IWebhook.from_json(json)
# print the JSON string representation of the object
print IWebhook.to_json()

# convert the object into a dict
i_webhook_dict = i_webhook_instance.to_dict()
# create an instance of IWebhook from a dict
i_webhook_form_dict = i_webhook.from_dict(i_webhook_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
