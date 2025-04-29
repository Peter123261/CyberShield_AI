> **Next-Gen AI for Smart Cyber Defense & Threat Detection 🚀🛡️**

# CyberShield AI 🛡️🚀

A high-performance Machine Learning model for cybersecurity threat detection, achieving **99.74% accuracy** on real-world network traffic data.

## 📚 Project Overview

- **Problem**: Detect and classify different types of cyberattacks automatically from network flow data.
- **Solution**: Built a supervised classification model using Random Forest (best performing model), achieving high precision, recall, and overall accuracy.
- **Dataset Size**: ~2.8 million rows, 79 features (full dataset).
- **Sample Dataset Provided**: Small sample (~1%) for testing purposes inside the repository.

## 📦 Repository Structure

```bash
cybershield-ai/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── model_building.ipynb
│
├── models/
│   └── RandomForest_final_model.pkl
│
├── outputs/
│   └── confusion_matrix_test_set.png
│
├── app/
│   └── ( Flask API code for deployment in progress)
│
└── data/
    └── sample_data.csv
```

## 📊 Model Performance

| Metric | Score |
|:------|:------|
| Accuracy | 99.74% |
| Precision | 99%+ |
| Recall | 99%+ |
| F1-Score | 99%+ |

✅ Model tested on unseen test data
✅ Confusion matrix, classification report, and model evaluation included.

## 🧠 Key Techniques Used

- Advanced **feature engineering** and **feature selection** (Top 15 features).
- **Random Forest Classifier** with hyperparameter tuning (GridSearchCV).
- Handling of **outliers** and **missing values**.
- **Confusion Matrix** visualization and saving.
- Smart project organization for **portfolio presentation**.

## 📂 Data

- **sample_data.parquet** is included inside the `/data/` folder for quick testing.
- **Full dataset (~2.8 million rows)** available upon request (to avoid GitHub storage limits).
- Original features include network traffic parameters like `Flow Duration`, `Packet Length`, `Total Fwd Packets`, etc.

## 🚀 How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Open `notebooks/model_building.ipynb` to view the full machine learning workflow.

3. Load the trained model for prediction:
   ```python
   import pickle

   with open('models/RandomForest_final_model.pkl', 'rb') as file:
       model = pickle.load(file)

   # Make predictions
   preds = model.predict(X_test)
   ```

4.  Deploy the model using Flask API inside the `/app/` folder.(In progress)

## 📈 Future Improvements

- Full deployment to Heroku or AWS
- Real-time threat detection system
- API integration with network monitoring tools

## 📣 Acknowledgements

- Dataset adapted from CICIDS 2017 Dataset.
- Thanks to open-source contributors who developed cybersecurity benchmarks.

## 📬 Contact

- **Author**: [Peter Olamojin]
- **Email**: [olapeter1010@gmail.com]
