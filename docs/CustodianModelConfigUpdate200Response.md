# CustodianModelConfigUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**CustodianModelConfig**](CustodianModelConfig.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_model_config_update200_response import CustodianModelConfigUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianModelConfigUpdate200Response from a JSON string
custodian_model_config_update200_response_instance = CustodianModelConfigUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianModelConfigUpdate200Response.to_json())

# convert the object into a dict
custodian_model_config_update200_response_dict = custodian_model_config_update200_response_instance.to_dict()
# create an instance of CustodianModelConfigUpdate200Response from a dict
custodian_model_config_update200_response_from_dict = CustodianModelConfigUpdate200Response.from_dict(custodian_model_config_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


