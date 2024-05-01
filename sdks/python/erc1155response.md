# Erc1155Response

## Properties

| Name                    | Type           | Description | Notes       |
| ----------------------- | -------------- | ----------- | ----------- |
| **type**                | **float**      |             | \[optional] |
| **chain\_id**           | **float**      |             | \[optional] |
| **data**                | **str**        |             | \[optional] |
| **gas**                 | **str**        |             | \[optional] |
| **gas\_price**          | **str**        |             | \[optional] |
| **gas\_tip\_cap**       | **str**        |             | \[optional] |
| **gas\_fee\_cap**       | **str**        |             | \[optional] |
| **value**               | **str**        |             | \[optional] |
| **nonce**               | **float**      |             | \[optional] |
| **var\_from**           | **str**        |             | \[optional] |
| **to**                  | **str**        |             | \[optional] |
| **blob\_gas**           | **str**        |             | \[optional] |
| **blob\_gas\_fee\_cap** | **str**        |             | \[optional] |
| **blob\_hashes**        | **List\[str]** |             | \[optional] |
| **v**                   | **str**        |             | \[optional] |
| **r**                   | **str**        |             | \[optional] |
| **s**                   | **str**        |             | \[optional] |
| **balance\_of**         | **str**        |             | \[optional] |
| **balance\_of\_batch**  | **str**        |             | \[optional] |

## Example

```python
from moonsdk.models.erc1155_response import Erc1155Response

# TODO update the JSON string below
json = "{}"
# create an instance of Erc1155Response from a JSON string
erc1155_response_instance = Erc1155Response.from_json(json)
# print the JSON string representation of the object
print Erc1155Response.to_json()

# convert the object into a dict
erc1155_response_dict = erc1155_response_instance.to_dict()
# create an instance of Erc1155Response from a dict
erc1155_response_form_dict = erc1155_response.from_dict(erc1155_response_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
