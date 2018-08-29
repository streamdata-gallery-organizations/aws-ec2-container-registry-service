---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 0
info:
  title: AWS EC2 Container Registry API Describe Repositories
  version: 1.0.0
  description: Describes image repositories in a registry.
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
  /?Action=CompleteLayerUpload:
    get:
      summary: Complete Layer Upload
      description: Inform Amazon ECR that the image layer upload for a specified registry,
        repository name, and upload ID, has completed.
      operationId: completeLayerUpload
      x-api-path-slug: actioncompletelayerupload-get
      responses:
        200:
          description: OK
      tags:
      - Layer Upload
  /?Action=CreateRepository:
    get:
      summary: Create Repository
      description: Creates an image repository.
      operationId: createRepository
      x-api-path-slug: actioncreaterepository-get
      parameters:
      - in: query
        name: repositoryName
        description: The name to use for the repository
        type: string
      responses:
        200:
          description: OK
      tags:
      - Repositories
  /?Action=DeleteRepository:
    get:
      summary: Delete Repository
      description: Deletes an existing image repository.
      operationId: deleteRepository
      x-api-path-slug: actiondeleterepository-get
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
      - Repositories
  /?Action=DeleteRepositoryPolicy:
    get:
      summary: Delete Repository Policy
      description: Deletes the repository policy from a specified repository.
      operationId: deleteRepositoryPolicy
      x-api-path-slug: actiondeleterepositorypolicy-get
      parameters:
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repository policy to delete
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository that is associated with the repository
          policy to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Repository Policies
  /?Action=DescribeImages:
    get:
      summary: Describe Images
      description: |-
        Returns metadata about the images in a repository, including image size, image
                    tags, and creation date.
      operationId: describeImages
      x-api-path-slug: actiondescribeimages-get
      parameters:
      - in: query
        name: filter
        description: The filter key and value with which to filter your DescribeImages            results
        type: string
      - in: query
        name: imageIds
        description: The list of image IDs for the requested repository
        type: string
      - in: query
        name: maxResults
        description: The maximum number of repository results returned by DescribeImages
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated            DescribeImages
          request where maxResults was used and            the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repository in            which to describe images
        type: string
      - in: query
        name: repositoryName
        description: A list of repositories to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Images
  /?Action=DescribeRepositories:
    get:
      summary: Describe Repositories
      description: Describes image repositories in a registry.
      operationId: describeRepositories
      x-api-path-slug: actiondescriberepositories-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of repository results returned by DescribeRepositories
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                DescribeRepositories
          request where maxResults was used and            the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repositories to be described
        type: string
      - in: query
        name: repositoryNames
        description: A list of repositories to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Repositories
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