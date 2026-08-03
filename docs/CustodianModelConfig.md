# CustodianModelConfig

CustodianModelConfig model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**entity_model_id** | **int** |  | [optional] 
**active** | **bool** |  | [optional] 
**custodian_id** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_model_config import CustodianModelConfig

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianModelConfig from a JSON string
custodian_model_config_instance = CustodianModelConfig.from_json(json)
# print the JSON string representation of the object
print(CustodianModelConfig.to_json())

# convert the object into a dict
custodian_model_config_dict = custodian_model_config_instance.to_dict()
# create an instance of CustodianModelConfig from a dict
custodian_model_config_from_dict = CustodianModelConfig.from_dict(custodian_model_config_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


