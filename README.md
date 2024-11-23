## Project: Q&A Chatbot with LangChain

### Overview
This project demonstrates the creation of an intelligent Q&A chatbot using LangChain. The chatbot processes lecture transcripts, generates embeddings, and provides a robust Q&A interface. It employs techniques like text splitting, vector storage, and prompt engineering to deliver accurate and context-aware responses.

### Features
- **Transcript Handling**: Supports uploading any lecture transcript for generating a Q&A interface. *(In this project, the Tableau course transcript was used.)*
- **Text Splitting**: Utilizes `MarkdownHeaderTextSplitter` and `TokenTextSplitter` for effective segmentation.
- **Embeddings & Vector Store**: 
  - **Chroma Database**: Used as the vector store for efficient retrieval. Benefits include its high-speed querying, support for various embedding models, and ease of integration with LangChain.
  - **Embedding Model**: Leveraged the `jinaai/jina-embeddings-v3` model for generating high-quality embeddings optimized for semantic understanding.
- **Custom Prompt Engineering**: Crafts prompts tailored for the chatbot's interactions.
- **Q&A Chain Integration**: Combines all components into a cohesive chain for end-user interactions.

### Prerequisites
- Python 3.8 or later
- API key for Huggingface API
- A `.env` file with the following configuration:
  ```
  HUGGINGFACEHUB_API_TOKEN=your_token_here
  ```

### Setup
1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Add your Huggingface API token to a `.env` file:
   ```
   HUGGINGFACEHUB_API_TOKEN=your_token_here
   ```
4. Run the Jupyter Notebook to execute the workflow.

### Usage
1. Upload any lecture transcript to the specified directory to generate a chatbot for querying it. *(In this project, the Tableau course transcript was used.)*
2. Execute the notebook cells step by step to preprocess the text, create embeddings, and initialize the chatbot.
3. Interact with the chatbot through the Q&A interface.

### Technologies Used
- **LangChain**: Framework for chaining language model prompts.
- **Huggingface API**: For generating embeddings and responses.
- **Chroma Database**: Provides fast and scalable vector storage for efficient information retrieval.
- **Python Libraries**: Includes tools for environment management, text processing, embeddings, and PDF handling.

### Files
- **Notebook**: Contains the implementation steps (`LangChain_Project_improved.ipynb`).
- **Transcript File**: A sample **Tableau course transcript** PDF is attached for chatbot training. You can replace it with any other transcript.
- **.env File**: Stores private Huggingface API tokens (user-provided).

### Future Improvements
- Add support for multilingual transcripts.
- Integrate more robust vector storage systems like Pinecone.
- Improve the Q&A interface with a web or mobile application.

---
