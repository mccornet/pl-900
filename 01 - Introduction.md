# 1. Introduction to Power Platform

Modern businesses run on data. Users interact with data daily from entering their time for payroll, seeking guidance on existing processes, and analyzing data to make decisions. In our technology driven world, users can be empowered to gain insights from and interact with data all while automating those menial responsibilities that seem to be more burden than job task. Microsoft Power Platform enables your business to craft solutions while empowering you to unite customized technology to help everyone, from the CEO to the front-line workers, drive the business with data.

In this module, you will:

- Learn the components and features of Microsoft Power Platform
- Identify when to use each Microsoft Power Platform component application to create business solutions
- Learn the value of using Microsoft Power Platform to create business solutions

Microsoft Power Platform is comprised of four key products: Power Apps, Power Automate, Power BI and Power Virtual Agents.

**Power Apps** provides a rapid low code development environment for building custom apps for business needs. It has services, connectors, and a scalable data service and app platform (Microsoft Dataverse) to allow simple integration and interaction with existing data. Power Apps enables the creation of web and mobile applications that run on all devices.
People use apps for every area of their lives, and business should be no exception. Most out of the box solutions do not meet exact business needs or integrate well with other business programs. Power Apps eases users into app development with a simple interface so that every business user or pro developer can build custom apps.

**Power Automate** lets users create automated workflows between applications and services. It helps automate repetitive business processes such as communication, data collections, and decision approvals. Don't waste important productive hours on drafting the same email for a weekly update or walking approvals through. Not only for the individual user, Power Automate allows for the creation of enterprise-grade process automation. Power Automate's simple interface allows every level of user to automate work tasks - from beginners to seasoned developers.

**Power BI** (Business Intelligence) is a business analytics service that delivers insights for analyzing data. It can share those insights through data visualizations which make up reports and dashboards to enable fast, informed decisions. Power BI scales across an organization, and it has built-in governance and security allowing businesses to focus on using data more than managing it.
You can consider Power BI as the analysis and insights leg of Microsoft Power Platform. It takes business data and allows you to display it in ways that makes the most sense to users. A Power BI dashboard could potentially replace a standing meeting to report out on company metrics such as sales data, progress against goals, or employee performance.

**Power Virtual Agents** enables anyone to create powerful chatbots using a guided, no-code graphical interface, without the need for data scientists or developers.
It minimizes the IT effort required to deploy and maintain a custom solution by empowering subject matter experts to build and maintain their own conversational solutions. Power Virtual Agents is part of Microsoft Power Platform, therefore integration into existing systems is streamlined with out-of-the-box integration with Power Automate and its ecosystems of hundreds of connectors. Users can enable chatbots to perform an action by simply calling a Power Automate flow. Flows help users automate activities or call back end systems. Users can utilize existing flows that have been created in their Power Apps environment or they can create a flow within Power Virtual Agents authoring canvas.

**Other Features**

Among the programs listed above, there are cross cutting features which enable Microsoft Power Platform to be leveraged to its full potential. Some of these are:

**AI Builder** lets users and developers add AI capabilities to the workflows and Power Apps they create and use. AI Builder is a turnkey solution that allows you to easily add intelligence to your workflows and apps and predict outcomes to help improve business performance without writing code.

**Microsoft Dataverse** is a scalable data service and app platform which lets users securely store and manage data from multiple sources and integrate that data in business applications using a common data model to ensure ease and consistency to users. Microsoft Dataverse is the common currency that enables the components of Microsoft Power Platform to work together. It’s the foundation that enables the consolidation, display, and manipulation of data.

**Connectors** enable you to connect apps, data, and devices in the cloud. Consider connectors the bridge across which information and commands travel. There are more than 275 connectors for Microsoft Power Platform, enabling all of your data and actions to connect cohesively. Examples of popular connectors include Salesforce, Office 365, Twitter, Dropbox, Google services, and more.

## 1.2 - Data Connectors

Microsoft Power Platform is made powerful by its ability to leverage data across many platforms. To do this, components of Microsoft Power Platform use connectors. You can think of connectors as a bridge from your data source to your app or workflow which allows information to be conveyed back and forth. Connectors allow you to extend your business solutions across platforms and add functionality for your users.

### 1.2.1 - Data Sources

In order to understand the types of connectors and what you can do with them, you must first understand the types of data sources to which they connect. The two types of data sources are tabular and function-based.

**Tabular data** - A tabular data source is one that returns data in a structured table format. Power Apps can directly read and display these tables through galleries, forms, and other controls. Additionally, if the data source supports it, Power Apps can create, edit, and delete data from these data sources. Examples include Microsoft Dataverse, SharePoint, and SQL Server.

