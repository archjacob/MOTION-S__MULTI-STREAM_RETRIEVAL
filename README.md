

# Motion-S: Multi-Stream TF-IDF & KNN Retrieval Baseline

## 📌 Suggested Title
**"Motion-S: Optimized Multi-Stream Retrieval Baseline (TF-IDF + KNN)"**

---

## 📝 Description
This project presents an advanced "Retrieval-Based" solution for the **Motion-S: Hierarchical Text-to-Motion Generation for Sign Language** competition. Instead of using complex generative models, this model uses textual similarity to find and transfer motion tokens from the training set to the test set.

It is an efficient, fast, and optimized solution to produce valid and stable results in the Leaderboard.

## 🚀 Key Features
- **Multi-Stream Vectorization**: Combined use of `Char n-grams` and `Word unigrams/bigrams` to capture both the morphological and semantic structure of the text.
- **KNN Retrieval with IDW**: Use of the *K-Nearest Neighbors* algorithm with Inverse Distance Weighting for maximum accuracy.
- **Robust Validation**: Integrated process for checking the length and validity of codes (tokens) according to the contest rules.
- **Visual Diagnostics**: Monitoring panels to analyze the data distance and the distribution of features in 3D space.

## 🛠️ Technologies Used
- **Python** (Pandas, NumPy, Scikit-learn)
- **NLP**: TF-IDF Vectorizer
- **Algorithms**: K-Nearest Neighbors (KNN)
- **Visualization**: Matplotlib, Seaborn

## 📊 Workflow (Pipeline)
1. **Data Preprocessing**: Cleaning and normalizing sentences and glosses.
2. **Feature Engineering**: Creating sparse matrices via TF-IDF.
3. **Similarity Search**: Finding nearest neighbors in the training set.
4. **Token Transfer**: Mapping 6 motion layers.
5. **Submission Generation**: Creating `submission.csv` file ready for upload.

## 📈 Results
The solution is designed to serve as a robust "baseline", ensuring that any predictions are within the technical limits of the competition, minimizing the risk of errors during validation on Kaggle.

---
*This notebook is designed to run on Kaggle environments with GPU support (GPU P100).*
