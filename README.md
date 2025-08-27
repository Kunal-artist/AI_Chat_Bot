# 🤖 Gemini-Powered RAG Language Tutor

A smart, conversational bot that remembers your mistakes and helps you learn a new language, one chat at a time.

---

## 🚀 Overview

This project is an intelligent command-line chatbot designed for language learners to practice their conversational skills. Unlike simple chatbots, this tutor uses a **Retrieval-Augmented Generation (RAG)** architecture to develop long-term memory of your past conversations. It learns from your mistakes, understands your proficiency level, and tailors new practice scenarios based on your history — ensuring a personalized and effective learning experience.

The bot provides real-time feedback on grammar, politeness, and context, and concludes each session with an intelligent summary of your performance, highlighting areas for improvement.

---

## ✨ Key Features

- **Personalized Scenarios with RAG**  
  The bot retrieves relevant memories from your past conversations to generate new, context-aware practice scenes. If you struggled with ordering coffee last time, it might test you on it again in a new way.

- **Real-Time, Intelligent Feedback**  
  Get instant analysis of your responses. The bot checks for grammatical errors, spelling, and contextual appropriateness. It’s also designed to recognize and correct impolite or vulgar language.

- **Smart Session Summaries**  
  At the end of each session, the bot provides a summary that analyzes patterns in your mistakes (e.g., “You consistently confuse noun genders”) and suggests what to focus on next.

- **Contextual Hints for Beginners**  
  If you're a beginner, the bot provides a list of relevant vocabulary and phrases to help you construct your response.

- **Modular Architecture**  
  Built with a clean, service-oriented structure that separates the LLM, database, and vector store, making it easy to maintain and extend.

---

## 🛠️ Tech Stack & Architecture

This project leverages modern AI tools and a robust architecture to create its intelligent behavior.

- **Core LLM**: Google Gemini 1.5 Pro (accessed via LiteLLM)  
- **Backend Logic**: Python  

**RAG Architecture:**
- **Vector Database**: FAISS for fast, in-memory semantic search  
- **Text Embeddings**: `sentence-transformers` to convert conversation text into vectors  
- **Persistent Storage**: SQLite to store conversation history and recorded mistakes  
- **Environment**: Designed to run seamlessly in Google Colab  

---

## 🔧 Setup & Usage

You can get the bot running in just a few steps using Google Colab.

### ✅ Prerequisites:

- A Google Account  
- A Google AI Studio (Gemini) API Key  
  > You can get one for free from [Google AI Studio](https://makersuite.google.com/)

---

### 🟢 Open in Colab:

1. Copy the final Python script into a new Google Colab notebook.

2. **Add API Key:**
   - In your Colab notebook, click the **🔑 (key)** icon in the left sidebar to open the *Secrets* tab.
   - Create a new secret with the name `GOOGLE_API_KEY` and paste your API key as the value.

3. **Run the Bot:**
   - Run the single code cell in the notebook. It will install all the required packages and start the bot.

4. **Interact:**
   - The bot will prompt you for your name, the language you want to learn, and your proficiency level directly in the output of the cell.
   - To end a session, simply type `quit` or `exit` and press Enter. The bot will then provide your session review.

---

Enjoy learning a new language with the help of an AI that actually remembers you! 🌍🗣️💬

