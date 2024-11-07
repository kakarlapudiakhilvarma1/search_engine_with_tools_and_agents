# 🔎 Search Engine with Tools & Agents

Welcome to the **Search Engine with Tools & Agents** app! This app allows users to interact with a chatbot that can search the web and external databases (like Arxiv and Wikipedia) to provide detailed, accurate responses to various questions. It integrates LangChain's agent system with **Groq's API** for language processing, combined with multiple search tools to provide results from sources like **DuckDuckGo**, **Arxiv**, and **Wikipedia**.

## Features ✨

- **💬 Chatbot Interaction**: Ask any question, and the chatbot will respond using language model processing.
- **🌐 Web Search Integration**: The app can search DuckDuckGo and external sources like **Wikipedia** and **Arxiv** to enhance the chatbot's responses.
- **🔄 Real-time Agent Action**: LangChain agents can perform multiple tasks, think through responses, and handle parsing errors gracefully.
- **💡 Groq API Support**: The chatbot is powered by **Groq’s Llama3-8b model** to process natural language and deliver high-quality answers.
- **👨‍💻 Interactive Streamlit UI**: The app is designed with a simple and interactive **Streamlit** interface for a seamless user experience.

## Tech Stack 🛠️

- **Streamlit**: A framework for building interactive web apps.
- **LangChain**: A powerful framework for developing language model applications.
- **Groq API**: Provides access to advanced **Llama3-8b** model for intelligent question answering.
- **Arxiv API**: Used for searching academic papers from Arxiv.org.
- **Wikipedia API**: Retrieves information from Wikipedia to answer general knowledge questions.
- **DuckDuckGo Search**: Searches the web using DuckDuckGo for additional data or answers.

## Installation ⚙️

### 1. Clone the Repository
Clone this repository to your local machine:
```bash
git clone https://github.com/your-username/langchain-chat-with-search.git
cd langchain-chat-with-search
```

### 2. Install Dependencies
Ensure Python 3.7+ is installed. Then, install the necessary dependencies:
```bash
pip install -r requirements.txt
```

### 3. Setup Environment Variables
The app uses **Groq API** for model processing. Create a `.env` file in the project root directory and add your API key:

```bash
GROQ_API_KEY=your_groq_api_key
```

You can also enter your **Groq API Key** directly into the sidebar input of the app.

### 4. Run the App 🚀
Once you've installed the dependencies and set up the `.env` file, you can run the Streamlit app:

```bash
streamlit run app.py
```

Visit [http://localhost:8501](http://localhost:8501) in your browser to interact with the chatbot.

## Usage 📝

1. **Enter your question**: Type any question into the chat box (e.g., "What is machine learning?").
2. **The chatbot will respond**: The app uses LangChain agents, which query **DuckDuckGo**, **Arxiv**, or **Wikipedia** if needed, to provide detailed answers.
3. **Interact with the chatbot**: Ask follow-up questions or request more details. The chatbot will handle complex queries by leveraging multiple search tools.
4. **View the thought process**: You can see the thought process and actions of the agent in real-time as it searches and reasons about the question.

## Example Questions ❓

- "What is machine learning?"
- "Tell me about the latest research on AI from Arxiv."
- "Explain quantum computing in simple terms."
- "What are the key differences between supervised and unsupervised learning?"

## Project Structure 🗂️

```plaintext
langchain-chat-with-search/
│
├── app.py                    # Main Streamlit app file
├── requirements.txt          # List of dependencies
├── .env                      # File to store API keys (e.g., GROQ_API_KEY)
├── README.md                 # Project documentation
└── assets/
    └── (optional)            # Folder for storing assets (e.g., images, icons)
```

## Screenshots 📸

![LangChain Chat with Search](screenshots/chat_with_search.png)
*Example of the LangChain chatbot interacting with the user and performing web searches.*

## Contributing 🤝

We welcome contributions to improve this project! If you'd like to contribute, follow these steps:

1. Fork the repository.
2. Create a new branch for your changes.
3. Implement your changes.
4. Submit a pull request explaining the changes you've made.

## Acknowledgements 🙏

- **LangChain**: For building the powerful framework that integrates language models and external tools.
- **Groq API**: For providing the **Llama3-8b** model for language processing.
- **Arxiv API**: For enabling access to scholarly papers and research.
- **Wikipedia API**: For integrating knowledge from Wikipedia.
- **DuckDuckGo Search**: For web searches and additional data retrieval.

---

**Note**: Ensure you provide a valid **Groq API Key** to make the search and response generation functional. 🔑

---

This `README.md` provides a detailed overview of how to set up, use, and contribute to the app. It also includes explanations of features, the tech stack, and setup instructions.
