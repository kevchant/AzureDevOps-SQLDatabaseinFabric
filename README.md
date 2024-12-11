# AzureDevOps-SQLDatabaseinFabric to perform CI/CD for SQL database in Fabric

Contains a template that you can use to perform CI/CD for SQL database in Fabric in two different ways. Based on a blog post I wrote called '[Two ways to perform CI/CD for SQL databases in Fabric using YAML Pipelines](https://www.kevinrchant.com/?p=12321)'.

A brief is below. However, there is also a [wiki for this project](https://github.com/kevchant/AzDo-SQLDatabaseinFabric/wiki) that covers multiple topics.

Both methods use a YAML pipeline, which you can find in the AzureDevOpsTemplates folder.

In order to use them in Azure Pipelines you can either import or fork this repository into another GitHub repository or into Azure Repos.

Afterwards, you can select the YAML file in Azure Pipelines and tailor the pipeline to suit your needs.

## Method one
First method is by creating a dacpac file based on a [SQL database project](https://learn.microsoft.com/en-us/sql/tools/sql-database-projects/sql-database-projects?view=sql-server-ver16&WT.mc_id=DP-MVP-5004032%3Fview%3Dsql-server-ver16) to a SQL database in Fabric. 

Which is the database project you see in this repository. 

You can find the template for the YAML pipeline in the '[AzureDevOpsTemplates/SQLDBinFabricDatabaseProject.yml](https://github.com/kevchant/AzDo-SQLDatabaseinFabric/blob/main/AzureDevOpsTemplates/SQLDBinFabricDatabaseProject.yml)'.

## Method two
Second method is by extracting the schema of an existing SQL database in Fabric into a dacpac file. Which you then deploy to another SQL database in Fabric. 

You can find the template for the YAML pipeline in the '[AzureDevOpsTemplates/SQLDBinFabricExtractSchematoDacpac.yml](https://github.com/kevchant/AzDo-SQLDatabaseinFabric/blob/main/AzureDevOpsTemplates/SQLDBinFabricExtractSchematoDacpac.yml)'.

This repository is provided "as is" based on the [MIT license](https://opensource.org/licenses/MIT). Basically, I am not responsible for your use of it.
