# QueryQuery200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | [**QueryQuery200ResponseDataUser**](QueryQuery200ResponseDataUser.md) |  | [optional] 
**registry** | [**QueryQuery200ResponseDataRegistry**](QueryQuery200ResponseDataRegistry.md) |  | [optional] 
**projects** | [**List[QueryQuery200ResponseDataProjectsInner]**](QueryQuery200ResponseDataProjectsInner.md) | Projects the queried user is linked to, scoped to the requesting custodian | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.query_query200_response_data import QueryQuery200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of QueryQuery200ResponseData from a JSON string
query_query200_response_data_instance = QueryQuery200ResponseData.from_json(json)
# print the JSON string representation of the object
print(QueryQuery200ResponseData.to_json())

# convert the object into a dict
query_query200_response_data_dict = query_query200_response_data_instance.to_dict()
# create an instance of QueryQuery200ResponseData from a dict
query_query200_response_data_from_dict = QueryQuery200ResponseData.from_dict(query_query200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


