## Recommendation System

A machine learning-based recommender system built to suggest the most relevant and personalized offers to users, using contextual behavioral data. The system is built using feature engineering techniques for both users and items based on contextual and interaction data.

---

## Technologies Used

- **Python 3.11+**
- **Pandas** – Data processing
- **NumPy** – Numerical computations
- **scikit-learn** – Feature scaling & preprocessing
- **Google Colab** – Notebook environment
- **Matplotlib / Seaborn** – (Optional) Visualization
- **CSV Dataset** – Provided by DataQuest 2025

---

## Features Engineered

### User Features:
- `total_interactions`: Total number of actions per user.
- `user_segment`: Broad customer segment (income-based).
- `user_beh_segment`: Detailed behavioral segmentation.
- `engagement_level`: User activity level (Active, Semi Active, Cold Start).
- `common_interaction_page`: Most frequently used app page.

All categorical features are **one-hot encoded**, and numeric features are **standardized**.

---

### Item Features:
- `total_interactions`: Total interactions per item.
- `interaction_type_counts`: Breakdown of DISPLAY, CLICK, CHECKOUT.
- `conversion_rate`: CHECKOUT ÷ DISPLAY.
- `item_type`: Category of item (e.g., INVEST, TRANSACT, etc.)

---

## The Process

1. **Data Cleaning**
   - Handled missing values, standardized text.
   - Removed duplicates and irrelevant rows (like DISPLAY with item='NONE').

2. **Feature Engineering**
   - Built detailed user and item features.
   - Encoded features using `OneHotEncoder` and `StandardScaler`.

3. **Model Readiness**
   - Produced a machine-learning ready dataset for:
     - User-based recommendations
     - Hybrid models
     - Ranking or classification models

---

## Running the Project

>  Google Colab recommended

1. Upload the dataset files to Google Drive.
2. Mount Google Drive in Colab.
3. Run the `generate_user_features()` and `generate_item_features()` functions.
4. Encode features using `encode_user_features()`.
5. Use the final dataset to train or simulate your recommender logic (e.g., cosine similarity, matrix factorization, ranking model).
