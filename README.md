📌 QA BOT USING WatsonX AI

📝 Overview

This project is a Question-Answering (QA) Bot powered by IBM WatsonX AI, LangChain, and ChromaDB. It allows users to upload PDF documents and query them using LLMs (Large Language Models) from IBM WatsonX AI. The bot processes user queries by retrieving relevant document segments and generating responses using AI models.

A Gradio web interface is implemented to enable seamless user interaction.

🚀 Features

✅ Leverages IBM WatsonX AI for text embedding and retrieval.✅ Uses LangChain for document loading, text chunking, and retrieval-based QA.✅ Integrates ChromaDB for vector storage and similarity search.✅ Supports PDF document uploads for knowledge extraction.✅ Gradio-powered web UI for easy interaction.✅ Automatic installation of required dependencies.

🔧 Installation

📌 Prerequisites

Ensure you have Python 3.11+ installed. You can install required dependencies using the following command:

pip install -r requirements.txt

Or manually install required packages:

pip install \
    gradio==4.44.0 \
    ibm-watsonx-ai==1.1.2 \
    langchain==0.2.11 \
    langchain-community==0.2.10 \
    langchain-ibm==0.1.11 \
    chromadb==0.4.24 \
    pypdf==4.3.1 \
    pydantic==2.9.1

⚙️ Configuration

Before running the bot, you need to set up IBM WatsonX AI Credentials. Follow these steps:

1️⃣ Create an IBM Cloud account and get API credentials for WatsonX AI.2️⃣ Save your credentials in a .env file:

IBM_API_KEY=your_api_key_here
IBM_PROJECT_ID=your_project_id_here
IBM_SERVICE_URL=your_service_url_here

▶️ Usage

Run the script using:

python qabot.py


🔍 How It Works:

1️⃣ Upload a PDF document through the web interface.2️⃣ The bot extracts text from the document and processes it into chunks.3️⃣ ChromaDB stores the vector embeddings for efficient retrieval.4️⃣ When a user asks a question, the system retrieves the most relevant text segments.5️⃣ IBM WatsonX AI generates a response based on the retrieved information.

📌 Demonstrating Chatbot Implementation in Colab & IBM Cloud

During my coursework on Coursera, I successfully implemented the chatbot within the IBM Cloud environment, where WatsonX AI was pre-integrated. This setup provided seamless access to AI capabilities without requiring manual API key configuration.

However, when attempting the same implementation in Google Colab, I encountered a limitation—IBM WatsonX requires an API key for authentication in external environments. Since my Coursera-provided IBM Cloud instance had pre-configured access, an API key was not required there.

Due to this restriction in Colab, I am unable to demonstrate the chatbot directly within this environment. Instead, I will provide screenshots from the IBM Cloud environment, showcasing the chatbot’s interface, query processing, and response generation, ensuring a clear demonstration of its capabilities.

🛠 Technologies Used

🔹 IBM WatsonX AI – for embedding and answering questions.

🔹 LangChain – for text processing and retrieval.

🔹 ChromaDB – for storing vector embeddings.

🔹 pypdf – for extracting text from PDFs.

🔹 Gradio – for building the web interface.
