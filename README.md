# QA-with-LlamaIndex-HuggingFace

# 🧠  Q&A with LlamaIndex + HuggingFace

This project extracts answers to natural language questions about skin cancer types using a PDF document and LlamaIndex (formerly GPT Index). It uses open-source HuggingFace embeddings and language models, avoiding the OpenAI API.

## 📄 Document Used

skin cancer types.pdf: An academic chapter detailing various types of skin cancer. This project uses this PDF as a sample input—you can replace it with your own document and update the query accordingly in the code.
## ⚙️ Tech Stack

- LlamaIndex
- HuggingFace Transformers
- sentence-transformers
- Python 3.11
- Google Colab

## 🚀 How It Works

1. Load and read the PDF using `SimpleDirectoryReader`.
2. Generate embeddings using `sentence-transformers/all-MiniLM-L6-v2`.
3. Use HuggingFace model (e.g., `tiiuae/falcon-rw-1b` or `flan-t5-small`) for query responses.
4. Ask a natural question like _“What are the types of skin cancer?”_ and get a concise answer from the content.

## 🧪 Sample Output

**Q**: What are the types of skin cancer?

**A**: Basal cell carcinoma, squamous cell carcinoma, melanoma, cutaneous T-cell lymphoma, Merkel cell carcinoma, and Kaposi carcinoma.

## 📦 Setup Instructions

Install requirements:
```bash
pip install llama-index sentence-transformers transformers
