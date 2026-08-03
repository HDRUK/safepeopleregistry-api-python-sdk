# IDVTPlugin

Model representing IDVT plugins

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the IDVT plugin | [optional] 
**function** | **str** | Function name of the plugin | [optional] 
**args** | **str** | Arguments passed to the plugin function | [optional] 
**config** | **str** | Configuration settings for the plugin | [optional] 
**enabled** | **int** | Indicates whether the plugin is enabled (1 for enabled, 0 for disabled) | [optional] 
**created_at** | **datetime** | Timestamp when the plugin was created | [optional] 
**updated_at** | **datetime** | Timestamp when the plugin was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.idvt_plugin import IDVTPlugin

# TODO update the JSON string below
json = "{}"
# create an instance of IDVTPlugin from a JSON string
idvt_plugin_instance = IDVTPlugin.from_json(json)
# print the JSON string representation of the object
print(IDVTPlugin.to_json())

# convert the object into a dict
idvt_plugin_dict = idvt_plugin_instance.to_dict()
# create an instance of IDVTPlugin from a dict
idvt_plugin_from_dict = IDVTPlugin.from_dict(idvt_plugin_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


