## Redis Session Connection

**Error:**

`throw new TypeError('Invalid argument type');` when all redis session connection setup is correct...

**Fix:**

```javascript
const sessionClient = redis.createClient({
  host: "localhost",
  port: 6379,
  legacyMode: false,
});
```

change `legacyMode` from `true` to `false`
