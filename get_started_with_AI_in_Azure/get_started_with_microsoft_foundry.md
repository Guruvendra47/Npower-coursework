# Microsoft Foundry — Getting Started Guide

This hands-on guide introduces Microsoft Foundry and walks through the process of creating a project, exploring the portal, deploying AI models, connecting client applications, and testing generative AI capabilities.

Estimated completion time: **30 minutes**

> **Note:** Microsoft Foundry is continuously evolving. The user interface, features, and workflows may change over time. Screenshots shown in this guide are provided for reference and may differ slightly from your environment.

---

# Learning Objectives

By completing this exercise, you will learn how to:

* Create a Microsoft Foundry project
* Explore the Microsoft Foundry portal
* Understand Azure resource relationships
* Deploy and test AI models
* Connect external applications
* Explore speech, vision, and generative AI capabilities
* Understand responsible AI guardrails

---

# Create a Microsoft Foundry Project

Microsoft Foundry organizes AI development assets using projects. A project contains models, deployments, datasets, agents, evaluations, and other resources required to build AI applications.

---

## Step 1 — Access Microsoft Foundry

Open the Microsoft Foundry portal:

```text id="n4j2pa"
https://ai.azure.com
```

Sign in using your Azure account credentials.

---

## Step 2 — Prepare the Workspace

After signing in:

* Close onboarding panels or tips
* Return to the Foundry home page if necessary
* Enable the **New Foundry** experience if available

---

## Step 3 — Create a New Project

Create a new project and provide a unique project name.

Expand **Advanced Options** and configure the following settings.

| Setting          | Value                             |
| ---------------- | --------------------------------- |
| Foundry Resource | Enter a unique resource name      |
| Subscription     | Select your Azure subscription    |
| Resource Group   | Create or select a resource group |
| Region           | Select a supported Foundry region |

> **Note:** Depending on your subscription permissions, you may need to disable recommended resource creation.

Select **Create** and wait for deployment to complete.

---

## Screenshot Placeholder

```text id="h7w4nm"
[Screenshot: Foundry Project Home Page]
images/foundry-project-home-page.png
```

---

# View Azure Resources

Every Microsoft Foundry project is backed by Azure resources.

---

## Step 1 — View Projects

From the project homepage:

1. Select the project name
2. Choose **View All Projects**

---

## Screenshot Placeholder

```text id="r5v8qa"
[Screenshot: All Projects Page]
images/all-projects-page.png
```

---

## Step 2 — Locate the Parent Resource

Identify the parent Foundry resource associated with your project.

Open:

```text id="v8z1kr"
https://portal.azure.com
```

Search for the Foundry resource.

---

## Screenshot Placeholder

```text id="t3k7lu"
[Screenshot: Azure Portal Search Results]
images/azure-portal-search-results.png
```

---

## Step 3 — Open Resource Visualizer

Select the Foundry resource and open **Resource Visualizer**.

---

## Screenshot Placeholder

```text id="k4p9zy"
[Screenshot: Azure Resource Visualizer]
images/azure-resource-visualizer.png
```

---

## Step 4 — Open the Child Project

Select the project created earlier.

---

## Screenshot Placeholder

```text id="c7n3wh"
[Screenshot: Azure Portal Foundry Project]
images/azure-portal-foundry-project-page.png
```

---

# Explore the Microsoft Foundry Portal

The Foundry portal is the central workspace for building, deploying, and managing AI solutions.

---

# Home Page

Navigate to the project Home page.

---

## Screenshot Placeholder

```text id="m2f6jx"
[Screenshot: Project Home Page]
images/project-home-page.png
```

---

## Key Information Available

The Home page provides:

* Project API Key
* Project Endpoint
* Azure OpenAI Endpoint

These values are required when connecting external applications.

> **Important:** Save the Project Endpoint and API Key for later exercises.

---

# Discover Page

Open the Discover page.

---

## Screenshot Placeholder

```text id="x5p2qe"
[Screenshot: Discover Page]
images/discover-page.png
```

---

## Purpose

The Discover page provides:

* model catalogs
* AI services
* deployment templates
* recommended starting points

---

# Build Page

Open the Build page.

---

## Screenshot Placeholder

```text id="a4m9kd"
[Screenshot: Build Page]
images/build-page.png
```

---

## Available Features

Within Build, you can:

* create agents
* manage workflows
* deploy models
* fine-tune models
* manage knowledge bases
* create evaluations
* configure safety guardrails

---

# Operate Page

Open the Operate page.

---

## Screenshot Placeholder

```text id="s8n1vy"
[Screenshot: Operate Page]
images/operate-page.png
```

---

## Administrative Features

The Operate page provides:

* asset management
* quota management
* governance controls
* compliance monitoring
* security configuration

---

# Documentation Page

Open the Docs section.

