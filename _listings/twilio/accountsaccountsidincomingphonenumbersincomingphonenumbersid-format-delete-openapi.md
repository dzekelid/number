---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Delete Incoming Phone Number
  description: Release this phone number from your account. Twilio will no longer
    answerncalls to this number, and you will stop being billed the monthly phonennumber
    fee. The phone number will eventually be recycled and potentiallyngiven to another
    customer, so use with care. If you make a mistake, contacnus. We may be able to
    give you the number back.n
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/AvailablePhoneNumbers/{IsoCountryCode}/Local.{format}:
    get:
      summary: Get Available Local Phone Numbers
      description: Returns a list of local AvailablePhoneNumber resource representationsnthat
        match the specified filters, each representing a phone number thanis currently
        available for provisioning within your account.n
      operationId: returns-a-list-of-local-availablephonenumber-resource-representationsthat-match-the-specified-filter
      x-api-path-slug: accountsaccountsidavailablephonenumbersisocountrycodelocal-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      - in: path
        name: IsoCountryCode
        description: ISO 3166-1 alpha-2
      responses:
        200:
          description: OK
      tags:
      - Phone Numbers
  /Accounts/{AccountSid}/AvailablePhoneNumbers/{IsoCountryCode}/Mobile.{format}:
    get:
      summary: Get Available Mobile Phone Numbers
      description: Returns a list of mobile AvailablePhoneNumber resource representations
        that match the specified filters, each representing a phone number that is
        currently available for provisioning within your account.
      operationId: returns-a-list-of-mobile-availablephonenumber-resource-representations-that-match-the-specified-filt
      x-api-path-slug: accountsaccountsidavailablephonenumbersisocountrycodemobile-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      - in: path
        name: IsoCountryCode
        description: ISO 3166-1 alpha-2
      responses:
        200:
          description: OK
      tags:
      - Phone Numbers
  /Accounts/{AccountSid}/AvailablePhoneNumbers/{IsoCountryCode}/TollFree.{format}:
    get:
      summary: Get Available Toll Free Phone Numbers
      description: Returns a list of toll-free AvailablePhoneNumber elements that
        match thenspecified filters, each representing a phone number that is currentlynavailable
        for provisioning within your account. To provision an availablenphone number,
        POST the number to the IncomingPhoneNumbers resource.n
      operationId: returns-a-list-of-tollfree-availablephonenumber-elements-that-match-thespecified-filters-each-repres
      x-api-path-slug: accountsaccountsidavailablephonenumbersisocountrycodetollfree-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      - in: path
        name: IsoCountryCode
        description: ISO 3166-1 alpha-2
      responses:
        200:
          description: OK
      tags:
      - Phone Numbers
  /Accounts/{AccountSid}/IncomingPhoneNumbers/Local.{format}:
    get:
      summary: Get Incoming Local Phone Numbers
      description: Returns a list of local <IncomingPhoneNumber> elements, each representing
        a local (not toll-free) phone number given to your account, under an <IncomingPhoneNumbers>
        list element that includes paging information. Works exactly the same as the
        IncomingPhoneNumber resource, but filters out toll-free numbers.
      operationId: returns-a-list-of-local-incomingphonenumber-elements-each-representing-a-local-not-tollfree-phone-nu
      x-api-path-slug: accountsaccountsidincomingphonenumberslocal-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Incoming Phone Numbers
    post:
      summary: Add Incoming Local Phone Numbers
      description: Adds a new phone number to your account. If a phone number is found
        for your request, Twilio will add it to your account and bill you for the
        first months cost of the phone number.
      operationId: adds-a-new-phone-number-to-your-account-if-a-phone-number-is-found-for-your-request-twilio-will-add-
      x-api-path-slug: accountsaccountsidincomingphonenumberslocal-format-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Incoming Phone Numbers
  /Accounts/{AccountSid}/IncomingPhoneNumbers/Mobile.{format}:
    get:
      summary: Get Incoming Phone Numbers
      description: Returns a list of local <IncomingPhoneNumber> elements, each representing
        a mobile phone number given to your account, under an <IncomingPhoneNumbers>
        list element that includes paging information. Works exactly the same as the
        IncomingPhoneNumber resource, but filters out local and toll free numbers.
      operationId: returns-a-list-of-local-incomingphonenumber-elements-each-representing-a-mobile-phone-number-given-t
      x-api-path-slug: accountsaccountsidincomingphonenumbersmobile-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Incoming Phone Numbers
  /Accounts/{AccountSid}/IncomingPhoneNumbers/{IncomingPhoneNumberSid}.{format}:
    delete:
      summary: Delete Incoming Phone Number
      description: Release this phone number from your account. Twilio will no longer
        answerncalls to this number, and you will stop being billed the monthly phonennumber
        fee. The phone number will eventually be recycled and potentiallyngiven to
        another customer, so use with care. If you make a mistake, contacnus. We may
        be able to give you the number back.n
      operationId: release-this-phone-number-from-your-account-twilio-will-no-longer-answercalls-to-this-number-and-you
      x-api-path-slug: accountsaccountsidincomingphonenumbersincomingphonenumbersid-format-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      - in: path
        name: IncomingPhoneNumberSid
        description: A 34 character string that uniquely identifies the incoming phone
          number
      responses:
        200:
          description: OK
      tags:
      - Incoming Phone Numbers
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