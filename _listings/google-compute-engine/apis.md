---
name: Google Compute Engine
x-slug: google-compute-engine
description: Google Compute Engine delivers virtual machines running in Googles innovative
  data centers and worldwide fiber network. Compute Engines tooling and workflow support
  enable scaling from single instances to global, load-balanced cloud computing.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Subnetwork
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subnetwork/master/_listings/google-compute-engine/apis.md
specificationVersion: "0.14"
apis:
- name: Compute Engine - Get Subnetworks
  x-api-slug: projectaggregatedsubnetworks-get
  description: Retrieves an aggregated list of subnetworks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subnetwork/master/_listings/google-compute-engine/projectaggregatedsubnetworks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subnetwork/master/_listings/google-compute-engine/projectaggregatedsubnetworks-get-openapi.md
- name: Compute Engine - Get Subnetworks
  x-api-slug: projectregionsregionsubnetworks-get
  description: Retrieves a list of subnetworks available to the specified project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subnetwork/master/_listings/google-compute-engine/projectregionsregionsubnetworks-get-openapi.md
- name: Compute Engine - Create Subnetwork
  x-api-slug: projectregionsregionsubnetworks-post
  description: Creates a subnetwork in the specified project using the data included
    in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subnetwork/master/_listings/google-compute-engine/projectregionsregionsubnetworks-post-openapi.md
- name: Compute Engine - Delete Subnetwork
  x-api-slug: projectregionsregionsubnetworkssubnetwork-delete
  description: Deletes the specified subnetwork.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subnetwork/master/_listings/google-compute-engine/projectregionsregionsubnetworkssubnetwork-delete-openapi.md
- name: Compute Engine - Get Subnetwork
  x-api-slug: projectregionsregionsubnetworkssubnetwork-get
  description: Returns the specified subnetwork. Get a list of available subnetworks
    list() request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subnetwork/master/_listings/google-compute-engine/projectregionsregionsubnetworkssubnetwork-get-openapi.md
- name: Compute Engine - Update Subnetwork
  x-api-slug: projectregionsregionsubnetworkssubnetworkexpandipcidrrange-post
  description: Expands the IP CIDR range of the subnetwork to a specified value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subnetwork/master/_listings/google-compute-engine/projectregionsregionsubnetworkssubnetworkexpandipcidrrange-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.vision.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.compute.engine.stack.network
- type: x-code
  url: https://cloud.google.com/compute/docs/api/libraries
- type: x-documentation
  url: https://cloud.google.com/compute/docs/reference/latest/
- type: x-guides
  url: https://cloud.google.com/compute/docs/api/how-tos/how-tos
- type: x-rate-limits
  url: https://cloud.google.com/compute/docs/api-rate-limits
- type: x-sla
  url: https://cloud.google.com/compute/sla
- type: x-website
  url: https://cloud.google.com/compute/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---