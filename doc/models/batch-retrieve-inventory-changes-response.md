
# Batch Retrieve Inventory Changes Response

## Structure

`Batch Retrieve Inventory Changes Response`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `errors` | [`List of Error`](../../doc/models/error.md) | Optional | Any errors that occurred during the request. |
| `changes` | [`List of Inventory Change`](../../doc/models/inventory-change.md) | Optional | The current calculated inventory changes for the requested objects<br>and locations. |
| `cursor` | `string` | Optional | The pagination cursor to be used in a subsequent request. If unset,<br>this is the final response.<br>See the [Pagination](https://developer.squareup.com/docs/working-with-apis/pagination) guide for more information. |

## Example (as JSON)

```json
{
  "changes": [
    {
      "physical_count": {
        "catalog_object_id": "W62UWFY35CWMYGVWK6TWJDNI",
        "catalog_object_type": "ITEM_VARIATION",
        "created_at": "2016-11-16T22:25:24.878Z",
        "id": "46YDTW253DWGGK9HMAE6XCAO",
        "location_id": "C6W5YS5QM06F5",
        "occurred_at": "2016-11-16T22:24:49.028Z",
        "quantity": "86",
        "reference_id": "22c07cf4-5626-4224-89f9-691112019399",
        "source": {
          "application_id": "416ff29c-86c4-4feb-b58c-9705f21f3ea0",
          "name": "Square Point of Sale 4.37",
          "product": "SQUARE_POS"
        },
        "state": "IN_STOCK",
        "team_member_id": "LRK57NSQ5X7PUD05"
      },
      "type": "PHYSICAL_COUNT"
    }
  ],
  "errors": []
}
```

