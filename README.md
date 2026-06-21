# DecodeLabs Data Science Internship - Project 1


A focused analysis and feature engineering project for e-commerce retail data.

---

## Project 1: Advanced EDA & Feature Engineering

**Goal:** Transform raw e-commerce transaction data into a clean, ML-ready dataset using exploratory analysis and new feature creation.

### Key Deliverables
- **Exploratory Data Analysis (EDA):** Data distribution, correlation insights, target relationships
- **Missing Value Handling:** Categorical imputation for CouponCode and numeric imputation for selected columns
- **Outlier Detection & Treatment:** IQR-based capping and careful value cleaning to preserve dataset quality
- **Feature Engineering:** Created predictive features such as:
  - Price Per Item
  - Cart Fill Ratio
  - High Value Order Indicator
  - Coupon Usage Flag
  - Referral Indicator

### Output
- `project_1_cleaned_dataset.csv` — cleaned dataset with engineered features
- Jupyter Notebook: `project_1.ipynb`

### Technologies
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---

## Dataset

**Source:** E-commerce retail transaction data

**Overview:** Raw transaction records with order details, product information, marketing fields, and customer identifiers.

**Included files:**
- `Dataset for Data Analytics - Sheet1.csv` — original input data
- `project_1_cleaned_dataset.csv` — cleaned output data produced by Project 1

---

## Repository Structure

```
.
├── README.md
├── requirements.txt
├── project_1.ipynb
├── project_1_cleaned_dataset.csv
├── Dataset for Data Analytics - Sheet1.csv
└── .gitignore
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
.venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Dependencies
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter

---

## Usage

### Run Project 1
```bash
.venv\Scripts\activate
jupyter notebook
```

Open and run:
- `project_1.ipynb`

### Expected Output
- Cleaned dataset: `project_1_cleaned_dataset.csv`
- Notebook analysis of data quality, missing values, outliers, and engineered features

---

## Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Missing value imputation
- Outlier detection and treatment
- Feature engineering
- Data visualization
- Jupyter notebook reporting

---

## Notes

This repository contains only Project 1 materials. Additional projects were removed so the repo stays focused on the first assignment.

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
