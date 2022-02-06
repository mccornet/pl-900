# Chapter 1 - Business Value

The Power Platform tools provide users with the ability to perform three key actions on their data: analyze, act, and automate.

Power BI is a data analytics service that allows users to discover and gather data from local and cloud sources and then visualize and share that data.

Power Apps is a development platform that allows users to act on their data by creating web and mobile applications without writing code.

Power Automate is an automation service that allows users to trigger complex processes and workflows.

Power Virtual Agents is a service that allows users to create chatbots using a graphical interface with no coding.

Power Platform provides connectivity both within and among the various applications and services in Dynamics 365, Microsoft 365, Microsoft Azure, and other third-party products.

The Power Platform tools—Power BI, Power Apps, Power Automate, and Power Virtual Agents, along with their underlying components (Common Data Service, Data Connectors, and AI Builder)—run as individual services, meaning that they are cloud-based software products that are hosted by Microsoft Azure on a software as a service (SaaS) basis.

All of the Power Platform tools rely on Azure Active Directory for user accounts and licensing.

The Power Platform admin center provides administrative access to the tenant’s existing environments, as well as the ability to create new ones.

Compliance Manager is a risk assessment tool that allows an organization to track and record the activities they undertake to achieve compliance with specific certification standards.



# Chapter 2 - Core Components

Common Data Service is a cloud-based data storage solution that the Power Platform applications can use to maintain their data in a secure, manageable environment.

The Power Platform tools are able to connect directly to many different data sources, including local files, network resources, and cloud-based services.

An entity is the Common Data Service equivalent of a table in other database management systems. A default Common Data Service instance has a base set of standard entities, which the developer can populate with data from outside sources.

Fields are the attributes within an entity that contain specific types of data. If an entity is the equivalent of a table, then a field is the equivalent of a column in the table.

An environment is a container for the apps and flows created in Power Apps and Power Automate, as well as the data they use.

Business process flows are tools that allow administrators to ensure that users follow specific procedures when performing certain tasks.

Business rules enable developers to implement logic on data stored in Common Data Service.

Common Data Model (CDM) is a Microsoft initiative that defines a shared data language, consisting of a unified system of schemas and metadata. The objective behind CDM is to create a standardized format for data sharing and storage that allows applications and services to share data without the need for custom implementations.

Connectors are Power Platform components that allow Power Apps and Power Automate to interact with outside applications, services, and data files and utilize their data.

Triggers are components in Power Automate that cause a flow to begin running. Actions are specific modifications made to the data provided by an outside application or service.

AI Builder adds intelligence to the apps and flows created in Power Apps and Power Automate.

To use AI Builder, developers choose from a collection of prebuilt and custom models that define scenarios in which an app can apply artificial intelligence to a business task.



# Chapter 3 - Power BI

Visualizations are the formats designers can use to display data in a Power BI dashboard or report. Power BI provides a large selection of visualizations to choose from, including various types of charts, tables, maps, gauges, apps, and cards.

Filters are a means by which Power BI designers and consumers can specify what data is displayed in reports.

The Power BI service interface has a menu on the left side of the workspace that provides the primary means for users to navigate around the site.

With Power BI, it is possible for organizations and users to create their own custom visualizations and share them within the organization or with the outside Power BI community.

When a user registers a Power BI account, the service creates a workspace for that user. A workspace is a private area of the service in which users can work on their content prior to sharing it.

The Power BI service is the cloud-based environment that both developers and consumers use to create and access dashboards, reports, and other content. Power BI Desktop is a Windows application that provides more advanced data modeling and report development capabilities.

The Power BI service allows developers to connect to any one of hundreds of data sources. However, in Power BI Desktop, it is possible to connect to multiple data sources at once and combine the information from them into a single data model.

Data modeling is a term that can refer to a variety of tasks, including modifying data types; removing rows or columns; and renaming tables, rows, or columns.

Power BI uses the term aggregate to refer to mathematical functions that it executes on values obtained from data sources.

Power BI makes it possible to share data sets with other users, so developers do not always need to have a complete understanding of the data they use to create reports, dashboards, and apps.

A dashboard is a single page composed of tiles, rectangular placeholders containing visualizations taken from existing reports and data sets that update in real time.

Because a dashboard is only a single page, developers must consider the size of the screen that consumers will be using to view it.

