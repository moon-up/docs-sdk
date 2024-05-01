# TatumTransactionEvent

## Properties

| Name                   | Type      | Description | Notes |
| ---------------------- | --------- | ----------- | ----- |
| **amount**             | **str**   |             |       |
| **test**               | **bool**  |             |       |
| **counter\_address**   | **str**   |             |       |
| **address**            | **str**   |             |       |
| **mempool**            | **bool**  |             |       |
| **subscription\_type** | **str**   |             |       |
| **block\_number**      | **float** |             |       |
| **tx\_id**             | **str**   |             |       |
| **chain**              | **str**   |             |       |
| **currency**           | **str**   |             |       |

## Example

```python
from moonsdk.models.tatum_transaction_event import TatumTransactionEvent

# TODO update the JSON string below
json = "{}"
# create an instance of TatumTransactionEvent from a JSON string
tatum_transaction_event_instance = TatumTransactionEvent.from_json(json)
# print the JSON string representation of the object
print TatumTransactionEvent.to_json()

# convert the object into a dict
tatum_transaction_event_dict = tatum_transaction_event_instance.to_dict()
# create an instance of TatumTransactionEvent from a dict
tatum_transaction_event_form_dict = tatum_transaction_event.from_dict(tatum_transaction_event_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
