---
swagger: "2.0"
x-collection-name: AWS Rekognition
x-complete: 1
info:
  title: AWS Rekognition API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=IndexFaces:
    get:
      summary: Index Faces
      description: Detects faces in the input image and adds them to the specified
        collection.
      operationId: indexFaces
      x-api-path-slug: actionindexfaces-get
      parameters:
      - in: query
        name: CollectionId
        description: ID of an existing collection to which you want to add the faces
          that are detected in the      input images
        type: string
      - in: query
        name: DetectionAttributes
        description: (Optional) Returns detailed attributes of indexed faces
        type: string
      - in: query
        name: ExternalImageId
        description: ID you want to assign to all the faces detected in the image
        type: string
      - in: query
        name: Image
        description: Provides the source image either as bytes or an S3 object
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces
---