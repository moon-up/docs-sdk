# SellQuote

## Properties

| Name                 | Type           | Description | Notes |
| -------------------- | -------------- | ----------- | ----- |
| **recommendations**  | **List\[str]** |             |       |
| **quote\_id**        | **str**        |             |       |
| **payment\_method**  | **str**        |             |       |
| **ramp**             | **str**        |             |       |
| **payout**           | **float**      |             |       |
| **transaction\_fee** | **float**      |             |       |
| **network\_fee**     | **float**      |             |       |
| **rate**             | **float**      |             |       |

## Example

```python
from moonsdk.models.sell_quote import SellQuote

# TODO update the JSON string below
json = "{}"
# create an instance of SellQuote from a JSON string
sell_quote_instance = SellQuote.from_json(json)
# print the JSON string representation of the object
print(SellQuote.to_json())

# convert the object into a dict
sell_quote_dict = sell_quote_instance.to_dict()
# create an instance of SellQuote from a dict
sell_quote_form_dict = sell_quote.from_dict(sell_quote_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
