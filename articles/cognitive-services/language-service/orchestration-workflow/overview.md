---
title: Orchestration workflows - Azure Cognitive Services
titleSuffix: Azure Cognitive Services
description: Learn how to use Orchestration workflows.
services: cognitive-services
author: aahill
manager: nitinme
ms.service: cognitive-services
ms.subservice: language-service
ms.topic: overview
ms.date: 04/14/2022
ms.author: aahi
ms.custom: language-service-orchestration
---

# What is orchestration workflow?


Orchestration workflow is one of the features offered by [Azure Cognitive Service for Language](../overview.md). It is a cloud-based API service that applies machine-learning intelligence to enable you to build orchestration models to connect [Conversational Language Understanding (CLU)](../conversational-language-understanding/overview.md), [Question Answering](../question-answering/overview.md) projects and [LUIS](../../luis/what-is-luis.md) applications.
By creating an orchestration workflow, developers can iteratively tag utterances, train and evaluate model performance before making it available for consumption. 
To simplify building and customizing your model, the service offers a custom web portal that can be accessed through the [Language studio](https://aka.ms/languageStudio). You can easily get started with the service by following the steps in this [quickstart](quickstart.md). 


This documentation contains the following article types:

* [Quickstarts](quickstart.md) are getting-started instructions to guide you through making requests to the service.
* [Concepts](concepts/evaluation-metrics.md) provide explanations of the service functionality and features.
* [How-to guides](how-to/create-project.md) contain instructions for using the service in more specific or customized ways.


## Example usage scenarios

Orchestration workflow can be used in multiple scenarios across a variety of industries. Some examples are:

### Enterprise chat bot

In a large corporation, an enterprise chat bot may handle a variety of employee affairs. It may be able to handle frequently asked questions served by a custom question answering knowledge base, a calendar specific skill served by conversational language understanding, and an interview feedback skill served by LUIS. The bot needs to be able to appropriately route incoming requests to the correct service. Orchestration workflow allows you to connect those skills to one project that handles the routing of incoming requests appropriately to power the enterprise bot.

## Project development lifecycle

Creating an orchestration workflow project typically involves several different steps. 

:::image type="content" source="media/development-lifecycle.png" alt-text="Diagram showing the development lifecycle." lightbox="media/development-lifecycle.png":::

Follow these steps to get the most out of your model:

1. **Build schema**: Know your data and define the actions and relevant information that needs to be recognized from user's input utterances. Create the [intents](glossary.md#intent) that you want to assign to user's utterances and the projects you want to connect to your orchestration project.

2. **Tag data**: The quality of data tagging is a key factor in determining model performance. 
<!--  TODO: TO INCLUDE MORE GUIDANCE  -->

3. **Train model**: Your model starts learning from your tagged data.

4. **View model evaluation details**: View the evaluation details for your model to determine how well it performs when introduced to new data.

5. **Deploy model**: Deploying a model makes it available for use via the [prediction API](https://aka.ms/clu-runtime-api).

6. **Predict intents**: Use your custom model to predict intents from user's utterances.

## Reference documentation and code samples

As you use orchestration workflow, see the following reference documentation and samples for Azure Cognitive Services for Language:

|Development option / language  |Reference documentation |Samples  |
|---------|---------|---------|
|REST APIs (Authoring)   | [REST API documentation](https://aka.ms/clu-authoring-apis)        |         |
|REST APIs (Runtime)    | [REST API documentation](https://aka.ms/clu-runtime-api)        |         |
|C#  (Runtime)   | [C# documentation](/dotnet/api/azure.ai.textanalytics?view=azure-dotnet-preview&preserve-view=true)        | [C# samples](https://github.com/Azure/azure-sdk-for-net/tree/main/sdk/cognitivelanguage/Azure.AI.Language.Conversations/samples)        |
|Python (Runtime)| [Python documentation](/python/api/overview/azure/ai-textanalytics-readme?view=azure-python-preview&preserve-view=true)        | [Python samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cognitivelanguage/azure-ai-language-conversations/samples) |

## Responsible AI 

An AI system includes not only the technology, but also the people who will use it, the people who will be affected by it, and the environment in which it is deployed. Read the transparency note for CLU and orchestration workflow to learn about responsible AI use and deployment in your systems. You can also see the following articles for more information:

[!INCLUDE [Responsible AI links](../includes/overview-responsible-ai-links.md)]

## Next steps

* Use the [quickstart article](quickstart.md) to start using orchestration workflow.  

* As you go through the project development lifecycle, review the [glossary](glossary.md) to learn more about the terms used throughout the documentation for this feature. 

* Remember to view the [service limits](service-limits.md) for information such as regional availability.
