🧠 NeuroRest

A High-Precision Medical RAG System Powered by Qdrant
Problem-first. Retrieval-driven. Clinically grounded.

🚨 The Problem We Are Solving 
OBSTRUCTIVE SLEEP APNEA 
Obstructive Sleep Apnea is not a sleep disorder it is a silent public-health crisis.
Every night, oxygen deprivation starves the brain and heart, until one night the body never wakes up.
The death certificate says “died in sleep” — the real cause is never named.

Medical information is everywhere — but reliable, relevant, and context-aware medical answers are not.
In conditions like Obstructive Sleep Apnea (OSA):
Symptoms are often misunderstood or ignored
Information online is fragmented and shallow
Keyword-based search fails to capture clinical meaning
Doctors rely on structured knowledge.
Patients rely on Google.
That gap is dangerous.

💡 The Core Idea Behind NeuroRest
NeuroRest is not a chatbot.
It is not a generic LLM wrapper.
It is a Retrieval-Augmented Generation (RAG) system designed specifically for medical accuracy, where:
Every answer is grounded in retrieved medical context — not hallucination.
We treat retrieval as the most critical step, not generation.

🧠 Why Qdrant Is the Backbone and not just a tool
Medical RAG systems fail when retrieval fails.
We chose Qdrant because medical knowledge requires:
Dense semantic understanding, not keywords
Fast similarity search with strict control
Reliable vector storage at scale
Explainable retrieval scores
Qdrant gives us:
Precise vector similarity search
Deterministic, controllable retrieval
Clean cloud deployment
Full ownership of the retrieval layer
Without Qdrant, NeuroRest would collapse into a shallow QA system.

🏗️ System Design (End-to-End)

Curated Medical Text (OSA)
        ↓
Sentence Transformer Embeddings
        ↓
Qdrant Vector Database (Cloud)
        ↓
Top-K Semantic Retrieval
        ↓
Context-Grounded Answer Generation
Every step is explicit, inspectable, and reproducible.

🔍 What Makes NeuroRest Different
Most RAG demos:
Retrieve blindly
Generate confidently
Explain nothing
NeuroRest:
Retrieves only clinically relevant context
Exposes similarity scores
Separates retrieval logic from generation
Prioritizes trust over fluency

🧪 Demonstrated Capability
Input Question:
What are the symptoms of sleep apnea?
Retrieved Context (via Qdrant):
Loud snoring
Daytime sleepiness
Chronic fatigue
Final Answer (Context-Bound):
Loud snoring, excessive daytime sleepiness, and persistent fatigue are common symptoms of obstructive sleep apnea.
This answer is not invented — it is retrieval-backed.

⚙️ Tech Stack 
Qdrant Cloud – Vector retrieval engine
Sentence Transformers – Medical-grade embeddings
Python – Core logic
Google Colab – Fully runnable, zero setup
No unnecessary frameworks.
No abstraction for the sake of abstraction.

🚀 How to Run 
Open NeuroRest_Qdrant_VectorDB.ipynb in Google Colab
Install dependencies (single cell)
Paste Qdrant Cluster URL + API Key
Run cells top-to-bottom
Ask questions and observe:
Retrieved context
Similarity scores
Final grounded answer

🧠 Why This Matters to Qdrant
NeuroRest demonstrates:
A real RAG use case, not a toy example
Why vector databases are non-optional in healthcare AI
How Qdrant enables trustworthy retrieval, not just speed
This project can be extended to:
Clinical decision support
Medical literature search
Hospital knowledge systems

👩‍💻 Author
Bhumika Gaddam
2nd year BTech Undergraduate of Computer Science | AI & Applied Research
Focused on building accurate, explainable, retrieval-first AI systems
🏁 Final Statement
NeuroRest is built on a simple belief:
In medicine, retrieval quality matters more than generation fluency.
Qdrant makes that belief technically possible.
