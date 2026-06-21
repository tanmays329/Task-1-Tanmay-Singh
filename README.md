# DecodeLabs Data Science Internship - Projects 1, 2, and 3

A comprehensive data science portfolio covering exploratory data analysis, supervised classification, and unsupervised clustering on e-commerce retail data.

---

## Project 1: Advanced EDA & Feature Engineering

**Goal:** Transform raw e-commerce data into a clean, ML-ready dataset through exploratory analysis and feature creation.

### Key Deliverables
- **Exploratory Data Analysis (EDA):** Distribution analysis, correlation heatmaps, statistical summaries
- **Missing Value Handling:** Categorical imputation for CouponCode; KNN imputation for numeric features
- **Outlier Detection & Treatment:** IQR and Z-score methods; values capped to preserve data integrity
- **Feature Engineering:** Created 5 new predictive features:
  - Price Per Item
  - Cart Fill Ratio
  - High Value Order Indicator
  - Coupon Usage Flag
  - Referral Feature

### Output
- `project_1_cleaned_dataset.csv` - Clean dataset with 25+ engineered features
- Jupyter Notebook: `project_1.ipynb`

### Technologies
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---

## Project 2: Supervised Learning - Fraud Detection Pipeline

**Goal:** Build and tune a classification model to identify fraudulent transactions in a highly imbalanced dataset.

### Key Requirements
- **SMOTE Oversampling:** Custom implementation to handle 97:3 class imbalance
- **Algorithms:** Logistic Regression and Random Forest trained on balanced data
- **Evaluation Metrics:** Precision, Recall, and ROC-AUC (accuracy discarded for imbalanced data)
- **Hyperparameter Tuning:** GridSearchCV optimized on ROC-AUC cross-validation score

### Key Features
- Scikit-Learn pipelines integrating scaling + SMOTE + classifiers
- Baseline and tuned model comparison
- ROC curve visualization comparing all 4 models
- Classification reports with precision/recall/F1 per class

### Output
- Jupyter Notebook: `Project_2_Fraud_Detection.ipynb`

### Technologies
Python, Scikit-Learn, NumPy, Pandas, Matplotlib (no external imblearn dependency - custom SMOTE implementation)

---

## Project 3: Unsupervised Learning - Customer Segmentation

**Goal:** Discover hidden customer groups using distance-based algorithms and translate them into actionable business personas.

### Key Requirements
- **Principal Component Analysis (PCA):** Reduce 20+ features to 3 principal components
  - PC1, PC2, PC3 explain ~85% of total variance
- **Optimal K Selection:** 
  - Elbow Method: Visual inspection of inertia vs K
  - Silhouette Score: Quantitative validation of cluster quality
- **K-Means Clustering:** Final segmentation with optimal K clusters
- **Business Persona Translation:** Clusters mapped to actionable customer segments

### Key Deliverables
- **Silhouette Analysis:** Per-cluster quality metrics and overall score
- **Visualizations:**
  - PCA scatter plots (PC1 vs PC2, PC1 vs PC3) with cluster centroids
  - Elbow curve and Silhouette score by K
  - Standardized heatmap of cluster profiles
- **Cluster Profiles:** Mean feature values by segment
- **Business Personas:** Segment-specific characteristics and marketing recommendations:
  - Premium Spenders
  - Discount Hunters
  - Referral Advocates
  - Bulk Buyers
  - Regular Customers

### Output
- Jupyter Notebook: `Project_3_Customer_Segmentation.ipynb`
- Actionable business recommendations per segment

### Technologies
Python, Scikit-Learn (PCA, K-Means, Silhouette), NumPy, Pandas, Matplotlib, Seaborn

---

## Dataset

**Source:** E-commerce retail transaction data

**Columns:** 14 raw features + 11 engineered features
- Order details (ID, Date, Status, Tracking)
- Customer info (CustomerID, ShippingAddress)
- Product info (Product name, Quantity, UnitPrice, TotalPrice)
- Marketing (PaymentMethod, ReferralSource, CouponCode)
- Engineered features (time-based, financial ratios, flags)

**Size:** 1,500+ transactions

---

## Repository Structure

```
.
├── README.md                           # This file
├── requirements.txt                    # Python dependencies
├── project_1.ipynb                     # Project 1 Notebook
├── project_1_cleaned_dataset.csv       # Cleaned output from Project 1
├── Project_2_Fraud_Detection.ipynb     # Project 2 Notebook
├── Project_3_Customer_Segmentation.ipynb  # Project 3 Notebook
├── Dataset for Data Analytics - Sheet1.csv  # Raw input data
└── .git/                               # Git version control
```

---

## Installation & Setup

### Prerequisites
- Python 3.12+
- pip or conda

### Installation Steps
```bash
# Clone repository
git clone <repository-url>
cd "Decodelabs internship/project 1"

# Create virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Dependencies
- pandas>=1.5.0
- numpy>=1.24.0
- matplotlib>=3.7.0
- seaborn>=0.12.0
- scikit-learn>=1.3.0
- jupyter>=1.0.0

---

## Usage

### Run Notebooks
```bash
# Activate environment
source .venv/bin/activate  # Or: .venv\Scripts\activate (Windows)

# Start Jupyter
jupyter notebook

# Open and run:
# - project_1.ipynb
# - Project_2_Fraud_Detection.ipynb
# - Project_3_Customer_Segmentation.ipynb
```

### Key Outputs
- **Project 1:** `project_1_cleaned_dataset.csv` (fed into Projects 2 & 3)
- **Project 2:** Model comparison table, ROC curves, classification metrics
- **Project 3:** Customer personas, silhouette analysis, segment heatmap

---

## Key Skills Demonstrated

### Data Science
- Exploratory Data Analysis (EDA)
- Feature Engineering & Selection
- Statistical Imputation (Median, KNN)
- Outlier Detection & Treatment

### Supervised Learning
- Classification algorithms (Logistic Regression, Random Forest)
- Imbalanced data handling (SMOTE)
- Hyperparameter tuning (GridSearchCV)
- Model evaluation (Precision, Recall, ROC-AUC)

### Unsupervised Learning
- Dimensionality reduction (PCA)
- Distance-based clustering (K-Means)
- Cluster validation (Silhouette Score, Elbow Method)
- Business intelligence translation

### Tools & Libraries
- **Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **ML:** Scikit-Learn
- **Version Control:** Git
- **Notebooks:** Jupyter

---

## Author

**Tanmay Singh**  
DecodeLabs Data Science Internship

---

## License

This project is part of the DecodeLabs internship program.

---

## Contact & Support

For questions or clarifications, refer to the individual project notebooks or contact the author.