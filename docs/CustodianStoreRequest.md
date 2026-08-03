# CustodianStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_store_request import CustodianStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianStoreRequest from a JSON string
custodian_store_request_instance = CustodianStoreRequest.from_json(json)
# print the JSON string representation of the object
print(CustodianStoreRequest.to_json())

# convert the object into a dict
custodian_store_request_dict = custodian_store_request_instance.to_dict()
# create an instance of CustodianStoreRequest from a dict
custodian_store_request_from_dict = CustodianStoreRequest.from_dict(custodian_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


