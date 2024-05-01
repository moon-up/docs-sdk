# AaveInput

## Properties

| Name                     | Type     | Description | Notes       |
| ------------------------ | -------- | ----------- | ----------- |
| **to**                   | **str**  |             | \[optional] |
| **data**                 | **str**  |             | \[optional] |
| **input**                | **str**  |             | \[optional] |
| **value**                | **str**  |             | \[optional] |
| **nonce**                | **str**  |             | \[optional] |
| **gas**                  | **str**  |             | \[optional] |
| **gas\_price**           | **str**  |             | \[optional] |
| **chain\_id**            | **str**  |             | \[optional] |
| **encoding**             | **str**  |             | \[optional] |
| **eoa**                  | **bool** |             | \[optional] |
| **contract\_address**    | **str**  |             | \[optional] |
| **token\_id**            | **str**  |             | \[optional] |
| **token\_ids**           | **str**  |             | \[optional] |
| **approved**             | **bool** |             | \[optional] |
| **broadcast**            | **bool** |             | \[optional] |
| **lending\_pool**        | **str**  |             | \[optional] |
| **amount**               | **str**  |             | \[optional] |
| **atoken\_to\_redeeem**  | **str**  |             | \[optional] |
| **ref\_code**            | **str**  |             | \[optional] |
| **interest\_rate\_mode** | **str**  |             | \[optional] |

## Example

```python
from moonsdk.models.aave_input import AaveInput

# TODO update the JSON string below
json = "{}"
# create an instance of AaveInput from a JSON string
aave_input_instance = AaveInput.from_json(json)
# print the JSON string representation of the object
print(AaveInput.to_json())

# convert the object into a dict
aave_input_dict = aave_input_instance.to_dict()
# create an instance of AaveInput from a dict
aave_input_form_dict = aave_input.from_dict(aave_input_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
