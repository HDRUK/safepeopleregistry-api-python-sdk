# OrganisationsInviteSroRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**role** | **str** | Job title | [optional] 
**department_id** | **int** | One of the organisation&#39;s departments | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_invite_sro_request import OrganisationsInviteSroRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsInviteSroRequest from a JSON string
organisations_invite_sro_request_instance = OrganisationsInviteSroRequest.from_json(json)
# print the JSON string representation of the object
print(OrganisationsInviteSroRequest.to_json())

# convert the object into a dict
organisations_invite_sro_request_dict = organisations_invite_sro_request_instance.to_dict()
# create an instance of OrganisationsInviteSroRequest from a dict
organisations_invite_sro_request_from_dict = OrganisationsInviteSroRequest.from_dict(organisations_invite_sro_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


