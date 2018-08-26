{
  "info": {
    "name": "GIGANDCROWD Get Message Chats Pagenumber Search",
    "_postman_id": "627e8b67-de89-40d7-8628-8162d28c79a7",
    "description": "Get message chats pagenumber search.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "4e87ef6f-5407-4960-b8e3-50afb6af09e4",
          "name": "getApiV1MessageChatsPagenumberSearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/message/chats/:pageNumber/:search"
              ],
              "query": [
                {
                  "key": "unread",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "pageNumber",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "search",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get message chats pagenumber search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3b83d27-be40-41a9-a7d3-030359e73e59"
            }
          ]
        },
        {
          "id": "632b8474-ce81-4a04-827a-3e204c09049b",
          "name": "getApiV1MessageChatFrom",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/message/chat/:id/:from"
              ],
              "variable": [
                {
                  "id": "from",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get message chat from."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe9af8dd-83fb-479a-93ab-734d80e20070"
            }
          ]
        }
      ]
    }
  ]
}