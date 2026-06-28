# This project develops a Gen AI Exam Simulator to assist users in preparing for a Google Cloud Generative AI Leader Exam. It encompasses the following key stages:

PDF Processing:

Utilizes pdfplumber to extract questions from PDF documents.
These extracted questions are then structured and saved as JSON.
Pinecone Integration:

Questions are embedded into vector representations using SentenceTransformer.
These vectors are subsequently uploaded to a Pinecone vector database for efficient semantic search and retrieval.
Gradio Interface Development:

A user-friendly web interface is built with Gradio.
The interface allows users to load new questions, either generally or filtered by category, which are fetched from Pinecone.
The retrieved context is sent to a Groq model to generate multiple-choice questions (MCQs) in a specific JSON format, including options and explanations.
Users can answer these MCQs and receive immediate feedback on their correctness.
The project aims to provide an interactive, dynamic, and comprehensive exam simulation experience.
