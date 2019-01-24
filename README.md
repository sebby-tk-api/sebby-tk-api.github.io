# Sebby.tk API
A versatile API for discord developers.

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
Returns a random XKCD comic
### GET /api/image/reddit/{subreddit}
Returns a picture from specified subreddit
### GET /api/image/reddit/json/{subreddit}
Returns a list of images from specified subreddit
### GET /api/image/achievement/{text}
Generates a Minecraft achievement with text
### GET /api/search/youtube/{query}
Searches for query on YouTube
### GET /api/search/google/{query}
Searches for query on Google
### GET /api/twitter/user/{user}
Gets latest tweets from user
### GET /api/twitter/user/{tag}
Gets latest tweets with hashtag
### GET /api/weather/{zip}
Gets local weather for specified zip code

## Related APIs
##### [TikTok API](http://tiktok.sebby.tk/api)
##### [Seb Bot API](http://api.sebbot.tk)
