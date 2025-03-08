CodeBase Search Using RAG (Retrieval-Augmented Generation)
Project Overview

This project is a Codebase Q&A Chatbot built using Retrieval-Augmented Generation (RAG) that enables users to ask questions related to their codebase. It is designed to search through large code repositories, extract relevant code snippets, and generate contextual answers using an advanced language model.

The chatbot combines:

✅ File-to-text conversion (converting all code files to text)

✅ FAISS-based embedding search (using sentence embeddings to retrieve relevant code chunks)

✅ RAG (Retrieval-Augmented Generation) for generating accurate and contextual answers

✅ Gradio interface for an easy-to-use chat UI
Folder Structure
├── corpus.txt                  # Combined text corpus from all code files
├── chunks.txt                  # Split text chunks for embeddings
├── index.faiss                 # FAISS index for fast retrieval
├── app.py                      # Gradio-based Chatbot Interface
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
├── src/
│   ├── convert_to_txt.py        # Script to convert code files to text
│   ├── embedding.py             # Script to create embeddings
│   ├── indexer.py               # Script to create FAISS index
│   ├── generator.py             # RAG-based text generation
│   ├── chatbot.py               # Chatbot logic

How It Works

1. Clone the Repository
git clone https://github.com/your-username/codebase-search-rag.git
cd codebase-search-rag
2. Install Dependencies
pip install -r requirements.txt
3. Convert Code Files to Text
python src/convert_to_txt.py
4. Generate Embeddings and Create FAISS Index
python src/embedding.py
This will generate:

✅ chunks.txt containing text chunks

✅ index.faiss containing the FAISS index
5. Launch the Chatbot
Finally, launch the chatbot interface.
python app.py

Technologies Used

Technology                                    Purpose
FAISS                                         Fast similarity search for embeddings
Sentence Transformers                         Text embedding generation
Gradio                                        Web-based chatbot interface
Huggingface Transformers                      Answer generation model

