# Custodian

Custodian model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**unique_identifier** | **str** | A unique identifier for Custodian&#39;s within SOURSD | [optional] 
**contact_email** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**invite_accepted_at** | **str** |  | [optional] 
**invite_sent_at** | **str** |  | [optional] 
**idvt_required** | **bool** |  | [optional] 
**gateway_app_id** | **str** |  | [optional] 
**gateway_client_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian import Custodian

# TODO update the JSON string below
json = "{}"
# create an instance of Custodian from a JSON string
custodian_instance = Custodian.from_json(json)
# print the JSON string representation of the object
print(Custodian.to_json())

# convert the object into a dict
custodian_dict = custodian_instance.to_dict()
# create an instance of Custodian from a dict
custodian_from_dict = Custodian.from_dict(custodian_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


