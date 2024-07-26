# Prompt Flow evaluation demo

## The value of Prompt Flow as an AI platform

Prompt Flow is the Microsoft recommended approach for taking apps to production and, while we have seen folks in AI excited about it, others in apps may have some doubts. Our first goal is to understand why PF is the recommended platform (not just a tool!) and why we call it a platform. This distinction is crucial for the Apps team to understand, as it underscores the platform's versatility and its capacity to orchestrate complex AI functionalities seamlessly.

- E2E LLMOps: DevOps best practices extend to LLMs via LLMOps by adding some key concepts such as evaluation. On top of developing, testing and deploying, we must evaluate our models for KPIs like groundness, cohesiveless, safety, etc. PF makes that step very simple and intuitive, as well as the other traditional ones that we know from Apps. You can work on PF from development till the monitoring phase, so it isn't just an orchestration tool. With PF we create a microservice containing the model that isolates that concern and we can manage separately as part of our architecture.

- Platform Versatility: Prompt Flow is described as a platform rather than a tool due to its extensive capabilities. It can orchestrate calls to different APIs, build chains of operations, and integrate with various Microsoft and third-party services. This flexibility allows developers to use Prompt Flow for a wide range of applications, from simple task automation to complex AI-driven solutions 1.

- Enterprise-Grade Support: One of the platform's significant advantages is its enterprise-grade support. This ensures that any applications built using Prompt Flow are backed by Microsoft's robust support infrastructure, providing peace of mind and reliability for businesses deploying critical applications 2.

- Developer Productivity: Prompt Flow accelerates developer productivity by offering built-in functionalities for common tasks, such as API orchestration and AI model evaluation. This allows developers to focus on refining their applications rather than building foundational components from scratch 3.

- Strategic Importance for Microsoft: The platform is strategically important for Microsoft, driving stickiness to Azure services. By offering a platform that integrates closely with Azure's ecosystem, Microsoft ensures that developers are more likely to use Azure services for their applications, enhancing customer retention and satisfaction 4.

For the Apps team, understanding these aspects of Prompt Flow is crucial. It's not just about leveraging a new tool but about embracing a platform that can significantly enhance how we develop, deploy, and manage AI-driven applications.

# Labs

## 1. Refresher: Create and run an evaluation flow on the AI Studio PF UI

During the general track of the AI Attached Bootcamp, you've learned about Azure Prompt Flow via the UI on AI Studio. You've convered the key aspects of it via the UI - development, evaluation, and high-level deployment. Please, refer to those recodings if you need a refresher.

Some questions to reflect or debate:
- What is PF? What's its value?
- What are the key stages of LLMOps? (development, evaluation, testing and deployment)
- What setbacks do you think user may encounter taking apps to production? Any counter arguments?
- How do you think PF fits in the overall AI App development from a software engineering perspective?
[E2E Prompt FLow UI guidance](https://learn.microsoft.com/en-us/azure/ai-studio/tutorials/deploy-copilot-ai-studio).

## 2. Managing Prompt Flow programatically: SDK evaluation focus
We've seen that prompt flow is a collaboration tool, allowing to use version control and git repos for collaboration, enabling both local (several IDEs work, but VSCode is recommended for its PF extention) and AI Studio development. Today, we're going to focus on how to configure and customize evaluation via code with the Prompt Flow SDK, allowing us to go a bit further than what the UI allows us. While it's true that most use cases will be covered by the UI configuration, some teams may want to take things further and hence the value of the PF SDK. By creating these evaluation flows programatically, we can address other concerns necessary in the LLMOps workload. Once these evaluations are created, we will explore how to run them during Week 8 as part of our CI/CD pipelines as well as testing and deployment, painting the E2E LLMOps SDLC, where Apps can add great value.

We will be following [this MS Learn Doc](https://learn.microsoft.com/en-us/azure/ai-studio/how-to/develop/flow-evaluate-sdk).

Content:
1. Getting started
2. Built-in evaluators
3. Composite evaluators
4. Custom evaluators
5. Evaluate on test dataset using evaluate()
6. Evaluate on a target
7. Related content


