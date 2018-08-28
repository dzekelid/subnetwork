---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Describe Cache Subnet Groups
  version: 1.0.0
  description: |-
    Returns a list of cache subnet group
                descriptions.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCacheSubnetGroup:
    get:
      summary: Create Cache Subnet Group
      description: Creates a new cache subnet group.
      operationId: createCacheSubnetGroup
      x-api-path-slug: actioncreatecachesubnetgroup-get
      parameters:
      - in: query
        name: CacheSubnetGroupDescription
        description: A description for the cache subnet group
        type: string
      - in: query
        name: CacheSubnetGroupName
        description: A name for the cache subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: A list of VPC subnet IDs for the cache subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
  /?Action=DeleteCacheSubnetGroup:
    get:
      summary: Delete Cache Subnet Group
      description: Deletes a cache subnet group.
      operationId: deleteCacheSubnetGroup
      x-api-path-slug: actiondeletecachesubnetgroup-get
      parameters:
      - in: query
        name: CacheSubnetGroupName
        description: The name of the cache subnet group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
  /?Action=DescribeCacheSubnetGroups:
    get:
      summary: Describe Cache Subnet Groups
      description: |-
        Returns a list of cache subnet group
                    descriptions.
      operationId: describeCacheSubnetGroups
      x-api-path-slug: actiondescribecachesubnetgroups-get
      parameters:
      - in: query
        name: CacheSubnetGroupName
        description: The name of the cache subnet group to return details for
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
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