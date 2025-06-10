# 🚀 RAG-Powered Resume Analysis Tool 📄✨

[](https://www.google.com/search?q=https://huggingface.co/spaces/abhi935680/resume-analyzer-rag-app)
[](https://streamlit.io/)
[](https://www.google.com/search?q=LICENSE)

-----

## 🌟 Overview

Tired of manually sifting through piles of resumes? 😩 Our **RAG-Powered Resume Analysis Tool** is here to revolutionize the hiring process\! This intelligent application leverages cutting-edge AI to quickly and accurately analyze resumes against job descriptions, helping recruiters find the perfect candidates faster. It also provides an interactive chat interface, allowing you to ask questions directly about the resume content.

-----

## ✨ Key Features

  * **⚡ Swift Resume-Job Matching:** Get instant compatibility analysis between a resume and a job description.
  * **🎯 Skill Identification:** Automatically highlights matched and unmatched skills based on your job requirements.
  * **🗣️ Interactive Chat Interface:** Chat directly with the resume content to extract specific information or clarify details.
  * **🚀 Powered by RAG & Groq:** Utilizes a Retrieval Augmented Generation (RAG) architecture with Groq's lightning-fast LLM inference for quick and accurate responses.
  * **📊 User-Friendly Frontend:** Built with Streamlit for an intuitive and interactive experience.

-----

## 🛠️ How It Works (The Magic Behind the Scenes)

This application orchestrates a powerful **RAG pipeline**:

1.  **📥 Data Ingestion:** When you upload a resume (PDF), it's loaded and intelligently split into smaller, manageable **chunks**.
2.  **🧠 Embedding & Vectorization:** These chunks are then converted into numerical representations (embeddings) using **HuggingFace Embeddings** and stored in a **FAISS** vector store. This creates a searchable knowledge base of the resume.
3.  **🔍 Intelligent Retrieval:** When you ask a question or request an analysis, relevant chunks are retrieved from the vector store based on their similarity to your query.
4.  **💡 Augmented Generation:** These retrieved chunks, along with your job description, are fed to **Groq's powerful LLM**. The LLM then generates a comprehensive analysis or answers your questions, grounded in the resume's actual content.



## ▶️ Live Demo

Experience the tool in action\! Click the badge below to visit our live demo hosted on Hugging Face Spaces:

[](https://www.google.com/search?q=https://huggingface.co/spaces/abhi935680/resume-analyzer-rag-app)


## 🚀 Getting Started (Run Locally)

Want to dive into the code and run it on your machine? Follow these simple steps:

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME.git
    cd YOUR_REPOSITORY_NAME
    ```

    *(Replace `YOUR_GITHUB_USERNAME` and `YOUR_REPOSITORY_NAME` with your actual GitHub details.)*

2.  **Set Up a Virtual Environment:**

    ```bash
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```

3.  **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure Environment Variables:**

      * Create a file named `.env` in the root of your project directory.
      * Add your Groq API Key to this file:
        ```
        GROQ_API_KEY="your_groq_api_key_here"
        ```
      * **Important:** Replace `"your_groq_api_key_here"` with your actual API key. Make sure `.env` is listed in your `.gitignore` file for security\!

5.  **Run the Streamlit Application:**

    ```bash
    streamlit run app.py
    ```

    Your application should open in your default web browser\! 🌐

-----

## 📁 Project Structure

```
.
├── app.py                  # Main Streamlit application entry point
├── requirements.txt        # Python dependencies
├── .env.example            # Example for setting environment variables (you create .env)
├── LICENSE                 # Project license (MIT)
├── backend/
│   ├── __init__.py
│   ├── analysis.py         # LLM interaction, prompt engineering, resume analysis logic
│   ├── pdf_ingestion.py    # PDF loading and text chunking
│   └── vector_store.py     # Embeddings and FAISS vector store creation
└── frontend/
    ├── __init__.py
    ├── main_app.py         # Handles resume/job description upload and analysis display
    └── chat_interface.py   # Manages the conversational chat with the resume
```

-----

## 💻 Tech Stack

  * **Framework:** 🐍 **Streamlit** (Frontend) & 🦜️🔗 **LangChain** (Backend Orchestration)
  * **LLM Provider:** ⚡ **Groq** (`mixtral-8x7b-32768`) for ultra-fast inference
  * **Embeddings:** 🤝 **HuggingFace Embeddings** (`sentence-transformers/all-mpnet-base-v2`)
  * **Vector Database:** 🤖 **FAISS** (Facebook AI Similarity Search)
  * **PDF Processing:** 📄 **PyPDFLoader**
  * **Environment Management:** dotenv
  * **Version Control:** ➕ **Git** & **GitHub**

-----

## 🔮 Future Enhancements

  * **Multi-Resume Analysis:** Allow comparing multiple resumes simultaneously.
  * **Resume Scoring:** Implement a more robust scoring system for compatibility.
  * **Skill Gap Analysis:** Provide detailed reports on missing skills and suggest learning paths.
  * **Persistent Vector Store:** Save and load vector stores to avoid re-ingestion.
  * **Deployment Monitoring:** Integrate more advanced monitoring tools for production.

-----

## 🤝 Contributing

Contributions are welcome\! If you have ideas for improvements or new features, feel free to:

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/YourFeature`).
3.  Make your changes.
4.  Commit your changes (`git commit -m 'Add new feature'`).
5.  Push to the branch (`git push origin feature/YourFeature`).
6.  Open a Pull Request.

-----

## 📄 License

This project is open-sourced under the **MIT License**. See the `LICENSE` file for more details.

-----

## 📬 Connect with Me

Have questions, suggestions, or just want to connect? Feel free to reach out\!
