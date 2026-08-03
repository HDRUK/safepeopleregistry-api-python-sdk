# SystemConfig

Model representing system configuration settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the system configuration | [optional] 
**name** | **str** | Name of the configuration setting | [optional] 
**value** | **str** | Value of the configuration setting | [optional] 
**description** | **str** | Description of the configuration setting | [optional] 
**created_at** | **datetime** | Timestamp when the configuration was created | [optional] 
**updated_at** | **datetime** | Timestamp when the configuration was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.system_config import SystemConfig

# TODO update the JSON string below
json = "{}"
# create an instance of SystemConfig from a JSON string
system_config_instance = SystemConfig.from_json(json)
# print the JSON string representation of the object
print(SystemConfig.to_json())

# convert the object into a dict
system_config_dict = system_config_instance.to_dict()
# create an instance of SystemConfig from a dict
system_config_from_dict = SystemConfig.from_dict(system_config_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