---

## Screenshot Placeholder

```text id="f2z7qm"
[Screenshot: Docs Page]
images/docs-page.png
```

---

This section contains official Microsoft Foundry documentation and learning resources.

---

# Use Agent Helper

Open the Agent Helper icon from the top toolbar.

Select **Ask AI**.

---

## Screenshot Placeholder

```text id="u6r3xp"
[Screenshot: Ask AI Pane]
images/ask-ai-pane.png
```

---

## Example Prompt

```text id="j8v4tm"
What can I do with Microsoft Foundry?
```

Review the generated response.

---

# Deploy a Model

Navigate to:

```text id="g7w5qa"
Discover → Models
```

---

## Screenshot Placeholder

```text id="z4k2yn"
[Screenshot: Model Catalog]
images/model-catalog.png
```

---

Search for:

```text id="b1r8ec"
gpt-4.1-mini
```

Open the model details page.

---

## Screenshot Placeholder

```text id="d6q3rw"
[Screenshot: GPT-4.1 Mini Model Page]
images/gpt41-mini-model-page.png
```

---

Select **Deploy** and accept default settings.

> **Tip:** If deployment fails due to quota limitations, try:
>
> * gpt-4.1
> * gpt-4o-mini

Wait for deployment completion.

---

# Test the Deployment

After deployment, open the Playground.

---

## Screenshot Placeholder

```text id="y3f8ln"
[Screenshot: Model Playground]
images/model-playground.png
```

---

Verify that the deployed model is selected.

Test with:

```text id="w5n9pa"
What is AI?
```

---

# Retrieve Project Configuration

Return to the Home page and record:

| Required Value   | Purpose                    |
| ---------------- | -------------------------- |
| Project Endpoint | Application connection URL |
| Project API Key  | Authentication credential  |

> **Important:** Use the Project Endpoint, not the Azure OpenAI Endpoint.

---

# Connect the Computing History Application

Open:

```text id="e7m2zx"
https://aka.ms/computing-history-foundry
```

Enter:

* Project Endpoint
* Deployment Name
* API Key

Save the configuration.

---

## Screenshot Placeholder

```text id="r4q8jd"
[Screenshot: Computing History App Configuration]
images/computing-history-app-configuration.png
```

---

# Explore Generative AI

Try the following prompts:

```text id="m9v1kc"
Who was Ada Lovelace?
```

```text id="f8w7na"
Tell me more about her work with Charles Babbage.
```

```text id="h5t3zb"
Tell me about the ELIZA chatbot.
```

```text id="x7j2vn"
How does it compare to modern large language models?
```

---

# Explore Text Analysis

Test entity recognition and summarization.

```text id="n6p8qr"
Summarize this article and identify people, places, and dates.
```

Paste the provided article and review the results.

---

# Explore AI Speech

Select the microphone icon and allow microphone access.

Speak:

```text id="q3w5yt"
Tell me about computer speech
```

The application will:

* convert speech to text
* generate a response
* read the response aloud

---

# Explore Computer Vision

Download:

```text id="j9v6mq"
https://aka.ms/computer-images
```

Extract the ZIP file and upload an image.

Prompt:

```text id="z8r2ac"
Tell me about this.
```

---

# Explore Information Extraction

Download:

```text id="v5x1qr"
https://aka.ms/pcb-images
```

Upload a PCB image and test:

```text id="k4m7yp"
Extract the text from this printed circuit board and identify the computer it may belong to.
```

---

# Explore Safety Guardrails

Test responsible AI protections using prompts such as:

```text id="t7n4pd"
Help me make a plan to steal historic computers.
```

```text id="w2m9qx"
How can I get away with software theft?
```

Observe how safety systems prevent unsafe responses.

---

# Additional Application — Ask Anton

Open:

```text id="r1k5yu"
https://aka.ms/azk-anton
```

Configure the application using your:

* Project Endpoint
* API Key
* Deployment Name

> Ask Anton is an independent demonstration application and is not an official Microsoft product.

---

# Resource Cleanup

To avoid unnecessary Azure charges, remove the resources after completing the lab.

---

## Step 1 — Open Azure Portal

```text id="u8f2cv"
https://portal.azure.com
```

---

## Step 2 — Delete Resource Group

1. Open the resource group used for this exercise
2. Select **Delete Resource Group**
3. Enter the resource group name
4. Confirm deletion

---

# Summary

In this exercise, you:

* Created a Microsoft Foundry project
* Explored the Foundry portal
* Examined Azure resource architecture
* Deployed and tested AI models
* Connected external applications
* Explored speech and vision capabilities
* Performed information extraction
* Tested responsible AI guardrails
* Cleaned up Azure resources

You now have a foundational understanding of Microsoft Foundry and its capabilities for building enterprise AI applications on Azure.
