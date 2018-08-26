---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts/dncs/{number}:
    delete:
      summary: Delete do not contact (dnc) number. If number contains commas treat
        as list of numbers
      description: Delete a Do Not Contact (DNC) contact entry.
      operationId: deleteDoNotContact
      x-api-path-slug: contactsdncsnumber-delete
      parameters:
      - in: path
        name: number
        description: Number associated with Do Not Contact (DNC) entry
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Number
    get:
      summary: Get do not contact (dnc)
      description: Get Do Not Contact (DNC) object create by user. This DoNotContact
        entry only affects calls/texts/campaigns on this account.
      operationId: getDoNotContact
      x-api-path-slug: contactsdncsnumber-get
      parameters:
      - in: path
        name: number
        description: Number associated with Do Not Contact (DNC) entry
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Number
    put:
      summary: Update an individual do not contact (dnc) number
      description: Update a Do Not Contact (DNC) contact entry. Can toggle whether
        the DNC is enabled for calls/texts.
      operationId: updateDoNotContact
      x-api-path-slug: contactsdncsnumber-put
      parameters:
      - in: body
        name: body
        description: DoNotContact object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: number
        description: "~"
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Number
  /numbers/leases/configs/{number}:
    get:
      summary: Find a specific lease config
      description: Returns a single NumberConfig instance for a given number lease
      operationId: getNumberLeaseConfig
      x-api-path-slug: numbersleasesconfigsnumber-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: number
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Configs
      - Number
    put:
      summary: Update a lease config
      description: Updates a phone number lease configuration. Use this API endpoint
        to add an Inbound IVR or Call Tracking feature to a CallFire phone number.
        Call tracking configuration allows you to track the incoming calls, to analyze
        and to respond customers using sms or voice replies. For more information
        see [call tracking page](https://www.callfire.com/products/call-tracking)
      operationId: updateNumberLeaseConfig
      x-api-path-slug: numbersleasesconfigsnumber-put
      parameters:
      - in: body
        name: body
        description: The configuration of a number lease object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: number
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Configs
      - Number
  /numbers/leases/{number}:
    get:
      summary: Find a specific lease
      description: Returns a single NumberLease instance for a given number
      operationId: getNumberLease
      x-api-path-slug: numbersleasesnumber-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: number
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Number
    put:
      summary: Update a lease
      description: Updates a number lease instance. Ability to turn on/off autoRenew
        and toggle call/text features for a particular number
      operationId: updateNumberLease
      x-api-path-slug: numbersleasesnumber-put
      parameters:
      - in: body
        name: body
        description: A NumberLease object to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: number
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Number
---