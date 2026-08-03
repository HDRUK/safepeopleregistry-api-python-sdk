# ValidationChecksStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_checks_store_request import ValidationChecksStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationChecksStoreRequest from a JSON string
validation_checks_store_request_instance = ValidationChecksStoreRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationChecksStoreRequest.to_json())

# convert the object into a dict
validation_checks_store_request_dict = validation_checks_store_request_instance.to_dict()
# create an instance of ValidationChecksStoreRequest from a dict
validation_checks_store_request_from_dict = ValidationChecksStoreRequest.from_dict(validation_checks_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


