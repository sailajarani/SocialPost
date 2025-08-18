# Marketing Campaign Assistant - Google ADK Tutorial Project

This repository contains the code for the Marketing Campaign Assistant project, built as part of a tutorial series on Google's Agent Development Kit (ADK).


This project demonstrates how to leverage Google ADK's code-first approach and workflow orchestration capabilities to build agents that collaborate on a complex task.



## Prerequisites

*   Python 3.7+
*   pip (Python package installer)
*   Access to an LLM provider (like Google AI Studio/Vertex AI, OpenAI, etc.) and an associated API Key. This tutorial uses Google's Gemini models via the Google AI client library, which is integrated with ADK.
*   A Google API Key with access to Gemini models. You can obtain one from [Google AI Studio](https://aistudio.google.com/).
*   Basic familiarity with Python.

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/AhsanAyaz/marketing-agents-adk
    cd marketing-agents-adk
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv .venv
    ```
3.  **Activate the virtual environment:**
    *   On macOS and Linux:
        ```bash
        source venv/bin/activate
        ```
    *   On Windows:
        ```bash
        .\venv\Scripts\activate
        ```
4.  **Install dependencies:**
    ```bash
    pip install -r backend/requirements.txt
    ```
    *(Note: The `requirements.txt` is located inside the `backend` folder, as Part 2 will add a frontend folder at the top level.)*
5.  **Set up your API Key:**
    *   Create a file named `.env` in the **directory** `marketing_campaign_agent`.
    *   Add your Google API Key to this file, using the environment variable name expected by the Google AI client library (usually `GOOGLE_API_KEY`).
        ```env
        GOOGLE_API_KEY='YOUR_ACTUAL_GOOGLE_API_KEY'
        ```
    *   Replace `'YOUR_ACTUAL_GOOGLE_API_KEY'` with your key.

## Project Structure (Part 1)

```
marketing-agents-adk/
├── marketing_campaign_agent/
│   ├── __init__.py         # Package initialization
    └── .env                # Stores your API key (not committed to git)
│   ├── agent.py            # Defines all LlmAgents and the SequentialAgent workflow
│   ├── requirements.txt    # Project dependencies
│   └── instruction.py      # Text files containing detailed instructions for each agent
```






MIT
"# SocialPostDepoly" 


