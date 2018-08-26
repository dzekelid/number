---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 1
info:
  title: Taxamo
  description: taxamos-elegant-suite-of-apis-and-comprehensive-reporting-dashboard-enables-digital-merchants-to-easily-comply-with-eu-regulatory-requirements-on-tax-calculation-evidence-collection-tax-return-creation-and-data-storage-
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/tax/vat_numbers/{tax_number}/validate:
    get:
      summary: Validate VAT Number
      description: Validate vat number.
      operationId: validateTaxNumber
      x-api-path-slug: apiv1taxvat-numberstax-numbervalidate-get
      parameters:
      - in: query
        name: country_code
        description: Two-letter ISO country code
      - in: path
        name: tax_number
        description: Tax number
      responses:
        200:
          description: OK
      tags:
      - Validate
      - VAT
      - Number
---