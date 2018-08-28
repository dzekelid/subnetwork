swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 1
info:
  title: AWS ElastiCache API
  version: 1.0.0
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
  /?Action=ModifyCacheSubnetGroup:
    get:
      summary: Modify Cache Subnet Group
      description: Modifies an existing cache subnet group.
      operationId: modifyCacheSubnetGroup
      x-api-path-slug: actionmodifycachesubnetgroup-get
      parameters:
      - in: query
        name: CacheSubnetGroupDescription
        description: A description of the cache subnet group
        type: string
      - in: query
        name: CacheSubnetGroupName
        description: The name for the cache subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: The EC2 subnet IDs for the cache subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups