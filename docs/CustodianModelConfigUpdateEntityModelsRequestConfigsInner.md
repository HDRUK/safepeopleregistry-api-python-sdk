# CustodianModelConfigUpdateEntityModelsRequestConfigsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**entity_model_id** | **int** |  | [optional] 
**active** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_model_config_update_entity_models_request_configs_inner import CustodianModelConfigUpdateEntityModelsRequestConfigsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianModelConfigUpdateEntityModelsRequestConfigsInner from a JSON string
custodian_model_config_update_entity_models_request_configs_inner_instance = CustodianModelConfigUpdateEntityModelsRequestConfigsInner.from_json(json)
# print the JSON string representation of the object
print(CustodianModelConfigUpdateEntityModelsRequestConfigsInner.to_json())

# convert the object into a dict
custodian_model_config_update_entity_models_request_configs_inner_dict = custodian_model_config_update_entity_models_request_configs_inner_instance.to_dict()
# create an instance of CustodianModelConfigUpdateEntityModelsRequestConfigsInner from a dict
custodian_model_config_update_entity_models_request_configs_inner_from_dict = CustodianModelConfigUpdateEntityModelsRequestConfigsInner.from_dict(custodian_model_config_update_entity_models_request_configs_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


