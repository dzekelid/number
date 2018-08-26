---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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
    post:
      summary: Create a market ident number
      description: Creates a market ident number (ASIN/ePID) for a variation.
      operationId: postRestItemsVariationsVariationMarketEntNumbers
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbers-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/market_ident_numbers
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Ident
      - Number
  /rest/items/{id}/variations/{variationId}/market_ident_numbers/{marketIdentNumberId}:
    delete:
      summary: Deletes a market ident number
      description: Deletes a market ident number (ASIN/ePID) of a variation.
      operationId: deleteRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Market
      - Ident
      - Number
    get:
      summary: Get a market ident number
      description: Gets a market ident number (ASIN/ePID) of a variation.
      operationId: getRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Ident
      - Number
    put:
      summary: Updates a market ident number
      description: Updates a market ident number (ASIN/ePID) of a variation.
      operationId: putRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/market_ident_numbers/{marketIdentNumberId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Market
      - Ident
      - Number
---