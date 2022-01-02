# PL-900 Dataverse

Microsoft Dataverse is a cloud-based, low-code data service and app platform, which allows you to leverage the security and connectivity of Microsoft services. Dataverse connects easily to all aspects of Microsoft Power Platform so that you can fully control, automate, and strengthen your business. With standard tables and columns, as well as the ability to easily define relationships between your data, Dataverse was built for powerful, scalable solutions.

## Overview

Microsoft Dataverse is a cloud-based solution that easily structures a variety of data and business logic to support interconnected applications and processes in a secure and compliant manner. Managed and maintained by Microsoft, Dataverse is available globally but deployed geographically to comply with your potential data residency. It is not designed for stand-alone use on your servers, so you will need an internet connection to access and use it.

Dataverse is designed to be your central data repository for business data, and you might even be using it already. Behind the scenes, it powers many Microsoft Dynamics 365 solutions such as Field Service, Marketing, Customer Service, and Sales. It is also available as part of Power Apps and Power Automate with native connectivity built right in. The AI Builder and Portals features of Microsoft Power Platform also utilize Dataverse.

Below is a visualization that brings together the many offerings of Microsoft Dataverse.

![Dataverse API options](https://docs.microsoft.com/en-us/learn/modules/introduction-common-data-service/media/common-data-service-diagram.png)

As you can see, Microsoft Dataverse offers a great deal of functionality. Below is a brief explanation of each category of features.

**Security**: Dataverse handles authentication with Azure Active Directory (Azure AD) to allow for conditional access and multi-factor authentication. It supports authorization down to the row and column level and provides rich auditing capabilities.

**Logic**: Dataverse allows you to easily apply business logic at the data level. Regardless of how a user is interacting with the data, the same rules apply. These rules could be related to duplicate detection, business rules, workflows, or more.

**Data**: Dataverse offers you the control to shape your data, allowing you to discover, model, validate, and report on your data. This control ensures your data looks the way you want regardless of how it is used.

**Storage**: Dataverse stores your physical data in the Azure cloud. This cloud-based storage removes the burden of worrying about where your data lives or how it scales. These concerns are all handled for you.

**Integration**: Dataverse connects in different ways to support your business needs. APIs, webhooks, eventing, and data exports give you flexibility to get data in and out.

As you can see, Microsoft Dataverse is a very powerful cloud-based solution for storing and working with your business data. In the following sections, you will look at Microsoft Dataverse from the lens of data storage for Microsoft Power Platform, where you will start your journey. Keep in mind the additional rich capabilities discussed above which you can explore further as your usage increases.

To get started, Microsoft Dataverse lets you create one or many cloud-based instances of a standardized database. The database includes predefined tables and columns which store data commonly found across nearly all organizations and businesses. You can customize and extend what is stored by adding new columns or tables. The ease of setting up a Microsoft Dataverse database and standardized data model under it simplifies your ability to concentrate your efforts on building solutions without worrying about infrastructure, storage, and data integration. With your data stored in Microsoft Dataverse, there are many different ways to access it. You can work with the data natively with tools such as Power Apps or Power Automate. Or through connectors and APIs you can connect to Microsoft Dataverse from any business solution. With the power of features such as role-based security and business rules you can trust your data is safe no matter how it is accessed.

### Dataverse defined

A Dataverse database is a single instance of Microsoft Dataverse which stores data in a set of standard and custom data structures called tables. A table is a logical set of rows that is used to store data. Rows within a table contain many columns to manage individual pieces of information about a single row.

You can create one or many database instances in Microsoft Dataverse to host data behind your business solutions. Each instance of a Microsoft Dataverse will start with the same set of tables to store data, but you can always extend and customize a Microsoft Dataverse database to meet specific business needs. This means that you can share business solutions that reference standard tables in Microsoft Dataverse across your organization or with any other organization by using it anywhere in the world.

### Scalability

A Dataverse database supports large data sets and complex data models. Tables can hold millions of items, and you can extend the storage in each instance of a Microsoft Dataverse database to four (4) terabytes per instance. The amount of data that is available in your instance of Microsoft Dataverse is based upon the number and type of licenses that are associated with it. Data storage is pooled between all licensed users, so you can allocate storage as needed for each solution that you build. Additional storage can be purchased if you need more storage than what is offered within standard licensing.

### Common Data Model vs. Microsoft Dataverse

The standard table design in a Microsoft Dataverse database is based upon an open data model standard called Common Data Model. Common Data Model is a logical design that includes a set of open-sourced, standardized, extensible data tables and relationships that Microsoft and its partners have published in an industry-wide initiative called the Open Data Initiative. This collection of predefined tables, columns, semantic metadata, and relationships form the basis of the Common Data Model.

### Microsoft Dataverse structure and benefits

The structure of a Microsoft Dataverse database is based upon the definitions and schema in the Common Data Model. The key benefit of using Common Data Model as the basis of a Microsoft Dataverse database is simplified integration of any solutions that use a Common Data Model schema, because the standard tables of the solution are the same. You will also be able to take advantage of a rich ecosystem of solutions that vendors have built from using Common Data Model. Best of all, there is practically no limit to how far you can extend a Microsoft Dataverse database.

## Tables & Columns

A table is a logical structure containing rows and columns that represents a set of data.

### Types of tables

- **Standard** - The base set of tables that are created for every instance of a Microsoft Dataverse database. You can add more columns to any table, but you can only delete columns from a custom table.
- **Complex** - Tables that contain complex, server-side business logic, including real-time workflows or plug-ins. Some of the tables that are used in Dynamics 365 applications are complex. Care must be taken if you add server-side logic to ensure that users have the proper license to use the complex table. Additional information about complex tables can be accessed by following the link within the summary unit of this module.

### Columns

Columns are a way to store a discrete piece of information within a row in a table. You might think of them as a column in Excel. Columns have data types, meaning that you can store data of a certain type in a column that matches that data type. For example, if you have a solution that requires dates, then you would store the date in a column with the type of Date. Similarly, if you want to store a number, then you store the number in a column with the type of Number.

The number of columns within a table varies from a few columns to a hundred or more. If you need more than a few hundred columns in a table, you might want to reconsider how you are structuring data storage for your solution because, likely, there is a better way.

Every database in Microsoft Dataverse starts with a standard set of tables and each standard table has a standard set of columns.

## Relationships

o make an efficient and scalable solution for most of the solutions that you build, you will need to split up data into different containers (tables). Trying to store everything into a single container would likely be inefficient and difficult to work with and understand.

The following example helps illustrate this concept.

Imagine that you need to create a system to manage sales orders. You will need a product list along with the inventory on hand, cost of the item, and the selling price. You also need a master list of customers with their addresses and credit ratings. Finally, you will need to manage invoices of sales that you make so you will want a way to store invoice data. The invoice should include information such as date, invoice number, and salesperson, customer information including address and credit rating, and a line item for each item on the invoice. Line items should include a reference to the product that you sold and be able to provide the proper cost and price for each product and decrease the quantity on hand based upon the quantity that you sold in that line item.

Trying to create a single table to support the functionality that was previously described would be inefficient. A better way to approach this business scenario is to create the following four tables:

- Customers
- Products
- Invoices
- Line Items

Creating a table for each of these items and relating them to one another will allow you to build an efficient solution that can scale while maintaining high performance. Splitting the data into multiple tables also means that you will not have to store repetitive data or support huge rows with large amounts of blank data. Additionally, reporting will be much easier if you split the data into separate tables.

Tables that relate to one another have a relational connection. Relationships between tables exist in many forms, but the two most common are one-to-many and many-to-many, both of which are supported by Microsoft Dataverse.

One-to-many relationships are also known as parent-child relationships. In the previous invoice example, the invoice table would be the parent and the line items would be a child table. An invoice can have zero, one, or many line items (child rows), but the line item will always be related to just one invoice (parent row). Typically, the child rows will not exist without a parent row.

A column that only allows unique values, such as invoice number, is used to identify the parent row. This unique column is called a key. The same value (the parent key) is stored in the related child rows. This column is called a foreign key when the child row is used to store the parent key value. Filtering is used to display child rows with a value in the foreign key that matches the key value in the parent row. This allows applications to display the child rows (line items in the previous example) that belong to a particular parent row (invoice in the previous example). This concept underlies many business software applications.

Splitting data into different tables makes for an efficient solution design that can scale, but knowing how to split up the data into tables can be difficult. Thankfully, Microsoft Dataverse already contains many of the tables that most organizations will need. Using standard tables and extending them will ensure that you are building solutions around a proven, scalable way of storing the data that is used by your solutions.

## Environments

Environments are used to store, manage, and share your organization's business data, apps, and flows in Microsoft Power Platform. Each environment allows you to provision one Microsoft Dataverse database for use within that environment. Microsoft Dataverse environments allow you to manage user access, security settings, and the storage that is associated with that database.

Each environment is created under a Microsoft Azure Active Directory (Azure AD) tenant, and its resources can only be accessed by users within that tenant. An environment is also bound to a geographic location, like the United States. When you create a Microsoft Dataverse database in an environment, that database is created within datacenters in that geographic location. Any items that you create in that environment (including connections, gateways, flows that are using Power Automate, and more) are also bound to their environment's location. ![Contoso tenant to environment map](https://docs.microsoft.com/en-us/learn/modules/introduction-common-data-service/media/environment.png)

You can create more than one environment to manage solution development and data storage by setting up one environment for development, another for testing, and another for production use. Also, you can set up an environment based on a geographical location. For example, you might set up an environment for Europe and another for Asia. Each of these environments will have zero or only one instance of Microsoft Dataverse.

## Business Rules

In Microsoft Dataverse you can define business rules. Business rules allow you to apply and maintain business logic at the data layer instead of the app layer. Put more simply, if you create business rules in Microsoft Dataverse, they are in effect regardless of where you interact with the data.

For example, business rules can be used in canvas and model-driven apps to set or clear values in one or many columns in a table. They can also be used to validate stored data or show error messages. Model-driven apps can use business rules to show or hide columns, enable or disable columns, and create recommendations based on business intelligence.

> **Tip**
>
> Business rules are usually defined for a table and apply to all forms, but you can define a business rule for a specific model-driven form. Canvas apps cannot have a business rule applied to a specific form, but they are still enforced when interacting with the data.

Business rules give you a powerful way to enforce rules, set values, or validate data regardless of the form that is used to input data. Additionally, business rules are effective in helping to increase the accuracy of data, simplify application development, and streamline the forms presented to end users.

The following business rule actions can be used by canvas and model-driven apps:

- Set column values
- Clear column values
- Validate data and show error messages

Model-driven apps can also use business rules to:

- Show or hide columns (model-driven apps only)
- Enable or disable columns (model-driven apps only)
- Create business recommendations based on business intelligence (model-driven apps only)

Below is an example of a simple, yet powerful use of business rules. The business rule is configured to change the field Credit Limit VP Approver to be a required field if the Credit Limit is set to greater than $1,000,000. If the credit limit is less than $1,000,000 then the field is optional.

![Example of business-rule](https://docs.microsoft.com/en-us/learn/modules/introduction-common-data-service/media/business-rule.png)

By applying this business rule at the data level instead of the app level, you have better control of your data. This can ensure your business logic is followed whether it is being accessed directly from Power Apps, Power Automate, or even via an API. The rule is tied to the data, not the app.

## Administer

Microsoft Dataverse has a rich set of administrative options that you can use to create new instances of a database or tailor access and features that are available for users of each Dataverse database instance. Several administrative portals are available for you to use to administer Microsoft Dataverse settings.

The Microsoft Power Platform admin center is discussed in this unit because it will satisfy most of your administrative needs. However, a few other administrative options are available, which are covered in the Manage permissions and administration for Microsoft Dataverse learning path.

### Microsoft Power Platform admin center

The Microsoft Power Platform admin center lets you manage the tasks of setting up users, permissions, and many other important features and capabilities of Microsoft Dataverse.

Most of the administration settings that you will need are available in the Microsoft Power Platform admin center. You should always check for administration settings as your first step when looking to administer Microsoft Dataverse.

Settings are grouped into the following broad categories and are accessible by selecting the link on the left-hand side of the portal, as shown in the following figure.

- **Environments** - This section lists all instances of Microsoft Dataverse.
- **Data policies** - This section lets you set up policies to restrict which data connectors can be used with Microsoft Dataverse to limit what data can flow into or out of Microsoft Dataverse tables.
- **Data integration** - This section lets you create or add pre-defined connections and monitor these connections between Microsoft Dataverse and other data stores like Salesforce or SQL Server.
- **Tenant** - This section lets you monitor licenses and quotas.

![Environment Listing](https://docs.microsoft.com/en-us/learn/modules/introduction-common-data-service/media/list-environments.png)