{
  "info": {
    "name": "Callfire Find a specific lease config",
    "_postman_id": "0e173a54-fa46-4c9b-9ad8-18b27cf8ffa6",
    "description": "Returns a single NumberConfig instance for a given number lease",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Numbers",
      "item": [
        {
          "id": "38a76846-c7de-4275-8cdd-9d350b0f429e",
          "name": "findNumberLeases",
          "request": {
            "url": "http://www.callfire.com/v2/numbers/leases?city=%7B%7D&fields=%7B%7D&labelName=%7B%7D&lata=%7B%7D&limit=%7B%7D&offset=%7B%7D&prefix=%7B%7D&rateCenter=%7B%7D&state=%7B%7D&zipcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for all numbers leased by account user. This API is useful for finding all numbers currently owned by the user. Returns a paged list of number leases."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2153dc55-d2ce-44e4-b078-d74cc198596b"
            }
          ]
        },
        {
          "id": "23e7aced-99ac-4a28-8f1e-74ffc7244e3b",
          "name": "findNumberLeaseConfigs",
          "request": {
            "url": "http://www.callfire.com/v2/numbers/leases/configs?city=%7B%7D&fields=%7B%7D&labelName=%7B%7D&lata=%7B%7D&limit=%7B%7D&offset=%7B%7D&prefix=%7B%7D&rateCenter=%7B%7D&state=%7B%7D&zipcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for all number lease configs for the user. Returns a paged list of NumberConfig"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "891faff9-496b-477e-9ba5-d6281205c199"
            }
          ]
        },
        {
          "id": "01c958f0-8b7e-4f9e-bf60-042291f10bcf",
          "name": "getNumberLeaseConfig",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.callfire.com",
              "path": [
                "v2",
                "numbers/leases/configs/:number"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single NumberConfig instance for a given number lease"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9957b5e-0a46-4e18-8305-82d8900ab8f5"
            }
          ]
        }
      ]
    }
  ]
}