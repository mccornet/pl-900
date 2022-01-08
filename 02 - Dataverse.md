# PL-900 Dataverse

***Dataverse is a cloud-based, (not designed for stand-alone use) low-code data service and app platform. Available globally but deployed geographically to comply with your potential data residency. It is designed to be your central data repository for business data.*** 

Which allows you to leverage the security and connectivity of Microsoft services. Dataverse connects easily to all aspects of Microsoft Power Platform so that you can fully control, automate, and strengthen your business. It powers many Microsoft Dynamics 365 solutions such as Field Service, Marketing, Customer Service, and Sales. It is also available as part of Power Apps and Power Automate with native connectivity built right in. The AI Builder and Portals features of Microsoft Power Platform also utilize Dataverse.

<p align="center">
	<img src="https://docs.microsoft.com/en-us/learn/modules/introduction-common-data-service/media/common-data-service-diagram.png" alt="Dataverse API options" width="750px" />
<p>

**Security**: - ***handle authentication with Azure Active Directory*** (Azure AD) to allow for conditional access and multi-factor authentication. It supports authorization down to the row and column level and provides rich auditing capabilities.

**Logic**: - ***apply business logic at the data level***. Regardless of how a user is interacting with the data, the same rules apply. These rules could be related to duplicate detection, business rules, workflows, or more.

**Data**: - ***control the shape of your data***, allowing you to discover, model, validate, and report on your data. 

**Storage**: - ***stores data in the Azure cloud***. 

**Integration**: - ***APIs, webhooks, eventing, and data exports offer flexibility to get data in and out***.

## Dataverse Defined

***A Dataverse database is a single instance of Microsoft Dataverse*** ***which stores data in a set of standard and custom data structures called tables.*** A table is a logical set of rows that is used to store data. Rows within a table contain many columns to manage individual pieces of information about a single row. You can create one or many database instances in Microsoft Dataverse to host data behind your business solutions. Each instance of a Microsoft Dataverse will start with the same set of tables to store data, but you can always extend and customize a Microsoft Dataverse database to meet specific business needs. This means that you can share business solutions that reference standard tables in Microsoft Dataverse across your organization or with any other organization by using it anywhere in the world.

### Scalability

***A Dataverse database supports large data sets and complex data models***. ***The amount of data that is available in your instance of Microsoft Dataverse is based upon the number and type of licenses that are associated with it.*** Tables can hold millions of items, and you can extend the storage in each instance of a Microsoft Dataverse database to four (4) terabytes per instance. Data storage is pooled between all licensed users, so you can allocate storage as needed for each solution that you build. Additional storage can be purchased if you need more storage than what is offered within standard licensing.

### Common Data Model

***The standard table design uses the  open data model standard called Common Data Model***. ***Common Data Model is a logical design that includes a set of open-sourced, standardized, extensible data tables and relationships*** that Microsoft and its partners have published in an industry-wide initiative called the Open Data Initiative. 

### Structure and Benefits

***The structure is based upon the definitions and schema in the Common Data Model. The key benefit is simplified integration into any other solution that use a Common Data Model schema***, because the standard tables of the solution are the same. You will also be able to take advantage of a rich ecosystem of solutions that vendors have built from using Common Data Model. 

### Tables & Columns

***A table is a logical structure containing rows and columns that represents a set of data.***

#### Types of Tables

- **Standard** - ***base set of tables that are created for every instance of a Microsoft Dataverse database***. You can add more columns to any table, but you can only delete columns from a custom table.
- **Complex** - ***Tables that contain complex, server-side business logic***, including real-time workflows or plug-ins. Some of the tables that are used in Dynamics 365 applications are complex. Care must be taken *if you add server-side logic to ensure that users have the proper license to use the complex table*. 

#### Columns

***Columns are a way to store a discrete piece of information within a row in a table***. Columns have data types. Every database in Microsoft Dataverse starts with a standard set of tables and each standard table has a standard set of columns.

### Relationships

***To make an efficient and scalable solution for most of the solutions it is needed to split up data into different containers (tables). The two most common relationships between tables are one-to-many and many-to-many***, both of which are supported by Microsoft Dataverse.

Knowing how to split up the data into tables can be difficult. Microsoft Dataverse already contains many of the tables that most organizations will need. Using standard tables and extending them will ensure that you are building solutions around a proven, scalable way of storing the data that is used by your solutions.

One-to-many relationships are also known as parent-child relationships. A column that only allows unique values, such as invoice number, is used to identify the parent row. This unique column is called a key. The same value (the parent key) is stored in the related child rows. This column is called a foreign key when the child row is used to store the parent key value.

## Environments

***Environments are used to store, manage, and share your organization's business data, apps, and flows***.***Each environment allows you to provision one Microsoft Dataverse database*** for use within that environment. Microsoft Dataverse environments allow you to manage user access, security settings, and the storage that is associated with that database.

***Each environment is created under a Microsoft Azure Active Directory (Azure AD) tenant, and its resources can only be accessed by users within that tenant.*** ***An environment is bound to a geographic location***. 

***A Microsoft Dataverse database is created within datacenters in that geographic location. Any items that you create in that environment (including connections, gateways, flows that are using Power Automate, and more) are also bound to their environment's location.*** 

<p align="center">
	<img src="https://docs.microsoft.com/en-us/learn/modules/introduction-common-data-service/media/environment.png" alt="Contoso tenant to environment map" width="750px" />
<p>
***You can create more than one environment to manage solution development and data storage*** by setting up one environment for development, another for testing, and another for production use. Also, you can set up an environment based on a geographical location. For example, you might set up an environment for Europe and another for Asia. 

## Business Rules

***In Dataverse you can define business rules that allow you to apply and maintain business logic at the data layer instead of the app layer.*** For example, business rules can be used in canvas and model-driven apps to set or clear values in one or many columns in a table. Or to validate stored data or show error messages. Model-driven apps can use business rules to show or hide columns, enable or disable columns, and create recommendations based on business intelligence.

> **Tip**
>
> Business rules are usually defined for a table and apply to all forms, but you can define a business rule for a specific model-driven form. Canvas apps cannot have a business rule applied to a specific form, but they are still enforced when interacting with the data.

***Business rules give you*** ***a powerful way to enforce rules, set values, or validate data*** regardless of the form that is used to input data. Additionally, business rules are effective in helping to increase the accuracy of data, simplify application development, and streamline the forms presented to end users.

***By applying business rules at the data level instead of the app level, you have better control of your data.*** This can ensure your business logic is followed whether it is being accessed directly from Power Apps, Power Automate, or even via an API. The rule is tied to the data, not the app.

### Rules Available Per App:

***Canvas and model-driven***:

- Set column values
- Clear column values
- Validate data and show error messages

***Model-driven apps:***

- Show or hide columns (model-driven apps only)
- Enable or disable columns (model-driven apps only)
- Create business recommendations based on business intelligence (model-driven apps only)

## Administer

***The Microsoft Power Platform admin center will satisfy most administrative needs.*** ***Other administrative options are covered in the Dataverse learning path.*** 

### Admin Center

***The admin center lets you manage the tasks of setting up users, permissions, and many other important features and capabilities.*** 

**Settings are grouped into categories:**

- **Environments** - This section lists all instances of Microsoft Dataverse.
- **Data policies** - This section lets you set up policies to restrict which data connectors can be used with Microsoft Dataverse to limit what data can flow into or out of Microsoft Dataverse tables.
- **Data integration** - This section lets you create or add pre-defined connections and monitor these connections between Microsoft Dataverse and other data stores like Salesforce or SQL Server.
- **Tenant** - This section lets you monitor licenses and quotas.

