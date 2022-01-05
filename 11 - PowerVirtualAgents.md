# Power Virtual Agents

Power Virtual Agents are ***adaptable Artificial Intelligence chatbots***. They can ***solve common issues*** with customers and internal-facing issues automatically, freeing up staff to focus on complex requests and high-value interactions. Easily ***created with a guided, no-code graphical interface***. 

**Integration** is possible with the ***products and services using connectors***. By building ***custom workflows using Power Automate***. Or ***creating complex scenarios with Microsoft Bot Framework***. 

**Monitor** and continuously improve chatbot performance using ***AI- and data-driven insights available in a dashboard***. 

Power Virtual Agents:

- **Empower your teams** by allowing them to easily build chatbots themselves without needing intermediaries, coding, or AI expertise.
- **Reduce costs** by easily automating common inquiries and freeing human agent time to deal with more complex issues.
- **Improve customer satisfaction** by allowing customers to self-help and resolve issues quickly, 24/7 using rich personalized bot conversations.

It minimizes the IT effort required to deploy and maintain a custom conversational solution. Check out this video for a brief overview of Power Virtual Agents: https://youtu.be/J5i7h4Uzju4

## Highlights of Power Virtual Agents

1. **Get started in seconds**. Power Virtual Agents is a software-as-a-service (SaaS) offering. It allows you to easily sign up, create your chatbot, and embed it into your website with just a few clicks. There is no infrastructure to maintain or complex systems to deploy.

2. **Empower your subject matter experts**. Using Power Virtual Agents, you are in the driver's seat. Your SMEs can create chatbots quickly and easily using a **novel, intuitive, code-free graphical interface**, eliminating the need for AI expertise or teams of developers.

3. **Enable rich, natural conversations.** Microsoft’s powerful conversational AI capabilities enable your end users to have rich multi-turn conversations that quickly guide them to the right solution. And, unlike most products on the market, there is no need to retrain AI models. Simply provide a few short examples of the topic you want the chatbot to handle, build the conversation using the graphical editor, and your chatbot is ready to handle customer requests. You can even try out your changes in real-time in the test pane!

4. **Enable chatbots to take action.** Chatbots that can chat with your users are great, but chatbots that can act on their behalf are even better. With Power Virtual Agents, you can easily integrate with services and back-end systems out-of-the-box or through hundreds of easy-to-add custom connectors using Power Automate. This makes it simple to create a chatbot that not only responds to the user, but also acts on their behalf.

5. **Monitor and improve chatbot performance.** Power Virtual Agents lets you keep an eye on how your chatbots are performing using powerful metrics and AI-driven dashboards. Easily see which topics are doing well and where the chatbot can improve, and quickly make adjustments to improve performance.


6. **Better together.** Power Virtual Agents works hand-in-hand with Dynamics 365 Customer Service Insights to provide a holistic view of your customer service operations. You can use Customer Service Insights and Power Virtual Agents together to determine which topics are trending or consuming support resources, and then easily automate them.

## Components of Power Virtual Agents

When you create chatbots with Power Virtual Agents, you author and edit topics. Topics are discrete conversation paths that, when used together within a single chatbot, allow for users to have a conversation with a chatbot that feels natural and flows appropriately. 

Creating a chatbot with Power Virtual Agents is easy to do with the no-code authoring canvas, and there are a number of ways you can manage how topics interact, how you want the conversation to flow, and what it should feel like. 

It is also easy to test the chatbot without having to fully deploy the chatbot whenever you make a small change. There are also lesson topics that guide you through topic authoring - from simple to complex scenarios, as well as default system topics. You can also choose what language you want your chatbot to use.

### Topics

In Power Virtual Agents, ***a topic defines how a chatbot conversation plays out***. You can author topics by customizing provided templates, create new topics from scratch, or get suggestions from existing help sites.

A topic has **trigger phrases**—these are ***phrases, keywords, or questions*** that a user is likely to type that is related to a specific issue—and **conversation nodes**—these are what you use to ***define how a chatbot should respond*** and what it should do.

The AI uses natural language understanding to parse what a customer actually types and find the most appropriate trigger phrase or node.

For example, a user might type "Open hours" into your chatbot—the AI will be able to match that to the **Store hours** topic and begin a conversation that asks which store the customer is interested in, and then display the hours the store is open.

### Entities

A big part of chatbot conversations in Power Virtual Agents is natural language understanding, which is the ability for the AI to understand a user's intent. For example, natural language understanding is involved when a user might say "I tried to use my gift card but it doesn't work" and the chatbot is able to route the user to the topic related to gift cards not working—even if that exact phrase isn't listed as a trigger phrase.

One fundamental aspect of natural language understanding is to identify *entities* in a user dialog. An entity can be viewed as an information unit that represents a certain type of a real-world subject, like a phone number, zip code, city, or even a person's name.

#### Prebuilt entities

Out of the box, Power Virtual Agents comes with a set of prebuilt entities, which represent the most commonly used information in real-world dialogs, such as age, colors, numbers, and names.

With the knowledge granted by entities, a chatbot can smartly recognize the relevant information from a user input and save it for later use.

#### Custom entities

The prebuilt entities cover commonly used information types, but on some occasions, such as when building a chatbot that serves a specific purpose, you will need to teach the chatbot's language understanding model some domain-specific knowledge.

### Actions

You can enable your chatbot to perform an action by calling a Microsoft Power Automate flow. Flows can help you automate activities or call backend systems. For example, you can use flows with end-user authentication to retrieve information about a user after they sign in.

You can call flows from within topics, as a discrete **Call an action** node. You can utilize flows that have already been created in your Power Apps environment, or you can create a flow from within the Power Virtual Agents authoring canvas.

> **Important**
>
> A flow can only be called from a topic located in the same **Microsoft Dataverse environment** as your chatbot. Flows must also be in a solution in Power Automate. You can **move flows into solutions,** so they are listed in the authoring canvas.

Flows typically use variables to input and output information. The variables can then be used in other nodes within the topic.

### Publishing

With Power Virtual Agents, you can publish chatbots to engage with your customers on multiple platforms or channels. These include live websites, mobile apps, and messaging platforms like Microsoft Teams and Facebook.

After you have published at least once, you can connect your chatbot to additional channels.

Each time you want to update your chatbot, you publish it again from within the Power Virtual Agents app itself. This will update the chatbot across all the channels where you've inserted or connected your chatbot.

You can also configure a Power Virtual Agents chatbot to provide authentication capabilities, so users can sign in with any OAuth2 identity provider, such as Azure Active Directory (Azure AD), a Microsoft account, or Facebook.

