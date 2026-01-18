# Netflix Content Clustering

## Project Overview
This project focuses on clustering Netflix movies and TV shows using unsupervised machine learning techniques. The objective is to identify hidden patterns in Netflix content by grouping similar titles based on textual and metadata features.

Instead of predicting a target variable, this project explores the structure of the dataset and analyzes how content naturally groups together.

---

## Problem Statement
Netflix hosts a massive and diverse content library. Manually categorizing content at scale is difficult.  
Using unsupervised learning, this project attempts to automatically group similar content together based on their characteristics and descriptions.

---

## Dataset
**Source:** Netflix Movies and TV Shows Dataset (Kaggle)

**Key features used:**
- Type (Movie / TV Show)
- Genre
- Release Year
- Duration
- Description (text data)
- Listed_in (text data)

Textual features were transformed into numerical representations suitable for clustering.

---

## Approach

### 1. Data Preprocessing
- Cleaned and standardized text data
- Removed missing and irrelevant values
- Converted text descriptions into numerical vectors using TF-IDF

### 2. Clustering
- Used **K-Means Clustering**
- Experimented with different numbers of clusters

### 3. Visualization
- Used **PCA** to project clusters into 2D space
- Visualized overlap and relative separation of clusters

---

## Key Insights
- Netflix content forms overlapping clusters rather than clearly separated groups
- Text-based clustering often shows gradual transitions between categories
- PCA visualizations help interpret structure but do not guarantee strong separation
- Evaluation metrics must be interpreted carefully for unsupervised learning

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Scipy
- Scikit-learn
- Matplotlib, Seaborn

---

## Limitations
- Clustering quality is sensitive to text representation
- Results depend heavily on the chosen number of clusters

---

## Future Improvements
- Experiment with advanced embeddings (Word2Vec, BERT)
- Try alternative clustering algorithms (Hierarchical, DBSCAN)
- Perform deeper cluster interpretation using keywords

---

## Conclusion
This project demonstrates the application of unsupervised machine learning on real-world textual data.  
It highlights the challenges of clustering high-dimensional text and emphasizes exploratory analysis over prediction accuracy.

