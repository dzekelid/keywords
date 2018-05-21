---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find keywords
  description: Searches for all keywords available for purchase on the CallFire platform.
    If a keyword appears in the response, it is available for purchase. List the 'keywords'
    in a query parameter to search for multiple keywords (at least one keyword should
    be sent in request)
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