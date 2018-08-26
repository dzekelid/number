---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/people/searchcontacts:
    post:
      summary: Search contacts based on the phone number provided
      description: Search contacts based on the phone number provided.
      operationId: People_SearchContactsBysearchCommandDataContract
      x-api-path-slug: apipeoplesearchcontacts-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchCommandDataContract
        description: Search data contract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Contacts
      - Based
      - "On"
      - Phone
      - Number
      - Provided
  /api/job/NormalisePhoneNumbers:
    post:
      summary: Normalises phone numbers for agency
      description: Normalises phone numbers for agency.
      operationId: Job_NormalisePhoneNumbersBynormalisePhoneNumbers
      x-api-path-slug: apijobnormalisephonenumbers-post
      parameters:
      - in: body
        name: normalisePhoneNumbers
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Normalises
      - Phone
      - Numbersagency
  /api/todo/getall:
    get:
      summary: "Get the list of all ToDo's if no parameter is sent;\r\n<param name=\"filterToDo\">if
        provided will filter by ToDo type</param><param name=\"pageSize\"></param><param
        name=\"pageNumber\"></param>"
      description: "Get the list of all todo's if no parameter is sent;\r\n<param
        name=\"filtertodo\">if provided will filter by todo type</param><param name=\"pagesize\"></param><param
        name=\"pagenumber\"></param>."
      operationId: DefaultToDo_GetAllBypageSizeBypageNumberByfilterToDo.filterCategoryByfilterToDo.toDoTypeByfilterToDo
      x-api-path-slug: apitodogetall-get
      parameters:
      - in: query
        name: filterToDo.branchId
      - in: query
        name: filterToDo.filterCategory
      - in: query
        name: filterToDo.negotiatorIds
      - in: query
        name: filterToDo.toDoType
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - ToDos
      - If
      - "No"
      - Parameter
      - Is
      - "Sent;\r\n<param"
      - Name=filterToDo>if
      - Provided
      - Will
      - Filter
      - By
      - ToDo
      - Type<
      - Param><param
      - Name=pageSize><
      - Param><param
      - Name=pageNumber><
      - Param>
---