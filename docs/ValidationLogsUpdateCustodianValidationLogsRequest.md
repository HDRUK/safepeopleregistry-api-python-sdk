# ValidationLogsUpdateCustodianValidationLogsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | 
**name** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_logs_update_custodian_validation_logs_request import ValidationLogsUpdateCustodianValidationLogsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationLogsUpdateCustodianValidationLogsRequest from a JSON string
validation_logs_update_custodian_validation_logs_request_instance = ValidationLogsUpdateCustodianValidationLogsRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationLogsUpdateCustodianValidationLogsRequest.to_json())

# convert the object into a dict
validation_logs_update_custodian_validation_logs_request_dict = validation_logs_update_custodian_validation_logs_request_instance.to_dict()
# create an instance of ValidationLogsUpdateCustodianValidationLogsRequest from a dict
validation_logs_update_custodian_validation_logs_request_from_dict = ValidationLogsUpdateCustodianValidationLogsRequest.from_dict(validation_logs_update_custodian_validation_logs_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


