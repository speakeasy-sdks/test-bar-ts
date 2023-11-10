<!-- Start SDK Example Usage -->
```typescript
import { AnotherTestBar } from "test-bar-ts";

(async () => {
    const sdk = new AnotherTestBar({
        apiKey: "",
    });

    const res = await sdk.drinks.getDrink({
        name: "string",
    });

    if (res.statusCode == 200) {
        // handle response
    }
})();

```
<!-- End SDK Example Usage -->