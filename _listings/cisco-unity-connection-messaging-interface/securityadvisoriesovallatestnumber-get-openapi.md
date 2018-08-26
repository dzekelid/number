---
swagger: "2.0"
x-collection-name: Cisco Unity Connection Messaging Interface
x-complete: 0
info:
  title: Cisco PSIRT open Vuln Get Security Advisories Oval Latest Number
  description: Used to obtain all the latest OVAL definitions given an absolute number.
    For instance, the latest 10 or latest 5.
  contact:
    name: Omar Santos
    email: os@cisco.com
  version: 0.0.3
host: api.cisco.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /security/advisories/cvrf/latest/{number}:
    get:
      summary: Get Security Advisories Latest Number
      description: Used to obtain all the latest security advisories in CVRF format
        given an absolute number. For instance, the latest 10 or latest 5.
      operationId: used-to-obtain-all-the-latest-security-advisories-in-cvrf-format-given-an-absolute-number--for-insta
      x-api-path-slug: securityadvisoriescvrflatestnumber-get
      parameters:
      - in: path
        name: number
        description: An absolute number to obtain the latest security advisories
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Latest
      - Number
  /security/advisories/oval/latest/{number}:
    get:
      summary: Get Security Advisories Oval Latest Number
      description: Used to obtain all the latest OVAL definitions given an absolute
        number. For instance, the latest 10 or latest 5.
      operationId: used-to-obtain-all-the-latest-oval-definitions-given-an-absolute-number--for-instance-the-latest-10-
      x-api-path-slug: securityadvisoriesovallatestnumber-get
      parameters:
      - in: path
        name: number
        description: The latest OVAL definitions (absolute number)
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Oval
      - Latest
      - Number
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