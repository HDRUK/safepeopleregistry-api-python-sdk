# CustodianModelConfigGetEntityModels200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[CustodianModelConfigGetEntityModels200ResponseDataInner]**](CustodianModelConfigGetEntityModels200ResponseDataInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_model_config_get_entity_models200_response import CustodianModelConfigGetEntityModels200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianModelConfigGetEntityModels200Response from a JSON string
custodian_model_config_get_entity_models200_response_instance = CustodianModelConfigGetEntityModels200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianModelConfigGetEntityModels200Response.to_json())

# convert the object into a dict
custodian_model_config_get_entity_models200_response_dict = custodian_model_config_get_entity_models200_response_instance.to_dict()
# create an instance of CustodianModelConfigGetEntityModels200Response from a dict
custodian_model_config_get_entity_models200_response_from_dict = CustodianModelConfigGetEntityModels200Response.from_dict(custodian_model_config_get_entity_models200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


