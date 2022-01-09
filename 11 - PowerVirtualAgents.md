# Power Virtual Agents

***Power Virtual Agents are adaptable Artificial Intelligence chatbots***. ***They solve common issues and are created with a guided, no-code graphical interface.*** 

***Integration is possible with the products and services using connectors. By building custom workflows using Power Automate. Or creating complex scenarios with Microsoft Bot Framework. Monitor and improve chatbot performance using AI- and data-driven insights.*** 

**Power Virtual Agents:**

- **Empower your teams** - ***They can easily build chatbots themselves.*** 
- **Reduce costs** - ***automate common inquiries*** 
- **Improve customer satisfaction** - ***allow customers to self-help and resolve issues quickly***

This will free up staff to focus on complex requests and high-value interactions. It minimizes the IT effort required to deploy and maintain a custom conversational solution. Check out this video for a brief overview of Power Virtual Agents: https://youtu.be/J5i7h4Uzju4

## Highlights of Power Virtual Agents

1. **Get started in seconds**. Power Virtual Agents is a software-as-a-service (SaaS) offering. It allows you to easily sign up, create your chatbot, and embed it into your website with just a few clicks. 

2. **Empower your subject matter experts**. Your SMEs can create chatbots quickly and easily using a novel, intuitive, code-free graphical interface, eliminating the need for AI expertise or teams of developers.

3. **Enable rich, natural conversations.** Microsoft’s powerful conversational AI capabilities enable your end users to have rich multi-turn conversations that quickly guide them to the right solution. 

4. **Enable chatbots to take action.** With Power Virtual Agents, you can easily integrate with services and back-end systems out-of-the-box or through hundreds of easy-to-add custom connectors using Power Automate. This makes it simple to create a chatbot that not only responds to the user, but also acts on their behalf.

5. **Monitor and improve chatbot performance.** Track how chatbots are performing using powerful metrics and AI-driven dashboards. See which topics are doing well and where the chatbot can improve.


6. **Better together.** Power Virtual Agents works hand-in-hand with Dynamics 365 Customer Service Insights to provide a holistic view of your customer service operations.

## Components of Power Virtual Agents

***When you create chatbots with Power Virtual Agents, you author and edit topics.*** ***Topics are discrete conversation paths that, when used together within a single chatbot, allow for users to have a conversation with a chatbot that feels natural and flows appropriately.*** 

### Topics

***A topic defines how a chatbot conversation plays out***. You can author topics by customizing provided templates, create new topics from scratch, or get suggestions from existing help sites. 

**A topic consists of:**

- **trigger phrases** - ***phrases, keywords, or questions related to that topic*** 
- **conversation nodes** - ***define how a chatbot should respond and what it should do.*** 

### Entities

***A big part in Power Virtual Agents is natural language understanding, the ability to understand a user's intent. One fundamental aspect is to identify "entities", information units, in a dialog.*** An entity can be viewed as an information unit that represents a certain type of a real-world subject, like a phone number, zip code, city, or even a person's name.

#### Prebuilt entities

***PVA comes with prebuilt entities, which represent the most commonly used information in real-world dialogs, such as age, colors, numbers, and names.*** With the knowledge granted by entities, a chatbot can smartly recognize the relevant information from a user input and save it for later use.

#### Custom entities

***When building a chatbot that serves a specific purpose, the language understanding model needs to be trained to understand domain-specific knowledge.***

### Actions

***Enable your chatbot to perform an action by calling a Microsoft Power Automate flow.*** Flows can help you automate activities or call backend systems. For example, you can use flows with end-user authentication to retrieve information about a user after they sign in.

***Flows can be called from within topics, as a discrete 'Call an action node'.*** You can utilize flows that have already been created in your Power Apps environment, or you can create a flow from within the Power Virtual Agents authoring canvas.

> **Important**
>
> A flow can only be called from a topic located in the same **Microsoft Dataverse environment** as your chatbot. Flows must also be in a solution in Power Automate. You can **move flows into solutions,** so they are listed in the authoring canvas.

***Flows typically use variables to input and output information. The variables can then be used in other nodes within the topic.***

### Publishing

***PVA can be published to engage with customers on multiple platforms or channels.*** These include live websites, mobile apps, and messaging platforms like Microsoft Teams and Facebook. After you have published at least once, you can connect your chatbot to additional channels.

***Each time there is an update for the chatbot, publish it again from within the Power Virtual Agents app.*** This will update the chatbot across all the channels where you've inserted or connected your chatbot.

***It is possible for a chatbot to provide authentication capabilities***, so users can sign in with any OAuth2 identity provider, such as Azure Active Directory (Azure AD), a Microsoft account, or Facebook.

