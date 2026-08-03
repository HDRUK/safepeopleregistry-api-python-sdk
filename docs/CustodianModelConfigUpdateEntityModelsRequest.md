# CustodianModelConfigUpdateEntityModelsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**configs** | [**List[CustodianModelConfigUpdateEntityModelsRequestConfigsInner]**](CustodianModelConfigUpdateEntityModelsRequestConfigsInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_model_config_update_entity_models_request import CustodianModelConfigUpdateEntityModelsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianModelConfigUpdateEntityModelsRequest from a JSON string
custodian_model_config_update_entity_models_request_instance = CustodianModelConfigUpdateEntityModelsRequest.from_json(json)
# print the JSON string representation of the object
print(CustodianModelConfigUpdateEntityModelsRequest.to_json())

# convert the object into a dict
custodian_model_config_update_entity_models_request_dict = custodian_model_config_update_entity_models_request_instance.to_dict()
# create an instance of CustodianModelConfigUpdateEntityModelsRequest from a dict
custodian_model_config_update_entity_models_request_from_dict = CustodianModelConfigUpdateEntityModelsRequest.from_dict(custodian_model_config_update_entity_models_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


