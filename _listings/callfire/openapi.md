swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
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
  /keywords/leases/{keyword}:
    get:
      summary: Find a specific lease
      description: Searches for all keywords owned by user
      operationId: getKeywordLease
      x-api-path-slug: keywordsleaseskeyword-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: keyword
        description: Keyword text that a lease is desired for
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Leases
      - Keyword
    put:
      summary: Update a lease
      description: Updates a keyword lease. Turns the autoRenew on/off.
      operationId: updateKeywordLease
      x-api-path-slug: keywordsleaseskeyword-put
      parameters:
      - in: body
        name: body
        description: A keyword lease object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: keyword
        description: To update a keyword lease
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Leases
      - Keyword
  /keywords/{keyword}/available:
    get:
      summary: Check for a specific keyword
      description: Searches for the specific keyword to purchase on the CallFire platform.
        Returns 'true' if keyword is available.
      operationId: isKeywordAvailable
      x-api-path-slug: keywordskeywordavailable-get
      parameters:
      - in: path
        name: keyword
        description: To specify a keyword to search for
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Keyword
      - Available
  /orders/keywords:
    post:
      summary: Purchase keywords
      description: Purchase keywords. Send a list of available keywords into this
        API to purchase them using CallFire credits. Make sure the account has enough
        credits before trying to purchase the keywords
      operationId: orderKeywords
      x-api-path-slug: orderskeywords-post
      parameters:
      - in: body
        name: body
        description: Request object which contains a list of keywords to buy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Keywords