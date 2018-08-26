{
  "info": {
    "name": "AWS Simple Notification Service API Check If Phone Number Is Opted Out",
    "_postman_id": "c9cba40c-d1ad-4f9c-b7c0-5dc3b3b8f990",
    "description": "Accepts a phone number and indicates whether the phone holder has opted out of receiving SMS messages from your account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "8d5fb795-b8af-437e-a87f-3fbda4865b9d",
          "name": "addPermission",
          "request": {
            "url": "http://example.com/api/?Action=AddPermission?ActionName.member.N=ActionName.member.N&AWSAccountId.member.N=AWSAccountId.member.N&Label=Label&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a statement to a topic's access control policy, granting access for the specified AWS accounts to the specified actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77737b14-202b-42bd-a582-0be1595ff2b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Opt Out",
      "item": [
        {
          "id": "b9044612-9413-4798-b97f-06fdc2bb3232",
          "name": "checkIfPhoneNumberIsOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=CheckIfPhoneNumberIsOptedOut?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts a phone number and indicates whether the phone holder has opted out of receiving SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67be764d-098a-486f-b499-1cdf1afb77d6"
            }
          ]
        }
      ]
    }
  ]
}