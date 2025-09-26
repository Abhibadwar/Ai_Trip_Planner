# 🌍 Travel Planner Agentic Application

This project is an AI-powered **Travel Planner** web application built with **Streamlit** for the frontend and **FastAPI** for the backend. It generates personalized travel plans using an agentic workflow powered by AI models (e.g., Groq) and provides visual representations of planning graphs.

---

## Features

* Interactive **chat interface** to plan trips.
* Generates **AI-driven travel itineraries** based on user queries.
* Produces a **graphical representation** of the trip planning workflow (`my_graph.png`).
* Outputs plans with **timestamps and creator information**.
* Saves results and provides guidance for travel verification.
* Works with multiple **LLM and API providers** (OpenAI, Groq, Google, Tavily, etc.).

---

## Tech Stack

* **Frontend:** Streamlit
* **Backend:** FastAPI
* **AI/Agentic Workflow:** LangChain, Groq, LangGraph
* **Data Management:** Pydantic, dotenv
---

## Installation
2. Create and activate environment:

```bash
uv venv
.venv\Scripts\activate      # Windows
```

3. Install dependencies:

```bash
uv pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file in the project root and add the following variables:

```ini
# AI/LLM Providers
OPENAI_API_KEY=""
GROQ_API_KEY=""

# Search & Maps
GOOGLE_API_KEY=""
GPLACES_API_KEY=""
FOURSQUARE_API_KEY=""

# Travel & Weather Data
TAVILAY_API_KEY=""
OPENWEATHERMAP_API_KEY=""
EXCHANGE_RATE_API_KEY=""
```

## Running the Application

1. **Start the backend (FastAPI):**

```bash
uvicorn main:app --reload
```

2. **Start the frontend (Streamlit):**

```bash
streamlit run app.py
```

