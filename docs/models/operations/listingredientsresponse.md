# ListIngredientsResponse


## Fields

| Field                                                    | Type                                                     | Required                                                 | Description                                              |
| -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| `contentType`                                            | *string*                                                 | :heavy_check_mark:                                       | HTTP response content type for this operation            |
| `error`                                                  | [shared.ErrorT](../../models/shared/errort.md)           | :heavy_minus_sign:                                       | An unknown error occurred interacting with the API.      |
| `ingredients`                                            | [shared.Ingredient](../../models/shared/ingredient.md)[] | :heavy_minus_sign:                                       | A list of ingredients.                                   |
| `statusCode`                                             | *number*                                                 | :heavy_check_mark:                                       | HTTP response status code for this operation             |
| `rawResponse`                                            | [AxiosResponse](https://axios-http.com/docs/res_schema)  | :heavy_minus_sign:                                       | Raw HTTP response; suitable for custom response parsing  |