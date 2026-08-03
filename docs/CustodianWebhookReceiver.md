# CustodianWebhookReceiver

Model representing webhook receivers for custodians

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the webhook receiver | [optional] 
**custodian_id** | **int** | ID of the custodian associated with the webhook receiver | [optional] 
**url** | **str** | URL of the webhook receiver | [optional] 
**webhook_event** | **int** | ID of the webhook event associated with the receiver | [optional] 
**created_at** | **datetime** | Timestamp when the webhook receiver was created | [optional] 
**updated_at** | **datetime** | Timestamp when the webhook receiver was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_webhook_receiver import CustodianWebhookReceiver

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianWebhookReceiver from a JSON string
custodian_webhook_receiver_instance = CustodianWebhookReceiver.from_json(json)
# print the JSON string representation of the object
print(CustodianWebhookReceiver.to_json())

# convert the object into a dict
custodian_webhook_receiver_dict = custodian_webhook_receiver_instance.to_dict()
# create an instance of CustodianWebhookReceiver from a dict
custodian_webhook_receiver_from_dict = CustodianWebhookReceiver.from_dict(custodian_webhook_receiver_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


