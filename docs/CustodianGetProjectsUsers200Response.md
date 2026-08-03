# CustodianGetProjectsUsers200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**CustodianGetProjectsUsers200ResponseData**](CustodianGetProjectsUsers200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_get_projects_users200_response import CustodianGetProjectsUsers200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianGetProjectsUsers200Response from a JSON string
custodian_get_projects_users200_response_instance = CustodianGetProjectsUsers200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianGetProjectsUsers200Response.to_json())

# convert the object into a dict
custodian_get_projects_users200_response_dict = custodian_get_projects_users200_response_instance.to_dict()
# create an instance of CustodianGetProjectsUsers200Response from a dict
custodian_get_projects_users200_response_from_dict = CustodianGetProjectsUsers200Response.from_dict(custodian_get_projects_users200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


