{
  "info": {
    "name": "Steem number of accounts",
    "_postman_id": "d225dc24-b83f-4770-8ac5-0efe6e4b023f",
    "description": "Get Number of Accounts from Steem",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Number",
      "item": [
        {
          "id": "ffc7ba33-12db-4496-bcae-353dc2c0e7ad",
          "name": "get-number-of-accounts-from-steem",
          "request": {
            "url": "http://api.steemjs.com/get_account_count",
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
            "description": "Get Number of Accounts from Steem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1467cdea-d1fd-47cc-8b9c-43ff31be1d59"
            }
          ]
        }
      ]
    }
  ]
}