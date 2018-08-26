{
  "info": {
    "name": "AWS Simple Notification Service API Opt In Phone Number",
    "_postman_id": "16ca3af1-d319-47bc-a6a8-e88fa991afb9",
    "description": "Use this request to opt in a phone number that is opted out, which enables you to resume sending SMS messages to the number.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "762ccb2e-ba7d-4a16-8211-f016d13949b3",
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
              "id": "953e0827-b993-4a5c-823b-30ec9a8688ca"
            }
          ]
        }
      ]
    },
    {
      "name": "Opt Out",
      "item": [
        {
          "id": "fb9dce20-e78e-49cf-b7e9-bb25abcec8c8",
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
              "id": "4a3d3317-78ab-42a2-a245-f835376f1fab"
            }
          ]
        },
        {
          "id": "cc540f30-8bf3-4acf-ade5-8f3492ccb3a5",
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
              "id": "58a1966c-cbfb-4c20-903b-a1ae21f33684"
            }
          ]
        },
        {
          "id": "8efe2ada-56cc-4a0d-b8c1-800e8f7de98c",
          "name": "optInPhoneNumber",
          "request": {
            "url": "http://example.com/api/?Action=OptInPhoneNumber?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this request to opt in a phone number that is opted out, which enables you to resume sending SMS messages to the number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee6a1108-aac5-434e-9265-582192f3c631"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "6383929d-66dc-40ca-b9e8-7049a54c0125",
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
              "id": "d3957141-c775-4b00-9ee9-2c1f3f630a86"
            }
          ]
        },
        {
          "id": "4128a5b5-79a1-499e-8ce1-635d793d29cd",
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
              "id": "96052ca4-04d5-4f59-9adf-67232236b645"
            }
          ]
        },
        {
          "id": "43607a4f-a926-4e40-b646-754a8d6ab08f",
          "name": "listSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptions?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9e62de5-2bdc-470d-9fa6-0dd9fcbdf171"
            }
          ]
        },
        {
          "id": "94a89360-7b82-4758-b792-0f14a0afc052",
          "name": "listSubscriptionsByTopic",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptionsByTopic?NextToken=NextToken&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the subscriptions to a specific topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d60690e-798a-44bb-b1db-bc72e9d54b7c"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Applications",
      "item": [
        {
          "id": "5c6d0049-359b-492e-a492-a73a0b426205",
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
              "id": "810b249b-2361-43b2-a0c6-87a860877c10"
            }
          ]
        },
        {
          "id": "ffc1f80b-c59a-4551-a8ec-d8a7411b5e3a",
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
              "id": "884c9fd1-2a04-48f9-ae9e-b1f82101115d"
            }
          ]
        },
        {
          "id": "430a27d0-f621-47e6-b9ba-b0e35a80f256",
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
              "id": "1412b96a-0b02-4b3f-9484-226068f21b5f"
            }
          ]
        },
        {
          "id": "22658367-9469-43f8-bc2e-ed5ede4e3c9f",
          "name": "listPlatformApplications",
          "request": {
            "url": "http://example.com/api/?Action=ListPlatformApplications?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the platform application objects for the supported push notification services, such as\n      APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4639f20-f853-429a-b148-10dc2daa8afe"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Endpoints",
      "item": [
        {
          "id": "2a8fcd92-c2ed-41e4-9e65-fa245dcb7169",
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
              "id": "577f3d1e-1bd3-4a45-a2ff-92bae07073f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Topics",
      "item": [
        {
          "id": "75a1cf25-5c48-4d6e-afd2-acb53b390299",
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
              "id": "e6ae34d4-8329-4d7f-8c7e-14a48c6c1765"
            }
          ]
        },
        {
          "id": "43da23c0-c7c4-4b2c-9576-6f7aa2bbc7d6",
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
              "id": "ab16c58a-6527-4020-ba9f-1652f276aaaa"
            }
          ]
        },
        {
          "id": "d4f9aba2-8a9f-444d-ac27-8a6203c70c2b",
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
              "id": "6f4da6bb-7183-40ee-a588-f12662b7e6e9"
            }
          ]
        },
        {
          "id": "a2977f67-7f42-4df8-8369-399c05577adc",
          "name": "listTopics",
          "request": {
            "url": "http://example.com/api/?Action=ListTopics?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2da28b29-5463-44e8-b148-c5044fe01099"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "d6c03ea6-6eb5-468c-94f2-51c6e919bbe4",
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
              "id": "d2683477-7525-45ae-8fb6-ece6443a6464"
            }
          ]
        },
        {
          "id": "4fb69806-84a5-4275-b379-ae310881383a",
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
              "id": "955faace-81ec-44a0-9a3b-d6b6e1f42381"
            }
          ]
        },
        {
          "id": "ab44b10e-a35c-464f-8cb5-54fe0cdb88ff",
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
              "id": "1a0e9421-4c14-490a-bc0e-2214308410f4"
            }
          ]
        }
      ]
    },
    {
      "name": "SMS",
      "item": [
        {
          "id": "4d1f301c-ad7a-4b24-9c6c-a663accd08c5",
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
              "id": "6626c841-0e2b-45d5-8eda-b0a423e02ace"
            }
          ]
        }
      ]
    }
  ]
}