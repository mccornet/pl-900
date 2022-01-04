# PL-900 Portals

Power Apps portals provide a great way to allow internal and external audiences to view and interact with data from Microsoft Dataverse or Dynamics 365 with a branded, personalized, self-service experience. Portals also allow you to set authentication requirements, customize data for each user, and allow users to submit their information privately with straightforward admin controls.

Portal capabilities empower online consumers who prefer to find answers on their own through self-service and community options. Portals help you provide an organized, searchable knowledge base to deliver consistent, up-to-date answers and community experience for peer-to-peer support and direct interaction with your subject matter experts. Additionally, portals provide simple navigation with seamless transitions between self and assisted support.

Consider a scenario where your business is already using Power Apps. The following are additional capabilities that Power Apps portals can deliver:

- **Provide self-service support** - When your business is growing, rather than having to employ extra staff in call centers, you could use Power Apps portals to add self-service capabilities to your website so that your customers can search knowledge articles, engage with other customers, find answers, and create support cases when needed (that go directly into Dynamics 365 Customer Service), all without a single interaction from your resources.
- **Build a sales pipeline** - When a lead fills out a **Contact Us** form on your company website, this information is recorded in Dynamics 365 Sales where the record can become part of your sales pipeline automatically.
- **Empower employees** - When an employee needs a new computer, they can fill out an online form, where the information will be recorded in Dataverse so the helpdesk staff can immediately access and process this information.
- **Engage mobile workforce** - Empower agents on any device, wherever they work. Field technicians can process and complete work orders in the field, instantly updating Dynamics 365 Field Service.

Portals are built on top of Microsoft Dataverse. This architecture comes with a major benefit. All the differentiating features of model-driven Power Apps are the features of Power Apps portals as well, including:

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

Businesses that have Dynamics 365 or a custom Microsoft Dataverse solution already in place can quickly build portals that are more secure and build their entire website, all without requiring developers. A portal is not automatically provisioned when a new Dataverse environment is created. You will need to provision a Power Apps portal and determine the name, default URL, language, and template.

> **Important**
>
> To provision a portal, you must be assigned the System Administrator role of the Microsoft Dataverse environment that is selected for the portal.

### Templates

When provisioning a Power Apps portal, the most important choices to consider are the audience, workload, and choosing a specific portal template that would best align with the business requirements. Several portal templates are available that can be provisioned. These templates will accelerate the configuration of portals based on the intended audience and workload.

If you are building a custom business application by using Microsoft Dataverse without Dynamics 365 apps enabled, your only choice is the **Portal from blank** option. If you are using Microsoft Dynamics 365 apps such as Dynamics 365 Sales or Dynamics 365 Service, you have a choice of five additional portal templates:

- **Community portal**

  Partner, Customer

  Choose this option to provision a portal that is focused on an online community. This portal will contain features such as forums, ideas, blogs, and case management.

- **Customer self-service portal**

  Partner, Customer

  This option provides the ability for portal users to search knowledge articles, submit cases, and participate in discussion forums to resolve issues.

- **Employee self-service portal**

  This portal allows employees to access a centralized knowledge article and to also submit cases.

- **Partner portal**

  Choose this option to build a portal where external partners can manage and collaborate on accounts and opportunities. Add-ons are available for Dynamics 365 Field Service or Dynamics 365 Project Service.

- **Customer portal**

  The Dynamics 365 Supply Chain Management Customer portal is a template that provides portal access to Dynamics 365 Supply Chain Management data by using dual-write Microsoft Dataverse tables and is meant for Enterprise B2B

- **Portal from blank**

  The **Portal from blank** option is meant for unique line-of-business scenarios where the other templates are not a good fit. The portal can be configured to address a variety of requirements. If **Portal from blank** is provisioned within a Microsoft Dataverse environment, specific features from the other portals can be incorporated into the portal later.

### Provision a portal

Only one Power Apps portals can be provisioned for each Microsoft Dataverse environment.

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

You can use Power Apps portals Studio to create and customize your website. It contains various options to add and configure webpages, components, forms, and lists.

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

Most of a portal's content is represented by webpages. A webpage is a document that is identified by a unique URL in a website. Through parent and child relationships to other webpages, webpages form the hierarchy of a website, that is, its site map. Webpages can be added and edited by using the Portal Studio, the portal front-side editor, or directly in Microsoft Dataverse by using the Portal Management app.

### Page templates

A webpage row does not define how the page looks when it is rendered on the portal. Instead, it is linked to the **Page template** row that defines the layout and the behavior. Think of the webpage as the exact URL and the Page template as the blueprint for displaying the content.

