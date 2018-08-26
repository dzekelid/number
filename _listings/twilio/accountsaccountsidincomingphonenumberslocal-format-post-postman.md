{
  "info": {
    "name": "Twilio Add Incoming Local Phone Numbers",
    "_postman_id": "368b9200-ec6b-4b91-9791-41a60aefffe2",
    "description": "Adds a new phone number to your account. If a phone number is found for your request, Twilio will add it to your account and bill you for the first months cost of the phone number.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "incoming phone numbers",
      "item": [
        {
          "id": "2c62a310-c0c2-4bb5-8679-a20f9d1958fb",
          "name": "adds-a-new-phone-number-to-your-account-if-a-phone-number-is-found-for-your-request-twilio-will-add-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/Local.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new phone number to your account"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"uri\": \"uri\",\r\n    \"firstpageuri\": \"firstpageuri\",\r\n    \"nextpageuri\": \"nextpageuri\",\r\n    \"previouspageuri\": \"previouspageuri\",\r\n    \"page\": \"page\",\r\n    \"pagesize\": \"pagesize\",\r\n    \"incoming_phone_numbers\": {}\r\n  }\r\n]",
              "status": "Successful response",
              "code": 201,
              "name": "Response_201",
              "id": "e44308d4-55ee-4522-bdc7-234c5a9499d8"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "The data given in the POST or PUT failed validation",
              "code": 400,
              "name": "Response_400",
              "id": "c42db6d0-67f9-4411-9320-731c412767bc"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "The supplied credentials, if any, are not sufficient to create or update the resource",
              "code": 401,
              "name": "Response_401",
              "id": "d53dc2d2-0df7-442d-9df2-8adc9b0a222d"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "You know this one",
              "code": 404,
              "name": "Response_404",
              "id": "46e7202e-e1fc-428b-9833-4601c73f3cdc"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "You can't POST or PUT to the resource",
              "code": 405,
              "name": "Response_405",
              "id": "7f569e8f-a4be-4ab7-b3c4-a40b9b58abc3"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "Your application is sending too many simultaneous requests",
              "code": 429,
              "name": "Response_429",
              "id": "7d093eae-cff7-4fe4-b5ce-280c867856d6"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "We couldn't create or update the resource",
              "code": 500,
              "name": "Response_500",
              "id": "8fc76636-d9bb-47ec-be8a-1edbd965012c"
            }
          ]
        }
      ]
    }
  ]
}