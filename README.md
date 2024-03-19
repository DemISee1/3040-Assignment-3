# Currency Converter

## Description
3040Crypto Currency Converter API enables users to seamlessly convert between digital currencies like Ethereum or Bitcoin and physical currencies such as USD dollars or yen and, the other way around.


## Endpoints

With parameters

## Resources

With json

## Sample Requests and Responses
- sample request :

```url
https://api.exchangeratesapi.io/v1/convert?from=GBP&to=JPY&amount=25
```
- sample response :
```json
{
    "success": true,
    "query": {
        "from": "GBP",
        "to": "JPY",
        "amount": 25
    },
    "info": {
        "timestamp": 1519328414,
        "rate": 148.972231
    },
    "historical": ""
    "date": "2018-02-22"
    "result": 3724.305775
}
```