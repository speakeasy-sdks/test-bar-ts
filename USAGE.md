<!-- Start SDK Example Usage [usage] -->
```typescript
import { AnotherTestBar } from "test-bar-ts";

async function run() {
    const sdk = new AnotherTestBar({
        apiKey: "<YOUR_API_KEY_HERE>",
    });

    const res = await sdk.drinks.getDrink({
        name: "<value>",
    });

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End SDK Example Usage [usage] -->