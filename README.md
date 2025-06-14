# Food-Recipe-Recommender-System
This project is a full-stack machine learning web application that recommends recipes based on user interactions and preferences. It uses a hybrid filtering approach combining content-based and collaborative filtering techniques to suggest food recipes.

<div align="center">
  🔗 <a href="https://data-mining-project-eight.vercel.app/">Live Demo</a> | 
  💻 <a href="https://github.com/The-Cow-addict/data-mining-project">Frontend GitHub</a> | 
  🔧 <a href="https://github.com/The-Cow-addict/data-mining-project-backend">Backend GitHub</a>
</div>

## Dataset

- **Source**: [Kaggle - Food.com Recipes and User Interactions](https://www.kaggle.com/datasets/shuyangli94/food-com-recipes-and-user-interactions)
- **Files Used**:
  - `RAW_recipes.csv`: Contains over 230K recipes with ingredients and steps
  - `RAW_interactions.csv`: Over 1 million user ratings and interactions


## Machine Learning Approach

### Preprocessing
- Cleaned recipe text fields (name, ingredients, steps)
- Removed missing values and duplicates
- Encoded features for modeling

### Recommendation Models
- **Content-Based Filtering**
  - TF-IDF vectorization on ingredients
  - Cosine similarity for recipe-to-recipe matching
- **Collaborative Filtering**
  - User-item rating matrix
  - KNN-based nearest neighbor recommendations

### Hybrid System
- Combines content and collaborative scores for more accurate results

## 🚀 Deployment

- **Frontend**: React.js (deployed on Vercel)
  - [Frontend GitHub Repository](https://github.com/The-Cow-addict/data-mining-project)
- **Backend**: FastAPI (deployed on Render)
  - [Backend GitHub Repository](https://github.com/The-Cow-addict/data-mining-project-backend)
- **Live App**: [https://data-mining-project-eight.vercel.app/](https://data-mining-project-eight.vercel.app/)

## Run Locally

### Backend
```bash
git clone https://github.com/The-Cow-addict/data-mining-project-backend.git
cd data-mining-project-backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### Frontend

```bash
git clone https://github.com/The-Cow-addict/data-mining-project.git
cd data-mining-project
npm install
npm run dev
```

### Sample Visualizations
- Ratings distribution
- Top-rated recipes
- User interaction patterns

### Features
- Ingredient-based search
- Recipe similarity ranking
- Personalized user recommendations
- Interactive web UI with real-time suggestions

### Acknowledgments
Dataset provided by Food.com via Kaggle

### Future Enhancements
- Add authentication and user profiles
- Allow filtering by dietary requirements
- Improve model scalability with deep learning
