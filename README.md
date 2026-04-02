# AI Job Search Agent (Langflow + Docker + Discord)

Automate your job hunt with a self-hosted AI agent that scans job boards, matches them with your resume, and sends real-time alerts to Discord.


## Features

* Resume parsing (PDF to structured data)
* AI-based job matching
* Multi-source job fetching
* Real-time Discord alerts
* Fully self-hosted and private


## Workflow

```text
Resume → AI Processing → Job Matching → Discord Alerts
```


## Tech Stack

* Langflow
* Docker
* Discord Webhooks
* [Pinggy](https://pinggy.io/) (for remote access)


## Quick Start

### 1. Run Langflow

```bash
docker run -p 7860:7860 langflowai/langflow:latest
```


### 2. Open UI

```
http://localhost:7860
```


### 3. Import Workflow

* Load the provided Langflow JSON (from this repo)

### 4. Add Your Config

* Resume (PDF input)
* LLM API key (Gemini/OpenAI)
* Discord Webhook URL


### 5. Run the Flow

* Start the pipeline
* Get matched jobs directly in Discord


## Optional: Make It Public

```bash
ssh -p 443 -R0:localhost:7860 [Pinggy_token]@pro.pinggy.io
```


## Why Use This?

* No manual job searching
* Better job relevance with AI
* Instant notifications
* Fully customizable workflow


## Use Cases

* Job seekers
* Freshers
* Career switchers


## Note

The core logic and implementation are inside the `.ipynb` file in this repository.


