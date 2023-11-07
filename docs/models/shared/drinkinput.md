# DrinkInput


## Fields

| Field                                                             | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `name`                                                            | *string*                                                          | :heavy_check_mark:                                                | The name of the drink.                                            |
| `price`                                                           | *number*                                                          | :heavy_check_mark:                                                | The price of one unit of the drink in US cents.                   |
| `productCode`                                                     | *string*                                                          | :heavy_minus_sign:                                                | The product code of the drink, only available when authenticated. |
| `type`                                                            | [shared.DrinkType](../../models/shared/drinktype.md)              | :heavy_minus_sign:                                                | The type of drink.                                                |