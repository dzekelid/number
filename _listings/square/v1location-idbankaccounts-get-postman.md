{
  "info": {
    "name": "Square Connect API Provides non-confidential details for all of a location's associated bank accounts. This endpoint does not provide full bank account numbers, and there is no way to obtain a full bank account number with the Connect API.",
    "_postman_id": "79cc3665-ec82-45f0-ac64-8bae37104d14",
    "description": "Provides non-confidential details for all of a location's associated bank accounts. This endpoint does not provide full bank account numbers, and there is no way to obtain a full bank account number with the Connect API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Provides",
      "item": [
        {
          "id": "09b80755-f298-40b6-9353-2975b0d252b4",
          "name": "ListBankAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "connect.squareup.com",
              "path": [
                "v1/:location_id/bank-accounts"
              ],
              "variable": [
                {
                  "id": "location_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides non-confidential details for all of a location's associated bank accounts. This endpoint does not provide full bank account numbers, and there is no way to obtain a full bank account number with the Connect API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "588af28d-fdfd-4091-9cf1-cacaeffb9880"
            }
          ]
        }
      ]
    }
  ]
}