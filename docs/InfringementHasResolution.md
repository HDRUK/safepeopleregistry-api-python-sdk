# InfringementHasResolution

Pivot model representing the relationship between infringements and resolutions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**infringement_id** | **int** | ID of the infringement | [optional] 
**resolution_id** | **int** | ID of the resolution | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.infringement_has_resolution import InfringementHasResolution

# TODO update the JSON string below
json = "{}"
# create an instance of InfringementHasResolution from a JSON string
infringement_has_resolution_instance = InfringementHasResolution.from_json(json)
# print the JSON string representation of the object
print(InfringementHasResolution.to_json())

# convert the object into a dict
infringement_has_resolution_dict = infringement_has_resolution_instance.to_dict()
# create an instance of InfringementHasResolution from a dict
infringement_has_resolution_from_dict = InfringementHasResolution.from_dict(infringement_has_resolution_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


