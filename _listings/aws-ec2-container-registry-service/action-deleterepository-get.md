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
  /?Action=DeleteRepository&k=1:
    get:
      summary: ' Delete Repository '
      description: Deletes an existing image repository
      operationId: deleteRepository
      parameters:
      - in: query
        name: force
        description: Force the deletion of the repository if it contains images
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repository to delete
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - repositories
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