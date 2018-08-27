---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create a variation barcode
  description: Creates a variation barcode. The ID of the item, the ID of the variation,
    the ID of the barcode and the code must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/barcodes:
    post:
      summary: Create a barcode
      description: Creates a barcode.
      operationId: postRestItemsBarcodes
      x-api-path-slug: restitemsbarcodes-post
      parameters:
      - in: body
        name: /rest/items/barcodes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Barcode
  /rest/items/barcodes/{barcodeId}:
    delete:
      summary: Delete a barcode
      description: Deletes a barcode. The ID of the barcode must be specified.
      operationId: deleteRestItemsBarcodesBarcode
      x-api-path-slug: restitemsbarcodesbarcodeid-delete
      parameters:
      - in: path
        name: barcodeId
      responses:
        200:
          description: OK
      tags:
      - Barcode
    get:
      summary: Get a barcode
      description: Gets a barcode. The ID of the barcode must be specified.
      operationId: getRestItemsBarcodesBarcode
      x-api-path-slug: restitemsbarcodesbarcodeid-get
      parameters:
      - in: path
        name: barcodeId
      responses:
        200:
          description: OK
      tags:
      - Barcode
    put:
      summary: Update a barcode
      description: Updates a barcode. The ID of the barcode must be specified.
      operationId: putRestItemsBarcodesBarcode
      x-api-path-slug: restitemsbarcodesbarcodeid-put
      parameters:
      - in: body
        name: /rest/items/barcodes/{barcodeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: barcodeId
      responses:
        200:
          description: OK
      tags:
      - Barcode
  /rest/items/{id}/variations/{variationId}/variation_barcodes:
    post:
      summary: Create a variation barcode
      description: Creates a variation barcode. The ID of the item, the ID of the
        variation, the ID of the barcode and the code must be specified.
      operationId: postRestItemsVariationsVariationVariationBarcodes
      x-api-path-slug: restitemsidvariationsvariationidvariation-barcodes-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_barcodes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
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