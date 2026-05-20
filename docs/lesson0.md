# What Do You Need to Learn for AI Agent Development?

We use various AI Agents every day, such as using Cursor to write code and Manus to automate different tasks.

So, have you ever thought about developing an AI Agent product yourself?

Someone might say, "Can't we just call the Large Language Model (LLM) directly?"

Think about it, doesn't the LLM have the following limitations:

Can it remember the messages you chatted about with it last week? No, it can't.

If you ask it to help you visit a webpage or do something, can it only give you the ideas and leave you to do it yourself?

If you want it to answer questions based on your company's internal private documents, will it have no clue what they are?

If you ask it about recent breaking news, does it not know? Because it lacked this data during training.

To solve these problems, we need to empower the LLM with Memory management, Tool calling capabilities, and RAG (Retrieval-Augmented Generation) document query capabilities.

No matter how LLMs evolve, they cannot natively solve these issues:

Its memory is always limited, requiring developers to handle Memory management.

The domain-specific tools it can invoke need to be developed and provided by developers as Tools.

It cannot answer questions about unknown private documents, requiring an extension of RAG knowledge base query capabilities.

These are exactly the AI technologies we need to learn—the core capabilities of AI Agent development.

What is an Agent?

Essentially, it is an LLM extended with Tools and Memory. It is inherently capable of reasoning and planning. When you expand its capabilities with Tools, it can automate tasks. When you manage its memory with Memory, it can remember what you want it to retain. Furthermore, it can utilize RAG to query internal knowledge bases for information.

Such an extended LLM—one that possesses internal knowledge, can reason and plan, has a memory, and can execute tasks for you—is an Agent.

[Image](../images/lesson0/0.png)

How does the AI IDE you use daily, like Cursor, read/write files and execute commands?

For instance, modifying code requires reading and writing files, and helping you run code requires executing commands. How are these features implemented? Obviously, by extending its Tools.

How does Manus, which helps you with various tasks, launch a browser to visit webpages automatically, execute commands, and help you operate different software?

Watch this video: How does Manus open a browser, visit webpages, click elements, summarize the content into a document, and write it into an md file? It is also done by extending its Tools.

How does the financial assistant in Alipay analyze and recommend funds for you? How does it know the data of these funds?

Watch this video: How does Alipay's Ma Xiaocai know the data of these funds? Does the LLM know it inherently? Absolutely not. It accesses internal knowledge bases based on RAG.

There are countless similar scenarios where we need to extend the capabilities of LLMs. Just knowing how to chat with an LLM is not enough; you must be able to extend its various capabilities to meet diverse AI demands. This is the ultimate goal of our AI technology learning journey.

Then, what frameworks do we use for RAG, Memory, Tool, and Agent development?

The most commonly used framework is LangChain, which encapsulates these capabilities into various APIs that you can use directly. When I build AI Agent products at my company, I develop them based on LangChain. It offers both Python and Node.js versions, and we are learning the Node.js version.

In fact, the programming language is secondary. Once you master the AI technology, switching to another language is very straightforward because the underlying logic and concepts remain identical. As a frontend developer, starting with JS and Node.js definitely offers a much smoother learning curve for AI!

Therefore, this course uses Node.js + LangChain + LangGraph to develop various Agents.

LangChain is used to develop a single Agent, where each Agent focuses on performing one specific task. However, when it comes to multi-Agent collaboration, maintaining the interactions among multiple Agents by yourself using LangChain becomes quite tedious. That is when we need to learn LangGraph. It is a framework built on top of LangChain specifically designed for multi-Agent interaction.

When learning AI, do not limit yourself to just building some tools with AI. It is best to learn it in combination with backend technologies—meaning, AI Full-Stack. Since AI code runs on the backend, you will need Redis to store memory and MySQL to store knowledge, which requires backend expertise.

Thus, we learn backend and AI together to build AI full-stack products, utilizing NestJS as our Node.js backend framework.

Summary

Extending an LLM with capabilities like Tools, Memory, and RAG so that it can perform specific tasks creates an Agent. The tools we use daily, like Cursor and Manus, are all AI Agents.

We will learn the LangChain framework for single-Agent development and the LangGraph framework for Multi-Agent systems. We will learn using the Node.js version; once mastered, switching to other languages later is seamless as the APIs and logic are identical.

We will integrate our learning with backend technologies to develop AI full-stack products. Only in this way can we land AI technology into real products, transform it into our competitive edge, and capitalize on the dividends of this AI era.
