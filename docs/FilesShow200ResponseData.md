# FilesShow200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**path** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.files_show200_response_data import FilesShow200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FilesShow200ResponseData from a JSON string
files_show200_response_data_instance = FilesShow200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FilesShow200ResponseData.to_json())

# convert the object into a dict
files_show200_response_data_dict = files_show200_response_data_instance.to_dict()
# create an instance of FilesShow200ResponseData from a dict
files_show200_response_data_from_dict = FilesShow200ResponseData.from_dict(files_show200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


