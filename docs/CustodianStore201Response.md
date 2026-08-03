# CustodianStore201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Custodian**](Custodian.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_store201_response import CustodianStore201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianStore201Response from a JSON string
custodian_store201_response_instance = CustodianStore201Response.from_json(json)
# print the JSON string representation of the object
print(CustodianStore201Response.to_json())

# convert the object into a dict
custodian_store201_response_dict = custodian_store201_response_instance.to_dict()
# create an instance of CustodianStore201Response from a dict
custodian_store201_response_from_dict = CustodianStore201Response.from_dict(custodian_store201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


