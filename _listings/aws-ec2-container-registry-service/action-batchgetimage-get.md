---
swagger: "2.0"
info:
  title: AWS EC2 Container Registry API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BatchGetImage:
    get:
      summary: ' Batch Get Image '
      description: Gets detailed information for specified images within a specified
        repository
      operationId: batchGetImage
      parameters:
      - in: query
        name: acceptedMediaTypes
        description: The accepted media types for the request
        type: string
      - in: query
        name: imageIds
        description: A list of image ID references that correspond to images to describe
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the images to describe
        type: string
      - in: query
        name: repositoryName
        description: The repository that contains the images to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - image
definitions: []
x-collection-name: AWS EC2 Container Registry Service
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