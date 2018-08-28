---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Get a representation of a GCMD keyword.
  description: Get JSON which represents the structure of a GCMD keyword.
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gcmd_keyword:
    get:
      summary: List GCMD keywords in the GCIS.
      description: List the GCMD keywords in the GCIS, 20 per page.
      operationId: list-the-gcmd-keywords-in-the-gcis-20-per-page
      x-api-path-slug: gcmd-keyword-get
      parameters:
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - GCMD
      - Keywords
      - GCIS
  /gcmd_keyword/{gcmd_keyword_identifier}:
    get:
      summary: Get a representation of a GCMD keyword.
      description: Get JSON which represents the structure of a GCMD keyword.
      operationId: get-json-which-represents-the-structure-of-a-gcmd-keyword
      x-api-path-slug: gcmd-keywordgcmd-keyword-identifier-get
      parameters:
      - in: path
        name: gcmd_keyword_identifier
        description: gcmd_keyword_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - GCMD
      - Keyword
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