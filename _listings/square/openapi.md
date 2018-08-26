---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/bank-accounts:
    get:
      summary: Provides non-confidential details for all of a location's associated
        bank accounts. This endpoint does not provide full bank account numbers, and
        there is no way to obtain a full bank account number with the Connect API.
      description: Provides non-confidential details for all of a location's associated
        bank accounts. This endpoint does not provide full bank account numbers, and
        there is no way to obtain a full bank account number with the Connect API.
      operationId: ListBankAccounts
      x-api-path-slug: v1location-idbankaccounts-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list bank accounts for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Non-confidential
      - Details
      - Of
      - Locations
      - Associated
      - Bank
      - Accounts
      - ""
      - This
      - Endpoint
      - Does
      - Not
      - Provide
      - Full
      - Bank
      - Account
      - Numbers
      - ""
      - There
      - Is
      - "No"
      - Way
      - To
      - Obtain
      - Full
      - Bank
      - Account
      - Number
      - Connect
  /v1/{location_id}/bank-accounts/{bank_account_id}:
    get:
      summary: Provides non-confidential details for a merchant's associated bank
        account. This endpoint does not provide full bank account numbers, and there
        is no way to obtain a full bank account number with the Connect API.
      description: Provides non-confidential details for a merchant's associated bank
        account. This endpoint does not provide full bank account numbers, and there
        is no way to obtain a full bank account number with the Connect API.
      operationId: RetrieveBankAccount
      x-api-path-slug: v1location-idbankaccountsbank-account-id-get
      parameters:
      - in: path
        name: bank_account_id
        description: The bank accounts Square-issued ID
      - in: path
        name: location_id
        description: The ID of the bank accounts associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Non-confidential
      - Detailsa
      - Merchants
      - Associated
      - Bank
      - Account
      - ""
      - This
      - Endpoint
      - Does
      - Not
      - Provide
      - Full
      - Bank
      - Account
      - Numbers
      - ""
      - There
      - Is
      - "No"
      - Way
      - To
      - Obtain
      - Full
      - Bank
      - Account
      - Number
      - Connect
---