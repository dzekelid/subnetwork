---
swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 0
info:
  title: Google Compute Engine API Delete Subnetwork
  description: Deletes the specified subnetwork.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/aggregated/subnetworks:
    get:
      summary: Get Subnetworks
      description: Retrieves an aggregated list of subnetworks.
      operationId: compute.subnetworks.aggregatedList
      x-api-path-slug: projectaggregatedsubnetworks-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Subnetwork
      - Aggregation
  /{project}/regions/{region}/subnetworks:
    get:
      summary: Get Subnetworks
      description: Retrieves a list of subnetworks available to the specified project.
      operationId: compute.subnetworks.list
      x-api-path-slug: projectregionsregionsubnetworks-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Subnetwork
    post:
      summary: Create Subnetwork
      description: Creates a subnetwork in the specified project using the data included
        in the request.
      operationId: compute.subnetworks.insert
      x-api-path-slug: projectregionsregionsubnetworks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Subnetwork
  /{project}/regions/{region}/subnetworks/{subnetwork}:
    delete:
      summary: Delete Subnetwork
      description: Deletes the specified subnetwork.
      operationId: compute.subnetworks.delete
      x-api-path-slug: projectregionsregionsubnetworkssubnetwork-delete
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      - in: path
        name: subnetwork
        description: Name of the Subnetwork resource to delete
      responses:
        200:
          description: OK
      tags:
      - Subnetwork
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