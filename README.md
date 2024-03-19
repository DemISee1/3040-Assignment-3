# Exchange Rate API

## Description
3040Crypto Exchange Rate API enables users to seamlessly convert between digital currencies like Ethereum or Bitcoin and physical currencies such as USD dollars or yen and, the other way around.


## Endpoints and parameters

The API endpoint accepts parameters for the source currency (from), the target (to)currency for conversion, and the amount to be converted that refers to the source currency.



Crypto to Traditional

```https://currencyconverter.org/api/crypto/ethereum/to/traditional/cad```

Traditional to Crypto

```https://currencyconverter.org/api/traditional/cad/to/crypto/ethereum```

Crypto to Crypto 

```https://currencyconverter.org/api/crypto/ethereum/to/crypto/bitcoin```

Traditional to Traditional

```https://currencyconverter.org/api/traditional/cad/to/traditional/usd```

Traditional to All

```https://currencyconverter.org/api/traditional/cad/to/all```

Crypto to All

```https://currencyconverter.org/api/crypto/ethereum/to/all```

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
