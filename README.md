# KultuRAG – An AI-Powered Language Learning Assistant
AI-powered language learning assistant for German that uses a RAG pipeline to create interactive, culturally-grounded exercises

[Deutsch](README.de.md) | [English](README.md)

This project is a web application designed as a cultural and interactive assistant for German language learners. Instead of generic content, KultuRAG creates learning materials based on cultural context and enriched with authentic language examples.

---

## Concept & Architecture

The application uses a **RAG** approach to ensure the quality and relevance of the generated content:

- **Contextual Enrichment:** A user query is first sent to the Wikipedia API to retrieve culturally relevant information in German.  
- **Authentic Language Examples:** In parallel, a retriever searches a Qdrant vector database. This database was populated with thousands of authentic German sentences from the Tatoeba corpus to provide the model with examples of natural language use.  
- **Content Generation:** The collected information, along with the user query, is packaged into a structured prompt for the Gemini model via Vertex AI. The LLM then generates a complete didactic block: reading text, vocabulary list, interactive exercise, and additional practice formats (writing, listening, speaking).  
- **Interactivity:** The application provides text-to-speech and speech-to-text functions and gives learners pedagogical feedback on their responses.  

---

## Applied Technologies & Skills

- **Frameworks & Libraries:** Python, LangChain, Hugging Face (Transformers, Datasets, TRL, PEFT), Google Vertex AI, PyTorch, FastAPI, Streamlit, Pandas, Uvicorn, MatPlotLib, Seaborn, Torch, Gradio  
- **Architectures & Techniques:** Retrieval-Augmented Generation, Agentic AI  
- **LLMs:** Google Gemini  

---

## Infrastructure & Tools

- **Vector Databases:** Qdrant  
- **APIs:** Google Cloud (Speech-to-Text, Text-to-Speech), Wikipedia  
- **Deployment:** Google Colab, Ngrok, Streamlit, FastAPI, GitHub.

---

## Demo
(1.png)

(2.png)

(3.png)

(4.png)

[▶️ Listen to sample](46cc27041fa015f25dac17c6f52933f7813781ed45f98960a26e44ff)
