# PL-900 Portals

***Portals are websites that allow internal and external audiences to view and interact with data from Dataverse or Dynamics 365 with a branded, personalized, self-service experience.*** 

Portals also allow you to set authentication requirements, customize data for each user, and allow users to submit their information privately with straightforward admin controls. Portal capabilities empower online consumers who prefer to find answers on their own through self-service and community options. Portals help you provide an organized, searchable knowledge base to deliver consistent, up-to-date answers and community experience for peer-to-peer support and direct interaction with your subject matter experts. Additionally, portals provide simple navigation with seamless transitions between self and assisted support. Consider a scenario where your business is already using Power Apps. 

**Portals can deliver:**

- **Provide self-service support** - When your business is growing, rather than having to employ extra staff in call centers, you could use Power Apps portals to add self-service capabilities to your website so that your customers can search knowledge articles, engage with other customers, find answers, and create support cases when needed (that go directly into Dynamics 365 Customer Service), all without a single interaction from your resources.
- **Build a sales pipeline** - When a lead fills out a Contact Us form on your company website, this information is recorded in Dynamics 365 Sales where the record can become part of your sales pipeline automatically.
- **Empower employees** - When an employee needs a new computer, they can fill out an online form, where the information will be recorded in Dataverse so the helpdesk staff can immediately access and process this information.
- **Engage mobile workforce** - Empower agents on any device, wherever they work. Field technicians can process and complete work orders in the field, instantly updating Dynamics 365 Field Service.

***All the differentiating features of model-driven apps are the features of portals as well, including:***

- Centralized management
- Common Data Model
- Roles and permissions
- Forms and views
- Business rules
- Declarative workflows and actions
- Plug-in architecture
- Integration with other services
- Microsoft Dataverse extensibility
- Audit

## Getting Started

***Businesses that have Dynamics 365 or a Dataverse solution already in place can quickly build portals and build their entire website without requiring developers.*** A portal is not automatically provisioned when a new Dataverse environment is created. You will need to provision a Power Apps portal and determine the name, default URL, language, and template.

> **Important**
>
> To provision a portal, you must be assigned the System Administrator role of the Microsoft Dataverse environment that is selected for the portal.

### Templates

***When provisioning a Power Apps portal, the most important choices to consider are the audience, workload, and choosing a specific portal template that would best align with the business requirements***. 

**Portal templates:**

- **Community portal** - ***Partner, Customer*** - ***Community features such as forums, ideas, blogs, and case management.***

- **Customer self-service portal** - ***Partner, Customer*** - ***Users can search knowledge articles, submit cases, and participate in discussion forums to resolve issues.***

- **Employee self-service portal** - ***Allow employees to access a centralized knowledge article and to submit cases***.

- ***Partner portal** - **External partners can manage and collaborate on accounts and opportunities.*** 

- **Customer portal** - ***Access to Supply Chain Management data by using dual-write Dataverse tables and is for Enterprise B2B***

- **Portal from blank** - ***Solution for unique scenarios where the other templates are not a good fit. Can be configured to address a variety of requirements.*** ***If D 365 apps is NOT enabled this is the only option.*** If Portal from blank is provisioned within a Dataverse environment, specific features from the other portals can be incorporated into the portal later. 

### Provision a portal

***Only one portals can be provisioned for each Dataverse environment.***

<details>
 <summary>Steps to provision a starter portal</summary>

