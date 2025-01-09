# Ollama Chatbot with ChromaDB Memory
This project demonstrates how to build a chatbot using Ollama's LLM (Language Model) and ChromaDB for maintaining contextual memory. The chatbot remembers previous interactions and leverages past conversation data to provide relevant and accurate responses. The app is built using Streamlit for the frontend interface.
A chatbot application built with Streamlit, leveraging ChromaDB for contextual memory and language models for interactive responses. The chatbot supports reading multiple `.txt` files for additional context, making it adaptable and responsive.

## Features
- Contextual memory using ChromaDB.
- Language model interaction via `OllamaLLM`.
- Upload and process multiple `.txt` files for extended context.
- **Streamlit-based** user interface for easy interaction.
- **Memory**: Uses ChromaDB to store conversation history and context for the chatbot, allowing it to generate responses based on past interactions.
- **Model Selection**: You can choose between different Ollama models from the sidebar.
- **Chat History**: The chatbot remembers previous exchanges, allowing for more meaningful conversations.
- **Clear Chat History**: Clears both the session's chat history and ChromaDB's stored data.

## Requirements

- Python 3.7 or higher
- Streamlit
- Langchain (Ollama integration)
- ChromaDB
- OpenAI API Key (for embeddings in ChromaDB)


## Usage
Interact with the chatbot using the text input box. The chatbot will retain context from previous conversations, providing more relevant responses.

## Examples
File Upload and Contextual Responses
Upload .txt files to provide additional context for your chatbot interaction. For example:

Upload a document about "Climate Change."
Ask the chatbot: "What are the main causes of climate change?"
Contextual Memory with ChromaDB
The application saves chat history to ChromaDB, enabling contextual responses:

User: "Tell me about AI."
Bot: "AI stands for Artificial Intelligence..."
User: "And how does it relate to ChatGPT?"
Bot: "Building on our earlier discussion about AI..."

llama3.2:1b :
You: Can you help me with programming?
Bot: I'd be happy to help you with programming. What kind of programming are you working on, or what problem do you need help with? Are you a beginner looking for explanations and resources, or are you an experienced programmer trying to solve something specific? Let me know how I can assist you.

llama3.1:8b :
You: Can you help me with programming?
Bot: I'd be happy to help with your programming-related questions or problems. What type of programming are you working on (e.g., web development, mobile app development, machine learning, etc.) and what specific issue or task do you need assistance with?

## Installation Guide

Follow these steps to set up and run the project on your local machine:

Prerequisites:
- Python 3.8 or later installed on your system.
- A Git client (optional, for cloning the repository).

Steps:

1. Clone the Repository
Clone the project repository to your local machine:

git clone https://github.com/your-repository-url.git
cd your-repository-folder

2. Create a Virtual Environment
Create and activate a Python virtual environment to isolate dependencies:

- For Linux/Mac:
  python3 -m venv venv
  source venv/bin/activate

- For Windows:
  python -m venv venv
  venv\Scripts\activate

3. Install Dependencies
Use pip to install the required Python packages:

pip install -r requirements.txt

4. Set Environment Variables
Create a .env file in the root directory.
Add your OpenAI API key to the .env file:

OPENAI_API_KEY=your-openai-api-key

5. Run the Application
Start the Streamlit application:

streamlit run src/app.py

Access the Application:
Open your browser and go to the URL provided by Streamlit, usually http://localhost:8501.

Notes:
- Replace your-openai-api-key with your actual OpenAI API key.
- Ensure you have a stable internet connection for API calls.



## Clone the repository:
[https://github.com/your-repo/ollama-chatbot.git](https://github.com/TLAN145/chatbotv2.git)
