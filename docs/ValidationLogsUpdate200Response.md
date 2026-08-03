# ValidationLogsUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ValidationLog**](ValidationLog.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_logs_update200_response import ValidationLogsUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationLogsUpdate200Response from a JSON string
validation_logs_update200_response_instance = ValidationLogsUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(ValidationLogsUpdate200Response.to_json())

# convert the object into a dict
validation_logs_update200_response_dict = validation_logs_update200_response_instance.to_dict()
# create an instance of ValidationLogsUpdate200Response from a dict
validation_logs_update200_response_from_dict = ValidationLogsUpdate200Response.from_dict(validation_logs_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


