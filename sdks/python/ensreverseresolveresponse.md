# ENSReverseResolveResponse

## Properties

| Name       | Type    | Description | Notes |
| ---------- | ------- | ----------- | ----- |
| **domain** | **str** |             |       |

## Example

```python
from moonsdk.models.ens_reverse_resolve_response import ENSReverseResolveResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ENSReverseResolveResponse from a JSON string
ens_reverse_resolve_response_instance = ENSReverseResolveResponse.from_json(json)
# print the JSON string representation of the object
print ENSReverseResolveResponse.to_json()

# convert the object into a dict
ens_reverse_resolve_response_dict = ens_reverse_resolve_response_instance.to_dict()
# create an instance of ENSReverseResolveResponse from a dict
ens_reverse_resolve_response_form_dict = ens_reverse_resolve_response.from_dict(ens_reverse_resolve_response_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
