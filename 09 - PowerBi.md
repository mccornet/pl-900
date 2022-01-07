# Power BI

***Power BI can build reports and dashboards with interactive visualizations to drive business with actionable insights.***

The business world is increasingly data driven. Small and large businesses alike use data to make decisions about sales, hiring, goals, and all areas for which they have data. While most businesses have access to data of one type or another, it can be intimidating to try to understand without a background in data analytics or statistics. Even if you do understand the data, a challenge may arise in displaying the data in an easy to understand way and communicating it to other relevant people. ***Power BI takes the intimidation and hassle out of data analysis and visualization***. 

## What is Power BI

***Data is only as good as the ability to interpret and communicate its meaning. That's where Power BI (Business Intelligence) comes into play.***

***Microsoft Power BI is a collection of software services, apps, and connectors that work together to*** ***turn your unrelated sources of data into coherent, visually immersive, and interactive insights.*** Power BI lets you easily connect to your data sources, clean, and model your data without affecting the underlying source, visualize (or discover) what's important, and share that with anyone or everyone you want.

![Different sources of data can be showcased in one place](https://docs.microsoft.com/en-us/learn/modules/introduction-power-bi/media/pbi-intro-01.png)

**Power BI consists of:**

- **Power BI Desktop** - Microsoft Windows desktop application
- **Power BI service** - an online SaaS (Software as a Service)
- **Mobile Power BI apps** that are available on phones and tablets.

***These three elements let people create, share, and consume business insights in the way that serves them, or their role, most effectively.***

## Power BI concepts

***The major building blocks of are: datasets, reports, and dashboards.*** 

***They are all organized into workspaces, and created on capacities.***

### Capacities

***Capacities are a core Power BI concept representing a set of resources used to host and deliver your Power BI content.*** ***Capacities are*** ***either shared or dedicated***. A shared capacity is shared with other Microsoft customers, while a dedicated capacity is fully committed to a single customer. ***Dedicated capacities require a subscription***. By default, workspaces are created on a shared capacity.

### Workspaces

***Workspaces are containers for dashboards, reports, datasets, and dataflows in Power BI***. 

#### Two types:

- **My workspace** is the ***personal workspace for any Power BI customer to work with their own content***. Only you have access to your My workspace. You can share dashboards and reports from your My Workspace. If you want to collaborate on dashboards and reports, or create an app, then you want to work in a workspace.
- **Workspaces** are ***used to collaborate and share content with colleagues***. You can add colleagues to your workspaces and collaborate on dashboards, reports, and datasets. With one exception, all workspace members need Power BI Pro licenses.

***Workspaces are also the places where you create, publish, and manage apps for your organization***. Think of workspaces as staging areas and containers for the content that will make up a Power BI app. So what is an *app*? An app is a collection of dashboards and reports built to deliver key metrics to the Power BI consumers in your organization. Apps are interactive, but consumers cannot edit them. App consumers, the colleagues who have access to the apps, do not necessarily need Pro licenses.

### Datasets

***A dataset is a collection of data that you import or connect to***. Power BI lets you connect to and import all sorts of datasets and bring all of it together in one place. ***Datasets can also source data from dataflows***.

***Datasets are associated with workspaces and a single dataset can be part of many workspaces***. When you open a workspace, the associated datasets are listed under the Datasets tab. Each listed dataset represents a collection of data, for example, a dataset can contain data from an Excel workbook on OneDrive, an on-premises SSAS tabular dataset, and/or a Salesforce dataset. There are many different data sources supported. Datasets added by one workspace member are available to the other workspace members with an *admin*, *member*, or *contributor* role.

#### Shared Datasets

***Business intelligence is a collaborative activity.*** It's important to establish standardized datasets that can be the 'one source of truth.' ***Expert data modelers can create and share optimized datasets, report creators can start with those datasets to build accurate reports.*** Your organization can have consistent data for making decisions, and a healthy data culture. To consume these shared datasets just choose Power BI datasets when creating your Power BI report.

### Reports

***A Power BI report is one or more pages of visualizations such as line charts, maps, and treemaps. Visualizations are also called visuals.*** You can create reports from scratch within Power BI, import them with dashboards that colleagues share with you, or Power BI can create them when you connect to datasets from Excel, Power BI Desktop, databases, and SaaS applications. For example, when you connect to an Excel workbook that contains Power View sheets, Power BI creates a report based on those sheets. And when you connect to a SaaS application, Power BI imports a pre-built report.

***There are two modes to view and interact with reports***: **Reading view** and **Editing view**. When you open a report, it opens in Reading view. If you have edit permissions, then you see Edit report in the upper-left corner, and you can view the report in Editing view. ***If a report is in a workspace, everyone with an admin, member, or contributor role can edit it.*** They have access to all the exploring, designing, building, and sharing capabilities of Editing view for that report. The people they share the report with can explore and interact with the report in Reading view.

***When you open a workspace, the associated reports are listed under the Reports tab. Each listed report represents one or more pages of visualizations based on only one of the underlying datasets.*** To open a report, select it. When you open an app, you are presented with a dashboard. To access an underlying report, select a dashboard tile (more on tiles later) that was pinned from a report. Keep in mind that not all tiles are pinned from reports, so you may have to click a few tiles to find a report.

### Dashboards

***A dashboard is a single canvas that contains zero or more tiles and widgets. Each tile pinned from a report or from Q&A displays a single visualization that was created from a dataset.*** Entire report pages can also be pinned to a dashboard as a single tile. 

**Use cases**:

- to ***see in one glance all the information needed*** to make decisions.
- to ***monitor the most-important information*** about your business.
- to ***ensure everyone is viewing and using the same information***.
- to ***create a personalized view of a larger dashboard*** and show all the metrics that matter to them.

***When you open a workspace, the associated dashboards are listed under the Dashboards tab***. To open a dashboard, select it. When you open an app, you will be presented with a dashboard. If you own the dashboard, you will also have edit access to the underlying dataset(s) and reports. If the dashboard was shared with you, you will be able to interact with the dashboard and any underlying reports but will not be able to save any changes.

### Template Apps

***The new Power BI template apps enable Power BI partners to build Power BI apps with little or no coding and deploy / publish them to any Power BI customer.*** As a Power BI partner, you create a set of out-of-the-box content for your customers and publish it yourself. You can build template apps that allow your customers to connect within their own accounts. As domain experts, they can unlock the data in a way that is easy for their business users to consume. ***Template apps are submitted to the Partner center to become publicly available in the [Power BI Apps marketplace](https://app.powerbi.com/getdata/services) and on [Microsoft AppSource](https://appsource.microsoft.com/?product=power-bi).*** 



Install a template app

------

1. In the nav pane in the Power BI service, select **Apps** > **Get apps**.

   ![Get Apps button](https://docs.microsoft.com/en-us/learn/modules/introduction-power-bi/media/get-apps-button.png)

2. In the Power BI apps marketplace that appears, select **Template apps**. All the template apps available in AppSource will be shown. Browse to find the template app you're looking for, or get a filtered selection by using the search box.

   ![Search in AppSource](https://docs.microsoft.com/en-us/learn/modules/introduction-power-bi/media/search-appsource.png)

3. When you find the template app you're looking for, click it. The template app offer will display. Click **GET IT NOW**.

   ![Template app offer](https://docs.microsoft.com/en-us/learn/modules/introduction-power-bi/media/template-app-offer.png)

4. In the dialog box that appears, select **Install**.

   ![Install app](https://docs.microsoft.com/en-us/learn/modules/introduction-power-bi/media/install-app.png)

The app is installed, along with a workspace of the same name that has all the artifacts needed for further [customization](https://docs.microsoft.com/en-us/power-bi/connect-data/service-template-apps-install-distribute#customize-and-share-the-app).

> ![!NOTE] If you use an installation link for an app that isn't listed on AppSource, a validation dialog box will ask you to confirm your choice.

> To be able to install a template app that is not listed on AppSource, you need to request the relevant permissions from your admin. See the [Template app settings](https://docs.microsoft.com/en-us/power-bi/admin/service-admin-portal#template-apps-settings) in Power BI admin portal for details.

When the installation finishes successfully, a notification tells you that your new app is ready.

![Go to app](https://docs.microsoft.com/en-us/learn/modules/introduction-power-bi/media/go-to-app.png)

## Data modeling and visualizations

When you launch Power BI Desktop, the **Getting Started** dialog box will appear, which provides useful links to forums, blogs, and introductory videos.

In Power BI Desktop, you will begin to build reports in the **Report** view. You will be working in five main areas:

![The five areas of Report view.](https://docs.microsoft.com/en-us/learn/modules/introduction-power-bi/media/power-bi-layout.png)

1. **Ribbon** - Displays common tasks that are associated with reports and visualizations.
2. **Report view, or canvas** - Where visualizations are created and arranged.
   1. The **Data view** allows you to view all of your data available in your report. This is an easy way to quickly check data types and validate data.
   2. The **Model view** allows you to visually set the relationship between tables or elements. A relationship is where two or more tables are linked together because they contain related data. This enables users to run queries for related data across multiple tables.
3. **Pages tab** - Located along the bottom of the page, this area is where you would select or add a report page.
4. **Visualizations pane** - Where you can change visualizations, customize colors or axes, apply filters, drag fields, and more.
5. **Fields pane** - Where query elements and filters can be dragged onto the **Report** view or dragged to the **Filters** area of the Visualizations pane.

### Visualizations in Power BI

Below are just some of the many different types of visualizations that can be added to Power BI reports, specified in Q&A, and pinned to dashboards.

- **Area charts** Basic (Layered) and Stacked, based on the line chart with the area between the axis and line filled in.

- **Bar and column charts** the standard for looking at a specific value across different categories.

- **Cards: Multi row / Single Number**

- **Pie charts** - show the relationship of parts to a whole.

- **Donut charts** - show the relationship of parts to a whole.

- **Gauge charts** - displays current status in the context of a goal.

- **KPIs** - Displays progress toward a measurable goal.

- **Line charts** - Emphasize the overall shape of an entire series of values, usually over time.

- **Maps** - associate both categorical and quantitative information with spatial locations.

- **Matrix** - makes it easier to display data meaningfully across multiple dimensions -- it supports a stepped layout. The matrix automatically aggregates the data and enables drill down.

- **Q&A visual** - lets you ask questions about your data using natural language.

- **Tables** - Work well with quantitative comparisons among items where there are many categories.

- **Treemaps** - charts of colored rectangles, with size representing value. They can be hierarchical, with rectangles nested within the main rectangles.

- **Waterfall charts** - show a running total as values are added or subtracted.

#### Custom visuals - AppSource

***Microsoft and community members contribute Power BI visuals for public benefit, and publish them to the [AppSource](https://appsource.microsoft.com/marketplace/apps?product=power-bi-visuals).*** You can download these visuals and add them to your Power BI reports. ***Microsoft has tested and approved these Power BI visuals for functionality and quality.*** AppSource connects millions of users of products such as Microsoft 365, Azure, Dynamics 365, Cortana, and Power BI, to solutions that help them get work done more efficiently and insightfully than before.

- By using Power BI visuals created with our SDK, you may be importing data from, or sending data to, third party or other services located outside of your Power BI tenant’s geographic area, compliance boundary, or national cloud instance.
- Power BI certified visuals are visuals in the AppSource meet certain specified code requirements that the Microsoft Power BI team has tested and approved. The tests are designed to check that the visual doesn't access external services or resources.
- Once Power BI visuals from AppSource are imported, visuals may be updated automatically without any additional notice.

### Filter data with Power BI

***Power BI offers several ways to filter and highlight reports***. Knowing how to filter data is the key to finding the right information. Filtering only applies to reports, not to dashboards.

#### Slicers

***A simple type of filtering that you can use is called a slicer***. ***Slicers provide cues to ways you can filter the results in the visuals on a report page. There are several different types of slicers: numeric, categorical, and date.*** Slicers make it easy to filter all the visuals on the page at once. To select more than one field, hold the Ctrl key and click additional fields.

### The Filters pane

***Another way to filter data is by opening and modifying filters in the Filters pane***. The Filters pane contains filters that were added to the report by the report designer. As a consumer, you can interact with the filters and save your changes but cannot add new filters. 

#### The four types of filters:

- **Report** – Applies to all pages in the report.
- **Page** – Applies to all the visuals on the current report page.
- **Visual** – Applies to a single visual on a report page. You only see visual level filters if you have selected a visual on the report canvas.
- **Drillthrough** – Allows you to explore successively more detailed views within a single visual.

### Buttons in Power BI

***Using buttons in Power BI lets you create reports that behave like apps***, and thereby, create an engaging environment so users can hover, click, and further interact with Power BI content. ***You can add buttons to reports in Power BI Desktop and in the Power BI service***. When you share your reports in the Power BI service, they provide an app-like experience for your users.

### Transform data

***Power BI Desktop includes the Power Query Editor tool, which can help you shape and transform data so that it's ready for your models and visualizations.***

***Power BI visualization and modeling tools work best with columnar data.*** Even though Power BI can import your data from almost any source. Sometimes, your data won't be formatted in simple columns, which is often the case with Excel spreadsheets. After you've cleaned your data into a usable format, you can begin to create powerful visuals in Power BI. For more information, see [Tutorial: Combine sales data from Excel and an OData feed ](https://docs.microsoft.com/en-us/power-bi/desktop-tutorial-analyzing-sales-data-from-excel-and-an-odata-feed/).

### Aggregates in the Power BI service

***To mathematically combine values in your data is called aggregating.*** ***The result is an aggregate***.

When Power BI service and Power BI Desktop create visualizations, they may aggregate your data. Often the aggregate is just what you need, but other times you may want to aggregate the values in a different way. For example, a sum versus an average. There are several different ways to manage and change the aggregate Power BI uses in a visualization. First, let's take a look at data *types* because ***the type of data determines how, and whether, Power BI can aggregate it.***

#### Types of data

***At the most basic level, the data is either numeric or it isn't***. Power BI can aggregate numeric data using a sum, average, count, minimum, variance, and much more. The service can even aggregate textual data, often called *categorical* data. If you try to ***aggregate a categorical field by placing it in a numeric-only bucket*** like **Values** or **Tooltips**, Power BI will count the occurrences of each category or count the distinct occurrences of each category. Special types of data, like dates, have a few of their own aggregate options: earliest, latest, first, and last.

#### Ways to aggregate your data

- **Sum**; **Average**; **Minimum**; **Maximum**; **Standard deviation**; **Variance**; **Median**
- **Do Not Summarize**. With this option chosen, Power BI treats each value in that field separately and doesn't summarize them. Use this option if you have a numeric ID column that the service shouldn't sum.
- **Count (Not Blanks).** Counts the number of values in that field that aren't blank.
- **Count (Distinct).** Counts the number of different values in that field.

## Security and administration

### Security

***Power BI is built on Azure which ensures the same level of security for Power BI as other Microsoft services.*** Users sign in with their credentials held in Azure Active Directory and control the level of sharing for every report, data or dashboard, determining whether recipients can edit or only view items.

***It's important to note that users are responsible for the data they share***. If a user connects to data sources using their credentials, they can share a report (or dashboard, or dataset) based on that data. Users with whom the dashboard is shared aren't authenticated against the original data source and will be granted access to the report. This is beneficial to allow users to share reports and dashboards they have created but does require responsibility on the user's part.

### Administration

***Power BI administration is the management of a Power BI tenant***, including the configuration of governance policies, usage monitoring, and provisioning of licenses, capacities, and organizational resources.  Power BI is designed for self-service business intelligence. ***The administrator is the guardian of data, processes, and policies in the Power BI tenant.*** A Power BI administrator is a key member of a team that includes BI developers, analysts, and other roles. The administrator can help support an organization to make sure that critical goals are met.

## Summary

1. Microsoft Power BI is a collection of software services, apps, and connectors that work together to turn your unrelated sources of data into coherent, visually immersive, and interactive insights.
2. Leveraging Power BI and other Microsoft technologies can lead to significant returns in terms of not only revenue, but your business users' ability to make beneficial decisions.
3. Power BI is built on Azure, Microsoft's cloud computing infrastructure and platform, ensuring your data is secure and only accessible by authenticated users.

## Resources

### Security and administration

- [Security Documentation](https://docs.microsoft.com/en-us/power-bi/service-admin-power-bi-security)
- [Power BI Security Whitepaper](https://docs.microsoft.com/en-us/power-bi/whitepaper-powerbi-security)
- [Administration Documentation](https://docs.microsoft.com/en-us/power-bi/service-admin-administering-power-bi-in-your-organization)

### More on Power BI

- [Power BI Documentation](https://docs.microsoft.com/en-us/power-bi/)

