---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List ident number of a variation
  description: Lists the ident number (ASIN/ePID) of a variation. The ID of the item
    and the ID of the variation must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/{id}/variations/{variationId}/market_ident_numbers:
    get:
      summary: List ident number of a variation
      description: Lists the ident number (ASIN/ePID) of a variation. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationMarketEntNumbers
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Ident
      - Number
      - Of
      - Variation
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