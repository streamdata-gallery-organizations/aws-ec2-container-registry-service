---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 0
info:
  title: AWS EC2 Container Registry API Batch Get Image
  version: 1.0.0
  description: Gets detailed information for specified images within a specified repository.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BatchCheckLayerAvailability:
    get:
      summary: Batch Check Layer Availability
      description: Check the availability of multiple image layers in a specified
        registry and repository.
      operationId: batchCheckLayerAvailability
      x-api-path-slug: actionbatchchecklayeravailability-get
      parameters:
      - in: query
        name: layerDigests
        description: The digests of the image layers to check
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the image layers to check
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository that is associated with the image
          layers to check
        type: string
      responses:
        200:
          description: OK
      tags:
      - Layer Availability
  /?Action=BatchDeleteImage:
    get:
      summary: Batch Delete Image
      description: Deletes a list of specified images within a specified repository.
      operationId: batchDeleteImage
      x-api-path-slug: actionbatchdeleteimage-get
      parameters:
      - in: query
        name: imageIds
        description: A list of image ID references that correspond to images to delete
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the image to delete
        type: string
      - in: query
        name: repositoryName
        description: The repository that contains the image to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Image
  /?Action=BatchGetImage:
    get:
      summary: Batch Get Image
      description: Gets detailed information for specified images within a specified
        repository.
      operationId: batchGetImage
      x-api-path-slug: actionbatchgetimage-get
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
      - Image
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