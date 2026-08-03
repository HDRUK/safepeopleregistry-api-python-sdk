# InfringementStore201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **int** | ID of the created Infringement entry | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.infringement_store201_response import InfringementStore201Response

# TODO update the JSON string below
json = "{}"
# create an instance of InfringementStore201Response from a JSON string
infringement_store201_response_instance = InfringementStore201Response.from_json(json)
# print the JSON string representation of the object
print(InfringementStore201Response.to_json())

# convert the object into a dict
infringement_store201_response_dict = infringement_store201_response_instance.to_dict()
# create an instance of InfringementStore201Response from a dict
infringement_store201_response_from_dict = InfringementStore201Response.from_dict(infringement_store201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


