---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
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
  /service/categoryentry/action/index:
    get:
      summary: Get Service Categoryentry Action Index
      description: Index CategoryEntry by Id
      operationId: categoryEntry.index
      x-api-path-slug: servicecategoryentryactionindex-get
      parameters:
      - in: query
        name: categoryId
      - in: query
        name: entryId
      - in: query
        name: No Name
      - in: query
        name: shouldUpdate
      responses:
        200:
          description: OK
      tags:
      - Service
      - Categoryentry
      - Action
      - Index
  /service/categoryuser/action/index:
    get:
      summary: Get Service Categoryuser Action Index
      description: Index CategoryUser by userid and category id
      operationId: categoryUser.index
      x-api-path-slug: servicecategoryuseractionindex-get
      parameters:
      - in: query
        name: categoryId
      - in: query
        name: No Name
      - in: query
        name: shouldUpdate
      - in: query
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Categoryuser
      - Action
      - Index
---