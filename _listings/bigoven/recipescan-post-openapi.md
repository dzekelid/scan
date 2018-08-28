---
swagger: "2.0"
x-collection-name: BigOven
x-complete: 0
info:
  title: "Big Oven POST an image as a new RecipeScan request\r\n                1)
    \ Fetch the filename -- DONE\r\n                2)  Copy it to the pics/scan folder
    - ENSURE NO NAMING COLLISIONS -- DONE\r\n                3)  Create 120 thumbnail
    size  in pics/scan/120 -- D"
  description: "Post an image as a new recipescan request\r\n                1)  fetch
    the filename -- done\r\n                2)  copy it to the pics/scan folder -
    ensure no naming collisions -- done\r\n                3)  create 120 thumbnail
    size  in pics/scan/120 -- d."
  termsOfService: Please see our [terms of service](http://api2.bigoven.com/web/documentation/termsofuse
  version: partner
host: api2.bigoven.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /recipe/scan:
    post:
      summary: "POST an image as a new RecipeScan request\r\n                1)  Fetch
        the filename -- DONE\r\n                2)  Copy it to the pics/scan folder
        - ENSURE NO NAMING COLLISIONS -- DONE\r\n                3)  Create 120 thumbnail
        size  in pics/scan/120 -- D"
      description: "Post an image as a new recipescan request\r\n                1)
        \ fetch the filename -- done\r\n                2)  copy it to the pics/scan
        folder - ensure no naming collisions -- done\r\n                3)  create
        120 thumbnail size  in pics/scan/120 -- d."
      operationId: Recipe_Scan
      x-api-path-slug: recipescan-post
      parameters:
      - in: query
        name: devicetype
      - in: query
        name: lat
      - in: query
        name: lng
      - in: query
        name: test
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Scan
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