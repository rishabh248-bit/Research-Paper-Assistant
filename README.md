#  AI-Powered Research Paper Assistant

An intelligent NLP-based research paper assistant that enables semantic search over research papers and provides AI-powered insights including summaries, keyword extraction, entity recognition, similar paper recommendations, paper comparison, and research trend analysis.

The project uses Sentence Transformers and FAISS for semantic retrieval, combined with modern NLP models to help researchers explore academic literature more efficiently.

---

#  Features

-  Semantic search using natural language queries
-  AI-generated research paper summaries
-  Automatic keyword extraction
-  Named Entity Recognition (NER)
-  Similar paper recommendation
-  Research paper comparison
-  Research trend analysis across retrieved papers

---

#  Technologies Used

- Python
- Pandas
- NumPy
- Sentence Transformers
- FAISS
- Transformers (DistilBART)
- KeyBERT
- spaCy
- Scikit-learn

---

#  Dataset

This project uses the **ML-ArXiv-Papers** dataset containing over **117,000 machine learning research papers** with paper titles and abstracts.

---

#  How It Works

### 1. Data Preprocessing
- Load the dataset
- Remove missing values
- Combine title and abstract into a single text field

### 2. Semantic Embedding Generation
- Generate sentence embeddings using **all-MiniLM-L6-v2**
- Store embeddings for faster retrieval

### 3. FAISS Indexing
- Build a FAISS vector index
- Perform fast semantic similarity search

### 4. AI Summarization
- Generate concise summaries using **DistilBART**

### 5. Keyword Extraction
- Extract important research topics using **KeyBERT**

### 6. Named Entity Recognition
- Identify important entities such as organizations, technical terms, and research concepts using **spaCy**

### 7. Similar Paper Recommendation
- Recommend semantically related research papers using vector similarity.

### 8. Paper Comparison
Compare two research papers based on:
- AI-generated summaries
- Keyword overlap
- Cosine similarity
- Common and unique concepts

### 9. Research Trend Analysis
Analyze the retrieved papers to identify frequently occurring research topics and emerging trends.

---

#  Project Structure

```
Research-Paper-Assistant/
│
├── data/
│   ├── cleaned_papers.csv
│   ├── paper_embeddings.npy
│   └── paper_index.faiss
│
├── notebook/
│   └── Research_Paper_Assistant.ipynb
│
├── README.md
│
└── requirements.txt
```

---

#  Running the Project

1. Clone the repository

```
git clone <repository-link>
```

2. Install dependencies

```
pip install -r requirements.txt
```

3. Open the notebook

```
jupyter notebook
```

4. Run all notebook cells sequentially.

---

#  Project Workflow

```
User Query
      │
      ▼
Semantic Search (FAISS)
      │
      ▼
Top Relevant Papers
      │
      ├── AI Summary
      ├── Keyword Extraction
      ├── Named Entity Recognition
      ├── Similar Paper Recommendation
      ├── Paper Comparison
      └── Research Trend Analysis
```

---

#  Future Improvements

- Build a web application using Streamlit or Flask
- Add citation recommendation
- Integrate Large Language Models for conversational Q&A
- Support PDF upload and analysis
- Expand support beyond machine learning research papers

---

#  Author

**Rishabh Bhardwaj**

Computer Science Engineering Student

Interested in Artificial Intelligence, Machine Learning, Deep Learning, NLP, and Generative AI.