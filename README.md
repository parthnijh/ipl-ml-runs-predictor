# ipl-ml-runs-predictor
Using the 2024 ipl dataset to make predictions for 2025 dataset
# IPL Runs Predictor (2024 ➝ 2025)

📊 Predicting player runs in IPL 2025 using historical data from IPL 2024  
Built using Scikit-learn pipelines, linear regression, and performance evaluation via R² and MAE.

---

## 🏏 Problem Statement

Can we use IPL 2024 player stats (matches, strike rate, 100s, etc.) to predict how many runs they'll score in IPL 2025?

---

## 🔧 Features Used

- Player Name (OneHotEncoded)
- Team Name (OneHotEncoded)
- Matches Played
- Innings
- Not Outs
- Average
- Balls Faced
- Strike Rate
- 0s, 50s, 100s, 4s, 6s

---

## 📦 Model & Pipeline

- Linear Regression
- `Pipeline` with `ColumnTransformer` for clean preprocessing
- OneHotEncoding for categorical features
- SimpleImputer for missing values

---

## 📈 Evaluation

- 📌 R² on 2024 test data: **0.97**
- 📌 R² on actual 2025 runs: **0.925**

Also included:
- Scatter plot of predicted vs actual


---

## 📁 Project Structure
ipl-runs-prediction/
├── IplPredictions.ipynb      # Main Jupyter notebook with end-to-end workflow
├── data/                     # Folder containing IPL 2024 and 2025 CSV files
│   ├── ipl_2024_data.csv
│   └── ipl_2025_data.csv
├── README.md                 # Project summary and documentation
├── .gitignore                # Ignore unnecessary files/folders
├── requirements.txt          # Python dependencies (optional)
└── model.pkl                 # Saved model pipeline (optional, if exporting)






---

## 🚀 Future Improvements

- Try ensemble models like Random Forest or XGBoost
- Add match context or player form
- Build a Streamlit app to predict runs live

---

## 📚 Learnings

- Built a full ML pipeline from scratch
- Used real sports data
- Understood importance of feature engineering and evaluation

