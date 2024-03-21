# Exchange Rate API

## Description
3040Crypto Exchange Rate API enables users to seamlessly convert between digital currencies like Ethereum or Bitcoin and physical currencies such as USD dollars or yen and, the other way around.


## Endpoints and parameters

This section covers the API endpoints and parameters, essential for currency conversion.

- Endpoints

- Parameters:
    - The API endpoint accepts a query string parameter consisting of:
    - The source currency (from),
    - The target currency (to) for conversion,
    - The amount to be converted, denoted in the source currency.

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
