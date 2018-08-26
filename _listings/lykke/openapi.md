---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Utils/isUSorCanadaNumber/{phoneNumber}:
    get:
      summary: Get API Utils Isusorcanadanumber Phonenumber
      description: Get api utils isusorcanadanumber phonenumber.
      operationId: ApiUtilsIsUSorCanadaNumberByPhoneNumberGet
      x-api-path-slug: apiutilsisusorcanadanumberphonenumber-get
      parameters:
      - in: path
        name: phoneNumber
      responses:
        200:
          description: OK
      tags:
      - Utils
      - Isusorcanadanumber
      - Phonenumber
---