# ONSSubmissionReceiveCSV400Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.ons_submission_receive_csv400_response import ONSSubmissionReceiveCSV400Response

# TODO update the JSON string below
json = "{}"
# create an instance of ONSSubmissionReceiveCSV400Response from a JSON string
ons_submission_receive_csv400_response_instance = ONSSubmissionReceiveCSV400Response.from_json(json)
# print the JSON string representation of the object
print(ONSSubmissionReceiveCSV400Response.to_json())

# convert the object into a dict
ons_submission_receive_csv400_response_dict = ons_submission_receive_csv400_response_instance.to_dict()
# create an instance of ONSSubmissionReceiveCSV400Response from a dict
ons_submission_receive_csv400_response_from_dict = ONSSubmissionReceiveCSV400Response.from_dict(ons_submission_receive_csv400_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


