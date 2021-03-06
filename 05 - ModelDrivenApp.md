# PL-900 Model Driven App

***Model-driven app design is a component-focused approach to app development that focuses on adding dashboards, forms, views, and charts; much of the layout is determined by the added components***. The emphasis is more on quickly viewing your business data and making decisions instead of on intricate app design.

## Making model-driven apps

***Building an app usually involves 3 steps.***

### 1. Model the Business Data

***To model business data, determine what data the app will need and how that data will relate to other data***. Model-driven design uses metadata-driven architecture so that designers can customize apps without writing code. Metadata means *data about data* and defines the structure of the data stored in Microsoft Dataverse.

### 2. Define the Business Processes

***Define and enforce a consistent business proces*** Consistent processes help ensure that users can focus on their work and not worry about having to remember to perform a set of manual steps. 

### 3. Build the app

***After modeling data and defining processes, the app is build by selecting and setting up the components in the App Designer***.

## Building blocks of model-driven apps

***A model-driven app consists of several components selected in the App Designer***. The components and component properties become the metadata. Let's look more closely at these components.

### Data

***There are different data components; created or edited using the Table designer; that determine what data the app will be based upon.*** 

- **Tables** - ***Items with properties***. Use standard tables or create a custom table.
- **Columns:** - ***properties with a data type that are associated with and define a table*** 
- **Relationships** -  ***how tables can be related to each other***. 
- **Choice** -  ***a column with a control to  select among predefined options***. 

### User interface

***UI components determine interaction with the app***

- **App** - ***App designer*** - ***App fundamentals, like components, properties, the client type, etc.***
- **Site map** - ***Site map designer*** - ***Specify the app navigation.***
- **Forms** - ***Form Designer*** - ***Include a set of data entry columns for a given table to create or edit data rows***. 
- **View** - ***View Designer*** - ***How a list of rows for a specific table appears in the app***.

### Logic Components

***The logic components determine the business processes, rules, and automation of the app***

- **Business process flows** -  ***Business process flow designer*** -  ***A standardized business process.***
- **Workflows** - ***Workflow designer*** - ***Uses for automation that does not require interaction.***
- **Actions** - ***Process designer*** - ***Manually invoked behaviors and custom actions.***
- **Business rules** - ***Business rule designer*** - ***Apply rules or recommendation logic to set field properties***. 
- **Flows** - ***Power Automate*** - ***Automate workflows between apps and services***

### Visualization Components

***These determine what type of data and reporting the app will show and have available*** 

- **Charts** -  ***Chart designer*** - ***Individual graphical visualizations for views, forms or dashboards.***

- **Dashboards** - ***Dashboard designer*** - ***Show one or more graphical visualizations in one place***

- **Embedded Power BI** - ***chart designer, dashboard designer, and Power BI*** - ***adds embedded Power BI tiles and dashboards*** 

## Design of model-driven apps

***The primary design goal is to get the data model in order. Created with App Designer, choose the components to include - like entities, dashboards, business process flows, forms, and others; and spend more time understanding what your user needs than how it is going to look***

-----

<details>
 <summary>App Designer Example</summary>

