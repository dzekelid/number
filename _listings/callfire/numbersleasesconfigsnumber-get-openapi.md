---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find a specific lease config
  description: Returns a single NumberConfig instance for a given number lease
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---