**Function-based data** - A function-based data source is one that uses functions to interact with the data source. These functions can be used to return a table of data but offer more extensive action such as the ability to send an email, update permissions, or create a calendar event. Examples include Office 365 Users, Project Online, and Azure Blob Storage.

Both of these data source types are commonly used to bring data and additional functionality to your solutions.

As you can see, connecting to data sources allows you to integrate disparate parts of your business solutions to build them out cohesively.

### 1.2.2 - Connectors

Now that you understand more about data sources, you are ready to learn about connectors.

**Connectors** are the bridges from your data source to your app, workflow, or dashboard. Microsoft Power Platform has more than 275 connectors available to common data sources. Connectors are divided into standard and premium. Some popular standard connectors are SharePoint, Outlook, and YouTube. Premium connectors require additional licensing for your app and/or users. A few premium connectors are SQL Server, Survey Monkey, and Mail Chimp. The connector reference in the summary and resources unit lists all connectors and whether they are considered standard or premium. You can also use AppSource to source and install apps and use the connectors to non-Microsoft services.

Connectors can provide input and output between the data source and Power Platform, which can accelerate the delivery of Microsoft Power Platform business solutions. For instance, using Dynamics 365 apps such as Customer Service, you can set up Power Automate to notify users when specific customer types are added. Or you can use a SharePoint document library to store files that are fed into Power Apps to manage and distribute. Microsoft also provides connectors to their Azure services, providing advanced AI techniques to do tasks such as reading text off images or cognitive services like recognizing faces in images.

All Microsoft Power Platform business solutions can be used and implemented into Microsoft 365 apps such as Teams. This allows users to play Power Apps within Teams or run Power Automate from actions and events within Teams.

### 1.2.3 - Triggers and Actions

Once you have established a data source and configured your connector, there are two types of operations you can use, triggers or actions.

**Triggers** are only used in Power Automate and prompt a flow to begin. Triggers can be time based, such as a flow which begins every day at 8:00 am, or they could be based off of an action like creating a new row in a table or receiving an email. You will always need a trigger to tell your workflow when to run.

**Actions** are used in Power Automate and Power Apps. Actions are prompted by the user or a trigger and allow interaction with your data source by some function. For example, an action would be sending an email in your workflow or app or writing a new line to a data source.

Now that you understand what connectors are and how to use them, let's look at what to do when there isn't a connector already built for your data source.

### 1.2.4 - Custom Connectors

While Microsoft Power Platform offers more than 200 connectors, you also have the option to build a custom connector. This will allow you to extend your app by calling a publicly available API, or a custom API you are hosting in a cloud provider, such as Azure. API stands for Application Programming Interface and holds a series of functions available for developers. Connectors work by sending information back and forth across these APIs and gathering available functions into Power Apps or Power Automate. Because these connectors are function-based, they will call specific functions in the underlying service of the API to return the corresponding data.

An advantage of building custom connectors is that they can be used in different platforms, such as Power Apps, Power Automate, and Azure Logic Apps.

You can create custom connectors using 3 different approaches:

