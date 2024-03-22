# Exchange Rate API

## Description

3040Crypto Exchange Rate API enables users to seamlessly convert between any crypto currency (e.g., Ethereum) and any traditional currency (e.g., USD). 

## Endpoints

This section covers the API endpoints and parameters they need.

GET `/v1/convert`

- The API endpoint accepts a query string parameter consisting of:
    - `from` The source currency.
    - `to` The target currency for conversion.
    - `amount` The amount to be converted, denoted in the source currency.

## Resources

The response of the API is structured in JSON format, providing a clear and easily interpretable set of data including the success status, request details, conversion rate, and the conversion result.

```json
{
    "success": true,
    "info": {
        "timestamp": unix_timestamp,
        "rate": conversion_rate
    },
    "date": "YYYY-MM-DD",
    "result": converted_amount
}
```

## Sample Requests and Responses

GET `https://api.exchangerates.io/v1/convert?from=GBP&to=JPY&amount=25`

- Response:

    ```json
    {
        "success": true,
        "info": {
            "timestamp": 1519328414,
            "rate": 148.972231
        },
        "historical": "",
        "date": "2018-02-22",
        "result": 3724.305775
    }
    ```
