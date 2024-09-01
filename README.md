Building a Basic RAG Tutorial Using Gemini 1.5 Pro
To illustrate the RAG concept, we’ll create a simple Python-based implementation using the Gemini-1.5-Pro model. The code will involve:

![image](https://github.com/user-attachments/assets/286fb0e0-1adc-4924-9b80-1a76d6b29437)

1. First you need to import the libraries:
-google.generativeai for the Gemini model
-SentenceTransformer for creating embeddings
-cosine_similarty for measuring the similarity between two texts by calculating the angle between their vector representations.
-numpy for handling data

2. Now you can set up your Gemini API key with your own key.
   
3. Then, we initialise:
-LLM → Gemini model that I am using Gemini 1.5 pro but feel free to replace it with any other model you prefer such as Gemini 1.5 flash.
-Embeddings: We’ll create embeddings for our sample knowledge base.
-Knowlege Base: a simple list of facts about Paris.

4. Defining functions:
-retrieve_context: finds the most pertinent data from the knowledge base based on the query using cosine similarity.
-generate_response: uses Gemini to create an answer using the retrieved information and the Gemini LLM.
-rag_with_gemini: brings together the retrieval and generation processes to produce a final response.

5. To test the model, let’s test our RAG system with a simple query: ‘What can you tell me about Paris?’ The system effectively retrieved relevant information from our basic knowledge base about Paris and generates a comprehensive response.
