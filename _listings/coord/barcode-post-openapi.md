---
swagger: "2.0"
x-collection-name: Coord
x-complete: 0
info:
  title: Coord Parking Access API Create a barcode
  description: Create a barcode for a user to be scanned upon entering/exiting a parking
    lot.
  version: 1.0.0
host: api.coord.co
basePath: /v1/access/parking
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /barcode:
    post:
      summary: Create a barcode
      description: Create a barcode for a user to be scanned upon entering/exiting
        a parking lot.
      operationId: create_barcode
      x-api-path-slug: barcode-post
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: body
        name: request
        description: A request to simulate an arrival/departure associated with the
          session
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Barcode
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