# CustodianAddProjectRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_add_project_request import CustodianAddProjectRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianAddProjectRequest from a JSON string
custodian_add_project_request_instance = CustodianAddProjectRequest.from_json(json)
# print the JSON string representation of the object
print(CustodianAddProjectRequest.to_json())

# convert the object into a dict
custodian_add_project_request_dict = custodian_add_project_request_instance.to_dict()
# create an instance of CustodianAddProjectRequest from a dict
custodian_add_project_request_from_dict = CustodianAddProjectRequest.from_dict(custodian_add_project_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


