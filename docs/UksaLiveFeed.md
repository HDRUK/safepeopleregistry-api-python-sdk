# UksaLiveFeed

Model representing UKSA live feed data

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the UKSA live feed record | [optional] 
**first_name** | **str** | First name of the individual | [optional] 
**last_name** | **str** | Last name of the individual | [optional] 
**organisation_name** | **str** | Name of the organisation | [optional] 
**accreditation_number** | **str** | Accreditation number | [optional] 
**accreditation_type** | **str** | Type of accreditation | [optional] 
**expiry_date** | **date** | Expiry date of the accreditation | [optional] 
**public_record** | **str** | Indicates whether the record is public | [optional] 
**stage** | **str** | Current stage of the accreditation process | [optional] 
**created_at** | **datetime** | Timestamp when the record was created | [optional] 
**updated_at** | **datetime** | Timestamp when the record was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.uksa_live_feed import UksaLiveFeed

# TODO update the JSON string below
json = "{}"
# create an instance of UksaLiveFeed from a JSON string
uksa_live_feed_instance = UksaLiveFeed.from_json(json)
# print the JSON string representation of the object
print(UksaLiveFeed.to_json())

# convert the object into a dict
uksa_live_feed_dict = uksa_live_feed_instance.to_dict()
# create an instance of UksaLiveFeed from a dict
uksa_live_feed_from_dict = UksaLiveFeed.from_dict(uksa_live_feed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


