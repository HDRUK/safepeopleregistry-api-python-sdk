# FeatureIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FeatureIndex200ResponseData**](FeatureIndex200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.feature_index200_response import FeatureIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FeatureIndex200Response from a JSON string
feature_index200_response_instance = FeatureIndex200Response.from_json(json)
# print the JSON string representation of the object
print(FeatureIndex200Response.to_json())

# convert the object into a dict
feature_index200_response_dict = feature_index200_response_instance.to_dict()
# create an instance of FeatureIndex200Response from a dict
feature_index200_response_from_dict = FeatureIndex200Response.from_dict(feature_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


