# IWebhook

## Properties

| Name                      | Type                                                      | Description | Notes |
| ------------------------- | --------------------------------------------------------- | ----------- | ----- |
| **block**                 | [**Block**](block.md)                                     |             |       |
| **chain\_id**             | **str**                                                   |             |       |
| **logs**                  | [**List\[Log\]**](log.md)                                 |             |       |
| **txs**                   | [**List\[Transaction\]**](transaction.md)                 |             |       |
| **txs\_internal**         | [**List\[InternalTransaction\]**](internaltransaction.md) |             |       |
| **abi**                   | [**List\[AbiItem\]**](abiitem.md)                         |             |       |
| **retries**               | **float**                                                 |             |       |
| **confirmed**             | **bool**                                                  |             |       |
| **tag**                   | **str**                                                   |             |       |
| **stream\_id**            | **str**                                                   |             |       |
| **erc20\_transfers**      | [**List\[IERC20Transfer\]**](ierc20transfer.md)           |             |       |
| **erc20\_approvals**      | [**List\[IERC20Approval\]**](ierc20approval.md)           |             |       |
| **nft\_transfers**        | [**List\[INFTTransfer\]**](infttransfer.md)               |             |       |
| **native\_balances**      | [**List\[INativeBalance\]**](inativebalance.md)           |             |       |
| **nft\_approvals**        | [**IOldNFTApproval**](ioldnftapproval.md)                 |             |       |
| **nft\_token\_approvals** | [**List\[INFTApproval\]**](inftapproval.md)               |             |       |

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
