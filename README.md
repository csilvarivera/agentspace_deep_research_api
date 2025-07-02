# Deep Research API Quickstart

This repository provides a Python script within a Jupyter Notebook (`DeepResearch_via__Agentspace.ipynb`) to demonstrate how to use the Deep Research API on Google Cloud's Agentspace. The script shows the full end-to-end process, from setting up a project to generating a research plan and streaming the final report with citations.

Full official documentation can be found here: [Agentspace Enterprise Docs](https://cloud.google.com/agentspace/agentspace-enterprise/docs/research-assistant)

***

## 📋 Prerequisites

Before you begin, ensure the following requirements are met in your Google Cloud project:

* **Agent Builder Service:** The Agent Builder API must be activated in your project.
* **Permissions:** Your user or service account must have the appropriate IAM roles. See [Access control for Agentspace Enterprise](https://cloud.google.com/agentspace/agentspace-enterprise/docs/before-you-begin#access-control) for details.
* **Google Cloud Storage:** At least one GCS bucket with read/write permissions should be available.
* **Datastore:** It is highly recommended to have a minimal datastore created. An easy way to do this is by creating a datastore from an empty Google Site.
* **Org Policies:** Verify that there are no organization policies restricting the creation of new resources for the Agent Builder service.

***

## 🚀 Getting Started

### 1. Installation

The notebook requires several Python libraries. Install them using the following command:

```bash
pip install --upgrade google-genai httpx json-stream markdown