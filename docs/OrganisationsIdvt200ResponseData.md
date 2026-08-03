# OrganisationsIdvt200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**idvt_result** | **bool** |  | [optional] 
**idvt_result_perc** | **float** |  | [optional] 
**idvt_errors** | **object** |  | [optional] 
**idvt_completed_at** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_idvt200_response_data import OrganisationsIdvt200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsIdvt200ResponseData from a JSON string
organisations_idvt200_response_data_instance = OrganisationsIdvt200ResponseData.from_json(json)
# print the JSON string representation of the object
print(OrganisationsIdvt200ResponseData.to_json())

# convert the object into a dict
organisations_idvt200_response_data_dict = organisations_idvt200_response_data_instance.to_dict()
# create an instance of OrganisationsIdvt200ResponseData from a dict
organisations_idvt200_response_data_from_dict = OrganisationsIdvt200ResponseData.from_dict(organisations_idvt200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


