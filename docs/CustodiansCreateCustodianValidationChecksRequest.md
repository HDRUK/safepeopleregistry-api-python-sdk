# CustodiansCreateCustodianValidationChecksRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**type** | **str** |  | 
**description** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodians_create_custodian_validation_checks_request import CustodiansCreateCustodianValidationChecksRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CustodiansCreateCustodianValidationChecksRequest from a JSON string
custodians_create_custodian_validation_checks_request_instance = CustodiansCreateCustodianValidationChecksRequest.from_json(json)
# print the JSON string representation of the object
print(CustodiansCreateCustodianValidationChecksRequest.to_json())

# convert the object into a dict
custodians_create_custodian_validation_checks_request_dict = custodians_create_custodian_validation_checks_request_instance.to_dict()
# create an instance of CustodiansCreateCustodianValidationChecksRequest from a dict
custodians_create_custodian_validation_checks_request_from_dict = CustodiansCreateCustodianValidationChecksRequest.from_dict(custodians_create_custodian_validation_checks_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