After creating a report or dashboard in the Power BI service, developers can share it with selected users.

For developers working in Power BI Desktop, their completed content is not accessible to consumers until they publish it to the Power BI service.



# Chapter 4 - Power Apps

Power Apps is designed for citizen developers with little or no coding experience.

Developers create canvas apps by dragging and dropping elements onto screens in Power Apps Studio; model-driven apps do not provide the same interface configuration capability.

A portal app is a means of providing users —both internal and external— with access to data stored in the Common Data Service using a website.

The process of building a canvas app involves connecting to a data source, placing controls on the app screens, and finally publishing and sharing the app to make it accessible to consumers.

The actual process of designing a canvas app involves placing controls on the app screens to create a usable interface for the consumers who will be running it.

After developers finish building their apps, they have to save them and share them with the users who will access them.

Creating a blank portal uses the Common Data Services database installed in the selected environment as its data source.

The starter page generated by a portal app created from a blank has a rudimentary design that is only intended to provide the developer with a basic structure on which to build.

Portal apps, by default, use local authentication based on accounts realized in the Contact entity of the Common Data Services database.

Themes are Cascading Style Sheets (CSS) definitions that specify the attributes to be applied to the webpages generated by a portal app.

Model-driven apps are centered around the data they gather and present and the business processes they realize for users.

Model-driven app designs are based on components, but in the App Designer interface, the components do not resemble the elements as they will appear on the final app screens.

Forms appear in model-driven apps when users view entity data in a table format and click the New button to create a new record in the entity.



# Chapter 5 - Power Automate

Power Automate supports five flow types: automated, instant, scheduled, UI, and business process.

To simplify the process of getting started in creating Power Automate flows, the tool also includes dozens of templates.

Power Automate uses connectors to access data sources in flows for both triggers and actions.

A flow can contain a condition, which is an if/then statement that defines two possible actions. Looping refers to flows that contain sequences of actions that intentionally repeat.

Power Automate supports the use of expressions, which can perform operations on existing values.

One of the common uses of Power Automate flows is to process approvals of documents, in which users must seek the approval of a superior before the task they are working on is completed.

One method of creating a flow is to start from a blank flow by selecting one of the tiles in the Power Automate portal representing the type of trigger that will launch it.

For many new developers, the easiest way to learn how to build a flow is to begin with one of the flow templates included with Power Automate. Templates often need some modification before they can run.

Power Automate’s Data Operation actions make it possible to reuse and reformat the data from previous actions in various ways.

To test a flow and examine how each step executes, the developer can click the Test button at the upper right of the workspace canvas.



# Chapter 6 - Power Virtual Agents

Power Virtual Agents is a no-code or low-code tool that allows customer service and technical support personnel themselves to create chatbots and update them as needed

Developers can publish chatbots to websites and many other types of platforms, including internal messaging platforms, such as Microsoft Teams, mobile apps, and social media. Power Virtual Agents refers to these places of publication as channels.

Power Virtual Agents breaks down the conversation between a bot and a user into discrete elements called topics. An entity is a dictionary of terms and phrases that a bot’s artificial intelligence uses to identify a concept in a conversation. An action is an element that allows a bot to
actually do something beyond conversing with the user.

After starting Power Virtual Agents, a developer must start by creating a bot, which involves selecting a name, a language, and the environment in which the bot will be created. The process occurs in the background and can take as long as 15 minutes.

Power Virtual Agents includes a collection of system topics that cover some of the most common exchanges between bots and customers. Developers can also create their own topics from scratch.

Power Virtual Agents can perform actions by working together with Power Automate. It is actually Power Automate flows that perform actions, but a bot can pass information to a flow and receive information back using variables.

The test pane allows the developer to interact with the bot as a customer while tracking the progress of the conversation through the nodes in the workspace.

The Publish page contains a single Publish button that makes the current version of the bot available for distribution to users. Developers must republish their bots each time they make changes to them so that the latest version is provided to users.

The Analytics page in the Power Virtual Agents portal provides an array of charts that allow developers and administrators to track the number of users that access a bot and examine the results of that usage.

Power Virtual Agents includes a prebuilt End of Conversation topic, which includes a survey question that allows users to state whether their session with the bot was successful in answering their questions or solving their problems.