### Content snippets

Content snippets are reusable fragments of editable content that can be placed within a web template. Using snippets allows for targeted editing of parts of a page without affecting the overall content.

Content snippets can include plain text, HTML layout, or template processing instructions, which helps enable dynamic content. 

<details>
 <summary>Mobile Header Snippet</summary>
In the example below, **Mobile Header** is a content snippet that can be updated with your company’s logo to quickly and easily tailor the portal to your needs.

![Title content snippet](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/content-snippets.png)

</details>

Snippets can be edited by using Portal Studio and Microsoft Dataverse rows by using the Portal Management app. Here is where you would replace the image source in the **Value** column with your company's logo.

![Edit Title content snippets](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/edit-title-content-snippet.png)

### Table lists and table forms

The strength of Power Apps portals is the ability to interact with information and data that is stored in Microsoft Dataverse. Table lists and table forms are used in Power Apps portals to define what data should render on the portal from Microsoft Dataverse, such as a list of rows from a table or a form to capture and display data for a specific row.

![Account entity list](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/member-directory-entity-list.png)

A webpage row can be linked to a **table list** or an **table form**. The linked list or form will be used by the template to render the page layout with data from Microsoft Dataverse, such as a list of all *Active Contacts* to form the above *Member Directory* list. In the **Properties** pane on the right of the above example, you see that this table list was created to display the *Active Contacts* view from the *contacts* table.

Table lists can include functionality like filtering and sorting and can also have actions associated with them to enable Create/Edit/Read abilities and to trigger workflows. With this, App Makers can determine what will happen when a user opens a row from a list, such as taking them to a form displaying the details of the selected row.

![Configuring entity lists](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/configure-entity-lists.png)

In the above example, the App Maker has dictated that the user will be taken to the **Table Form** if they want to *create* or view *details* for a specific row from a list.

## Themes

In Power Apps portals, the **Enable basic theme** feature is set to **Off**. When you turn on this feature, you can use default themes called **Presets**. You can also create copies of the preset themes for additional customization.

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

You can set any existing theme in your portal to the default theme.

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

It is also possible to create a new theme

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

You can update theme name, description, color, and other typography settings in Power Apps Studio.

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

Users of Power Apps portals are tracked in Microsoft Dataverse as contacts. The Portal Management model-driven app provides access to the contact table and has forms to manage passwords, view portal-specific contact information, and provide registration and profile management forms for the portal. All interactions and actions that a portal user takes (for example, leaving a comment on a page) are tied to their contact row in Microsoft Dataverse.

### Authentication

Portal users can authenticate by using the following methods:

- **Local authentication** - Basic authentication with usernames and passwords are stored in the Microsoft Dataverse contact row internally.
- **External authentication** - Credentials and password management are handled by other identity providers. Supported authentication providers include:
  - OAuth2 (Microsoft, Twitter, Facebook, Google, LinkedIn, Yahoo)
  - Open ID (Azure Active Directory, Azure Active Directory B2C)
  - WS-Federation and SAML 2.0 (used for integration with on-premises Active Directory and other identity services)

Portal administrators can choose to enable or disable any combination of authentication options through portal **Authentication Settings**.

> **Important**
>
> Azure Active Directory B2C is the recommended identity provider for authentication. If another provider support is required, then it can be configured in Azure Active Directory B2C.

### Authorization

After the user is authenticated and associated with a contact, Power Apps portals use numerous tables to define authorization, that is, what a user is allowed to do. Selecting **Share** from the portal app options will provide information on how to share the portal app with internal and external users.

[![Portals security constructs](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/share-portal.png)](https://docs.microsoft.com/en-us/learn/modules/introduction-power-apps-portals/media/share-portal.png#lightbox)

**Web roles** allow an administrator to control user access to portal content and Microsoft Dataverse rows. A web role can be associated with the following table rows:

- **Website permissions** - Define what (if any) front-side editing permissions that a web role should have.
- **Webpage access rules** - Define what pages are visible to a web role and what actions can be taken.
- **Table permissions** - Define what access a web role has to individual Microsoft Dataverse tables.

A portal contact might be assigned to one or more web roles at a time. Access rules and permissions of individual roles are combined to determine the resulting permissions set.

One of the web roles in the portal can be marked as **Anonymous** and all of the others are **Authenticated**. These roles allow you to apply permissions and access rules to all portal users based on whether they are signed in. If a user is not signed in, they will view the portal with the Anonymous web role permissions, which should be the most restrictive permissions.

