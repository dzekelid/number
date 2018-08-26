---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/message/chats/{pageNumber}/{search}:
    get:
      summary: Get Message Chats Pagenumber Search
      description: Get message chats pagenumber search.
      operationId: getApiV1MessageChatsPagenumberSearch
      x-api-path-slug: apiv1messagechatspagenumbersearch-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: pageNumber
      - in: path
        name: search
      - in: query
        name: unread
      responses:
        200:
          description: OK
      tags:
      - Message
      - Chats
      - Pagenumber
      - Search
---