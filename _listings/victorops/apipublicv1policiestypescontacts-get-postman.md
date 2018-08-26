{
  "info": {
    "name": "Victor Ops Get the available contact types",
    "_postman_id": "9161832b-6cdc-4487-a1b2-3cf6e1a59968",
    "description": "Get the available contact types\n\ndescription: \"Email Address\", type: \"email\"\ndescription: \"Phone Number\", type: \"phone\"\n\nThis API may be called a maximum of 15 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Policies",
      "item": [
        {
          "id": "55164875-66e0-4db5-8aaf-ba7f662a74c2",
          "name": "api_public.v1.policies.types.contacts.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/contacts?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available contact types\n\ndescription: \"Email Address\", type: \"email\"\ndescription: \"Phone Number\", type: \"phone\"\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "035dedc5-e23e-4c9a-abb2-d6dbcf7e69b4"
            }
          ]
        }
      ]
    }
  ]
}