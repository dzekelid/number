{
  "info": {
    "name": "Plentymarkets List ident number of a variation",
    "_postman_id": "4f33a2ef-7323-48e5-908d-72eaa09b4fde",
    "description": "Lists the ident number (ASIN/ePID) of a variation. The ID of the item and the ID of the variation must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "1736da78-1d3a-4d9d-86d1-fcf3ce68d8ff",
          "name": "getRestItemsVariationsVariationMarketEntNumbers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/market_ident_numbers"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists the ident number (ASIN/ePID) of a variation. The ID of the item and the ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a05ef936-b2e1-4923-8541-68ce84caebad"
            }
          ]
        }
      ]
    }
  ]
}