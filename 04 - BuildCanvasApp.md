# PL-900 Canvas Apps

## Basic Elements

### Power Apps Studio

Power Apps Studio is the name of the web interface you use to build your app. Everything is done from the browser by logging into [https://make.PowerApps.com](https://make.powerapps.com/).

### App format

The first step in creating your app is to choose the format of your app: Mobile or Tablet. While both formats can be used interchangeably on a mobile device, a tablet, or a computer, each has different defaults around sizing of the screens and controls. Once you choose the format for an app, you cannot change it.

### Galleries

The Gallery control is used to display rows from a table of data. The display of a row is then defined by a template, which you can customize to meet your needs. Power Apps will then apply this template automatically to every row in your data.

### Forms

Forms are focused on working with a specific record, often based on a selection from a gallery. In this experience, a user browses a gallery to find and select the desired row to view the details on the form. Forms enable a user to not only view detailed information, but to save new records and edit existing ones. The various actions performed with forms are controlled by form modes allowing the form to serve many purposes.

### Input Controls

To allow you maximum flexibility in customizing your apps, Power Apps has a large selection of Input controls. Text inputs, buttons, dropdowns, toggles, date pickers, and sliders are a few examples. You can add these controls to galleries, forms, and screens to build a functional and aesthetic experience for your app. All inputs have a multitude of settings for default data, formatting, and actions which allow you to build an app that has the right user experience for your business process.

### Intelligent Controls

In addition to common inputs as covered above, Power Apps also provides a rich set of controls for more advanced operations. There are hardware-based controls which allow access to the camera, bar code scanner, GPS, and more hardware features. There are also service backed controls like the business card reader or object detector which allow you to add artificial intelligence to your app without writing code.

### Functions

Functions are the glue that binds all these controls, inputs, and data sources together. You can use one or more functions to create formulas in your apps. These formulas are similar to the language you use in Excel and can be used for actions such as sending data to a data source, formatting information, creating animations, and more. No complicated code is necessary, simply powerful functions with straightforward inputs to enhance your app.

## Build the App

Tutorial

## Functions in Power Apps

When using Microsoft Power Apps, you don't have to write complicated application code the way that a traditional developer does. However, you must express logic in an app and control its navigation, filtering, sorting, and other functionality. This is where formulas come in.

If you've used Microsoft Excel functions, you'll be comfortable building apps in Power Apps. To create a formula, you will combine one or more formulas with the required and optional parameters. Here are some common functions and an explanation of what they do:

- **Filter** - This function is often used with galleries or tables of data to narrow down the rows returned from your data source. You do this by specifying one or more columns in your data set to perform a logic test on, which will allow you to return data that falls in a certain date range, has a set value, or was created by the user for example.
- **Match** - This function allows you to check a value to see if it follows a given pattern. You can use this to check if the user entered a properly formatted email address and, if they did not, show them a warning that a valid email is required. This function serves well for conditional formatting.
- **Distinct** - This function allows you to return the unique values from a list of data, making it easier to build dynamic dropdowns that show users only the valid values for the given column.
- **Math functions** - Power Apps includes a range of math formulas for working with your data from the simple such as Sum or Average to the complex such as Atan and Sin to work with radians.

This is a small sampling of the large library of Power Apps functions that are available. Also, remember you can combine functions into one formula to solve complex problems. This is the power of the platform. You start with simple formulas and then as your comfort grows you learn to combine them.

For a complete list of all of the functions available in Power Apps, check out the documentation [here](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/formula-reference#s). To learn more about using formulas, check out the Microsoft Learning Path - Use basic formulas to make better Power Apps canvas apps.

## Sharing an App

Now that you've created an app, you can share it with specific users, groups, or your whole organization. When you share an app with other people, they can run it in a browser, or in the players for Apple iOS and Google Android.

Even better, you can give someone permission to update the app.

Sharing your app is your final step as an app creator. You will want to share the app to test the full functionality with some stakeholders. This will give them a chance to provide feedback and help you become a better app creator.

### Prepare to share an app

To complete the following steps, open the app that you want to share in Edit mode.

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

### Permissions and licensing

There is some basic information about permissions and licensing of which you should be aware:

- Users and contributors need permissions to any data connections and gateways that a shared app uses.
- Some permissions come implicitly with the app, but you must explicitly grant others.
- If you create an app based on Microsoft Dataverse, you must also ensure that the users with whom you share the app have the appropriate permissions for the table or tables on which the app relies. Specifically, those users must belong to a security role that can perform tasks such as creating, reading, writing, and deleting relevant rows.
- In many cases, you'll want to create one or more custom security roles with the exact permissions that users need to run the app. You can then assign a role to each user as appropriate.

Sharing an app is simple, and it's a great way to make an app that you find useful available to people across your organization.

 