1. Go to [https://make.powerapps.com](https://make.powerapps.com/).
2. Select a target environment by using the environment selector in the upper-right corner.
3. On the left menu, select **+ Create**.
4. Select **Portal from blank**. If you have Dynamics 365 apps deployed in your Microsoft Dataverse environment, additional portal templates, such as Customer self-service, will be available.
5. Provide a name for the portal.
6. Provide a unique address (URL) for the portal.
7. Select the language.
8. Select **Create** to start the portal provisioning process. After portal provisioning has completed, the portal will appear in the list as an app of type Portal.
9. Select the ellipsis (**...**) next to the portal app name and then select **Browse** to open the portal website.
</details>

## Core Components

This section describes the core components

### Power Apps portals Studio

***Power Apps portals Studio is used to create and customize the website. It contains various options to add and configure webpages, components, forms, and lists.***

<details>
 <summary>Anatomy of Power Apps portals Studio</summary>

![Power Apps portals studio](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/power-apps-portals-studio.png) Power Apps portals Studio components:

1. **Command bar** - Allows you to:
   - Create a webpage.
   - Delete a component.
   - Sync Configuration - synchronizes the latest portal configuration changes in Microsoft Dataverse database with your current Studio session. For example, use Sync Configuration to reflect the changes in Studio when using the Portal Management app to change the configuration of pages, forms or any other objects.
   - Browse website - clears the portal cache and opens the current portal page.
2. **Toolbelt** - Allows you to:
   - View and manage webpages
   - Add components
   - Edit templates
3. **Canvas** - Contains components that build a webpage.
4. **Footer** - Displays autosave status and allows you to open-source code editor.
5. **Properties pane** - Displays properties of webpage and selected components and lets you edit them as required.
</details>

### Webpages

***Most of a portal's content is represented by webpages***. A webpage is a document that is identified by a unique URL in a website. Through parent and child relationships to other webpages, webpages form the hierarchy of a website, that is, its site map. Webpages can be added and edited by using the Portal Studio, the portal front-side editor, or directly in Microsoft Dataverse by using the Portal Management app.

### Page templates

***Page templates are the blueprint for displaying the content of a webpage located at an exact URL.***

### Content snippets

***Content snippets are reusable fragments of editable content that can be placed within a web template***. Using snippets allows for targeted editing of parts of a page without affecting the overall content. Content snippets can include plain text, HTML layout, or template processing instructions, which helps enable dynamic content. 

<details>
 <summary>Mobile Header Snippet</summary>
In the example below, **Mobile Header** is a content snippet that can be updated with your company’s logo to quickly and easily tailor the portal to your needs.

![Title content snippet](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/content-snippets.png)

Snippets can be edited by using Portal Studio and Microsoft Dataverse rows by using the Portal Management app. Here is where you would replace the image source in the **Value** column with your company's logo.

![Edit Title content snippets](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/edit-title-content-snippet.png)

</details>


### Table lists and table forms

***The strength of portals is the ability to interact with information and data that is stored in Dataverse. Table lists and table forms are used in portals to define what data should be rendered.*** Such as a list of rows from a table or a form to capture and display data for a specific row.

***A webpage row can be linked to a "table list" or a "table form". The linked list or form will be used by the template to render the page layout with data from Dataverse***, such as a list of all *Active Contacts* to form the above *Member Directory* list. 

***"Table lists" can include functionality like filtering, sorting, and also actions associated with them to enable Create/Edit/Read abilities and to trigger workflows.*** With this, App Makers can determine what will happen when a user opens a row from a list, such as taking them to a form displaying the details of the selected row.

## Themes

***In portals by default the "Enable basic theme feature" is disabled - set to "Off". When you turn on this feature, you can use default themes called Presets. Create copies of the preset themes for additional customization.***

<details>
 <summary>Enabling a Theme</summary>

1. Sign in to Power Apps by navigating to make.powerapps.com

2. Select **Apps** from the left navigation pane, and then select your portal.

   ![Select Apps and a portal](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/select-portal.png)

3. Select **More Commands (...)**, and then select **Edit**.

   ![Edit a portal](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/edit-portal.png)

4. Select Themes from the left navigation pane, and then turn on the Enable basic theme toggle.

   ![Enable basic themes](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/enable-basic-theme.png)

</details>

### Changing Themes

***Any existing theme in your portal can be set to be the default theme.***

<details>
 <summary>How to set a theme</summary>

1. Sign in to Power Apps by navigating to make.powerapps.com

2. Select **Apps** from the left navigation pane, and then select your portal.

3. Select **More Commands (...)**, and then select **Edit**.

4. Select **Theme** from the components pane.

   ![Select theme icon](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/edit-theme.png)

5. Select any default theme from the available presets (in this example, we selected Blue).

   ![Select a default theme](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/choose-theme.png)

The selected theme is applied to your portal.

</details>


### Create a new theme

***It is also possible to create a new theme.***

<details>
 <summary>Guide to Create a new Theme</summary>

1. Sign in to Power Apps by navigating to make.powerapps.com

2. Select **Apps** from the left navigation pane, and then select your portal.

3. Select **More Commands (...)**, and then select **Edit**.

4. Select **Theme** from the components pane.

5. Select **New Theme**.

   ![Create a new theme](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/create-new-theme.png)
</details>

### Edit theme details

***It is possible to edit the theme name, description, color, and other typography settings.***

<details>
 <summary>Editing a Theme</summary>

1. Sign in to Power Apps by navigating to make.powerapps.com

2. Select **Apps** from the left navigation pane, and then select your portal.

3. Select **More Commands (...)**, and then select **Edit**.

4. Select **Theme** from the components pane.

5. Select the theme that's currently applied or select a new theme from the presets. Selecting a theme opens the details pane on the right side of your workspace.

   ![Theme details](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/theme-details.png)

6. Edit theme details such as name, description, and color for different areas.

7. Save and publish the changes.

</details>

## Security

***Portals users are tracked in Dataverse as contacts. All interactions and actions are tied to that contact row.*** The Portal Management model-driven app provides access to the contact table and has forms to manage passwords, view portal-specific contact information, and provide registration and profile management forms for the portal. 

### Authentication

***Administrators can choose to enable or disable any combination of authentication options through "portal Authentication Settings"***.

**Portal users can authenticate by using the following methods:**

- **Local authentication** - ***Authentication with usernames and passwords stored in the Dataverse contact row***.
- **External authentication** - ***Credentials and password management are handled by other identity providers.*** 
  - OAuth2 (Microsoft, Twitter, Facebook, Google, LinkedIn, Yahoo)
  - Open ID (Azure Active Directory, Azure Active Directory B2C)
  - WS-Federation and SAML 2.0 (used for integration with on-premises Active Directory and other identity services)

> **Important**
>
> Azure Active Directory B2C is the recommended identity provider for authentication. If another provider support is required, then it can be configured in Azure Active Directory B2C.

### Authorization

***After authentication, "portals" use numerous tables to define authorization. Web roles allow an administrator to control user access to portal content and Dataverse rows. A contact might be assigned to one or more web roles at a time. In that case access rules and permissions of individual roles are combined.*** One of the web roles in the portal can be marked as "*Anonymous*" and all of the others are "*Authenticated*". If a user is not signed in, they will view the portal with the Anonymous web role permissions, which should be the most restrictive permissions.

**A web role can be associated with the following table rows:**

- **Website permissions** - ***Define the (if any) front-side editing permissions.***
- **Webpage access rules** - ***Define what pages are visible to a role and what actions can be taken.***
- **Table permissions** - ***Define what access a role has to individual Dataverse tables.***



