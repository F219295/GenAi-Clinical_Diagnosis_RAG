# 🩺 Clinical Diagnosis RAG Chat

An AI chatbot designed to **assist with clinical diagnosis** by combining powerful language models with medical case knowledge. It uses **Retrieval-Augmented Generation (RAG)** to give smarter, more accurate answers.

## 🔍 What It Does
- Combines **Bio_ClinicalBERT** embeddings with **FAISS** vector search for smart document retrieval.
- Uses **LLaMA-3.3-70b** (via Groq API) to generate reliable, medically informed responses.
- Supports **clinical flowcharts** and real **patient case studies**.
- Includes an **evaluation module** to measure how accurate and trustworthy the answers are.

## ⚙️ Tech Stack
- **Frontend**: Streamlit  
- **LLM**: LLaMA-3.3-70b via Groq API  
- **Embeddings**: Bio_ClinicalBERT  
- **Search Engine**: FAISS  
- **Backend Logic**: LangChain  

---

## 🚀 How to Get Started

### 1. Clone the Repo
```bash
git clone https://github.com/yourusername/clinical-rag-chat.git
cd clinical-rag-chat
```

### 2. Set Up a Virtual Environment
```bash
# For Mac/Linux
python -m venv venv
source venv/bin/activate

# For Windows
python -m venv venv
venv\Scripts\activate
```

### 3. Install All Required Packages
```bash
pip install -r requirements.txt
```

### 4. Add Your API Key
Create a `.env` file in the root folder and add your Groq API key like this:
```
GROQ_API_KEY=your_api_key_here
```

### 5. Run the App
```bash
streamlit run app.py
```

---

## 🗂️ Project Structure
```
clinical-rag-chat/
├── Diagnosis_flowchart/    # JSON flowcharts for diagnostics
├── Finished/               # Organized patient case studies
├── app.py                  # Main Streamlit app
├── evaluation.py           # Module to check model accuracy
├── requirements.txt        # Python dependencies
├── .env                    # Your API key lives here
└── README.md               # Project guide
```

---

## 🧑‍⚕️ How to Use It
1. Click **"🛠️ Initialize System"** to load medical data.
2. Ask any diagnostic or case-related question.
3. The chatbot finds relevant info and gives you a reliable answer.
4. Check the **evaluation scores** to see how accurate and faithful the response is.

---

## 📊 Evaluation Metrics
The evaluation tool helps you measure:
- **Hit Rate** – How often the right documents are retrieved.
- **Faithfulness** – How well the AI's answer matches the actual data.



