# RegistryUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Registry**](Registry.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_update200_response import RegistryUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryUpdate200Response from a JSON string
registry_update200_response_instance = RegistryUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(RegistryUpdate200Response.to_json())

# convert the object into a dict
registry_update200_response_dict = registry_update200_response_instance.to_dict()
# create an instance of RegistryUpdate200Response from a dict
registry_update200_response_from_dict = RegistryUpdate200Response.from_dict(registry_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


