---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4528049998/fulfillments/count.json:
    get:
      summary: Count all the total number of fulfillments for an order.
      description: Count all the total number of fulfillments for an order..
      operationId: getAdminOrders4528049998FulfillmentsCount.json
      x-api-path-slug: adminorders4528049998fulfillmentscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Total
      - Number
      - Fulfillmentsan
      - Order
---