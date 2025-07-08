# Semantic Search Engine Using Embeddings

A simple semantic search engine that finds similar text using AI embeddings. Instead of exact keyword matching, it understands the meaning behind your search queries.

## What's in this project?

- `SentenceTransformer.ipynb` - Learn the basics of sentence embeddings
- `SemanticSearchEngine.ipynb` - The full search engine you can run

## Quick Start

### 1. Set up your environment
```bash
# Create a virtual environment
python -m venv venv

# Activate it (macOS/Linux)
source venv/bin/activate
# Or on Windows: venv\Scripts\activate
```

### 2. Install the required packages
```bash
pip install sentence-transformers numpy scikit-learn matplotlib plotly jupyter
```

### 3. Run the search engine
```bash
jupyter notebook
```

Then open `SemanticSearchEngine.ipynb` and run all cells (Cell → Run All).

## How it works

The search engine converts text into numbers (embeddings) that capture meaning. When you search for "artificial intelligence", it finds documents about "machine learning" and "deep learning" even though those exact words aren't in your query.

### Example search results:
```
Query: "artificial intelligence and learning"
→ Machine learning algorithms can automatically learn patterns from data
→ Deep learning is a subset of machine learning that uses neural networks
```

## Try it yourself

The engine comes with sample documents about programming, AI, cybersecurity, and more. You can:

- **Add your own documents**: Just modify the `documents` list in the notebook
- **Change the model**: Use `model_name='all-mpnet-base-v2'` for potentially better results
- **Get more results**: Change `top_k=5` to get the top 5 matches instead of 3

## What you need

- Python 3.7+
- Jupyter Notebook
- Internet connection (to download the AI model on first run)

## Troubleshooting

- **First run is slow**: The AI model downloads automatically - just wait
- **Import errors**: Make sure you installed all packages in step 2
- **Memory issues**: The model needs about 1GB of RAM

That's it! The search engine is ready to use. You can now search through documents by meaning, not just exact words.
