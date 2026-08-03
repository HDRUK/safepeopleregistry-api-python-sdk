# OrganisationsUpdateApprovedRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**system_approved** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_update_approved_request import OrganisationsUpdateApprovedRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsUpdateApprovedRequest from a JSON string
organisations_update_approved_request_instance = OrganisationsUpdateApprovedRequest.from_json(json)
# print the JSON string representation of the object
print(OrganisationsUpdateApprovedRequest.to_json())

# convert the object into a dict
organisations_update_approved_request_dict = organisations_update_approved_request_instance.to_dict()
# create an instance of OrganisationsUpdateApprovedRequest from a dict
organisations_update_approved_request_from_dict = OrganisationsUpdateApprovedRequest.from_dict(organisations_update_approved_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


