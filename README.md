

## Problem Statement

This project demonstrates how to use LangChain for Retrieval Augmented Generation (RAG) with a YouTube video. The problem is to efficiently retrieve relevant information from a video transcription and use it to answer questions.


## Methodology

1. **Install Dependencies**: Install necessary libraries such as LangChain, Pinecone, DocArray, PyPDF, and YouTube Transcript API.
2. **Download Transcript**: Use YouTube Transcript API to download the transcription of a YouTube video.
3. **Select LLM Model**: Choose and download the desired LLM model (e.g., llama3).
4. **Instantiate Models**: Initialize the LLM and embedding models.
5. **Load Transcription**: Use TextLoader to load the transcription.
6. **Split Document**: Split the transcription into chunks using RecursiveCharacterTextSplitter.
7. **Store in Vector Space**: Store the transcription content in a vector space using DocArrayInMemorySearch.
8. **Create Retriever**: Create a retriever to find similar vectors for context.
9. **Generate Conversation**: Use the retriever to generate context and answer questions based on the transcription content.

## Dataset

- **Source**: The dataset is a transcription of a YouTube video downloaded using YouTube Transcript API.
- **Size**: The size of the dataset depends on the length of the video transcription.
- **Features**: Key features include the text content of the video transcription.
- **Preprocessing**: The transcription is split into chunks and stored in a vector space for efficient retrieval.
