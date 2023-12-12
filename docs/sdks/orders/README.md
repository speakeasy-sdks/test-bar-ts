# Orders
(*orders*)

## Overview

The orders endpoints.

### Available Operations

* [createOrder](#createorder) - Create an order.

## createOrder

Create an order for a drink.

### Example Usage

```typescript
import { AnotherTestBar } from "test-bar-ts";
import { OrderType } from "test-bar-ts/dist/sdk/models/shared";

async function run() {
  const sdk = new AnotherTestBar({
    apiKey: "<YOUR_API_KEY_HERE>",
  });

  const res = await sdk.orders.createOrder({
    requestBody: [
      {
        productCode: "APM-1F2D3",
        quantity: 26535,
        type: OrderType.Drink,
      },
    ],
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                          | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `request`                                                                          | [operations.CreateOrderRequest](../../sdk/models/operations/createorderrequest.md) | :heavy_check_mark:                                                                 | The request object to use for the request.                                         |
| `config`                                                                           | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                       | :heavy_minus_sign:                                                                 | Available config options for making requests.                                      |


### Response

**Promise<[operations.CreateOrderResponse](../../sdk/models/operations/createorderresponse.md)>**
### Errors

| Error Object     | Status Code      | Content Type     |
| ---------------- | ---------------- | ---------------- |
| errors.APIError  | 5XX              | application/json |
| errors.SDKError  | 400-600          | */*              |
