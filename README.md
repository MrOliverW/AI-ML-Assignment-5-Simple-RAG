AI-ML-Assignment-5-Simple-RAG
Oliver Warlick
YouTube Video: 

Generation LLM used: Simulated LLM
Purpose:Receives the augmented prompt (query + context) and synthesizes the final, coherent answer.
Key Characteristic: Behavior was simulated to replicate the instruction-following capability of models like GPT-4 or fine-tuned Llama/T5 models.

Embedding Model used: all-MiniLM-L6-v2
Purpose: Converts text chunks and the user query into 384-dimensional dense vector embeddings.
Key Characteristic: A highly efficient, fast, and lightweight Sentence Transformer model from Hugging Face, suitable for local deployment.


Retrieval process summary:
Factual - Chunk 0
Foil/General - Chunk 1
Synthesis - Chunk 0 & 1

Result analysis: The RAG system successfully mitigated the risk of hallucination and ensured factual grounding by enforcing two core RAG principles - Grounding & Refusal/Boundary Setting.

By setting the scope of the RAG system to be very narrow and focused on relevant chunks while applying strict prompt templates the ability for the LLM to hallucinate or provide faulty information was contained.
