Here’s a draft for your README file with icons and relevant changes for your Honeywell Hackathon project:

---

# 🔥 Honeywell Hackathon Project: Fire Solutions RAG Chatbot

![LangChain](https://img.shields.io/badge/Framework-LangChain-blue)
![Streamlit](https://img.shields.io/badge/UI-Streamlit-brightgreen)
![Google Gen AI](https://img.shields.io/badge/API-Google%20Generative%20AI-red)

## 💡 Overview

This project was developed during the Honeywell Hackathon, where we built a **Retrieval-Augmented Generation (RAG) Chatbot** for answering questions about **fire safety solutions**. Using **Google Gen AI** and **LangChain**, the chatbot can interact with users based on PDF documents related to fire solutions, providing relevant and accurate responses.

### 🔧 Technologies Used:
- **Streamlit**: For creating the user interface.
- **Google Generative AI**: To generate and embed contextual answers.
- **LangChain**: For managing the chatbot workflow.
- **FAISS**: To store and query document embeddings for similarity search.
- **PyPDF2**: To extract text from PDF files.
- **Python**: For backend development.

## 🚀 Features
- **PDF Upload & Processing**: Upload multiple PDF files to be analyzed.
- **RAG-Based Q&A**: Ask questions based on fire safety PDFs. If the answer is in the document, it provides a detailed response; if not, the bot indicates that the answer is unavailable in the provided context.
- **Custom Embedding Search**: Uses **Google Generative AI Embeddings** to enhance document search accuracy.

## 🛠️ How It Works

1. **PDF Text Extraction**: Extracts text from uploaded PDFs using `PyPDF2`.
2. **Text Chunking**: Splits the extracted text into manageable chunks with `LangChain`'s `RecursiveCharacterTextSplitter`.
3. **Embedding Creation**: Converts text chunks into embeddings using **Google Generative AI Embeddings**.
4. **Document Storage**: Stores the document chunks in **FAISS** for efficient similarity search.
5. **Conversational Chain**: Handles user queries by retrieving relevant document chunks and generating responses using **LangChain** and **Google Generative AI**.
6. **Interactive UI**: A clean, user-friendly interface built with **Streamlit** for seamless interaction.

## 🖥️ Usage

### 1. Clone the repository:
```bash
git clone https://github.com/YourUsername/YourRepo.git
cd YourRepo
```

### 2. Install dependencies:
```bash
pip install -r requirements.txt
```

### 3. Set up environment variables:
Create a `.env` file with your **Google API Key**:
```
GOOGLE_API_KEY=your-google-api-key
```

### 4. Run the application:
```bash
streamlit run app.py
```

### 5. Upload PDFs & Ask Questions:
- Upload your fire solutions PDF files.
- Ask questions, and the chatbot will provide context-aware answers.

## 📝 Example Questions
- "What are the fire safety regulations for commercial buildings?"
- "What is the ideal temperature range for fire alarms?"

## 📂 Project Structure

```
.
├── app.py                 # Main Streamlit app
├── vectorstore/           # FAISS vector storage
├── .env                   # API Key configuration
├── requirements.txt       # Project dependencies
└── README.md              # Project documentation
```

## 🔧 Future Improvements
- Add more advanced error handling and conversational features.
- Enhance support for non-PDF document formats.
- Include multi-language support for broader accessibility.

---

Feel free to adjust any specific sections, including icons and shields.