swagger: "2.0"
x-collection-name: AT&T Dev Program
x-complete: 1
info:
  title: AT&T Dev Program Merged API
  version: 1.0.0
host: api.att.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /myMessages/v2/messages/index:
    post:
      summary: Post My Messages Index
      description: /myMessages/v2/messages/index
      operationId: mymessagesv2messagesindex
      x-api-path-slug: mymessagesv2messagesindex-post
      responses:
        200:
          description: OK
      tags:
      - MyMessages
      - VMessages
      - Index
  /myMessages/v2/messages/index/info:
    get:
      summary: Get My Messages Index Info
      description: /myMessages/v2/messages/index/info
      operationId: mymessagesv2messagesindexinfo
      x-api-path-slug: mymessagesv2messagesindexinfo-get
      responses:
        200:
          description: OK
      tags:
      - MyMessages
      - VMessages
      - Index
      - Info