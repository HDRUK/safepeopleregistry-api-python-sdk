# RegistryHasProfessionalRegistration

Pivot model representing the relationship between registries and professional registrations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the registry-professional registration relationship | [optional] 
**registry_id** | **int** | ID of the registry | [optional] 
**professional_registration_id** | **int** | ID of the professional registration | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_has_professional_registration import RegistryHasProfessionalRegistration

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryHasProfessionalRegistration from a JSON string
registry_has_professional_registration_instance = RegistryHasProfessionalRegistration.from_json(json)
# print the JSON string representation of the object
print(RegistryHasProfessionalRegistration.to_json())

# convert the object into a dict
registry_has_professional_registration_dict = registry_has_professional_registration_instance.to_dict()
# create an instance of RegistryHasProfessionalRegistration from a dict
registry_has_professional_registration_from_dict = RegistryHasProfessionalRegistration.from_dict(registry_has_professional_registration_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


