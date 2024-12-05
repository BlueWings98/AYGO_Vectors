# AYGO_Vectors
This repo is a test of Langchain and Pinecone to use Vector Databases to query data faster from web pages or sources with too mucho content for the context window of a LLM.

# Files
Base File: Langchain that writes to a in memory database named Chroma.
Just Pinecone: A simple invocation of Pinecone, that is a hosted Vector Database.
Improved File: The same logic of the Base File but instead of using Chroma it uses Pinecone

# Results 
Base File: 9.29 Seconds
Just Pinecone: 11.55 Seconds
Improved File: 18.10 Seconds

# Conclusion
For localy run code a hosted database results in around double the time that an in memory batabase. Just a simple invocation of Pinecone is around 9 seconds.
Not recommended for small workloads but for larger ones where the stored data is important.
