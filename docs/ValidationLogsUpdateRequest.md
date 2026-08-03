# ValidationLogsUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**complete** | **bool** | Mark the validation log as complete | [optional] 
**incomplete** | **bool** | Mark the validation log as incomplete | [optional] 
**var_pass** | **bool** | Mark the validation log as passed | [optional] 
**fail** | **bool** | Mark the validation log as failed | [optional] 
**enable** | **bool** | Mark the validation log as enabled | [optional] 
**disable** | **bool** | Mark the validation log as disabled | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_logs_update_request import ValidationLogsUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationLogsUpdateRequest from a JSON string
validation_logs_update_request_instance = ValidationLogsUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationLogsUpdateRequest.to_json())

# convert the object into a dict
validation_logs_update_request_dict = validation_logs_update_request_instance.to_dict()
# create an instance of ValidationLogsUpdateRequest from a dict
validation_logs_update_request_from_dict = ValidationLogsUpdateRequest.from_dict(validation_logs_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


