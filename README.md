# AI Career Coach

AI Career Coach is a Flask-based web application designed to offer personalized career guidance through AI-driven resume analysis and coaching. The application parses PDF resumes, extracts relevant information using NLP techniques, and provides actionable career advice based on comprehensive resume summaries.

## Features
- **Resume Analysis & Summarization:** 
  - Extracts text from PDF resumes using PyPDF2.
  - Utilizes a custom text splitting method to efficiently process large documents.
  - Generates a concise resume summary using LangChain’s LLMChain and a custom prompt template.
- **Advanced Query Response:**
  - Implements a retrieval-based QA system with FAISS and HuggingFace embeddings.
  - Enables users to ask follow-up questions and get additional insights on their resumes.
- **Interactive Web Interface:**
  - Built with HTML/CSS, Tailwind CSS, and Framer Motion for smooth animations.
  - Provides intuitive screens for resume upload, analysis results, and querying.

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/mannatsingla22/ai-career-coach.git
   cd ai-career-coach
   ```

2. **Create a virtual environment and install dependencies**
   ```bash
   python -m venv venv
   source venv\Scripts\activate  # For Linux, `venv/bin/activate`
   pip install -r requirements.txt
   ```

3. Set up Environment Variables
   - Create a .env file (or set environment variables) for your OpenAI API key:
   ```ini
   OPENAI_API_KEY=your_openai_api_key
   ```

4. **Run the Flask application**
   ```bash
   python app.py
   ```

