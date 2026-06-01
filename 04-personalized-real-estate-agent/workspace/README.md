# 🏡 HomeMatch – Personalized real estate agent

**HomeMatch** is an AI-powered real estate assistant that transforms traditional listings into personalized recommendations based on each buyer’s unique preferences.

Built for **Future Homes Realty**, this application leverages **Large Language Models (LLMs)** and **vector search** to make property searching smarter and more human.

---

## Features

-  **LLM-Powered Listing Generation**  
  Automatically generates realistic and diverse real estate listings using GPT.

-  **Vector Database with Semantic Search**  
  Uses ChromaDB and OpenAI embeddings to semantically match listings to buyer preferences.

-  **Buyer Preference Understanding**  
  Interprets natural language preferences and uses them to find the best-fit homes.

-  **Personalized Descriptions**  
  Uses GPT to rewrite property descriptions in a tone and focus that resonates with the buyer — without changing factual details.

---

##  How to Run the Project

This project is designed to run in a **Jupyter Notebook**. Simply open `HomeMatch.ipynb` and run the cells step-by-step.

>  Note: You need an **OpenAI API key for Vocareum**, set in your environment.

---

##  Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
```

Or, install individually if needed:

```bash
pip install langchain openai chromadb tiktoken
```

No need for `sentence-transformers` in this version due to environment limitations.

---

##  Project Structure

```
HomeMatch/
├── HomeMatch.ipynb          ← Main Jupyter Notebook
├── listings_raw.txt         ← GPT-generated raw listings
├── listings.json            ← Parsed structured listings
├── requirements.txt         ← All dependencies
└── README.md                ← This file
```

---

##  Example Output

**Buyer Profile:**
```
A quiet neighborhood, good local schools, and convenient shopping options...
```

**Matched Listing:**
- Neighborhood: Green Oaks
- Price: $800,000
- Bedrooms: 3

**Personalized Description:**
> Welcome to this tranquil eco-conscious home in Green Oaks, perfect for families who value peace, sustainability, and walkable amenities...

---

##  Ideas for Future Work

-  Add listing photos + CLIP for image-based search
-  Build a simple front-end interface
-  Rank listings with a personalized score
