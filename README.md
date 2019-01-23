# Sebby.tk API
A dynamic API for any kind of developer, composed of many endpoints.

### Authorization
Supply your authorization token in every request. If you do not have one, you can [get one here]()
```php
curl --request GET \
--url 'https://api.sebby.tk/api/image/xkcd' \
--header 'Token: 9118b4777fe86402f27h48dj29he886e19ffe8f7'
```

### Making requests
> This examples requires the dependency: "request" v2.88.0

```js
const request = require("request");
request.get({ url: "https://api.sebby.tk/api/image/xkcd", headers: { token: "9118b4777fe86402f27h48dj29he886e19ffe8f7" } }, function (err, resp, body) {
  console.log(body);
});
```

## Endpoints
### GET /api/image/xkcd
