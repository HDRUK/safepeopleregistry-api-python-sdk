# AccreditationIndexByRegistryId200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[Accreditation]**](Accreditation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.accreditation_index_by_registry_id200_response import AccreditationIndexByRegistryId200Response

# TODO update the JSON string below
json = "{}"
# create an instance of AccreditationIndexByRegistryId200Response from a JSON string
accreditation_index_by_registry_id200_response_instance = AccreditationIndexByRegistryId200Response.from_json(json)
# print the JSON string representation of the object
print(AccreditationIndexByRegistryId200Response.to_json())

# convert the object into a dict
accreditation_index_by_registry_id200_response_dict = accreditation_index_by_registry_id200_response_instance.to_dict()
# create an instance of AccreditationIndexByRegistryId200Response from a dict
accreditation_index_by_registry_id200_response_from_dict = AccreditationIndexByRegistryId200Response.from_dict(accreditation_index_by_registry_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


