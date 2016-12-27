# Azure Sql Server and Database

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fpascalnaber%2FEnterpriseARMTemplates%2Fmaster%2FResourcesWithNamingConvention%2FMicrosoft.Sql%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fpascalnaber%2FEnterpriseARMTemplates%2Fmaster%2FResourcesWithNamingConvention%2FMicrosoft.Sql%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>


This template deploys an Azure Sql Server and Azure SQL database. The template decides the namingconvention. The convention uses the metadata which is passed as a parameter to the template. See the parameter file for an example. The metadata is also used to add tags to the resources.  

`Tags: SQL, SQL Azure, Server, Database, SQL Azure Database, SQL Azure Server`

## remarks

- When using this template when creating a HDInsight metadata store make sure the name of the database does not contain dashes (-)
 
## design decisions
- One template for both the Server and Database, not two separate templates. Because the database is dependent on the Server. Azure only supports one resourcegroup for both the Server and Database(s). When you need to deploy multiple databases, just call this ARM template multiple times with the same parameters for the Server. You pay only per database, not for a server. 

## supports

Besides the standard configuration

- [Transparent Data encryption](https://msdn.microsoft.com/en-us/library/dn948096(v=sql.120).aspx)

## not supported yet

- [Auditing & Thread detection](https://docs.microsoft.com/nl-nl/azure/sql-database/sql-database-threat-detection-get-started)
- [Geo Replication](https://docs.microsoft.com/nl-nl/azure/sql-database/sql-database-geo-replication-overview)
- [Elastic Sql database](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-elastic-pool)
