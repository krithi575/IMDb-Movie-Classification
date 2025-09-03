# IMDb Movie Classification 🎬

This project applies **Machine Learning classification models** to predict a movie's certificate (e.g., PG, R, etc.) using the IMDb Top 1000 dataset.  
The workflow covers data preprocessing, visualization, dimensionality reduction, and model evaluation with ensemble methods.

---

## 📂 Dataset
- Source: IMDb Top 1000 Movies dataset (`imdb_top_1000.csv`)
- Columns include:
  - `Series_Title`, `Released_Year`, `Genre`, `IMDB_Rating`, `Meta_score`, `Certificate`, etc.
- Target variable: **Certificate** (movie ratings like PG, R, U, etc.)

---

## ⚙️ Project Workflow
1. **Data Preprocessing**
   - Removed less useful columns (`Poster_Link`, `Overview`, `Gross`)
   - Handled missing values with forward fill
   - Encoded categorical variables using `LabelEncoder`

2. **Exploratory Data Analysis**
   - Correlation heatmap to understand feature relationships
   - PCA projection to visualize class separability

3. **Modeling**
   - Implemented three classification models:
     - Bagging Classifier
     - Random Forest Classifier
     - K-Nearest Neighbors (KNN)

4. **Evaluation**
   - Metrics used: Accuracy, Precision, Recall, F1-score
   - Visualized:
     - Confusion Matrix per model
     - Feature Importance (for ensemble models)
     - Performance metrics comparison

---

## 📊 Results
- Random Forest achieved the **highest accuracy** among the tested models.
- PCA visualization provided clear insight into class separability.
- Comparative bar plots show performance differences.

---

## 📈 Visualizations
- Correlation Heatmap  
- PCA Feature Projection  
- Confusion Matrices  
- Feature Importances  
- Accuracy & Metrics Comparison  

---

## 🚀 Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (Bagging, Random Forest, KNN, PCA)

---

## ▶️ How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/krithi575/imdb-movie-classification.git
   cd imdb-movie-classification
