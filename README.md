# Ai-Chatbot
AI chatbot agent with Streamlit UI, FastAPI backend, and LangGraph orchestration. Supports Groq &amp; OpenAI models, custom prompts, and web search. Interact with AI agents seamlessly!
AI Chatbot Agents with LangGraph, Streamlit, Groq, OpenAI, and FastAPI
This project is a web-based AI chatbot agent that allows users to interact with AI models from different providers (Groq and OpenAI) through a user-friendly interface. The chatbot is built using LangGraph for agent orchestration, Streamlit for the frontend UI, FastAPI for the backend, and integrates with Groq and OpenAI for AI model inference. Users can define custom system prompts, select models, enable web search, and interact with the AI agent seamlessly.

Features
Multi-Model Support:

Choose between Groq (e.g., llama-3.3-70b-versatile, mixtral-8x7b-32768) and OpenAI (e.g., gpt-4o-mini) models.

Dynamically switch between providers and models.

Customizable AI Agent:

Define a system prompt to customize the behavior of the AI agent.

Example: "You are a helpful assistant specialized in answering questions about Python programming."

Web Search Integration:

Enable or disable web search to allow the agent to fetch real-time information from the web.

User-Friendly UI:

Built with Streamlit, the UI is simple, intuitive, and responsive.

Users can input queries, select models, and view responses in real-time.

FastAPI Backend:

The backend is built with FastAPI, providing a robust and scalable API for handling requests.

The backend processes user queries, interacts with the selected AI model, and returns responses.

LangGraph for Agent Orchestration:

LangGraph is used to manage the flow and logic of the AI agent, ensuring smooth interactions and task execution.

Tech Stack
Frontend: Streamlit

Backend: FastAPI

AI Models: Groq, OpenAI

Agent Orchestration: LangGraph

Web Search: (Optional integration with tools like SerpAPI or Tavily)

Deployment: (Optional: Docker, Kubernetes, or cloud platforms like AWS/GCP)

How It Works
User Interaction:

The user interacts with the Streamlit UI to:

Define a system prompt.

Select a model provider (Groq or OpenAI) and a specific model.

Enable or disable web search.

Enter a query.

Backend Processing:

The Streamlit frontend sends the user's input to the FastAPI backend via an API call.

The backend processes the request, interacts with the selected AI model, and optionally performs a web search.

AI Response:

The backend sends the AI's response back to the Streamlit UI, where it is displayed to the user.

Project Structure
Copy
ai-chatbot-agents/
├── frontend/                  # Streamlit UI code
│   └── app.py                 # Streamlit application
├── backend/                   # FastAPI backend code
│   └── main.py                # FastAPI server and endpoint logic
├── agents/                    # LangGraph agent logic
│   └── agent.py               # Agent orchestration and logic
├── requirements.txt           # Python dependencies
├── README.md                  # Project documentation
└── .gitignore                 # Git ignore file
Setup and Installation
Clone the repository:

bash
Copy
git clone https://github.com/your-username/ai-chatbot-agents.git
cd ai-chatbot-agents
Install dependencies:

bash
Copy
pip install -r requirements.txt
Set up API keys:

Add your Groq and OpenAI API keys to the environment variables or a .env file.

Run the backend:

bash
Copy
cd backend
uvicorn main:app --reload --port 9999
Run the frontend:

bash
Copy
cd frontend
streamlit run app.py
Access the UI:

Open your browser and navigate to http://localhost:8501.

Usage
Define a system prompt to customize the AI agent's behavior.

Select a model provider (Groq or OpenAI) and a specific model.

Enable or disable web search based on your needs.

Enter your query and click "Ask Agent!" to get a response.

Future Enhancements
Add support for more AI providers (e.g., Anthropic, Cohere).

Implement chat history and context management.

Improve error handling and user feedback.

Deploy the application using Docker or a cloud platform.

Contributing
Contributions are welcome! If you'd like to contribute, please fork the repository and submit a pull request. For major changes, open an issue first to discuss the proposed changes.