---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 1
info:
  title: Victor Ops
  description: this-api-allows-you-to-interact-with-the-victorops-platform-in-various-ways--your-account-may-be-limitedto-a-total-number-of-api-calls-per-month--also-some-of-these-api-calls-have-rate-limits-note-in-this-documentation-when-creating-a-sample-curl-request-clicking-the-try-it-out-button-in-some-apiviewing-interfaces-the--in-an-email-address-may-be-encoded--please-note-that-the-rest-endpoints-will-notprocess-the-encoded-version--make-sure-that-the-encoded-character-40-is-changed-to-its-unencoded-form-beforesubmitting-the-curl-request-
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v1/policies/types/contacts:
    get:
      summary: Get the available contact types
      description: |-
        Get the available contact types

        description: "Email Address", type: "email"
        description: "Phone Number", type: "phone"

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.policies.types.contacts.get
      x-api-path-slug: apipublicv1policiestypescontacts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Policies
      - Types
      - Contacts
---