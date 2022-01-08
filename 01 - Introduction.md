# PL-900 Power Platform

***Modern businesses run on data***. ***Microsoft Power Platform makes it possible to drive the business with this data***. Users interact with data daily from entering their time for payroll, seeking guidance on existing processes, and analyzing data to make decisions. In our technology driven world, users can be empowered to gain insights from and interact with data all while automating those menial responsibilities that seem to be more burden than job task. 

### Key Products

**Power Apps** - ***a rapid low code development environment*** for building custom apps for business needs. Power Apps enables the creation of web and mobile applications that run on all devices. Power Apps eases users into app development with a simple interface so that every business user or pro developer can build custom apps.

**Power Automate** - ***automated workflows between applications and services***. It helps automate repetitive business processes such as communication, data collections, and decision approvals.

**Power BI (Business Intelligence)** - ***a business analytics service that delivers insights for analyzing data***. It can share those insights through data visualizations which make up reports and dashboards to enable fast, informed decisions.

**Power Virtual Agents** - ***create powerful chatbots using a guided, no-code graphical interface***, without the need for data scientists or developers. Users can enable chatbots to perform an action by simply calling a Power Automate flow. Flows help users automate activities or call back end systems. Users can utilize existing flows that have been created in their Power Apps environment or they can create a flow within Power Virtual Agents authoring canvas.

### Other Features

**AI Builder** - ***add AI capabilities to the workflows and Power Apps***. AI Builder is a turnkey solution that allows you to easily add intelligence to your workflows and apps and improve business performance without writing code.

**Microsoft Dataverse** - ***a scalable data service and app platform to store and manage data*** from multiple sources and integrate that data in business applications using a common data model to ensure ease and consistency to users. 

**Connectors** - ***connect apps, data, and devices in the cloud***. Consider connectors the bridge across which information and commands travel. 

## Data Connectors

***Connectors make it possible to leverage data across many platforms.*** ***The two types of data sources are: tabular and function-based***. 

1. **Tabular data** - ***A source that returns data in a structured table format***. Power Apps can directly read and display these tables through galleries, forms, and other controls. Additionally, if the data source supports it, Power Apps can create, edit, and delete data from these data sources. Examples include Microsoft Dataverse, SharePoint, and SQL Server.

2. **Function-based data** - ***A source that uses functions to interact with the data source. Can return a table of data but also offer more extensive actions*** such as the ability to send an email, update permissions, or create a calendar event. Examples include Office 365 Users, Project Online, and Azure Blob Storage.

### Connectors

***Provide input and output between the data source and Power Platform, Connectors are the bridges from your data source to your app, workflow, or dashboard.*** ***Connectors are divided into standard and premium***. 

#### Custom Connectors

***These connectors are function-based and allow the app to call an API.*** Either a publicly available API, or a custom API, you are hosting in a cloud provider, such as Azure. Connectors work by sending information back and forth across these APIs and gathering available functions into Power Apps or Power Automate. Because these connectors are function-based, they will call specific functions in the underlying service of the API to return the corresponding data.

**Create custom connectors using 3 different approaches**: 

> **Note**:
>
> ***Custom connectors require a Power Apps per app or per user plan.*** 

- [Using a blank custom connector](https://docs.microsoft.com/en-us/connectors/custom-connectors/define-blank)
- [From an OpenAPI definition](https://docs.microsoft.com/en-us/connectors/custom-connectors/define-openapi-definition)
- [From a Postman collection](https://docs.microsoft.com/en-us/connectors/custom-connectors/define-postman-collection)

### Triggers and Actions

***Once you have established a data source and configured your connector, there are two types of operations you can use, triggers or actions.***

***Triggers are used in Power Automate and prompt a flow to begin***. Triggers can be time based, such as a flow which begins every day at 8:00 am, or they could be based off of an action like creating a new row in a table or receiving an email. You will always need a trigger to tell your workflow when to run.

***Actions are in Automate and Apps; activated by the user or a trigger and allow interaction with a data source by some function.*** 

## DLP, Compliance, Privacy, Accessibility

### Data loss prevention policies

***Data is likely one of the most important assets you are responsible for safeguarding as an administrator***. Power Apps and Power Automate allow for rapid build and rollout of these high-value apps so that users can measure and act on the data in real time. 

***Create data loss prevention (DLP) policies that can act as guardrails to help prevent users from unintentionally exposing organizational data.*** ***DLP policies can be scoped at the environment level or tenant level***, offering flexibility to craft sensible policies that strike the right balance between protection and productivity. To create a DLP policy, you need to be a tenant admin or have the Environment Admin role.

For tenant-level policies, you can define the scope to be all environments, selected environments, or all environments except ones you specifically exclude.

***Connectors can be classified***: **Business** or **Non-Business** in the context of your organization. ***Connectors that host business-use data should be classified as* Business** and connectors that ***host personal-use data should be classified as*** **Non-Business**. Any connectors that you want ***to restrict usage of across one or more environments connectors should be classified as*** **Blocked**. When a new policy is created, ***all connectors are defaulted to*** **Non-Business** group. 

### Compliance and data privacy

***Microsoft’s broad suite of cloud products and services are all built to address the most rigorous security and privacy demands.*** 

***Microsoft provides the most comprehensive set of compliance offerings to help comply with national, regional, and industry-specific requirements governing the collection and use of individuals’ data.*** Microsoft provides the most comprehensive set of compliance offerings (including certifications and attestations) of any cloud service provider. There are also tools for administrators to support your organization’s efforts. 

#### Data Protection

***Data in transit is secured using industry-standard TLS***. API access from the customer endpoint to the server is also similarly protected. Currently, TLS 1.2 (or higher) is required for accessing the server endpoints.

#### GDPR compliance

The European Union General Data Protection Regulation (GDPR) is one of the newest privacy regulations enacted that gives rights to people to manage their personal data. ***Microsoft Power Platform does fully support the GDPR.*** 

#### Accessibility

***An accessible canvas app will allow users with vision, hearing, and other impairments to successfully use the app***. In addition to being a requirement for many governments and organizations, following the below guidelines increases usability for all users, regardless of their abilities. 

## Putting it together

***We live in a data driven world, so take advantage of the data*** you have access to. Sales, customer, and employee data should drive our business decisions. Microsoft Power Platform can add value by helping to analyze, act, and automate. 

- ***Act*** by building custom apps in ***Power Apps***, 
- ***Automate*** processes in ***Power Automate***
- ***Analyze*** in ***Power BI***.

