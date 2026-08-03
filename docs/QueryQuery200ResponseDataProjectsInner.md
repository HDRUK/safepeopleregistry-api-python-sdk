# QueryQuery200ResponseDataProjectsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project_id** | **int** |  | [optional] 
**project_title** | **str** |  | [optional] 
**project_user_validation_status** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.query_query200_response_data_projects_inner import QueryQuery200ResponseDataProjectsInner

# TODO update the JSON string below
json = "{}"
# create an instance of QueryQuery200ResponseDataProjectsInner from a JSON string
query_query200_response_data_projects_inner_instance = QueryQuery200ResponseDataProjectsInner.from_json(json)
# print the JSON string representation of the object
print(QueryQuery200ResponseDataProjectsInner.to_json())

# convert the object into a dict
query_query200_response_data_projects_inner_dict = query_query200_response_data_projects_inner_instance.to_dict()
# create an instance of QueryQuery200ResponseDataProjectsInner from a dict
query_query200_response_data_projects_inner_from_dict = QueryQuery200ResponseDataProjectsInner.from_dict(query_query200_response_data_projects_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


