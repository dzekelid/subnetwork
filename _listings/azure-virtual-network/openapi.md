---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 1
info:
  title: NetworkManagementClient
  description: the-microsoft-azure-network-management-api-provides-a-restful-set-of-web-services-that-interact-with-microsoft-azure-networks-service-to-manage-your-network-resources--the-api-has-entities-that-capture-the-relationship-between-an-end-user-and-the-microsoft-azure-networks-service-
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
---