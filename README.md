# ![LOGO](logo.png) Azure SQL Database replication links **flow**ground Connector

## Description

A generated **flow**ground connector for the Azure SQL Database replication links API (version 2014-04-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/sql-replicationLinks/2014-04-01/swagger.json<br/>
Generated at: 2019-05-07T17:39:10+03:00

## API Description

Provides read, delete, and failover functionality for Azure SQL Database replication links.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists a database's replication links.

*Tags:* `DatabaseReplicationLinks`

#### Input Parameters
* `api-version` - _required_ - The API version to use for the request.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `serverName` - _required_ - The name of the server.
* `databaseName` - _required_ - The name of the database to retrieve links for.

### Deletes a database replication link. Cannot be done during failover.

*Tags:* `DatabaseReplicationLinks`

#### Input Parameters
* `api-version` - _required_ - The API version to use for the request.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `serverName` - _required_ - The name of the server.
* `databaseName` - _required_ - The name of the database that has the replication link to be dropped.
* `linkId` - _required_ - The ID of the replication link to be deleted.

### Gets a database replication link.

*Tags:* `DatabaseReplicationLinks`

#### Input Parameters
* `api-version` - _required_ - The API version to use for the request.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `serverName` - _required_ - The name of the server.
* `databaseName` - _required_ - The name of the database to get the link for.
* `linkId` - _required_ - The replication link ID to be retrieved.

### Sets which replica database is primary by failing over from the current primary replica database.

*Tags:* `DatabaseReplicationLinks`

#### Input Parameters
* `api-version` - _required_ - The API version to use for the request.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `serverName` - _required_ - The name of the server.
* `databaseName` - _required_ - The name of the database that has the replication link to be failed over.
* `linkId` - _required_ - The ID of the replication link to be failed over.

### Sets which replica database is primary by failing over from the current primary replica database. This operation might result in data loss.

*Tags:* `DatabaseReplicationLinks`

#### Input Parameters
* `api-version` - _required_ - The API version to use for the request.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `serverName` - _required_ - The name of the server.
* `databaseName` - _required_ - The name of the database that has the replication link to be failed over.
* `linkId` - _required_ - The ID of the replication link to be failed over.

## License

**flow**ground :- Telekom iPaaS / azure-com-sql-replication-links-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
