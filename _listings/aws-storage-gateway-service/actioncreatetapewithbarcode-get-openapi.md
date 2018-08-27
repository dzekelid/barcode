---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Create Tape With Barcode
  version: 1.0.0
  description: Creates a virtual tape by using your own barcode.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateTapeWithBarcode:
    get:
      summary: Create Tape With Barcode
      description: Creates a virtual tape by using your own barcode.
      operationId: createTapeWithBarcode
      x-api-path-slug: actioncreatetapewithbarcode-get
      parameters:
      - in: query
        name: GatewayARN
        description: The unique Amazon Resource Name (ARN) that represents the gateway
          to associate the         virtual tape with
        type: string
      - in: query
        name: TapeBarcode
        description: The barcode that you want to assign to the tape
        type: string
      - in: query
        name: TapeSizeInBytes
        description: The size, in bytes, of the virtual tape that you want to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tape With Barcode
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