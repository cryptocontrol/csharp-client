CryptoControl - C# Crypto News API
=========================

Official C# client for the [CryptoControl.io](https://cryptocontrol.io) API. The CryptoControl PHP client lets developers access rich formatted articles from cryptonews sources from all around the world.

Credit goes to Andrew Thomas Cowan for helping implement this client

## Installation
installation details go in here

## Usage
First make sure that you've recieved an API key by visiting [https://cryptocontrol.io/apis](https://cryptocontrol.io/apis). With the API key you can write the following code.


```
demo of code goes here

```

## Available Functions

- **getTopNews()** Get the top news articles from the CryptoControl News API.
- **getLatestNews()** Get the latest news articles from the CryptoControl News API.
- **getTopNewsByCategory()** Get news articles grouped by category from the CryptoControl News API.
- **getTopNewsByCoin(coinSlug: String)** Get the top news articles for a specific coin from the CryptoControl API.
- **getLatestNewsByCoin(coinSlug: String)** Get the latest news articles for a specific coin from the CryptoControl News API.
- **getTopNewsByCoinCategory(coinSlug: String)** Get news articles grouped by category for a specific coin from the CryptoControl News API.

The coin slugs are the coin id's used from the CoinMarketCap api. You can see the full list of coins here: [https://api.coinmarketcap.com/v1/ticker/?limit=2000](https://api.coinmarketcap.com/v1/ticker/?limit=2000)

## Sample Response from the API
```javascript
[
    {
        "publishedAt": "2018-05-23T06:30:51.000Z",
        "hotness": 70698.68569444444,
        "activityHotness": 1.6,
        "primaryCategory": "General",
        "words": 302,
        "similarArticles": [
            {
                "publishedAt": "2018-05-23T03:00:05.000Z",
                "_id": "5b04de8d18f173000f9a6d72",
                "title": "PayPal: We’ll ‘Definitely Support’ Bitcoin If It Becomes ‘Better Currency’",
                "url": "https://cryptocontrol.io/r/api/article/5b04de8d18f173000f9a6d72?ref=5ac11440ec0af7be35528459"
            }
        ],
        "coins": [
            {
                "_id": "59cb59e81c073f09e76f614b",
                "name": "Bitcoin",
                "slug": "bitcoin",
                "tradingSymbol": "btc"
            }
        ],
        "_id": "5b07ea76214428000f55a513",
        "description": "Welcome to Crypto Daily™ News, this news piece \"Ripple XRP And Bitcoin Cash Now Live On Revolut\" is breaking news from the Crypto sector.",
        "title": "Ripple XRP And Bitcoin Cash Now Live On Revolut - Crypto Daily™",
        "url": "https://cryptocontrol.io/r/api/article/5b07ea76214428000f55a513?ref=5ac11440ec0af7be35528459",
        "thumbnail": "https://cryptocontrol.io/r/thumbnail/5b07ea76214428000f55a513?ref=5ac11440ec0af7be35528459",
        "originalImageUrl": "https://cryptodaily.co.uk/wp-content/uploads/2018/05/ripple-bitcoincash-credit.jpg"
    }
]
```