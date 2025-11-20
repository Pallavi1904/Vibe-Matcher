# 🪩 Vibe Matcher — AI-Powered Fashion Recommender  

## ✨ Overview  
**Vibe Matcher** is a prototype recommendation system that matches a user’s *vibe query* (like “urban chic” or “cozy casual”) with fashion products based on their descriptions.  
It uses **OpenAI embeddings** and **cosine similarity** to find the top 3 products that best fit the vibe.   

---      

## 🧠 How It Works   
1. **Data Preparation:**  
   A small dataset (5–10 mock fashion products) with names, descriptions, and vibe tags is created using Pandas.  

2. **Embeddings Generation:**  
   Each product description is converted into an embedding vector using OpenAI’s `text-embedding-ada-002` model.  

3. **Vector Search (Cosine Similarity):**  
   User vibe queries are embedded and compared to product vectors using cosine similarity from scikit-learn.  

4. **Ranking & Output:**  
   Top 3 matching products are displayed with similarity scores.  
   If no strong match is found, a fallback message is returned.  

5. **Evaluation:**  
   - Three queries are tested and evaluated.  
   - “Good” match threshold: cosine similarity > 0.7  
   - Latency measured using `timeit` and plotted.  

---

## 🛠️ Tech Stack  
- **Python** 🐍  
- **Pandas** (Data Handling)  
- **scikit-learn** (Cosine Similarity)  
- **OpenAI API** (Embeddings)  
- **Matplotlib** (Visualization)  

---

## 🚀 Run the Notebook  
1. Open the `Vibe_Matcher.ipynb` file in **Google Colab** or **Jupyter Notebook**.  
2. Install dependencies:  
   ```bash
   pip install openai pandas scikit-learn matplotlib
---
