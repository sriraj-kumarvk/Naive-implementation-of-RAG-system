**Simple RAG(Retrieval Augmented Generation) system**

***Overview***

This code Implements a simple Retrieval-Augmented Generation (RAG) system for processing and querying text documents. The complete modules aim to get an understanding a naive implementation without using a vector db.

***Components***



1.   Installing required libraries - The main libraries include components of building RAG, like text splitters, openai, runnables, transformers, prompt etc
2.   Importing relevant libraries - The main libraries include components of building RAG, like text splitters, openai, runnables, transformers, prompt etc
3.   Import tokens - Load the documents/files from the directory from which we want to retrieve the responses.
4.   Chunker - Create chunks of the documents, every chunk will have a chunk ID stored in a document ID , we can define the chunk size
5.   Embedding - Use openai model to create embeddings of the chunks created above
6.   Similarity score - Retreiver class contains a cosine similarity function which will generate a similarity score between the document embeddings and the prompt. The top 3 embeddings which have a high similarity score will be retreiver by the retriever.
7.   LLM - The openai gpt model will take the retriever output and the prompt as the user query and return the output response.


***Benefits of the code***
1.   Simple implementation of text chunking and retrieval
2.   Modularized structure
3.   Scalable
4.   Processing History, so that LLM can continue conversation

***Further improvements***
1.   Implement advanced text splitters
2.   Vector db approach for efficient storage of embedings
3.   Auto processing of history