- [Using a blank custom connector](https://docs.microsoft.com/en-us/connectors/custom-connectors/define-blank)
- [From an OpenAPI definition](https://docs.microsoft.com/en-us/connectors/custom-connectors/define-openapi-definition)
- [From a Postman collection](https://docs.microsoft.com/en-us/connectors/custom-connectors/define-postman-collection)

While the requirements for each approach will vary, they all require a Power Apps per app or per user plan. Each link above points to the instructions for each approach.

## 1.3 - DLP, Compliance, Privacy, Accessibility

### 1.3.1 - Data loss prevention policies

Your organization's data is likely one of the most important assets you are responsible for safeguarding as an administrator. The ability to build apps and automation to use that data is a large part of your company's success. You can use Power Apps and Power Automate for rapid build and rollout of these high-value apps so that users can measure and act on the data in real time. Apps and automation are becoming increasingly connected across multiple data sources and multiple services. Some of these might be external, third-party services and might even include some social networks. Users generally have good intentions, but they can easily overlook the potential for exposure from data leakage to services and audiences that should not have access to the data.

You can create data loss prevention (DLP) policies that can act as guardrails to help prevent users from unintentionally exposing organizational data. DLP policies can be scoped at the environment level or tenant level, offering flexibility to craft sensible policies that strike the right balance between protection and productivity. For tenant-level policies, you can define the scope to be all environments, selected environments, or all environments except ones you specifically exclude.

Connectors can be classified as either **Business** or **Non-Business** in the context of your organization. Connectors that host business-use data should be classified as **Business** and connectors that host personal-use data should be classified as **Non-Business**. Any connectors that you want to restrict usage of across one or more environments should be classified as **Blocked**. When a new policy is created, all connectors are defaulted to the **Non-Business** group. From there they can be moved to **Business** or **Blocked** based on your preference. You can manage connectors when you create or modify the properties of a DLP policy from the [Microsoft Power Platform admin center](https://admin.powerplatform.microsoft.com/). These affect Microsoft Power Platform canvas apps and Power Automate flows. To create a DLP policy, you need to be a tenant admin or have the Environment Admin role.

### 1.3.2 Compliance and data privacy

Microsoft is committed to the highest levels of trust, transparency, standards conformance, and regulatory compliance. Microsoft’s broad suite of cloud products and services are all built from the ground up to address the most rigorous security and privacy demands of our customers.

To help your organization comply with national, regional, and industry-specific requirements governing the collection and use of individuals’ data, Microsoft provides the most comprehensive set of compliance offerings (including certifications and attestations) of any cloud service provider. There are also tools for administrators to support your organization’s efforts. In this part of the document we will cover in more detail the resources available to help you determine and achieve your own organization requirements.

**Data Protection**

Data as it is in transit between user devices and the Microsoft datacenters are secured. Connections established between customers and Microsoft datacenters are encrypted, and all public endpoints are secured using industry-standard TLS. TLS effectively establishes a security-enhanced browser to server connection to help ensure data confidentiality and integrity between desktops and datacenters. API access from the customer endpoint to the server is also similarly protected. Currently, TLS 1.2 (or higher) is required for accessing the server endpoints.

**GDPR compliance**

The European Union General Data Protection Regulation (GDPR) is one of the newest privacy regulations enacted that gives rights to people to manage their personal data. A complete discussion of GDPR is beyond the scope of this content, however Microsoft Power Platform does fully support the GDPR. For more GDPR resources and information, visit the Trust Center at https://www.microsoft.com/TrustCenter/Privacy/gdpr/default.aspx.

**Accessibility**

One of the things that Microsoft values the most is making sure that Power Platform is accessible and inclusive to all kinds of users all over the world. An accessible canvas app will allow users with vision, hearing, and other impairments to successfully use the app. In addition to being a requirement for many governments and organizations, following the below guidelines increases usability for all users, regardless of their abilities. You can use the [Accessibility Checker](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/accessibility-checker) to help review potential accessibility issues in your app. For more details and suggestions on making your canvas apps more accessible, visit [Create accessible canvas apps in Power Apps](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/accessible-apps).

## 1.4 - Putting it together

Although we live in a data driven world, your business can find it difficult to take advantage of the data you have access to. Sales, customer, and employee data should drive our business decisions, but where do we even start? Microsoft Power Platform can add value to any business by helping you to analyze, act, and automate. Act by building custom apps in Power Apps, automate processes based on the data you collect in Power Automate, and analyze the data you have collected in Power BI.

Consider a business that has IT equipment for general use. Currently, equipment check-out is conducted by visiting the IT office, checking if the product is available, then writing your name and the equipment name in a notebook. Employees may have to visit IT several times before equipment becomes available, and IT personnel must drop their tasks to check on equipment status or go to collect it for the employee. Sometimes employees hold onto the equipment longer than they intend and an IT personnel spends time tracking it down. In addition, important equipment information such as serial number, warranty details, and instructions for use are kept somewhere in the IT office. How can Microsoft Power Platform improve this process?

Power Apps allows us to build an app that has all equipment listed, the status of that equipment, and even important details such as use instructions. This way employees can check out available equipment, walk to IT at a specified pickup time where the equipment will be ready, and even access the use instructions or flag an equipment malfunction from their phone or tablet. Power Automate can read when equipment needs to be returned and send out reminder emails, or even a warning that the equipment is late being checked in. Users can see when equipment is booked through the app and request check-out for a future date at which time Power Automate can send them a reminder to pick up the equipment and IT a reminder to have it ready. Power BI can take all the data generated from the app and analyze it to help you understand what equipment is used most often and by whom. This way you can decide if you need other equipment, if some users or departments need dedicated equipment, and when your equipment has reached the end of its usefulness.

This is only one common scenario in which Microsoft Power Platform can transform the way businesses work. Consider your own business and what processes take up valuable time and are a burden to customers or employees. How can you leverage Microsoft Power Platform to improve them?

