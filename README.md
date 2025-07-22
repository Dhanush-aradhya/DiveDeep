AI ResearchBot

AI ResearchBot is an AI-driven research assistant that retrieves, ranks, and summarizes research papers based on a user's query. It combines the power of web scraping and large language models (LLMs) to offer relevant results with minimal effort from the user. The interface is built using Streamlit and served via a Flask wrapper for better integration and launch flexibility.

---

## Setup Instructions (Locl Environment)

### 1. Download Project Files

Download all the project files and place them in a single directory on your system.

### 2. Set Up a Virtual Environment (Optional but Recommended)

Create a virtual environment:
```bash
python -m venv venv
```

Activate the virtual environment:

- **On Windows:**
```bash
venv\Scripts\activate
```

- **On macOS/Linux:**
```bash
source venv/bin/activate
```

### 3. Install Dependencies

Make sure you have Python installed, then run:
```bash
pip install -r requirements.txt
```

### 4. Add API Key

Create a `.env` file in the same directory as the code and add your API key:
```
GOOGLE_API_KEY=your_api_key_here
```

> **Note:** You can also paste your API key directly inside `main.py` for quick testing, but using a `.env` file is recommended for security.

### 5. Run the App

Start the Streamlit application:
```bash
streamlit run app.py
```

---

## Features

- **Multi-Agent Architecture**: Uses specialized agents for different tasks
- **Intelligent Ranking**: LLM-powered selection of most relevant papers
- **Caching System**: Stores results for faster repeated queries
- **Follow-up Q&A**: Interactive questioning about found papers
- **Academic Source Focus**: Targets scholarly databases and repositories
- **Modern UI**: Cyberpunk-themed Streamlit interface

## Project Structure

- `app.py` - Main Streamlit application interface
- `main.py` - Core logic with agent system
- `style.css` - Custom styling for the interface
- `requirements.txt` - Python dependencies
- `memory.json` - Cache storage for previous queries
- `.env` - Environment variables (create this file)

## Dependencies

- streamlit
- requests
- beautifulsoup4
- googlesearch-python
- fuzzywuzzy
- python-Levenshtein
- google-generativeai
- reportlab
- python-dotenv
