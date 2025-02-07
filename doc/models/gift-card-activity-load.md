
# Gift Card Activity Load

Represents details about a `LOAD` [gift card activity type](../../doc/models/gift-card-activity-type.md).

## Structure

`Gift Card Activity Load`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amount_money` | [`Money`](../../doc/models/money.md) | Optional | Represents an amount of money. `Money` fields can be signed or unsigned.<br>Fields that do not explicitly define whether they are signed or unsigned are<br>considered unsigned and can only hold positive amounts. For signed fields, the<br>sign of the value indicates the purpose of the money transfer. See<br>[Working with Monetary Amounts](https://developer.squareup.com/docs/build-basics/working-with-monetary-amounts)<br>for more information. |
| `order_id` | `string` | Optional | The ID of the [order](../../doc/models/order.md) that contains the `GIFT_CARD` line item.<br><br>Applications that use the Square Orders API to process orders must specify the order ID in the<br>[CreateGiftCardActivity](../../doc/api/gift-card-activities.md#create-gift-card-activity) request. |
| `line_item_uid` | `string` | Optional | The UID of the `GIFT_CARD` line item in the order that represents the additional funds for the gift card.<br><br>Applications that use the Square Orders API to process orders must specify the line item UID<br>in the [CreateGiftCardActivity](../../doc/api/gift-card-activities.md#create-gift-card-activity) request. |
| `reference_id` | `string` | Optional | A client-specified ID that associates the gift card activity with an entity in another system.<br><br>Applications that use a custom order processing system can use this field to track information related to<br>an order or payment. |
| `buyer_payment_instrument_ids` | `List of string` | Optional | The payment instrument IDs used to process the order for the additional funds, such as a credit card ID<br>or bank account ID.<br><br>Applications that use a custom order processing system must specify payment instrument IDs in<br>the [CreateGiftCardActivity](../../doc/api/gift-card-activities.md#create-gift-card-activity) request.<br>Square uses this information to perform compliance checks.<br><br>For applications that use the Square Orders API to process payments, Square has the necessary<br>instrument IDs to perform compliance checks. |

## Example (as JSON)

```json
{
  "amount_money": null,
  "order_id": null,
  "line_item_uid": null,
  "reference_id": null,
  "buyer_payment_instrument_ids": null
}
```

