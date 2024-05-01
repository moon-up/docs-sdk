# DeployInput

## Properties

| Name                  | Type    | Description | Notes       |
| --------------------- | ------- | ----------- | ----------- |
| **chain\_id**         | **str** |             | \[optional] |
| **abi**               | **str** |             |             |
| **bytecode**          | **str** |             |             |
| **constructor\_args** | **str** |             | \[optional] |

## Example

```python
from moonsdk.models.deploy_input import DeployInput

# TODO update the JSON string below
json = "{}"
# create an instance of DeployInput from a JSON string
deploy_input_instance = DeployInput.from_json(json)
# print the JSON string representation of the object
print(DeployInput.to_json())

# convert the object into a dict
deploy_input_dict = deploy_input_instance.to_dict()
# create an instance of DeployInput from a dict
deploy_input_form_dict = deploy_input.from_dict(deploy_input_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
