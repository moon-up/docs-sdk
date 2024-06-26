# Log

## Properties

| Name                  | Type                                          | Description | Notes       |
| --------------------- | --------------------------------------------- | ----------- | ----------- |
| **triggers**          | [**List\[TriggerOutput\]**](triggeroutput.md) |             | \[optional] |
| **log\_index**        | **str**                                       |             |             |
| **transaction\_hash** | **str**                                       |             |             |
| **address**           | **str**                                       |             |             |
| **data**              | **str**                                       |             |             |
| **topic0**            | **str**                                       |             |             |
| **topic1**            | **str**                                       |             |             |
| **topic2**            | **str**                                       |             |             |
| **topic3**            | **str**                                       |             |             |

## Example

```python
from moonsdk.models.log import Log

# TODO update the JSON string below
json = "{}"
# create an instance of Log from a JSON string
log_instance = Log.from_json(json)
# print the JSON string representation of the object
print Log.to_json()

# convert the object into a dict
log_dict = log_instance.to_dict()
# create an instance of Log from a dict
log_form_dict = log.from_dict(log_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
