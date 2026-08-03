# SubsidiariesStore201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Subsidiary**](Subsidiary.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.subsidiaries_store201_response import SubsidiariesStore201Response

# TODO update the JSON string below
json = "{}"
# create an instance of SubsidiariesStore201Response from a JSON string
subsidiaries_store201_response_instance = SubsidiariesStore201Response.from_json(json)
# print the JSON string representation of the object
print(SubsidiariesStore201Response.to_json())

# convert the object into a dict
subsidiaries_store201_response_dict = subsidiaries_store201_response_instance.to_dict()
# create an instance of SubsidiariesStore201Response from a dict
subsidiaries_store201_response_from_dict = SubsidiariesStore201Response.from_dict(subsidiaries_store201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


