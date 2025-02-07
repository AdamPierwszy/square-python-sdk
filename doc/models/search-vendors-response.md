
# Search Vendors Response

Represents an output from a call to [SearchVendors](../../doc/api/vendors.md#search-vendors).

## Structure

`Search Vendors Response`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `errors` | [`List of Error`](../../doc/models/error.md) | Optional | Errors encountered when the request fails. |
| `vendors` | [`List of Vendor`](../../doc/models/vendor.md) | Optional | The [Vendor](../../doc/models/vendor.md) objects matching the specified search filter. |
| `cursor` | `string` | Optional | The pagination cursor to be used in a subsequent request. If unset,<br>this is the final response.<br><br>See the [Pagination](https://developer.squareup.com/docs/working-with-apis/pagination) guide for more information. |

## Example (as JSON)

```json
{
  "errors": null,
  "vendors": null,
  "cursor": null
}
```

