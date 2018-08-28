---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Category Action Index
  description: Index Category by id
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/baseentry/action/index:
    get:
      summary: Get Service Baseentry Action Index
      description: Index an entry by id.
      operationId: baseEntry.index
      x-api-path-slug: servicebaseentryactionindex-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: shouldUpdate
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Index
  /service/category/action/index:
    get:
      summary: Get Service Category Action Index
      description: Index Category by id
      operationId: category.index
      x-api-path-slug: servicecategoryactionindex-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: shouldUpdate
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Index
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