# ProfessionalRegistration

Model representing professional registrations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the professional registration | [optional] 
**member_id** | **str** | Member ID associated with the professional registration | [optional] 
**name** | **str** | Name of the professional registration | [optional] 
**created_at** | **datetime** | Timestamp when the professional registration was created | [optional] 
**updated_at** | **datetime** | Timestamp when the professional registration was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.professional_registration import ProfessionalRegistration

# TODO update the JSON string below
json = "{}"
# create an instance of ProfessionalRegistration from a JSON string
professional_registration_instance = ProfessionalRegistration.from_json(json)
# print the JSON string representation of the object
print(ProfessionalRegistration.to_json())

# convert the object into a dict
professional_registration_dict = professional_registration_instance.to_dict()
# create an instance of ProfessionalRegistration from a dict
professional_registration_from_dict = ProfessionalRegistration.from_dict(professional_registration_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


