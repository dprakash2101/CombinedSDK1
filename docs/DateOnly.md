# DateOnly


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**year** | **int** |  | [optional] 
**month** | **int** |  | [optional] 
**day** | **int** |  | [optional] 
**day_of_week** | [**DayOfWeek**](DayOfWeek.md) |  | [optional] 
**day_of_year** | **int** |  | [optional] [readonly] 
**day_number** | **int** |  | [optional] [readonly] 

## Example

```python
from openapi_client.models.date_only import DateOnly

# TODO update the JSON string below
json = "{}"
# create an instance of DateOnly from a JSON string
date_only_instance = DateOnly.from_json(json)
# print the JSON string representation of the object
print DateOnly.to_json()

# convert the object into a dict
date_only_dict = date_only_instance.to_dict()
# create an instance of DateOnly from a dict
date_only_form_dict = date_only.from_dict(date_only_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


