
# Loyalty Event Expire Points

Provides metadata when the event `type` is `EXPIRE_POINTS`.

## Structure

`Loyalty Event Expire Points`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `loyalty_program_id` | `string` | Required | The Square-assigned ID of the [loyalty program](../../doc/models/loyalty-program.md).<br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `36` |
| `points` | `int` | Required | The number of points expired. |

## Example (as JSON)

```json
{
  "loyalty_program_id": "loyalty_program_id0",
  "points": 236
}
```

