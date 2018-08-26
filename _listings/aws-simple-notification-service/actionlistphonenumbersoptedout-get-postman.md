{
  "info": {
    "name": "AWS Simple Notification Service API List Phone Numbers Opted Out",
    "_postman_id": "1144919d-3590-4846-b769-cea1fbeb5e79",
    "description": "Returns a list of phone numbers that are opted out, meaning you cannot send SMS messages to them.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "4a0cbd7a-101e-4357-b063-23416f821674",
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
              "id": "deb1a663-2915-4110-9e44-a17d0f0bf144"
            }
          ]
        }
      ]
    },
    {
      "name": "Opt Out",
      "item": [
        {
          "id": "b1362bb6-f73d-49a1-9339-92ffe0560fdc",
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
              "id": "23e077e5-ff26-45f0-8d0a-3116cba28e1b"
            }
          ]
        },
        {
          "id": "684da065-57c7-4519-bdb7-94024ab10508",
          "name": "listPhoneNumbersOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=ListPhoneNumbersOptedOut?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of phone numbers that are opted out, meaning you cannot send SMS messages to them."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5c73b3a-820f-453e-8b2b-00bfb3de560d"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "9f69d2f4-2ede-4c4c-be34-414694c9a8e1",
          "name": "confirmSubscription",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmSubscription?AuthenticateOnUnsubscribe=AuthenticateOnUnsubscribe&Token=Token&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Verifies an endpoint owner's intent to receive messages by validating the token sent to the\n      endpoint by an earlier Subscribe action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb4ecfd7-5eb2-42dd-b3f8-699e904b326e"
            }
          ]
        },
        {
          "id": "34e3fe83-53f3-4260-b9c8-99cee55c21e1",
          "name": "getSubscriptionAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSubscriptionAttributes?SubscriptionArn=SubscriptionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af7c7481-e1f4-48c2-8ad6-162ed41a2fc5"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Applications",
      "item": [
        {
          "id": "1032ab91-2406-4ac2-bab5-1504182ac056",
          "name": "createPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformApplication?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&Name=Name&Platform=Platform",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a platform application object for one of the supported push notification services,\n      such as APNS and GCM, to which devices and mobile apps may register."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1f1cfee-ff70-414a-9a95-46c77aee74af"
            }
          ]
        },
        {
          "id": "19c89d05-beca-4955-b9b4-cb70095828e2",
          "name": "deletePlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=DeletePlatformApplication?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a platform application object for one of the supported push notification services,\n      such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a9c0b77-6988-4d94-824d-fdac55ff4637"
            }
          ]
        },
        {
          "id": "8fc419cb-f7e1-4b08-bd85-6d6be32dab15",
          "name": "getPlatformApplicationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetPlatformApplicationAttributes?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the attributes of the platform application object for the supported push\n      notification services, such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b32ce1f4-8752-434f-9427-1788f13dedd0"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Endpoints",
      "item": [
        {
          "id": "7a2c41a3-b3a0-4944-995b-2470f59c94c3",
          "name": "createPlatformEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformEndpoint?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&CustomUserData=CustomUserData&PlatformApplicationArn=PlatformApplicationArn&Token=Token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an endpoint for a device and mobile app on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "365e6396-9d65-41ea-8fa1-d5b9cde8d8a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Topics",
      "item": [
        {
          "id": "235a594a-0f80-4f08-b9c5-99fe713091a3",
          "name": "createTopic",
          "request": {
            "url": "http://example.com/api/?Action=CreateTopic?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a topic to which notifications can be published."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c88c235-5a5a-408f-b638-69d92c002033"
            }
          ]
        },
        {
          "id": "426611e5-6ca5-46eb-afa0-f8eaa7573f2f",
          "name": "deleteTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTopic?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a topic and all its subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a66bb6c-a147-4ffd-83bf-7523d1f7695d"
            }
          ]
        },
        {
          "id": "5db6f4df-da56-47a9-9442-a1da08c51352",
          "name": "getTopicAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetTopicAttributes?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abbae6bf-7178-47d5-a05c-7e3d7a7d5a7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "9aa2621c-3a54-4a1d-843b-c0dc430f9583",
          "name": "deleteEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEndpoint?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the endpoint for a device and mobile app from Amazon SNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c1866e0-5e09-49a3-89f5-0abfdac70224"
            }
          ]
        },
        {
          "id": "8c0daf92-fbbe-4b3a-8938-16f5f963c62d",
          "name": "getEndpointAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetEndpointAttributes?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the endpoint attributes for a device on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abe6a0df-ed78-4078-b793-5bdb1bb18b34"
            }
          ]
        },
        {
          "id": "d74756da-c184-4b36-a546-567cdb5f9511",
          "name": "listEndpointsByPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=ListEndpointsByPlatformApplication?NextToken=NextToken&PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the endpoints and endpoint attributes for devices in a supported push notification\n      service, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37b92f8a-31cc-4999-b361-89d31cca6c1a"
            }
          ]
        }
      ]
    },
    {
      "name": "SMS",
      "item": [
        {
          "id": "71137fdc-e501-4c36-ab6e-23411eaeeabc",
          "name": "getSMSAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSMSAttributes?attributes.member.N=attributes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the settings for sending SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7bec375-90c6-4bf1-8a66-714a016e2f70"
            }
          ]
        }
      ]
    }
  ]
}