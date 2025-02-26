# BITS_Dissertation
Application of Prompt Engineering using NLP in generating Programming Code


# 📌 Project Overview
This project explores the **application of Prompt Engineering and NLP** for **automatic code generation** in Python and Java. The primary objective is to **enhance code generation capabilities** using advanced **prompt engineering techniques** such as:
- **Zero-Shot Learning (ZSL)**
- **Few-Shot Learning (FSL)**
- **Chain-of-Thought (CoT)**
- **Tree-of-Thought (ToT)**
- **Instruction-Based Prompting**

**Retrieval-Augmented Generation (RAG)** is integrated with **FAISS indexing** to improve contextual accuracy before code generation.

---

## 🔍 Key Features
✔ **Utilizes multiple datasets**: CodeParrot, CodeXGLUE (Python & Java)  
✔ **Implements Prompt Engineering Techniques**  
✔ **Retrieval-Augmented Generation (RAG) with FAISS** for relevant context retrieval  
✔ **Fine-tuned models** on Python, Java, and CodeParrot dataset  
✔ **Uses CodeT5/FLAN-T5 for prompt refinement**  
✔ **Evaluates generated code using BLEU, ROUGE, and CodeBLEU**  
✔ **Streamlit UI Integration** (Prototype - Not Fully Functional)  

---

## 📂 Project Structure
```
📦 Project-Repo
 ┣ 📂 datasets/             # Python, Java, and CodeParrot datasets
 ┣ 📂 models/               # Pretrained and fine-tuned models
 ┣ 📂 notebooks/            # Google Colab Notebooks
 ┣ 📂 scripts/              # Python scripts for training and evaluation
 ┣ 📂 faiss_index/          # FAISS embeddings for code retrieval
 ┣ 📂 outputs/              # Generated code and evaluation metrics
 ┣ 📜 README.md             # Project Documentation
 ┣ 📜 requirements.txt      # Dependencies
 ┗ 📜 app.py                # Streamlit UI script (Prototype)
```

---

## 🛠️ Installation & Setup
To run this project, follow these steps:

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run Model Training
Train the fine-tuned model using:
```bash
python scripts/train_model.py
```

### 4️⃣ Run FAISS Retrieval
To index and retrieve relevant code snippets:
```bash
python scripts/faiss_retrieval.py
```

### 5️⃣ Run Streamlit UI
Launch the interactive UI (prototype):
```bash
streamlit run app.py
```

---

## 📊 Evaluation Metrics
The generated code is evaluated using the following metrics:
- **BLEU Score**: Measures the n-gram overlap between generated and reference code.
- **ROUGE Score**: Evaluates the recall-oriented similarity.
- **CodeBLEU Score**: Measures syntax correctness and code structure similarity.

---

## 🔬 Research & Findings
- Prompt engineering techniques significantly influence **code quality**.
- RAG with FAISS **improves contextual accuracy**.
- CodeT5/FLAN-T5 helps in **refining vague prompts**.
- The Streamlit-based chatbot **did not yield effective results** due to model limitations.

---

## 🚀 Future Work
- **Improve RAG retrieval quality** using better embeddings.
- **Experiment with GPT-4 & StarCoder** for better code generation.
- **Enhance prompt engineering techniques** with self-refinement.
- **Develop a more interactive and robust UI** for usability.


