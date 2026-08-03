# CustodianModelConfigGetEntityModels200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**entity_model_type_id** | **int** |  | [optional] 
**description** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**active** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_model_config_get_entity_models200_response_data_inner import CustodianModelConfigGetEntityModels200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianModelConfigGetEntityModels200ResponseDataInner from a JSON string
custodian_model_config_get_entity_models200_response_data_inner_instance = CustodianModelConfigGetEntityModels200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(CustodianModelConfigGetEntityModels200ResponseDataInner.to_json())

# convert the object into a dict
custodian_model_config_get_entity_models200_response_data_inner_dict = custodian_model_config_get_entity_models200_response_data_inner_instance.to_dict()
# create an instance of CustodianModelConfigGetEntityModels200ResponseDataInner from a dict
custodian_model_config_get_entity_models200_response_data_inner_from_dict = CustodianModelConfigGetEntityModels200ResponseDataInner.from_dict(custodian_model_config_get_entity_models200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


