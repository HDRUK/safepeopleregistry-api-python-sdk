# RegistryIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Registry**](Registry.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_index200_response import RegistryIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryIndex200Response from a JSON string
registry_index200_response_instance = RegistryIndex200Response.from_json(json)
# print the JSON string representation of the object
print(RegistryIndex200Response.to_json())

# convert the object into a dict
registry_index200_response_dict = registry_index200_response_instance.to_dict()
# create an instance of RegistryIndex200Response from a dict
registry_index200_response_from_dict = RegistryIndex200Response.from_dict(registry_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


