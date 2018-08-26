---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 0
info:
  title: AWS Database Migration Service API Delete Replication Subnet Group
  version: 1.0.0
  description: Deletes a subnet group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateReplicationSubnetGroup:
    get:
      summary: Create Replication Subnet Group
      description: Creates a replication subnet group given a list of the subnet IDs
        in a VPC.
      operationId: createReplicationSubnetGroup
      x-api-path-slug: actioncreatereplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupDescription
        description: The description for the subnet group
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The name for the replication subnet group
        type: string
      - in: query
        name: SubnetIds
        description: The EC2 subnet IDs for the subnet group
        type: string
      - in: query
        name: Tags
        description: The tag to be assigned to the subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Group
  /?Action=DeleteReplicationSubnetGroup:
    get:
      summary: Delete Replication Subnet Group
      description: Deletes a subnet group.
      operationId: deleteReplicationSubnetGroup
      x-api-path-slug: actiondeletereplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The subnet group name of the replication instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Group
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