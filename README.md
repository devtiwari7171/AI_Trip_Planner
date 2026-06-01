# AI Trip Planner Agent

An AI-powered travel planning application that generates personalized travel itineraries using Agentic AI workflows, real-time APIs, and Large Language Models (LLMs).

The system combines weather information, attraction discovery, currency conversion, expense estimation, and itinerary generation to create comprehensive travel plans for destinations worldwide.

## Features

*  Generate personalized multi-day travel itineraries
*  Real-time weather information
*  Tourist attractions and activity recommendations
*  Hotel cost estimation
*  Live currency conversion
*  Travel expense calculation
*  AI-generated travel summary
*  Agentic workflow powered by LangGraph
*  Fast response generation using Groq LLMs

---

## Architecture

```text
User Query
     │
     ▼
LangGraph Agent Workflow
     │
 ┌───┼─────────────────────┐
 │   │         │          │
 ▼   ▼         ▼          ▼
Weather   Places   Currency   Expense
 Tool      Tool      Tool      Tool
 │          │         │         │
 └──────────┴─────────┴─────────┘
                 │
                 ▼
          LLM Reasoning
                 │
                 ▼
      Personalized Travel Plan
```

---

## Tech Stack

### Backend

* FastAPI
* Python

### AI / GenAI

* LangGraph
* LangChain
* Groq LLM

### APIs

* OpenWeatherMap API
* Google Places API
* Foursquare API
* Exchange Rate API

### Frontend

* Streamlit

### Developer Tools

* Git
* GitHub
* VS Code
* UV Package Manager

---

## Getting Started

### Clone Repository

```bash
git clone https://github.com/devtiwari7171/AI_Trip_Planner.git

cd AI_Trip_Planner
```

### Create Virtual Environment

```bash
uv venv env

env\Scripts\activate
```

### Install Dependencies

```bash
uv pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file:

```env
GROQ_API_KEY=
GOOGLE_API_KEY=
GPLACES_API_KEY=
FOURSQUARE_API_KEY=
OPENWEATHERMAP_API_KEY=
EXCHANGE_RATE_API_KEY=
```

### Run Application

```bash
uvicorn main:app --reload
```

or

```bash
streamlit run app.py
```

---

## Example Prompt

```text
Plan a trip to Goa for 5 days
```

### Generated Output

* Day-wise itinerary
* Weather forecast
* Tourist attractions
* Hotel suggestions
* Budget estimation
* Currency conversion
* Travel summary

---

## Learning Outcomes

This project demonstrates:

* Agentic AI Workflows
* LangGraph State Management
* Tool Calling Architecture
* API Integration
* Prompt Engineering
* LLM Application Development
* FastAPI Backend Development
* Real-time Data Processing
* AI System Design

---

## Future Improvements

* Flight price integration
* Hotel booking APIs
* Interactive maps
* Multi-agent planning system
* LangSmith monitoring
* Docker deployment
* CI/CD pipeline
* User authentication
* Travel history dashboard

---

## Author

Dev Tiwari

* LinkedIn: https://www.linkedin.com/in/dev-tiwari-9ab41b300/
* GitHub: https://github.com/devtiwari7171

If you found this project useful, consider giving it a ⭐ on GitHub.
