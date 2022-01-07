# Power Automate

***Power Automate is used to automate repetitive processes***. Anyone with knowledge of the business process can create repeatable flows that when triggered leap into action and perform the process for them.

Beyond simple workflows, Power Automate can send reminders on past due tasks, move business data between systems on a schedule, talk to more than 275 data sources or any publicly available API, and can even automate tasks on your local computer like computing data in Excel. 

**Common scenarios:**

- ***Automate repetitive tasks*** like moving data from one system to another
- ***Guiding a user through a process*** so they can complete the different stages
- ***Connecting to external data sources*** via one of the hundreds of connectors or directly via an API
- ***Automating desktop based processes*** with robotic process automation (RPA) capabilities

***Power Automate flows are built with triggers and actions. Triggers determine what starts the flows, while actions determine what happens.***


<details>
<summary>Example: a purchase order approval</summary>

Approvals are a great process to build in Power Automate. They are often defined yet manual.  A user starts the process by going into a Power Apps app and creating a purchase order request. Once they submit the request, the information is sent to a Power Automate flow.

The flow can be built to evaluate the request and then route the request based on criteria such as submitting user and request amount. The first action could be to send the request to the user's manager. The manager could be automatically retrieved from Azure AD, avoiding prompting for duplicate information.

Here is the starting point of the flow: ![Flow edit form](https://docs.microsoft.com/en-us/learn/modules/introduction-power-automate/media/starting-point.png)

After the manager receives the approval and approves, the flow can then provide conditional logic. Typically, this might be something like: if the purchase order request is greater than $10,000, send it to VP; if not, then automatically approve the purchase order.

Here is an example of what this flow may look like. ![flowchart logic for support emails](https://docs.microsoft.com/en-us/learn/modules/introduction-power-automate/media/flow-example.png)

As you can see, even the business process has many decision points. The flow easily handles the decisions without you writing any code.
</details>

## Working with Data

***Power Platform supports multiple data connections allowing to use data from many platforms into a single automation using connectors***. Through these connectors easily ***connect to data and services across the web and even on-premises***. 

## Three types of flows

- **Event driven flows** - Flows that ***contain a trigger and then one or more actions***. There are a multitude of triggers and actions available, thanks to the existing connectors. ***There are My flows and Team flows.*** ***The difference between a My flow and a Team flow is ownership***. With a My flow you are the sole owner, while a Team flow has more than one owner.
- **Business process flows** - Used to create a ***guided experience in Model-driven apps***.
- **Desktop flows** - These **robotic process automation** (RPA) flows allows to ***record actions on a desktop*** or within a web browser. Then ***trigger a flow to perform that process***. ***It is possible to pass data in or get data out of the process***, letting you automate even "manual" business processes.

## Add Artificial Intelligence

***Add AI with a*** ***wizard-based interface for building and training the model***. ***This uses Azure Machine Learning and Cognitive services*** without writing a single line of code. To take advantage of these AI capabilities first build a model. 

### Four AI models

- **Form processor** - This model ***extracts text from an image*** or taken photo.
- ***Object detector*** - This model ***identifies and counts objects*** in an image
- **Prediction** - This model ***predict a yes or no outcome based on historical data***. 
- **Text classification** - This model ***categorizes text by its meaning***, making it is easier to analyze.

### The prediction model

***The prediction model is a model that can predict a yes or no outcome based on historical data.*** Train the model by providing historical data which includes the yes/no outcome and then artificial intelligence does the rest. You can build prediction models to solve business problems such as:

- Will your customer be satisfied with the project outcome?
- Will a project be profitable?
- Will a customer churn based on activity?

Once you have a trained model, then you can interact with the model in your flow to send and receive information to the AI system. 

## Security and Administration

***There are three tools for an administrator.***

1. **Admin center**. Located at [https://admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/). From the Microsoft Power Platform admin center you have ***full access to Power Automate tenant wide***. You have the ability to ***create and manage environments, implement Data Loss Prevention policies, work with Data integrations, manage user licenses, and quotas.*** 

2. **PowerShell cmdlets** - Power Automate also offers a set of PowerShell cmdlets ***for deeper controls and to work better in large-scale scenarios***. Using the cmdlets for auditing gives you more control and insight on Power Automate's usage throughout your tenant.

3. **Flows** - There are built in ***flow actions for managing both Power Automate and Power Apps***. An example of a helpful flow is one that runs everyday at 8 AM to discover all of the flows and Power Apps that have been created and then add someone from IT as a co-owner of each. That way IT has access and awareness of the solutions within the organization. 

## Driving business value

***Power Automate flows are built with triggers and actions. Triggers determine what starts the flows, while actions determine what happens***. 

***Power Automate provides the ability to specify the business logic to determine the necessary conditions; that means these automations do not have to be driven from IT but instead directly from the business.*** The same way that the Sales department builds its manual processes today by emailing spreadsheets between people, they can build their flow to automate the process going forward.

***With Power Automate there are many security, governance, and reporting capabilities to provide the necessary oversight for IT.*** You can even write a flow to manage all of the other flows. Also, Power Automate doesn't circumvent security in any way. Users cannot build flows to do things they don't already have permission to do today.

## Summary

1. Power Automate is a web-based service for automating your business processes.
2. Power Automate has different offerings to meet your needs. Event-driven flows, business process flows, and desktop flows each have their own unique properties.
3. Power Automate can connect to hundreds of data sources with the built-in connectors or you can build your own custom connectors.
4. If you know your business process, you can bring automation to it with Power Automate and without writing any traditional code.

