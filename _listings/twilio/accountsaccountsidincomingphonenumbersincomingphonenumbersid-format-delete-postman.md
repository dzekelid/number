{
  "info": {
    "name": "Twilio Delete Incoming Phone Number",
    "_postman_id": "2b6eeed5-bbfb-431b-a5da-4f16d7ffb79a",
    "description": "Release this phone number from your account. Twilio will no longer answerncalls to this number, and you will stop being billed the monthly phonennumber fee. The phone number will eventually be recycled and potentiallyngiven to another customer, so use with care. If you make a mistake, contacnus. We may be able to give you the number back.n",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "incoming phone numbers",
      "item": [
        {
          "id": "ae032619-ef2a-44e4-abc7-19bcd70e1076",
          "name": "release-this-phone-number-from-your-account-twilio-will-no-longer-answercalls-to-this-number-and-you",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/:IncomingPhoneNumberSid.json"
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
                },
                {
                  "id": "IncomingPhoneNumberSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Release this phone number from your account"
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
              "code": 200,
              "name": "Response_200",
              "id": "5b36c142-0454-4e92-b35a-132b0c8931a3"
            }
          ]
        }
      ]
    }
  ]
}