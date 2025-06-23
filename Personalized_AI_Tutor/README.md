# 🧠 Personalized AI Tutor for Advanced NLP

[![Python](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)
[![Gradio](https://img.shields.io/badge/UI-Gradio-orange.svg)](https://www.gradio.app/)
[![LangChain](https://img.shields.io/badge/Framework-LangChain-brightgreen)](https://www.langchain.com/)
[![OpenAI](https://img.shields.io/badge/LLM-OpenAI-lightblue)](https://openai.com/)

> Interactive, topic-driven NLP tutor built using LLMs, retrieval-augmented generation, and Gradio.  
> Created by **Anirban Bose** for advanced learners exploring Natural Language Processing.


## 🚀 Features

- 📖 **Ask a Question (RAG)** — Retrieve and answer questions using vector search + LLM.
- 📚 **Personalized Quiz Engine** — Topic-wise MCQs with feedback and scoring.
- 🗣️ **Conversational Tutor** — Memory-aware chat agent for contextual dialogue.
- 🔍 **Reasoning Check (DNLI)** — Determine if a hypothesis logically follows from a premise.
- 🧠 **LLM Summarization** — Summarizes technical content for easier understanding.


## 🛠️ Tech Stack

| Layer         | Technology                                  |
|---------------|----------------------------------------------|
| LLM           | OpenAI GPT / ChatGPT                        |
| Framework     | LangChain                                   |
| UI            | Gradio                                      |
| Vector Store  | FAISS + HuggingFaceEmbeddings               |
| Datasets      | HuggingFace + Custom Topic Docs             |
| Libraries     | Transformers, NLTK, SentenceTransformers    |


## ⚙️ Installation

```bash
pip install -q gradio transformers datasets sentence-transformers langchain faiss-cpu \
                langchain-community trafilatura nltk langchain-openai openai
````

Then download required NLTK packages:

```python
import nltk
nltk.download("punkt")
```


## 🧪 How to Use

1. Clone the repo and open the notebook:

   ```bash
   git clone https://github.com/anirbanbose83/GenerativeAI_LLM.git
   cd personalized-ai-tutor
   ```

2. Run the notebook:
   `personalized_ai_tutor_gradio.ipynb`

3. Launch the app:

   ```python
   app.launch(share=True)
   ```


## 🧩 App Modules

### 📖 Ask a Question

Ask topic-related questions. Uses retrieval-augmented generation with LangChain + vector DB.

### 📚 Take a Quiz

Generates 4-option MCQs with immediate scoring and feedback.

### 🗣️ Conversational Tutor

Chat with an LLM using `ConversationBufferMemory` to maintain context.

### 🔍 Reasoning Check

DNLI-style entailment detection — classify hypothesis as:

* `entailment`
* `neutral`
* `contradiction`


## 📂 Project Structure

```
├── personalized_ai_tutor_gradio.ipynb     # Main notebook
└── README.md                              # This file
```


## ✅ Output Examples

* "What is LLM?" → LLM stands for...
* Quiz score: ✅ 4/5 Correct
* Reasoning: 🔎 **Result: Contradiction**


## 👤 Author

**Anirban Bose**
🎓 NUS MBA, Northwestern MSDS AI
💼 Head of Product Architecture and Design

