# 🎯 Tech Career Recommender

An AI-powered recommendation system that suggests the most relevant tech career paths based on a user's skills, using **Content-Based Filtering** with TF-IDF and Cosine Similarity.

Built as Project 3 of my AI Engineering Internship at DecodeLabs — focused on mastering recommendation system fundamentals.

## 📌 Project Overview

This project answers the question: *"Given my skills, which tech career path fits me best?"*

Rather than relying on collaborative filtering (which needs historical user behavior data), this system uses **content-based filtering** — matching the user's skill profile directly against the required skills of each job role using mathematical similarity.

## 🎯 How It Works

1. User inputs at least 3 skills (e.g., Python, Cloud, Automation)
2. These skills are converted into numerical vectors using **TF-IDF** (Term Frequency-Inverse Document Frequency), which gives more weight to specific/rare skills and less weight to generic ones
3. **Cosine Similarity** measures how closely the user's skill vector aligns with each job role's skill vector
4. Results are ranked and the **Top 3** most relevant career paths are returned

## 🛠️ Tech Stack

- **Python 3**
- **scikit-learn** — TF-IDF Vectorization & Cosine Similarity
- **pandas** — data handling
- **matplotlib & seaborn** — visualization
- **Google Colab** — development environment

## 🔄 Pipeline

1. **Ingestion** — Capture user skill input
2. **Vectorization** — Convert text skills into TF-IDF weighted vectors
3. **Scoring** — Calculate cosine similarity between user and all job roles
4. **Sorting & Filtering** — Rank results and return Top 3 matches

## 📊 Sample Output
TOP 3 RECOMMENDED CAREER PATHS FOR YOU
Machine Learning Engineer — 78.4% Match
Data Scientist — 71.2% Match
Cloud Architect — 45.6% Match
### Visualization
![Career Recommendations]
<img width="890" height="590" alt="career_recommendations" src="https://github.com/user-attachments/assets/3b9a216e-90cb-4516-b97c-2e87b62e68d7" />

## 💡 Key Learnings

- Why binary (0/1) matching fails for nuanced text comparison
- How TF-IDF mathematically penalizes generic words and rewards specific ones
- Why Cosine Similarity (angle-based) outperforms Euclidean Distance (magnitude-based) for text similarity
- The Cold Start Problem and how direct user input bypasses it
- The complete content-based recommendation pipeline: Ingestion → Scoring → Sorting → Filtering

## 🚀 How to Run

```bash
git clone https://github.com/your-username/tech-career-recommender-ai.git
```

Open `career_recommender.ipynb` in Google Colab or Jupyter Notebook and run all cells sequentially.

## 📁 Repository Structure
├── career_recommender.ipynb # Main notebook with full code
├── career_recommendations.png # Top 3 match visualization
├── all_jobs_comparison.png # Full dataset comparison
└── README.md # Project documentation

## 🔗 Connect

Feel free to connect with me — documenting my AI Engineering learning journey!

---

*Part of the DecodeLabs AI Engineering Internship — Project 3 of 4*<img width="989" height="490" alt="all_jobs_comparison" src="https://github.com/user-attachments/assets/384429ff-8a81-429f-9276-dd6993ad91d6" />

