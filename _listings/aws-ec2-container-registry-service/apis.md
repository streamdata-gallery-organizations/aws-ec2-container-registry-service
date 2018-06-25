---
name: AWS EC2 Container Registry Service
x-slug: aws-ec2-container-registry-service
description: Amazon EC2 Container Registry (ECR) is a fully-managedDockercontainer
  registry that makes it easy for developers to store, manage, and deploy Docker container
  images. Amazon ECR is integrated withAmazon EC2 Container Service (ECS), simplifying
  your development to production workflow. Amazon ECR eliminates the need to operate
  your own container repositories or worry about scaling the underlying infrastructure.
  Amazon ECR hosts your images in a highly available and scalable architecture, allowing
  you to reliably deploy containers for your applications. Integration with AWS Identity
  and Access Management (IAM) provides resource-level control of each repository.
  With Amazon ECR, there are no upfront fees or commitments. You pay only for the
  amount of data you store in your repositories and data transferred to the Internet.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
x-kinRank: "10"
x-alexaRank: "0"
tags: AWS EC2 Container Registry Service
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS EC2 Container Registry API Batch Check Layer Availability
  x-api-slug: aws-ec2-container-registry-api
  description: Check the availability of multiple image layers in a specified registry
    and repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=BatchCheckLayerAvailability
  tags: Layer Availability
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionbatchchecklayeravailability-get-openapi.md
- name: AWS EC2 Container Registry API Batch Delete Image
  x-api-slug: aws-ec2-container-registry-api
  description: Deletes a list of specified images within a specified repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=BatchDeleteImage
  tags: Image
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionbatchdeleteimage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionbatchdeleteimage-get-openapi.md
- name: AWS EC2 Container Registry API Batch Get Image
  x-api-slug: aws-ec2-container-registry-api
  description: Gets detailed information for specified images within a specified repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=BatchGetImage
  tags: Image
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionbatchgetimage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionbatchgetimage-get-openapi.md
- name: AWS EC2 Container Registry API Complete Layer Upload
  x-api-slug: aws-ec2-container-registry-api
  description: Inform Amazon ECR that the image layer upload for a specified registry,
    repository name, and upload ID, has completed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=CompleteLayerUpload
  tags: Layer Upload
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actioncompletelayerupload-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actioncompletelayerupload-get-openapi.md
- name: AWS EC2 Container Registry API Create Repository
  x-api-slug: aws-ec2-container-registry-api
  description: Creates an image repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=CreateRepository
  tags: Repositories
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actioncreaterepository-get-openapi.md
- name: AWS EC2 Container Registry API Delete Repository
  x-api-slug: aws-ec2-container-registry-api
  description: Deletes an existing image repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=DeleteRepository
  tags: Repositories
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actiondeleterepository-get-openapi.md
- name: AWS EC2 Container Registry API Delete Repository Policy
  x-api-slug: aws-ec2-container-registry-api
  description: Deletes the repository policy from a specified repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=DeleteRepositoryPolicy
  tags: Repository Policies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actiondeleterepositorypolicy-get-openapi.md
- name: AWS EC2 Container Registry API Describe Images
  x-api-slug: aws-ec2-container-registry-api
  description: |-
    Returns metadata about the images in a repository, including image size, image
                tags, and creation date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=DescribeImages
  tags: Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actiondescribeimages-get-openapi.md
- name: AWS EC2 Container Registry API Describe Repositories
  x-api-slug: aws-ec2-container-registry-api
  description: Describes image repositories in a registry.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=DescribeRepositories
  tags: Repositories
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actiondescriberepositories-get-openapi.md
- name: AWS EC2 Container Registry API Get Authorization Token
  x-api-slug: aws-ec2-container-registry-api
  description: Retrieves a token that is valid for a specified registry for 12 hours.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=GetAuthorizationToken
  tags: Authorization Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actiongetauthorizationtoken-get-openapi.md
- name: AWS EC2 Container Registry API Get Download Url For Layer
  x-api-slug: aws-ec2-container-registry-api
  description: .Retrieves the pre-signed Amazon S3 download URL corresponding to an
    image layer. You can only get URLs for image layers that are referenced in an
    image.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=GetDownloadUrlForLayer
  tags: Layers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actiongetdownloadurlforlayer-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actiongetdownloadurlforlayer-get-openapi.md
- name: AWS EC2 Container Registry API Get Repository Policy
  x-api-slug: aws-ec2-container-registry-api
  description: Retrieves the repository policy for a specified repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=GetRepositoryPolicy
  tags: Repository Policies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actiongetrepositorypolicy-get-openapi.md
- name: AWS EC2 Container Registry API Initiate Layer Upload
  x-api-slug: aws-ec2-container-registry-api
  description: Notify Amazon ECR that you intend to upload an image layer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=InitiateLayerUpload
  tags: Layer Upload
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actioninitiatelayerupload-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actioninitiatelayerupload-get-openapi.md
- name: AWS EC2 Container Registry API List Images
  x-api-slug: aws-ec2-container-registry-api
  description: Lists all the image IDs for a given repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=ListImages
  tags: Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionlistimages-get-openapi.md
- name: AWS EC2 Container Registry API Put Image
  x-api-slug: aws-ec2-container-registry-api
  description: Creates or updates the image manifest and tags associated with an image.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=PutImage
  tags: Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionputimage-get-openapi.md
- name: AWS EC2 Container Registry API Set Repository Policy
  x-api-slug: aws-ec2-container-registry-api
  description: Applies a repository policy on a specified repository to control access
    permissions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=SetRepositoryPolicy
  tags: Repository Policies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionsetrepositorypolicy-get-openapi.md
- name: AWS EC2 Container Registry API Upload Layer Part
  x-api-slug: aws-ec2-container-registry-api
  description: Uploads an image layer part to Amazon ECR.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: ://///?Action=UploadLayerPart
  tags: Layer Parts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionuploadlayerpart-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/actionuploadlayerpart-get-openapi.md
- name: AWS EC2 Container Registry API
  x-api-slug: aws-ec2-container-registry-api
  description: Amazon EC2 Container Registry (ECR) is a fully-managedDockercontainer
    registry that makes it easy for developers to store, manage, and deploy Docker
    container images. Amazon ECR is integrated withAmazon EC2 Container Service (ECS),
    simplifying your development to production workflow. Amazon ECR eliminates the
    need to operate your own container repositories or worry about scaling the underlying
    infrastructure. Amazon ECR hosts your images in a highly available and scalable
    architecture, allowing you to reliably deploy containers for your applications.
    Integration with AWS Identity and Access Management (IAM) provides resource-level
    control of each repository. With Amazon ECR, there are no upfront fees or commitments.
    You pay only for the amount of data you store in your repositories and data transferred
    to the Internet.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonECR.png
  humanURL: https://aws.amazon.com/ecr/
  baseURL: :///
  tags: AWS EC2 Container Registry Service
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-ec2-container-registry-service/master/_listings/aws-ec2-container-registry-service/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonECR/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/ecr/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/ecr/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/ecr/pricing/
- type: x-website
  url: https://aws.amazon.com/ecr/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---