>Here is a quick look at the App Designer for an example Model-driven app called ???Fundraiser.??? As you can see, there are two tables: Donation and Fundraiser. Each table also contains four assets:
>
>- **Forms** ??? Defining how users will see and interact with the data
>- **Views** ??? A list view of the rows for each table
>- **Charts** - Showing the data in a meaningful, visual representation
>- **Dashboards** ??? Providing an insightful, graphical overview of the data
>
>[<img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/fundraiser-app-designer.png" alt="Model driven app layout in studio." width="500px" />](https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/fundraiser-app-designer.png#lightbox)
>
>By selecting the Play button in the top right, the app is put into **Play mode**. You can see it then looks completely different and shows the data based on the choices made in the design process.
>
>[<img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/app-play-mode.png" alt="Model driven app in play mode." width="500px" />>](https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/app-play-mode.png#lightbox)

</details>

-----

### Data model

***During the modelling process there are several things to consider***.

- ***The type of data the solution be storing and or collecting ***
- ***How will this data relate or coincide with the other data***

***These considerations are important because model-driven applications use a metadata-driven architecture; a large portion of the model-driven app is based on how the data is modeled***, ***When considering the data model, also consider data type as the data type will determine how users enter and view that data.***. 

> **Important**
>
> If a column needs to be changed to a different data type, (i.e. text column to a choice column), then you will need to delete that column and recreate with the correct data type. This will cause you to lose any data associated with that column.

-----

<details>
 <summary>Metadata Visual Example</summary>

>You can view the app metadata by reviewing the Table in Microsoft Dataverse.
>
>[<img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/entity-metadata.png" alt="Example of metadata." width="500px"/>](https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/entity-metadata.png#lightbox)
>
>You can also view the app **Play mode** to see a preview of what the app will look like.
>
>[<img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/entity-play-mode.png" alt="Example of app in play mode." width="500px"/>](https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/entity-play-mode.png#lightbox)
>
>In the example above, for the Fundraiser table, there are several pieces of data being collected, such as: Name, Fundraiser, Goal, Owner, Total Donations, Created On
</details>

-----

### Business Logic

***When incorporating business logic in your app, there are two primary options:  Business Rules  or Business Process Flows.***

**Business Rules,** - ***define behaviors at the data layer***. This is great for setting conditions for when a field is required, setting a default value, or even showing or hiding a field based on criteria. An example could be a table for tracking expenses. You could have a column for type of travel and then build a business rule that dictates that if a user chooses automobile then the mileage field is required, else it is optional. This gives you the power to make sure you maintain data consistency in all scenarios.

**Business process flows** -  ***guide users through using your app***. These workflows can provide visuals on next steps based on the status of the data and facilitate other actions that you want to occur as the user uses the app. Business Process Flows let you bring automation to your app and make it more of a guided experience than just a place to enter data.

### Dashboards

***A common output to visualize the data; use dashboards with custom filters and visual graphics to tie data together*** right in your app. When creating your dashboards, make sure they are simple for your users to consume without overwhelming them with all the data. Provide high-level snapshots of your data and allow them to use filters to dive deeper into the data if needed.

### Additional third-party solutions and app accelerators

It is also important to know about the different App accelerators and third-party solutions available Microsoft has released a number of accelerators or foundational components to assist you with quickly standing up your solution. For more information, see [Industry accelerators overview](https://docs.microsoft.com/en-us/common-data-model/industry-accelerators?azureportal=true).

## Create a model-driven app

In this unit, you will create a model-driven app by using one of the standard entities that is available in your Microsoft Power Apps environment.

-----

<details>
 <summary>Tutorial to Create a Model-Driven App</summary>

 1. Sign in to [Power Apps](https://make.powerapps.com/) by using your organizational account.

 2. Select the environment you want, or go to the [Power Apps admin center](https://admin.powerapps.com/) to create a new one.

 3. On the **Home** page, select **Model-driven app from blank**.

 4. Select **Classic App Designer** and click **Create**.

   <img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/model-driven-app-from-blank.png" alt="Model-driven" width="250x"/>

 5. On the **Create a New App** page, enter a name and description for the app.

 6. Select **Done**. Your new app appears in the App Designer, and you can now add components to it.

 ### Add components to your app

 You add components to your app by using the App Designer.

 1. Select the **Open the Site Map Designer** pencil icon to open the site map designer.

   [<img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/app-designer-configuration.png" alt="Create a new site map" width="500px" />](https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/app-designer-configuration.png#lightbox)

 2. In the site map designer, select **New Subarea**, and then, in the right pane on the **Properties** tab, select the following properties:

   - **Type**: *Entity*

   - **Entity**: *Account*

     [<img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/sitemap-designer.png" alt="Add components to the site map" style="zoom:50%;" />](https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/sitemap-designer.png#lightbox)

 3. Select **Save And Close**.

 4. In the App Designer, select **Forms**, and then, in the right pane under **Main Forms**, select the **Account** form.

   <img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/account-forms.png" alt="Account main form" width="250px" />

 5. In the App Designer, select **Views**, then select the following properties:

   - Active Accounts
   - All Accounts
   - My Active Accounts

 6. In the App Designer, select **Charts**, then select the **Accounts by Industry** chart.

 7. On the App Designer toolbar, select **Save And Close**.

 ### Create a form

 1. On the left navigation pane, expand **Dataverse**, and then select **Tables**.
 2. Select a table, such as the account table, and then select the **Forms** tab.
 3. Select **Add form**, and then select one of the following
   - **Main form** The contents of the new form are filled using the existing main form definition. If multiple main forms exist, the form at the top of the list in the form order is used to fill the new form.
   - **Quick create form**
   - **Quick view form**
 4. When you are done making changes to the form, select **Save** to save the form.

 ### Edit a form

 1. On the left navigation pane, expand **Dataverse**, and then select **Tables**.
 2. Select a table, such as the account table, and then select the **Forms** tab.
 3. Select the form name that you want to edit.
   - You can also select the row for a form, and then in the command bar, select **Edit form**
   - Another alternative is to select **...** next to the form name, and then in the menu, select **Edit form**.
 4. When you are done making changes to the form, select **Save** to save the form.

 ### Open and add a view in the app designer

 The following steps explain how to open and add a view in the app designer.

 1. In the app designer **Entity View** section, select **Views**.

   - In this example, we have selected **Views** from the **Account** table.

   [<img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/app-designer-add-view.png" alt="Account views" width="500px" />](https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/app-designer-add-view.png#lightbox)

 2. To add a view, select it by using view types such as Public, Advanced Find, Associated, and Lookup. The view is automatically added to the **Views** list.

 >   Note
 >
 >  Views are displayed based on the table that you have selected. For example, when you select Account, views that are related to the Account table are displayed.

 For more information about the app designer visit [Design custom business apps by using the app designer](https://docs.microsoft.com/en-us/powerapps/maker/model-driven-apps/design-custom-business-apps-using-app-designer)

 ### Add a column to your view in app designer

 Views display rows and columns in a table. Each row is a record with columns you add to the view.

 1. In app designer, select the entity view that you want and then on the right pane next to the view that you want select edit (pencil button).

 2. On the **Components** tab, select the **Column Attributes** list for either the **Primary Entity** or **Related Entity**.

   <img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/column-attributes.png" alt="Column Attributes" width="300px" />

 3. From the list, select the column you want and drag it to the column heading. You can also add the column by double-clicking it.

 4. Repeat step 3 until you have added all the columns you want to display in your view.

 As you add columns, you can drag them to any position among existing column headings. You can also move columns around after you add them to your view.

 For more detailed options on creating and editing views visit [https://docs.microsoft.com/powerapps/maker/model-driven-apps/create-edit-views-app-designer](https://docs.microsoft.com/en-us/powerapps/maker/model-driven-apps/create-edit-views-app-designer)


 ### Publish your app
 On the App Designer toolbar, select **Publish**. After you publish the app, it is ready for you to run or share with others.

 Above My Active Accounts, select **Show Chart**.

 If the sample data for your accounts does not have an Industry populated, go into a few accounts and add an Industry. Once you have updated a few accounts with an industry, the chart will update as well.

 [<img src="https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/account-charts.png" alt="Simple account entity app" width="500px" />](https://docs.microsoft.com/en-us/learn/modules/how-build-model-driven-app/media/account-charts.png#lightbox)

</details>

-----

## Controlling Security & Sharing

***Power Apps use role-based security for sharing. All app users must be assigned at least one security role. Roles can be assigned to individual users or to teams***. When a user or a team is assigned to a role, that user or all members of that team are granted the set of privileges associated with the role.

***To share an app, you must have the Environment Admin or System Admin role.***

### Create or set up a security role

***Power Apps environments include predefined security roles***. These roles reflect common user tasks, and the access levels that are defined follow the security best practice of providing access to the minimum amount of business data that is required to use the app. Security roles control a user's access to data through a set of access levels and permissions. The combination of access levels and permissions that are included in a specific security role sets limits on the user's view of data and interactions with that data. One or more security roles must be assigned to the app. The apps that users can use depend on the security roles they are assigned to. 

*** An appsbased on a custom table requires explicitly specified privileges***

- **Expand an existing predefined security role** so that it includes privileges for rows that are in the custom table.
- **Create a custom security role** to manage privileges for users of the app.

### Predefined Roles

***The following predefined roles are available with a Power Apps environment. Unless otherwise noted, all the privileges have global scope.***

- **Environment Maker** - Privileges: None

  ***This role can create new resources that are associated with an environment***, including apps, connections, custom application programming interfaces (APIs), gateways, and flows that use Power Automate. 

  ***But these users can't access the data*** in an environment. To learn more about environments, see [Announcing Power Apps environments](https://powerapps.microsoft.com/blog/powerapps-environments/).

- **System Administrator** - Privileges:  Create, Read, Write, Delete, Customize

  ***This role has full permission to customize or administer the environment***, including creating, changing, and assigning security roles. User who have this role can view all data in the environment. To learn more, see [Privileges required for customization](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/customize/privileges-required-customization)

- **System Customizer** - Privileges: Create (self), Read (self), Write (self), Delete (self), Customizations

  ***This role has full permission to customize the environment. But can view rows only for environment tables that they create***. To learn more, see [Privileges required for customization](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/customize/privileges-required-customization).

- **Microsoft Dataverse User** - Privileges: Read, Create (self), write (self), delete (self)

  ***This role can run an app in the environment and perform common tasks for the rows they own.***

- **Delegate** - Privileges: Act on behalf of another user

  ***This role lets code run as or impersonate another user; typically used with another security role to provide access to rows.*** To learn more, see [Impersonate another user](https://docs.microsoft.com/en-us/powerapps/developer/data-platform/impersonate-another-user).

### Share the link to your app

> **Note**
>
> Unlike sharing canvas apps, sharing model-driven apps does not currently send an email with a link to the app.

***Sharing a model-driven app involves two primary steps:***

1. associate one or more security role(s) with the app
2. assign the security role(s) to users.

------

<details>
<summary>Steps to Share an App</summary>

1. Select a model-driven app and click **Share**.

2. Select the app then choose a security role from the list.

3. Search for a user

4. Select the user, then select a role from the list.

5. Click **Share**.

6. Share the link to your app by following the steps below.

7. Edit the app and click the **Properties** tab

8. Copy the **Unified Interface URL.**

9. Paste the app URL in a location so that your users can access it, such as by posting it on a SharePoint site or sending via email.

</details>