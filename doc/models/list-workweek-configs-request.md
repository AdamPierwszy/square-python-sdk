
# List Workweek Configs Request

A request for a set of `WorkweekConfig` objects.

## Structure

`List Workweek Configs Request`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `int` | Optional | The maximum number of `WorkweekConfigs` results to return per page. |
| `cursor` | `string` | Optional | A pointer to the next page of `WorkweekConfig` results to fetch. |

## Example (as JSON)

```json
{
  "limit": null,
  "cursor": null
}
```

