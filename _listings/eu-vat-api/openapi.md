---
swagger: "2.0"
x-collection-name: EU VAT API
x-complete: 1
info:
  title: VAT API
  description: a-developer-friendly-api-to-help-your-business-achieve-vat-compliance
  version: "1"
host: vatapi.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /vat-number-check:
    get:
      summary: Validate a VAT number
      description: Validate a vat number.
      operationId: vat_number_validate
      x-api-path-slug: vatnumbercheck-get
      parameters:
      - in: header
        name: Response-Type
        description: The default response type is application/json if you would like
          to receive an XML response then set this to XML
      - in: query
        name: vatid
        description: The VAT number to validate
      responses:
        200:
          description: OK
      tags:
      - Validate
      - VAT
      - Number
---