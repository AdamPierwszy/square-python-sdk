
# V1 Payment Tax

V1PaymentTax

## Structure

`V1 Payment Tax`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `errors` | [`List of Error`](../../doc/models/error.md) | Optional | Any errors that occurred during the request. |
| `name` | `string` | Optional | The merchant-defined name of the tax. |
| `applied_money` | [`V1 Money`](../../doc/models/v1-money.md) | Optional | - |
| `rate` | `string` | Optional | The rate of the tax, as a string representation of a decimal number. A value of 0.07 corresponds to a rate of 7%. |
| `inclusion_type` | [`str (V1 Payment Tax Inclusion Type)`](../../doc/models/v1-payment-tax-inclusion-type.md) | Optional | - |
| `fee_id` | `string` | Optional | The ID of the tax, if available. Taxes applied in older versions of Square Register might not have an ID. |

## Example (as JSON)

```json
{
  "errors": null,
  "name": null,
  "applied_money": null,
  "rate": null,
  "inclusion_type": null,
  "fee_id": null
}
```

