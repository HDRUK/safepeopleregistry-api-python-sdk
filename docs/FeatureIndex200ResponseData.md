# FeatureIndex200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**scope** | **str** |  | [optional] 
**value** | **bool** |  | [optional] 
**description** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.feature_index200_response_data import FeatureIndex200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FeatureIndex200ResponseData from a JSON string
feature_index200_response_data_instance = FeatureIndex200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FeatureIndex200ResponseData.to_json())

# convert the object into a dict
feature_index200_response_data_dict = feature_index200_response_data_instance.to_dict()
# create an instance of FeatureIndex200ResponseData from a dict
feature_index200_response_data_from_dict = FeatureIndex200ResponseData.from_dict(feature_index200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


