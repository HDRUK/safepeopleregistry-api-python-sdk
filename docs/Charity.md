# Charity

Charity model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the charity | [optional] 
**registration_id** | **str** | Registration ID of the charity | [optional] 
**name** | **str** | Name of the charity | [optional] 
**website** | **str** | Website URL of the charity | [optional] 
**address_1** | **str** | First line of the charity&#39;s address | [optional] 
**address_2** | **str** | Second line of the charity&#39;s address | [optional] 
**town** | **str** | Town where the charity is located | [optional] 
**county** | **str** | County where the charity is located | [optional] 
**country** | **str** | Country where the charity is located | [optional] 
**postcode** | **str** | Postcode of the charity&#39;s address | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.charity import Charity

# TODO update the JSON string below
json = "{}"
# create an instance of Charity from a JSON string
charity_instance = Charity.from_json(json)
# print the JSON string representation of the object
print(Charity.to_json())

# convert the object into a dict
charity_dict = charity_instance.to_dict()
# create an instance of Charity from a dict
charity_from_dict = Charity.from_dict(charity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


