# hand
An extension to the standard fetch that speeds up and simplifies development

First you need to configure the handConfig for example

```typescript
import { handConfig } from 'hand';

export const DOMAIN = 'localhost:4040';

handConfig.credentials = 'include';
handConfig.domain = DOMAIN;
```

Then you can use the hand. Example usage

```typescript
const res = hand("/api/users/1", {
    method: RestApiMethods.Get,
});
```

The code above will send a request to the server and log it.