# ProfessionalRegistrationsUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**member_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.professional_registrations_update_request import ProfessionalRegistrationsUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ProfessionalRegistrationsUpdateRequest from a JSON string
professional_registrations_update_request_instance = ProfessionalRegistrationsUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(ProfessionalRegistrationsUpdateRequest.to_json())

# convert the object into a dict
professional_registrations_update_request_dict = professional_registrations_update_request_instance.to_dict()
# create an instance of ProfessionalRegistrationsUpdateRequest from a dict
professional_registrations_update_request_from_dict = ProfessionalRegistrationsUpdateRequest.from_dict(professional_registrations_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


