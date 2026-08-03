# FilesShow200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FilesShow200ResponseData**](FilesShow200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.files_show200_response import FilesShow200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FilesShow200Response from a JSON string
files_show200_response_instance = FilesShow200Response.from_json(json)
# print the JSON string representation of the object
print(FilesShow200Response.to_json())

# convert the object into a dict
files_show200_response_dict = files_show200_response_instance.to_dict()
# create an instance of FilesShow200Response from a dict
files_show200_response_from_dict = FilesShow200Response.from_dict(files_show200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


