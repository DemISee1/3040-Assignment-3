# Exchange Rate API

## Description
3040Crypto Exchange Rate API enables users to seamlessly convert between digital currencies like Ethereum or Bitcoin and physical currencies such as USD dollars or yen and, the other way around.


## Endpoints and parameters

This section covers the API endpoints and parameters, essential for currency conversion.

- Endpoints
  - **Endpoint:** `/v1/convert`
  - **Method:** `GET`
- Parameters
  The API endpoint accepts a query string parameter consisting of:
    - `from` The source currency ,
    - `to`The target currency for conversion,
    - `amount` The amount to be converted, denoted in the source currency.

## Resources

The response of the API is structured in JSON format, providing a clear and easily interpretable set of data, including the success status, request details, conversion rate, and the conversion result.


```json
{
    "success": true,
    "query": {
        "from": "currency_code",
        "to": "currency_code",
        "amount": numeric_value
    },
    "info": {
        "timestamp": unix_timestamp,
        "rate": conversion_rate
    },
    "date": "YYYY-MM-DD",
    "result": converted_amount
}
```
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
