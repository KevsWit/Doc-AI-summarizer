# **Doc AI summarizer** 📝🤖  
🚀 **AI-powered Multi-Agent RAG system for intelligent document querying with fact verification**  

![Doc AI summarizer Cover Image](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/zSuj0yrlvjcVkkbW4frkNA/docchat-landing-page.png)

---

## **📌 Overview**  

**Doc AI summarizer** is a **multi-agent Retrieval-Augmented Generation (RAG) system** designed to help users query **long, complex documents** with **accurate, fact-verified answers**. Unlike traditional chatbots like **ChatGPT or DeepSeek**, which **hallucinate responses and struggle with structured data**, Doc AI summarizer **retrieves, verifies, and corrects** answers before delivering them.  

💡 **Key Features:**  
✅ **Multi-Agent System** – A **Research Agent** generates answers, while a **Verification Agent** fact-checks responses.  
✅ **Hybrid Retrieval** – Uses **BM25 and vector search** to find the most relevant content.  
✅ **Handles Multiple Documents** – Selects the most relevant document even when multiple files are uploaded.  
✅ **Scope Detection** – Prevents hallucinations by **rejecting irrelevant queries**.  
✅ **Fact Verification** – Ensures responses are accurate before presenting them to the user.  
✅ **Web Interface with Gradio** – Allowing seamless document upload and question-answering.  

---

## **🎥 Demo Video**  

📹 **[Click here to watch the DocChat demo](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/zyARt3f3bnm5T-6C4AE3mw/docchat-demo.mp4)**  
*(Opens in a new tab)*

---

## **🛠️ How Doc AI summarizer Works**  

### **1️⃣ Query Processing & Scope Analysis**  
- Users **upload documents** and **ask a question**.  
- Doc AI summarizer **analyzes query relevance** and determines if the question is **within scope**.  
- If the query is **irrelevant**, Doc AI summarizer **rejects it** instead of generating hallucinated responses.  

### **2️⃣ Multi-Agent Research & Retrieval**  
- **Docling** parses documents into a structured format (Markdown, JSON).  
- **LangChain & ChromaDB** handle **hybrid retrieval** (BM25 + vector embeddings).  
- Even when **multiple documents** are uploaded, **Doc AI summarizer finds the most relevant sections** dynamically.  

### **3️⃣ Answer Generation & Verification**  
- **Research Agent** generates an answer using retrieved content.  
- **Verification Agent** cross-checks the response against the source document.  
- If **verification fails**, a **self-correction loop** re-runs retrieval and research.  

### **4️⃣ Response Finalization**  
- **If the answer passes verification**, it is displayed to the user.  
- **If the question is out of scope**, Doc AI summarizer informs the user instead of hallucinating.  

---

## **🎯 Why Use Doc AI summarizer Instead of ChatGPT or DeepSeek?**  

| Feature | **ChatGPT/DeepSeek** ❌ | **Doc AI summarizer** ✅ |
|---------|-----------------|---------|
| Retrieves from uploaded documents | ❌ No | ✅ Yes |
| Handles multiple documents | ❌ No | ✅ Yes |
| Extracts structured data from PDFs | ❌ No | ✅ Yes |
| Prevents hallucinations | ❌ No | ✅ Yes |
| Fact-checks answers | ❌ No | ✅ Yes |
| Detects out-of-scope queries | ❌ No | ✅ Yes |

🚀 **Doc AI summarizer is built for enterprise-grade document intelligence, research, and compliance workflows.**  

---

## **📦 Installation**  

### **1️⃣ Clone the Repository**  
```bash
git clone https://github.com/KevsWit/Doc-AI-summarizer.git docchat
cd docchat
```

### **2️⃣ Set Up Virtual Environment**  
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### **3️⃣ Install Dependencies**  
```bash
pip install -r requirements.txt
```

### **4️⃣ Set Up API Keys**  
Doc AI summarizer requires an OpenAI API key for processing. Add it to a `.env` file:
```bash
OPENAI_API_KEY=your-api-key-here
```


### **5️⃣ Run the Application as Administrator** 
```bash
python app.py
```

Doc AI summarizer will be accessible at `http://localhost:7860`.


## 🖥️ Usage Guide  

1️⃣ **Upload one or more documents** (PDF, DOCX, TXT, Markdown).  

2️⃣ **Enter a question** related to the document.  

3️⃣ **Click "Submit"** – Doc AI summarizer retrieves, analyzes, and verifies the response.  

4️⃣ **Review the answer & verification report** for confidence.  

5️⃣ **If the question is out of scope**, Doc AI summarizer will inform you instead of fabricating an answer.  


## 🤝 Contributing  

Want to **improve Doc AI summarizer**? Feel free to:  

- **Fork the repo**  
- **Create a new branch** (`feature-xyz`)  
- **Commit your changes**  
- **Submit a PR (Pull Request)**  

We welcome contributions from **AI/NLP enthusiasts, researchers, and developers!** 🚀  

---

## 📜 License  

This project is licensed under a Customed Non-Commercial License – check LICENSE for more details.

---

## 💬 Contact & Support  

📧 **Email:** [kev.gcastillo@outlook.com]  

