# Chat Interaction with ReAct Agent

This project is a Streamlit-based interactive chatbot application that leverages the power of multiple large language models (LLMs) and tools. It provides a configurable interface for users to interact with advanced AI agents for generating images, performing web searches, and analyzing web pages.

---

## Features

- **Multiple LLMs**: Supports OpenAI's GPT-4, Google's Gemini Pro, and Anthropic's Claude.
- **Image Generation**: Integrates DALL-E 3 and Stable Diffusion XL for generating images based on text prompts.
- **Search Engines**: Allows users to choose between DuckDuckGo and Tavily for web searches.
- **Web Scraping**: Provides webpage content analysis via BeautifulSoup.
- **Configurable Interface**: Users can customize the agent's behavior through a user-friendly Streamlit sidebar.

---

## Installation

### Prerequisites

1. Python 3.11
2. Virtual environment setup (recommended)

### Dependencies

Install the required Python packages:

```bash
pip install -r requirements.txt
```

The `requirements.txt` file should include the following (and their dependencies):

- `streamlit`
- `langchain`
- `langchain-openai`
- `langchain-google-genai`
- `langchain-community`
- `requests`
- `beautifulsoup4`
- `python-dotenv`

### Environment Variables

Create a `.env` file in the project root and add your API keys:

```env
openai_apikey=YOUR_OPENAI_API_KEY
google_apikey=YOUR_GOOGLE_API_KEY
anthropic_apikey=YOUR_ANTHROPIC_API_KEY
tavily_apikey=YOUR_TAVILY_API_KEY
stabilityai_apikey=YOUR_STABILITY_API_KEY
```

---

## Usage

1. **Run the Application**:

   ```bash
   streamlit run react_chat.py
   ```

2. **Configure the Agent**:

   Use the sidebar to select the desired language model, search engine, image generator, and web scraping tool.

3. **Interact**:

   - Enter your query in the chat input box.
   - View the AI agent's response in real-time.
   - Reset the chat history using the sidebar button.

---

## Project Structure

```plaintext
├── app.py                # Main Streamlit application
├── customtools.py        # Custom tools for image generation and web scraping
├── .env                  # Environment variables (not included in source control)
├── requirements.txt      # Python dependencies
├── img/                  # Directory for storing generated images
└── README.md             # Project documentation
```




