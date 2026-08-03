# QueryQuery200ResponseDataRegistry

The matched Registry record

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**deleted_at** | **str** |  | [optional] 
**digi_ident** | **str** |  | [optional] 
**dl_ident** | **str** |  | [optional] 
**pp_ident** | **str** |  | [optional] 
**verified** | **int** |  | [optional] 
**training** | [**List[Training]**](Training.md) | Training records linked to the registry | [optional] 
**history** | [**List[QueryQuery200ResponseDataRegistryAllOfHistoryInner]**](QueryQuery200ResponseDataRegistryAllOfHistoryInner.md) | History records linked to the registry, each with its related affiliation and project | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.query_query200_response_data_registry import QueryQuery200ResponseDataRegistry

# TODO update the JSON string below
json = "{}"
# create an instance of QueryQuery200ResponseDataRegistry from a JSON string
query_query200_response_data_registry_instance = QueryQuery200ResponseDataRegistry.from_json(json)
# print the JSON string representation of the object
print(QueryQuery200ResponseDataRegistry.to_json())

# convert the object into a dict
query_query200_response_data_registry_dict = query_query200_response_data_registry_instance.to_dict()
# create an instance of QueryQuery200ResponseDataRegistry from a dict
query_query200_response_data_registry_from_dict = QueryQuery200ResponseDataRegistry.from_dict(query_query200_response_data_registry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


