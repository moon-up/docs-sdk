# Erc721Response

## Properties

| Name                       | Type           | Description | Notes       |
| -------------------------- | -------------- | ----------- | ----------- |
| **type**                   | **float**      |             | \[optional] |
| **chain\_id**              | **float**      |             | \[optional] |
| **data**                   | **str**        |             | \[optional] |
| **gas**                    | **str**        |             | \[optional] |
| **gas\_price**             | **str**        |             | \[optional] |
| **gas\_tip\_cap**          | **str**        |             | \[optional] |
| **gas\_fee\_cap**          | **str**        |             | \[optional] |
| **value**                  | **str**        |             | \[optional] |
| **nonce**                  | **float**      |             | \[optional] |
| **var\_from**              | **str**        |             | \[optional] |
| **to**                     | **str**        |             | \[optional] |
| **blob\_gas**              | **str**        |             | \[optional] |
| **blob\_gas\_fee\_cap**    | **str**        |             | \[optional] |
| **blob\_hashes**           | **List\[str]** |             | \[optional] |
| **v**                      | **str**        |             | \[optional] |
| **r**                      | **str**        |             | \[optional] |
| **s**                      | **str**        |             | \[optional] |
| **name**                   | **str**        |             | \[optional] |
| **symbol**                 | **str**        |             | \[optional] |
| **balance\_of**            | **str**        |             | \[optional] |
| **owner\_of**              | **str**        |             | \[optional] |
| **token\_uri**             | **str**        |             | \[optional] |
| **contract\_address**      | **str**        |             | \[optional] |
| **is\_approved\_for\_all** | **str**        |             | \[optional] |

## Example

```python
from moonsdk.models.erc721_response import Erc721Response

# TODO update the JSON string below
json = "{}"
# create an instance of Erc721Response from a JSON string
erc721_response_instance = Erc721Response.from_json(json)
# print the JSON string representation of the object
print Erc721Response.to_json()

# convert the object into a dict
erc721_response_dict = erc721_response_instance.to_dict()
# create an instance of Erc721Response from a dict
erc721_response_form_dict = erc721_response.from_dict(erc721_response_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
