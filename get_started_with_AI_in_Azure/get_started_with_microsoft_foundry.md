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
<img width="1200" height="849" alt="foundry-portal-home" src="https://github.com/user-attachments/assets/d2d993b4-df00-4fb4-9a5b-b66fe6ebd800" />

---

# View Azure Resources

Every Microsoft Foundry project is backed by Azure resources.

---

## Step 1 — View Projects

From the project homepage:

1. Select the project name
2. Choose **View All Projects**

---

<img width="600" height="497" alt="0-all-projects" src="https://github.com/user-attachments/assets/547f2166-bcff-460e-a335-02a27552ec7d" />


---

## Step 2 — Locate the Parent Resource

Identify the parent Foundry resource associated with your project.

Open:

```text id="v8z1kr"
https://portal.azure.com
```

Search for the Foundry resource.

---

<img width="600" height="497" alt="0-azure-portal-search" src="https://github.com/user-attachments/assets/36b5c886-a045-4a55-96bb-f52fb30b2754" />


---

## Step 3 — Open Resource Visualizer

Select the Foundry resource and open **Resource Visualizer**.

---

<img width="600" height="497" alt="0-azure-resource-visualizer" src="https://github.com/user-attachments/assets/093c7290-4a08-4d52-a85e-b153f7107478" />


---

## Step 4 — Open the Child Project

Select the project created earlier.

---

<img width="600" height="497" alt="0-azure-project" src="https://github.com/user-attachments/assets/1f08001d-bbd2-4f28-9fab-9ec2266c1b4a" />


---

# Explore the Microsoft Foundry Portal

The Foundry portal is the central workspace for building, deploying, and managing AI solutions.

---

# Home Page

Navigate to the project Home page.

---

<img width="1200" height="849" alt="foundry-portal-home (1)" src="https://github.com/user-attachments/assets/508cf925-0ce6-4c85-b125-06d635d2385f" />


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

<img width="600" height="497" alt="0-discover" src="https://github.com/user-attachments/assets/806a0d6c-9066-4cd6-90fb-e444adcf1079" />


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

<img width="1200" height="871" alt="0-build" src="https://github.com/user-attachments/assets/804d0d72-9d2a-4e76-b7f7-ab9de04a690d" />


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

<img width="600" height="497" alt="0-operate" src="https://github.com/user-attachments/assets/c03646b3-0986-470d-a235-eaa9b3290a98" />


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

<img width="600" height="497" alt="0-docs" src="https://github.com/user-attachments/assets/cfe051de-66a4-426e-8d68-e683ffbfc96a" />


---

This section contains official Microsoft Foundry documentation and learning resources.

---

# Use Agent Helper

Open the Agent Helper icon from the top toolbar.

Select **Ask AI**.

---

<img width="600" height="497" alt="0-ask-ai" src="https://github.com/user-attachments/assets/7cd26400-bb4a-40dc-ab65-214de60eb163" />


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

<img width="600" height="473" alt="0-foundry-models" src="https://github.com/user-attachments/assets/7c86acc0-33c6-40d1-884d-6a473d91f28c" />


---

Search for:

```text id="b1r8ec"
gpt-4.1-mini
```

Open the model details page.

---

<img width="600" height="473" alt="0-gpt-4 1-mini" src="https://github.com/user-attachments/assets/c3d30734-a56f-49aa-91f9-88ec49305eb0" />


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

<img width="600" height="473" alt="0-model-playground" src="https://github.com/user-attachments/assets/6a7d10f3-865e-4cc6-8e66-f08804febb3d" />


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



<img width="1200" height="764" alt="configure-computing-history" src="https://github.com/user-attachments/assets/8b4787ca-dd5a-4f1d-abe1-878d585ee4d6" />


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
