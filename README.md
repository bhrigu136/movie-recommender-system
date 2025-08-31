# 🎬 Movie Recommendation System

A **Content-Based Movie Recommendation System** that suggests movies similar to the one selected by the user.  
The project uses **textual metadata** (genres, cast, crew, overview, keywords) from the TMDB dataset, applies **CountVectorizer** for text vectorization, and computes **Cosine Similarity** to recommend the top 5 most relevant movies.  
It is deployed on **Streamlit** with poster images fetched dynamically from the **TMDB API**.  

🔗 **Live Demo**: [Movie Recommender System App](https://movie-recommender-system-527ydffaajaykatymnjsl8.streamlit.app/)

---

## 🚀 Features
- Search and select any movie from the dropdown.  
- Get **top 5 similar movie recommendations**.  
- Displays **movie posters** along with names.  
- Powered by **Content-Based Filtering** (no explicit user ratings needed).  
- Simple and interactive **Streamlit UI**.  

---

## 📊 Dataset
- Source: **TMDB 5000 Movies + Credits dataset**  
- Important features used:
  - **Overview**
  - **Genres**
  - **Keywords**
  - **Cast**
  - **Crew (Director)**

We combined these into a single column called **`tags`**, which represents each movie in terms of its content.  

---

## ⚙️ Tech Stack
- **Python**  
- **Pandas, NumPy** → Data preprocessing  
- **scikit-learn** → CountVectorizer, Cosine Similarity  
- **Streamlit** → Web app deployment  
- **Pickle** → Save processed data & similarity matrix  
- **TMDB API** → Fetch movie posters  

---

## 🔑 Workflow
1. **Data Preprocessing**: Extracted metadata (genres, keywords, cast, director, overview).  
2. **Feature Engineering**: Created a combined `tags` column.  
3. **Vectorization**: Converted tags into numerical vectors using **CountVectorizer**.  
4. **Similarity Computation**: Applied **Cosine Similarity** to measure movie closeness.  
5. **Recommendation Function**: For a selected movie, retrieved top 5 similar movies.  
6. **API Integration**: Used **TMDB API** to fetch and display posters.  
7. **Deployment**: Built UI with Streamlit and deployed on Streamlit Cloud.  

---

## 🖥️ Project Structure
```
├── app.py                # Streamlit app (frontend)
├── m_r_s.ipynb           # Jupyter Notebook (data preprocessing & model building)
├── movie_list.pkl        # Pickle file with processed movie dataframe
├── similarity.pkl        # Pickle file with similarity matrix
├── README.md             # Project documentation
```

---

## ⚡ How to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommender-system.git
   cd movie-recommender-system
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```
4. Open browser at **http://localhost:8501**

---

Problem → Dataset → Preprocessing → Tags → Vectorization → Cosine Similarity → Recommendation → API → Streamlit Deployment

---

## 📚 Learnings
- Understanding of **content-based recommendation systems**.  
- Working with **text preprocessing & feature engineering**.  
- Using **CountVectorizer & Cosine Similarity** for similarity-based recommendations.  
- Deployment with **Streamlit**.  
- API integration (TMDB) for enhancing user experience.  

---

## 👩‍💻 Author
**Tamanna Bhrigunath**  
- 🌐 [LinkedIn](https://linkedin.com/in/tamanna-bhrigunath-578b43190)  
- 💻 [GitHub](https://github.com/bhrigu136)  
