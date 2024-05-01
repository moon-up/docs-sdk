# Quote

## Properties

| Name                            | Type                                                            | Description | Notes |
| ------------------------------- | --------------------------------------------------------------- | ----------- | ----- |
| **recommendations**             | **List\[str]**                                                  |             |       |
| **payment\_method**             | **str**                                                         |             |       |
| **quote\_id**                   | **str**                                                         |             |       |
| **ramp**                        | **str**                                                         |             |       |
| **available\_payment\_methods** | [**List\[AvailablePaymentMethod\]**](AvailablePaymentMethod.md) |             |       |
| **payout**                      | **float**                                                       |             |       |
| **transaction\_fee**            | **float**                                                       |             |       |
| **network\_fee**                | **float**                                                       |             |       |
| **rate**                        | **float**                                                       |             |       |

## Example

```python
from moonsdk.models.quote import Quote

# TODO update the JSON string below
json = "{}"
# create an instance of Quote from a JSON string
quote_instance = Quote.from_json(json)
# print the JSON string representation of the object
print(Quote.to_json())

# convert the object into a dict
quote_dict = quote_instance.to_dict()
# create an instance of Quote from a dict
quote_form_dict = quote.from_dict(quote_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
