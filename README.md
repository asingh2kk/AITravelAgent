# AI Travel Agent

An interactive AI agent that generates personalized day-trip itineraries based on your chosen city, interests, and real-time weather data. Built using LangGraph, LangChain, and a LLaMA-3 model, with a Gradio-powered user interface.

## Features

- Accepts user input for city and interests
- Fetches real-time geolocation and weather data via Open-Meteo APIs
- Uses LLaMA-3 (via Groq + LangChain) to generate tailored trip itineraries
- Modular agent logic with LangGraph for step-by-step reasoning
- Deployed with an interactive Gradio interface

## Tech Stack

| Component       | Tech / Tool                             |
|----------------|------------------------------------------|
| Agent Framework | LangGraph                               |
| LLM Integration | LangChain + Groq-hosted LLaMA-3          |
| Weather API     | Open-Meteo (Geocoding + Forecasting)     |
| UI              | Gradio                                   |
| Runtime         | Python (Jupyter Notebook or Colab)       |

## How It Works

1. **User Input**: City name and comma-separated interests.
2. **Geocoding & Weather**: Retrieves latitude/longitude and weather using Open-Meteo APIs.
3. **Itinerary Generation**: Passes contextual state into a LangGraph node powered by LLaMA-3.
4. **Interactive Output**: Itinerary is displayed via a Gradio web interface.
