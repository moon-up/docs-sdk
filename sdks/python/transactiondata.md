# TransactionData

## Properties

| Name                    | Type                                                    | Description | Notes       |
| ----------------------- | ------------------------------------------------------- | ----------- | ----------- |
| **moon\_scan\_url**     | **str**                                                 |             | \[optional] |
| **transaction\_hash**   | **str**                                                 |             |             |
| **signed\_transaction** | **str**                                                 |             |             |
| **signed\_message**     | **str**                                                 |             | \[optional] |
| **raw\_transaction**    | **str**                                                 |             | \[optional] |
| **signature**           | **str**                                                 |             | \[optional] |
| **transaction**         | [**Tx**](tx.md)                                         |             | \[optional] |
| **user\_ops**           | [**List\[TransactionRequest\]**](transactionrequest.md) |             | \[optional] |
| **userop\_transaction** | **str**                                                 |             | \[optional] |

## Example

```python
from moonsdk.models.transaction_data import TransactionData

# TODO update the JSON string below
json = "{}"
# create an instance of TransactionData from a JSON string
transaction_data_instance = TransactionData.from_json(json)
# print the JSON string representation of the object
print(TransactionData.to_json())

# convert the object into a dict
transaction_data_dict = transaction_data_instance.to_dict()
# create an instance of TransactionData from a dict
transaction_data_form_dict = transaction_data.from_dict(transaction_data_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
