# AccreditationUpdateByRegistryId200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Accreditation**](Accreditation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.accreditation_update_by_registry_id200_response import AccreditationUpdateByRegistryId200Response

# TODO update the JSON string below
json = "{}"
# create an instance of AccreditationUpdateByRegistryId200Response from a JSON string
accreditation_update_by_registry_id200_response_instance = AccreditationUpdateByRegistryId200Response.from_json(json)
# print the JSON string representation of the object
print(AccreditationUpdateByRegistryId200Response.to_json())

# convert the object into a dict
accreditation_update_by_registry_id200_response_dict = accreditation_update_by_registry_id200_response_instance.to_dict()
# create an instance of AccreditationUpdateByRegistryId200Response from a dict
accreditation_update_by_registry_id200_response_from_dict = AccreditationUpdateByRegistryId200Response.from_dict(accreditation_update_by_registry_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


