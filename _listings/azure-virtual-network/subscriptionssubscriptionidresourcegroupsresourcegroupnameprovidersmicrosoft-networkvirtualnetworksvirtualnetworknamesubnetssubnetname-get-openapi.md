---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 0
info:
  title: Azure Virtual Network API Subnets Get
  description: Gets the specified subnet by virtual network and resource group.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}
  : delete:
      summary: Subnets Delete
      description: Deletes the specified subnet.
      operationId: Subnets_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkvirtualnetworksvirtualnetworknamesubnetssubnetname-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: subnetName
        description: The name of the subnet
      - in: path
        name: virtualNetworkName
        description: The name of the virtual network
      responses:
        200:
          description: OK
      tags:
      - Subnets
    get:
      summary: Subnets Get
      description: Gets the specified subnet by virtual network and resource group.
      operationId: Subnets_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkvirtualnetworksvirtualnetworknamesubnetssubnetname-get
      parameters:
      - in: query
        name: $expand
        description: Expands referenced resources
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: subnetName
        description: The name of the subnet
      - in: path
        name: virtualNetworkName
        description: The name of the virtual network
      responses:
        200:
          description: OK
      tags:
      - Subnets
    put:
      summary: Subnets Create Or Update
      description: Creates or updates a subnet in the specified virtual network.
      operationId: Subnets_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkvirtualnetworksvirtualnetworknamesubnetssubnetname-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: subnetName
        description: The name of the subnet
      - in: body
        name: subnetParameters
        description: Parameters supplied to the create or update subnet operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: virtualNetworkName
        description: The name of the virtual network
      responses:
        200:
          description: OK
      tags:
      - Subnets
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}/subnets
  : get:
      summary: Subnets List
      description: Gets all subnets in a virtual network.
      operationId: Subnets_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networkvirtualnetworksvirtualnetworknamesubnets-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: virtualNetworkName
        description: The name of the virtual network
      responses:
        200:
          description: OK
      tags:
      - Subnets
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