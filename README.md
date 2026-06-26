# Food Recommendation RAG System with ChromaDB

A Retrieval-Augmented Generation (RAG) system for semantic food search and AI-powered recommendations, built with ChromaDB, Sentence Transformers, and Google Gemini.

## Features

- **Semantic similarity search** — find food items by description, ingredients, or taste profile using vector embeddings (`all-MiniLM-L6-v2`)
- **Filtered search** — narrow results by cuisine type or calorie limit
- **Interactive CLI chatbot** — conversational food recommendations without an LLM
- **Enhanced RAG chatbot** — full RAG pipeline powered by Google Gemini for natural language responses
- **Advanced search** — multi-faceted queries combining semantic and metadata filters

## Project Structure

```
├── utils.py                  # Core ChromaDB utilities (load, embed, search)
├── interactive_search.py     # CLI chatbot (no LLM required)
├── enhanced_RAG_chatbot.py   # RAG chatbot powered by Google Gemini
├── advanced_search.py        # Advanced filtered search examples
├── utils.ipynb               # Notebook version of utils
├── chromaPractice.ipynb      # Exploration notebook
├── requirements.txt          # Python dependencies
└── .python-version           # Python version pin
```


## Usage

**Interactive search (no API key needed):**
```bash
python interactive_search.py
```

**Enhanced RAG chatbot (requires Gemini API key):**
```bash
python enhanced_RAG_chatbot.py
```

## Requirements 

- Python 3.12+
- Google Gemini API key (for the RAG chatbot only)
- See `requirements.txt` for the full dependency list

## Key Dependencies

| Package | Purpose |
|---|---|
| `chromadb` | Vector database |
| `sentence-transformers` | Text embeddings |
| `google-genai` | Gemini LLM integration |
| `langchain` / `langgraph` | Agent orchestration |
