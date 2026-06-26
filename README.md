Movie RAG Chatbot :
A simple Retrieval-Augmented Generation (RAG) chatbot that helps users explore a movie dataset through natural language. Instead of relying only on the language model's knowledge, the chatbot retrieves relevant movie information from a vector database and uses it to generate accurate, context-aware responses.
This project was built to learn and demonstrate the complete RAG workflow using LangChain, Hugging Face embeddings, ChromaDB, and Groq LLM.

What the chatbot can do :
1. Answer questions about movies using the provided dataset
2.Recommend movies based on genre, plot, or user preferences
3.Perform semantic search instead of simple keyword matching
4.Retrieve relevant movie information before generating responses
5.Maintain short conversation history for follow-up questions

Tech Stack :
1. Python
2.LangChain
3.Hugging Face Embeddings
4.ChromaDB
5.Groq LLM
6.Pandas
7.Jupyter Notebook

How it works :

1. Load the movie dataset.
2. Convert each movie into a document.
3. Split documents into smaller chunks.
4. Generate embeddings using a Hugging Face embedding model.
5. Store the embeddings in ChromaDB.
6. Retrieve the most relevant movie information based on the user's query.
7. Provide the retrieved context to the Groq LLM.
8. Generate a context-aware response.

Example Questions :

1.Recommend sci-fi movies similar to Interstellar.
2.What genre is The Dark Knight?
3.Suggest comedy movies released after 2018.
4.Who directed Inception?
5.Give me movies with high IMDb ratings.

Current Constraints :

This project is intended as a learning implementation of RAG, so it has a few limitations:

- Responses are limited to the movies available in the dataset.
- Recommendation quality depends on the completeness of the dataset.
- Conversation memory is short-term and resets when the session ends.
- No web search or live movie information is supported.
- The chatbot cannot answer questions about movies that are not present in the vector database.

Getting Started :

1.Clone the repository

```bash
git clone https://github.com/your-username/movie-rag-chatbot.git
cd movie-rag-chatbot
```

2.Install dependencies

```bash
pip install -r requirements.txt
```

3.Create a `.env` file

```env
GROQ_API_KEY=your_api_key_here
```

4.Run the notebook

```bash
jupyter notebook
```

Future Improvements :

1.Build a Streamlit web interface
2. Add hybrid search (keyword + semantic search)
3.Integrate the TMDB API for live movie information
4.Improve conversation memory
5.Support filtering by year, rating, language, and cast
6.Deploy the application on the cloud

License :

This project is licensed under the MIT License.
