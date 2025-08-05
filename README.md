This 4-week program focused on providing practical skills in AI and Cloud Computing. It was structured with weekly virtual sessions, mentor guidance, and hands-on labs. The curriculum included:

Week 1: Internship Orientation, IBM Cloud Registration, Artificial Intelligence.
Week 2: Data Analytics concepts, Hands-On Labs, and Cloud EDA.
Week 3 & 4: Building a Chat Bot, AI/ML experiments on the cloud, and a deep dive into AutoAI experiments on IBM Cloud.
Successful completion required active participation, completion of at least two courses on IBM SkillsBuild, and the submission of a final project presentation. 


## Project Overview

**SmartFinance Assistant** is a smart, polite, and informative AI agent designed to help users manage personal or small business finances. It can answer queries, analyze spending, help create budgets, summarize financial documents, and provide financial guidance—all in natural language.

> **Model**: `mistral-large`\
> **Platform**: IBM watsonx.ai\
> **Deployment Type**: AI Agent (Web-based Assistant)\
> **Owner**: Sara Joshi
> 
> **Public endpoints**:
> https://us-south.ml.cloud.ibm.com/ml/v4/deployments/56b2edf9-eeb6-4afe-a266-41051b6f63d5/ai_service?version=2021-05-01
>
> https://us-south.ml.cloud.ibm.com/ml/v4/deployments/56b2edf9-eeb6-4afe-a266-41051b6f63d5/ai_service_stream?version=2021-05-01

***

## Features

* Answers financial queries in simple language
* Creates monthly budgets based on user input
* Tracks expenses by category (e.g., food, utilities)
* Offers saving tips based on spending habits
* Summarizes financial documents uploaded
* Searches the web for trusted financial knowledge (via integrated tools)

***

## Use Case Examples

### Quick Start Questions:

1. What is my current account balance and recent activity?
2. Can you help me create a monthly budget?
3. How much have I spent on food this month?
4. What are some ways I can save money based on my expenses?

***

## &#x20;AI Limitations & Safety

* **No legal/tax/investment advice**
* Does **not** process sensitive information like bank login details
* Avoids hallucinations by relying only on:

  * Uploaded user documents
  * Integrated tools (web search, Wikipedia, etc.)
  * Verified built-in financial knowledge
* Uses **plain English** and explains jargon when used

***

## &#x20;Technical Setup

### IBM Watsonx Configuration:

* **Model**: `mistral-large`
* **Architecture**: AI Agent with conversational UI
* **Tools Added**:

  * Google Search
  * DuckDuckGo Search
  * Wikipedia Search
  * Webcrawler
  * \[Optional] Upload tool (if enabled)

***

## &#x20;Deployment

### Accessing the Deployed Assistant:

If deployed using IBM watsonx.ai:

* You’ll get a **Deployment URL** like this:

  ```
  bash
  ```

  CopyEdit

  `https://us-south.ml.cloud.ibm.com/ml/v4/deployments/<deployment-id>/ai_service?version=2021-05-01 `&#x20;

> 🔗 This is **not** a direct public-facing link. To make the agent usable as a public-facing assistant, embed it in a web app or create an API wrapper around it.

***

## Exporting the Project to GitHub

You can use **IBM Cloud CLI** or manual methods:

1. **CLI (IBM Cloud Shell)**:

   ```
   bash
   ```
 `ibmcloud login ibmcloud ml deployment-download --deployment-id <your-id> git init git remote add origin https://github.com/yourusername/SmartFinance-Assistant.git git add . git commit -m "Initial commit" git push -u origin main `&#x20;
2. **Manual**:

   * Download assets and model files from `Assets` in IBM watsonx
   * Add them to a GitHub repo manually via drag & drop or `git push`

***

## &#x20;Future Enhancements

* Integrate bank APIs (with OAuth) for real-time finance data
* Enable user-specific dashboards for reports and charts
* Add multilingual support
* Improve data privacy with end-to-end encryption for document uploads

***

## &#x20;Contact

> **Created by**: Sara Joshi\
> &#x20;**GitHub**: https://github.com/Sara-J-86
> 
> &#x20;**Email**: sara.j.08604@gmail.com
> 
> &#x20;**IBM Cloud Region**: Dallas (us-south)
