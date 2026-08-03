# CustodianGetProjects200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**CustodianGetProjects200ResponseData**](CustodianGetProjects200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_get_projects200_response import CustodianGetProjects200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianGetProjects200Response from a JSON string
custodian_get_projects200_response_instance = CustodianGetProjects200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianGetProjects200Response.to_json())

# convert the object into a dict
custodian_get_projects200_response_dict = custodian_get_projects200_response_instance.to_dict()
# create an instance of CustodianGetProjects200Response from a dict
custodian_get_projects200_response_from_dict = CustodianGetProjects200Response.from_dict(custodian_get_projects200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


