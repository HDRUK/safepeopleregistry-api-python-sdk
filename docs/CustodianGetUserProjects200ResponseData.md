# CustodianGetUserProjects200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**per_page** | **int** |  | [optional] 
**total** | **int** |  | [optional] 
**data** | [**List[Project]**](Project.md) |  | [optional] 
**first_page_url** | **str** |  | [optional] 
**last_page_url** | **str** |  | [optional] 
**next_page_url** | **str** |  | [optional] 
**prev_page_url** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_get_user_projects200_response_data import CustodianGetUserProjects200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianGetUserProjects200ResponseData from a JSON string
custodian_get_user_projects200_response_data_instance = CustodianGetUserProjects200ResponseData.from_json(json)
# print the JSON string representation of the object
print(CustodianGetUserProjects200ResponseData.to_json())

# convert the object into a dict
custodian_get_user_projects200_response_data_dict = custodian_get_user_projects200_response_data_instance.to_dict()
# create an instance of CustodianGetUserProjects200ResponseData from a dict
custodian_get_user_projects200_response_data_from_dict = CustodianGetUserProjects200ResponseData.from_dict(custodian_get_user_projects200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


