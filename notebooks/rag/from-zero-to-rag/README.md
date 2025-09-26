# From Zero to RAG: An Incremental, Hands-On Notebook

This folder contains a comprehensive RAG (Retrieval-Augmented Generation) tutorial that demonstrates how to build a complete RAG pipeline from scratch.

## Files

- **`prompt.poml`** - The structured POML (Prompt Orchestration Markup Language) file that defines the requirements and specifications for the RAG tutorial
- **`notebook.ipynb`** - The Jupyter notebook generated from the POML prompt, containing the complete hands-on RAG tutorial

## Generation Process

The `notebook.ipynb` was generated using **Claude Code based** on the detailed prompt specification in `prompt.poml`. This POML file contains:

- **Role definition** for a senior RAG SME and Jupyter notebook author
- **Comprehensive task description** for creating a beginner-friendly yet advanced RAG tutorial
- **Detailed constraints** including Python 3.10+ compatibility and open-source model requirements
- **Complete notebook structure** with 20+ sections covering everything from basic concepts to advanced techniques
- **Quality requirements** ensuring thorough documentation and reproducible code

## What You'll Learn

The notebook provides an incremental learning experience covering:

- RAG fundamentals and architecture
- TF-IDF and BM25 retrieval methods
- Semantic embeddings with open-source models
- Hybrid retrieval strategies
- Rank fusion techniques (RRF)
- Re-ranking with cross-encoders
- End-to-end RAG pipeline with OpenAI integration
- Evaluation methods and best practices

## Getting Started

### Prerequisites

Before running the notebook, you'll need to set up the following environment variables:

- **`HF_TOKEN`** - Hugging Face API token for accessing models and datasets
- **`OPENAI_API_KEY`** - OpenAI API key for the RAG pipeline integration

**Setting Environment Variables:**

**Recommended Method: Using a .env file**

Create a `.env` file in this directory (`/notebooks/rag/from-zero-to-rag/`) to store your API keys securely:

1. Create the `.env` file:
   ```bash
   touch .env
   ```

2. Add your API keys to the `.env` file:
   ```bash
   HF_TOKEN=your_hugging_face_token_here
   OPENAI_API_KEY=your_openai_api_key_here
   ```

3. The notebook will automatically load these variables using Python's `python-dotenv` library

**Alternative Methods:**

```bash
# Option 2: Export in your terminal session (temporary)
export HF_TOKEN="your_hugging_face_token_here"
export OPENAI_API_KEY="your_openai_api_key_here"

# Option 3: Add to your shell profile (~/.bashrc, ~/.zshrc, etc.)
echo 'export HF_TOKEN="your_hugging_face_token_here"' >> ~/.zshrc
echo 'export OPENAI_API_KEY="your_openai_api_key_here"' >> ~/.zshrc
source ~/.zshrc
```

**Important:** Make sure to add `.env` to your `.gitignore` file to avoid committing your API keys to version control.

**Getting API Keys:**
- **Hugging Face Token**: Visit [huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)
- **OpenAI API Key**: Visit [platform.openai.com/api-keys](https://platform.openai.com/api-keys)

### Running the Notebook

1. Ensure you have the required VS Code extensions installed (see repository root README)
2. Set up the environment variables as described above
3. Open `notebook.ipynb` in VS Code
4. Follow the step-by-step tutorial from the first cell
5. Each cell is thoroughly documented and ready to run

The notebook is designed to be self-contained and runnable as-is, with automatic dependency installation where needed.

Also available on [Kaggle](https://www.kaggle.com/code/gabe4ai/notebook) with free GPU access.