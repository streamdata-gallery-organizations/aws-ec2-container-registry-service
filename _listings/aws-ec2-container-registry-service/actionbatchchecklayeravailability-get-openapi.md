---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 0
info:
  title: AWS EC2 Container Registry API Batch Check Layer Availability
  version: 1.0.0
  description: Check the availability of multiple image layers in a specified registry
    and repository.
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