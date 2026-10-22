# OrganisationsAppointSroRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | ID of the claimed member to appoint | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_appoint_sro_request import OrganisationsAppointSroRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsAppointSroRequest from a JSON string
organisations_appoint_sro_request_instance = OrganisationsAppointSroRequest.from_json(json)
# print the JSON string representation of the object
print(OrganisationsAppointSroRequest.to_json())

# convert the object into a dict
organisations_appoint_sro_request_dict = organisations_appoint_sro_request_instance.to_dict()
# create an instance of OrganisationsAppointSroRequest from a dict
organisations_appoint_sro_request_from_dict = OrganisationsAppointSroRequest.from_dict(organisations_appoint_sro_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


