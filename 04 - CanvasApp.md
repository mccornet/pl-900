# PL-900 Canvas Apps

***Canvas apps are used to make Mobile or Tablet focused applications.*** 

### Basic Elements

- **Power Apps Studio** - [https://make.PowerApps.com](https://make.powerapps.com/).

- **App format** - **Mobile or Tablet.**

- **Galleries** - ***The Gallery control is used to display rows from a table of data defined by a customizable template.*** Power Apps will then apply this template automatically to every row in the data.

- **Forms** - ***to work with a specific record: viewing and editing existing ones or, saving new records.***. 

- **Input Controls** - ***Such as text inputs, buttons, dropdowns, date pickers; with settings for default data, formatting, and actions.***

- **Intelligent Controls** - ***For more advanced operations:  *Hardware-based controls* allow access to  hardware features. *Service backed controls* make it possible to add AI***

  > Knowledge check
  >
  > "The barcode scanner control is a part of the Media category of controls."

- **Functions** - ***Based on the Excel language, to binds actions, controls, inputs, and data together***

## Building an App

**The basic steps:**

- ***Identify a business need.***
- ***Connect to any necessary data***.
- ***Design the app.***
- ***Save and publish the app and test functionality.***
- ***Share the app.*** 

-----

<details>
 <summary>Tutorial to Build an App</summary>

>### Connect to a data source
>
>1. Download the [Contoso-Site-Tracking.zip](https://github.com/MicrosoftDocs/mslearn-build-app-solution/raw/master/downloads/Contoso-Site-Tracking.zip) file, extract all of the files, and save them to your OneDrive for Business.
>
>2. Go to [https://make.powerapps.com](https://make.powerapps.com/) and sign in with your organizational account.
>
>3. In the left pane, select **Create**.
>
>4. In the **Start from data** section, select **Other data sources**.
>
>5. Under Connections, choose **OneDrive for Business**. If you don't have the connection available, click **New connection** to create one.
>
>6. For **Choose an Excel file** on the right select the **Contoso Site Tracking.xlsx** file.
>
>7. For **Choose a table** click **SiteInspector** and click **Connect**.
>
>   <img src="https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/site-inspector.png" alt="App published view" style="zoom:25%;" />
>
>Power Apps generates the app by inspecting your data and matching it with Power Apps capabilities so that you get a working app as a starting point. Generated apps are always based on a single list or table, but you can add more data to the app later.
>
>### Explore the generated app
>
>Your new three-screen app now opens in Power Apps Studio. The following figure shows the main development window for Power Apps Studio.
>
>[![App editor view](https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/power-apps-edit.png)](https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/power-apps-edit.png#lightbox)
>
>Select Play ![Start app preview arrow](https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/forward-arrow.png) in the upper-right corner to practice using the app. Notice that it includes all the data from the table and provides a good default experience. All apps that are generated from data have the same set of screens that you can view from the Screens pane:
>
>- **Browse screen** - This screen appears by default. In it, you can browse, sort, search, and refresh the data from the data source. In the browse screen, you can add items to the data source by selecting the plus sign (**+**).
>- **Details screen** - The details screen shows all information about a single item. In this screen, you can open an item to edit or delete it.
>- **Edit/create screen** - In this screen, you can edit an existing item or create a new one.
>
>Close out of preview mode by selecting the "X" in the upper-right corner. To make your app visible on the phone, it needs to be saved. Select **File**, **Save as**. Replace the current title "App" with **Contoso Site Tracking app**, and then select **Save**. You will see a green check mark when all changes are successfully saved. You can now open the app on your phone.
>
>### Install the app on your device
>
>To see how the app runs on mobile, install the Power Apps Mobile app on your phone. 
>
>1. Download Power Apps Mobile 
>2. Sign in 
>3. On your phone or tablet, run the **Contoso Site Tracking app** in Power Apps Mobile.
>
>### Customize the app
>
>While the default screens make a useful app out of the box, customize a generated app to suit your needs. To improve the layout, use the following procedure:
>
>1. On the Screens pane on the left, select **BrowseGallery1**. The selection box around the gallery confirms your choice.
>
>   <img src="https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/browse-screen.png" alt="Browse screen" style="zoom:25%;" />
>
>2. On the right pane, open the **Data** pane by selecting the drop-down menu next to **Layout**.
>
>   <img src="https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/layout-templates.png" alt="Layout templates" style="zoom:25%;" />
>
>3. Select the layout **Image, title, and subtitle** for a cleaner look.
>
>4. Select the **Address** of the item at the top of the gallery.
>
>   <img src="https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/power-apps-text-edit-view.png" alt="Text edit view" style="zoom:25%;" />
>
>5. Change **ThisItem.Address** to **ThisItem.Title** in the formula bar.
>
>6. Repeat the previous two steps, but change the other **Label** control to show the description of each item by setting it to **ThisItem.Description**.
>
>   <img src="https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/power-apps-text-preview.png" alt="Text edit confirmed preview" style="zoom:25%;" />
>
>### Add an additional data source
>
>Sometimes when creating a canvas app, you need to combine data from multiple data sources. Follow these steps to add Office 365 Outlook as an additional data source. 
>
>1. Select **View** > **Data sources** to open the **Data** pane.
>
>2. Select **Add Data**.
>
>3. In the search bar, type or paste the first few letters of **Office 365 Outlook:**
>
>   <img src="https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/canvas-app-outlook.png" alt="Office 365 Outlook in data sources list" style="zoom:25%;" />
>
>4. Select **Connect**, and if prompted to sign in, enter your work account.
>
>See this documentation for the types of commands you can do with the **Office 365 Outlook** connector: [/connectors/office365/](https://docs.microsoft.com/en-us/connectors/office365/)
>
>### Details screen
>
>On the details screen, change the order of the fields. The controls on this screen differ from the controls on the browse screen, so the process for changing them is also slightly different.
>
>1. On the Tree view on the left, select **DetailScreen1 > DetailForm1**. This will change the screen shown in the studio.
>
>2. On the right pane, select **Edit fields**.
>
>   [![Detail edit form](https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/detail-edit-form.png)](https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/detail-edit-form.png#lightbox)
>
>3. Click the **+ Add field** button at the top of the Fields section.
>
>4. Here you can add any of the data source fields that were not added by default. Check the box next to **Title** and **SubTitle** and click **Add**.
>
>5. Now you can rearrange the order by **clicking and holding on Title** and then **dragging** it to the **top** of the screen.
>
>6. You can also remove fields that you don't want to display to the users like the ID column. From the list of Fields click **ID** to expand it, click the **…**, and choose **X Remove**.
>
>   ![field edit form view](https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/field-edit-form-view.png)
>
>### Edit/create screen
>
>On the screen where your users edit and create entries, you want to make it easier for them to enter information in a text box.
>
>1. On the Tree view on the left, select **EditScreen1 > EditForm1**.
>
>2. On the right pane, select **Edit fields**.
>
>3. Expand **Description**. Select the drop-down arrow for the **Control type** and then select **Edit multi-line text**.
>
>   <img src="https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/control-text-edit-options.png" alt="Control text edit options" style="zoom: 50%;" />
>
>4. A multi-line edit control will simplify your user's ability to add more than a few words in this field. You could also reorder the fields to match the order from the Details screen to give the user a more consistent experience.
</details>

-----

## Controls in Power Apps

***A control is a UI element that produces an action or shows information***. Many controls in Power Apps are similar to controls that you've used in other apps: labels, text-input boxes, drop-down lists, navigation elements, and so on. In addition to these typical controls, Power Apps has more specialized controls, which you can find on the Insert tab.

<p align="center">
	<img src="https://docs.microsoft.com/en-us/learn/modules/build-app-solution/media/control-type-list.png" alt="Control type list" width="750px" />
</p>

### A few controls:

- **Galleries** - ***layout containers that hold a set of controls that show rows from a data source.***
- **Forms** -  ***show details about the data and allows creation and editing of records***.
- **Media** - ***add background images, include a camera button, a barcode reader, and more.***
- **Charts** - ***add charts to allow instant analysis***.

## Functions

***Formulas are used to express logic in an app and control its navigation, filtering, sorting, and other functionality. It is possible to combine one or more formulas with the required and optional parameters***. 

### Common Functions

- **Filter** -  ***narrow down the rows by specifying column(s) to perform a logic test on***.
- **Match** - ***Check if a value follows a given pattern; serves well for conditional formatting.***
- **Distinct** -  ***return the unique values from a list of data***
- **Math functions** - ***Math formulas like in Excel***

A complete list of all of the functions available can be found [here](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/formula-reference#s). 

## Sharing an App

***Sharing the app is the final step as an app creator. Share the app to test the full functionality with some stakeholders***. This will give them a chance to provide feedback. When you share an app, they can run it in a browser, or in the players for Apple iOS and Google Android. It is  possible to give someone permission to update the app.

-----

<details>
<summary>Tutorial to Share an App</summary>

**To share an app** complete the following steps, open the app that you want to share in Edit mode.

1. In Power Apps Studio, select the **File** menu and then select **Save as** and then select **The cloud**.

2. Click **Save** in the bottom right corner.

3. After the app is successfully saved click **Share**.

4. On the Share tab, specify the users or groups with whom you want to share the app. To add everyone in your organization, type Everyone and select **Everyone** in **Company Name**. If you need to share with a large group of users, a best practice is to share through an Azure Active Directory Security Group.

   By default, the user receives the User permission. If you want the user to also be able to edit the app, then select the co-owner check box. The following is a description of both permissions:

   - **Co-owner** - Users can use, edit, and share the app, but can't delete or change the owner.
   - **User** - Users can view and use the app, but they can't change it.

5. Consider security groups.

   - If you share an app with a security group, existing members of that group and anyone who joins it will have the permission that you specify for that group. Anyone who leaves the group loses that permission unless they belong to a different group that has access or if you give them permission as an individual.
   - Every member of a security group has the same permission for an app as the overall group does. However, you can specify greater permissions for one or more members of that group to allow them greater access. For example, you can give Security Group A permission to run an app, but you can also give User B, who belongs to that group, Co-owner permission. Every member of the security group can run the app, but only User B can edit it. If you give Security Group A Co-owner permission and User B permission to run the app, User B can still edit the app.

6. To notify users by email, leave the **Send an email invitation to new users** check box selected.

   If you select to notify the users by email, everyone you shared the app with will receive an email message that has a link to the app. People whom you granted Co-owner permission for the app will also receive a link to Edit App in Power Apps Studio.

7. Click **Share**.

   If you make and save changes to a shared app, the people whom you shared it with will see your changes as soon as you publish them. This can be useful if you improve the app, but it can also negatively affect users if you remove or significantly change features. Remember to create a notification plan for alerting your users of major updates.


</details>

-----

### Permissions and licensing

**Some basic information about permissions and licensing:**

- Users and contributors need permissions to any data connections and gateways that a shared app uses.
- Some permissions come implicitly with the app, but you must explicitly grant others.
- If you create an app based on Microsoft Dataverse, you must also ensure that the users with whom you share the app have the appropriate permissions for the table or tables on which the app relies. Specifically, those users must belong to a security role that can perform tasks such as creating, reading, writing, and deleting relevant rows.
- In many cases, there is a need to create one or more custom security roles with the exact permissions that users need to run the app. 



 