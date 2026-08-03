# Resolution

Model representing resolutions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the resolution | [optional] 
**comment** | **str** | Comment associated with the resolution | [optional] 
**custodian_by** | **int** | ID of the custodian who resolved the issue | [optional] 
**registry_id** | **int** | ID of the registry associated with the resolution | [optional] 
**resolved** | **bool** | Indicates whether the resolution is resolved | [optional] 
**created_at** | **datetime** | Timestamp when the resolution was created | [optional] 
**updated_at** | **datetime** | Timestamp when the resolution was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.resolution import Resolution

# TODO update the JSON string below
json = "{}"
# create an instance of Resolution from a JSON string
resolution_instance = Resolution.from_json(json)
# print the JSON string representation of the object
print(Resolution.to_json())

# convert the object into a dict
resolution_dict = resolution_instance.to_dict()
# create an instance of Resolution from a dict
resolution_from_dict = Resolution.from_dict(resolution_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


