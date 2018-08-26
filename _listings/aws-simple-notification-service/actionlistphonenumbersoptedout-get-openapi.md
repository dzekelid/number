---
swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 0
info:
  title: AWS Simple Notification Service API List Phone Numbers Opted Out
  version: 1.0.0
  description: Returns a list of phone numbers that are opted out, meaning you cannot
    send SMS messages to them.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CheckIfPhoneNumberIsOptedOut:
    get:
      summary: Check If Phone Number Is Opted Out
      description: Accepts a phone number and indicates whether the phone holder has
        opted out of receiving SMS messages from your account.
      operationId: checkIfPhoneNumberIsOptedOut
      x-api-path-slug: actioncheckifphonenumberisoptedout-get
      parameters:
      - in: query
        name: phoneNumber
        description: The phone number for which you want to check the opt out status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Opt Out
  /?Action=ListPhoneNumbersOptedOut:
    get:
      summary: List Phone Numbers Opted Out
      description: Returns a list of phone numbers that are opted out, meaning you
        cannot send SMS messages to them.
      operationId: listPhoneNumbersOptedOut
      x-api-path-slug: actionlistphonenumbersoptedout-get
      parameters:
      - in: query
        name: nextToken
        description: A NextToken string is used when you call the      ListPhoneNumbersOptedOut
          action to retrieve additional records that are      available after the
          first page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Opt Out
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