# **Tatweerak Guide Task (Web Api Project)**

In this task, you will develop a set of REST APIs capable of reading a JSON data deployed
on a server and returning information by using a collection of simple HTTP requests using postman.

# **Nuget Package Requirement:**

You need to install a storeak nuget package (Storeak.Api.Core) using link https://storeak-nuget-service.azurewebsites.net/nuget on your web api project where you can access important libraries thats need for project like 
* Generic repository pattern,
* Custom required attributes,
* Trackable dto,
* Paging methods,
* Filters,
* Logging methods
* Api Custom response methods.

This package will help us to avoid repeated code thats need in every api project and make projects fast development.

# **Database Configuration:**

You need to create environment variable for making connection string. Storeak Core nuget package get these variables and make connection string for your project.

* AzurePool_DataSource: Database Server Name
 
* AzurePool_UserID :  Database Server User Id
 
* AzurePool_Password:  Database Server Password
 
* ENVIRONMENT : LocalHost
 
* Enco: set to empty

# **Project Folder Structure (Demo project):**
> 


***In wwwroot/App_Data folder you need to create xml file that handle multilanguage messages.***

> 

***In Application/BusinessUseCases you need to create (Create,Update,Delete) Operations***

> 

***In Application/Queries you need to create select operations.***


> 

***In Application/UnitOfWork you need to add repositories.***
> 
> 
***In Controller you need to create all apis crud.***



***In Infrastructure/DataModels path you need to create database entities(DTO).***
> 

***In Infrastructure/Mapping you need to create configuration of entities.***


***In Infrastructure/DemoContext you need to add dbset with entity configuration (mapping) also inherit with core store db context class to inherit all db methods for database interaction.***


***In Infrastructure/ResponseMessages you need to add messages variables that return message based on language (Multilanguage handling).***


***In Models you need to create Api Request and Response models.***

***In MapperProfile you need to add mapping of entities using automapper.***


***In Startup you need to inherit core startup class and configure your project setting(dependencies resolver,mappers,database etc)***


