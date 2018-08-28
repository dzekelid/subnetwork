---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Delete Cluster Subnet Group
  version: 1.0.0
  description: Deletes the specified cluster subnet group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateClusterSubnetGroup:
    get:
      summary: Create Cluster Subnet Group
      description: Creates a new Amazon Redshift subnet group.
      operationId: createClusterSubnetGroup
      x-api-path-slug: actioncreateclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name for the subnet group
        type: string
      - in: query
        name: Description
        description: A description for the subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: An array of VPC subnet IDs
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=DeleteClusterSubnetGroup:
    get:
      summary: Delete Cluster Subnet Group
      description: Deletes the specified cluster subnet group.
      operationId: deleteClusterSubnetGroup
      x-api-path-slug: actiondeleteclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group name to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
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