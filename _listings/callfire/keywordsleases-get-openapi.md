---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find keyword leases
  description: Searches for all keywords owned by user. A keyword lease is the ownership
    information involving a keyword
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /keywords:
    get:
      summary: Find keywords
      description: Searches for all keywords available for purchase on the CallFire
        platform. If a keyword appears in the response, it is available for purchase.
        List the 'keywords' in a query parameter to search for multiple keywords (at
        least one keyword should be sent in request)
      operationId: findKeywords
      x-api-path-slug: keywords-get
      parameters:
      - in: query
        name: keywords
        description: A keyword to search for
      responses:
        200:
          description: OK
      tags:
      - Keywords
  /keywords/leases:
    get:
      summary: Find keyword leases
      description: Searches for all keywords owned by user. A keyword lease is the
        ownership information involving a keyword
      operationId: findKeywordLeases
      x-api-path-slug: keywordsleases-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Leases
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