---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Create Subnet
  version: 1.0.0
  description: Creates a subnet in an existing VPC.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateSpotDatafeedSubscription:
    get:
      summary: Create Spot Datafeed Subscription
      description: Creates a data feed for Spot instances, enabling you to view Spot
        instance usage logs.
      operationId: createspotdatafeedsubscription
      x-api-path-slug: actioncreatespotdatafeedsubscription-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet
  /?Action=CreateSubnet:
    get:
      summary: Create Subnet
      description: Creates a subnet in an existing VPC.
      operationId: createsubnet
      x-api-path-slug: actioncreatesubnet-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: SubnetId
        description: The ID of the subnet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet
  /?Action=DeleteSubnet:
    get:
      summary: Delete Subnet
      description: Deletes the specified subnet.
      operationId: deletesubnet
      x-api-path-slug: actiondeletesubnet-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: SubnetId.N
        description: One or more subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet
  /?Action=ModifySubnetAttribute:
    get:
      summary: Modify Subnet Attribute
      description: Modifies a subnet attribute.
      operationId: modifysubnetattribute
      x-api-path-slug: actionmodifysubnetattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: ResourceId.N
        description: The IDs of one or more resources to tag
        type: string
      - in: query
        name: Tag.N
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet
  /?Action=DescribeSubnets:
    get:
      summary: Describe Subnets
      description: Describes one or more of your subnets.
      operationId: describesubnets
      x-api-path-slug: actiondescribesubnets-get
      parameters:
      - in: query
        name: AssociationId
        description: The association ID for the CIDR block
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnets
  /?Action=AssociateSubnetCidrBlock:
    get:
      summary: Associate Subnet Cidr Block
      description: Associates a CIDR block with your subnet.
      operationId: associatesubnetcidrblock
      x-api-path-slug: actionassociatesubnetcidrblock-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone for the subnet
        type: string
      - in: query
        name: CidrBlock
        description: The IPv4 network range for the subnet, in CIDR notation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Ipv6CidrBlock
        description: The IPv6 network range for the subnet, in CIDR notation
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - CIDR Block
  /?Action=DisassociateSubnetCidrBlock:
    get:
      summary: Disassociate Subnet Cidr Block
      description: Disassociates a CIDR block from a subnet.
      operationId: disassociatesubnetcidrblock
      x-api-path-slug: actiondisassociatesubnetcidrblock-get
      parameters:
      - in: query
        name: AssignIpv6AddressOnCreation
        description: Specify true to indicate that network interfaces created in the            specified
          subnet should be assigned an IPv6 address
        type: string
      - in: query
        name: MapPublicIpOnLaunch
        description: Specify true to indicate that network interfaces created in the            specified
          subnet should be assigned a public IPv4 address
        type: string
      - in: query
        name: SubnetId
        description: The ID of the subnet
        type: string
      responses:
        200:
          description: OK
      tags:
      - CIDR Block
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