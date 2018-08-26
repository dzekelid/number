{
  "info": {
    "name": "Square Connect API Provides non-confidential details for a merchant's associated bank account. This endpoint does not provide full bank account numbers, and there is no way to obtain a full bank account number with the Connect API.",
    "_postman_id": "19dcea3b-abaf-45dd-95ac-d2bb9c036515",
    "description": "Provides non-confidential details for a merchant's associated bank account. This endpoint does not provide full bank account numbers, and there is no way to obtain a full bank account number with the Connect API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Provides",
      "item": [
        {
          "id": "4fe3b691-59da-4dda-9619-d3f75e69c628",
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
              "id": "0644f0f8-ee62-48b6-b6d9-2cb201daa5f0"
            }
          ]
        },
        {
          "id": "1f7b6001-b116-4e57-bbf1-aba5ddc27e89",
          "name": "RetrieveBankAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "connect.squareup.com",
              "path": [
                "v1/:location_id/bank-accounts/:bank_account_id"
              ],
              "variable": [
                {
                  "id": "bank_account_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Provides non-confidential details for a merchant's associated bank account. This endpoint does not provide full bank account numbers, and there is no way to obtain a full bank account number with the Connect API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "125a299d-81d3-4d62-9ddf-e8cf42830536"
            }
          ]
        }
      ]
    }
  ]
}