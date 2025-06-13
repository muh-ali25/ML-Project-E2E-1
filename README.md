# ML-Project-E2E-1
Big Mart Sales Prediction

bigmart_sales_prediction/
│
├── notebooks/
│   ├── 1_data_exploration.ipynb           # EDA & visualization
│   ├── 2_data_cleaning.ipynb              # Handling missing values, encoding, etc.
│   ├── 3_feature_engineering.ipynb        # Feature transformations
│   ├── 4_model_selection_automl.ipynb     # AutoML using PyCaret or H2O + XGBoost comparison
│
├── src/
│   ├── data/
│   │   ├── load.py                        # Load data from source
│   │   ├── preprocess.py                  # Clean and preprocess raw data
│   ├── features/
│   │   ├── build_features.py              # Feature engineering utilities
│   ├── models/
│   │   ├── train_model.py                 # Model training script
│   │   ├── evaluate_model.py              # Evaluation and metrics
│   │   ├── predict_model.py               # Prediction on test data
│   ├── utils/
│   │   ├── logger.py                      # Logging utility
│   │   ├── config.py                      # Config file for paths, parameters
│
├── streamlit_app/
│   ├── app.py                             # Streamlit dashboard to infer test samples
│
├── dagshub_wandb/
│   ├── wandb_integration.py              # Code to log runs to Weights & Biases
│   ├── dagshub_integration.py            # Save model artifacts to DagsHub
│
├── data/
│   ├── raw/
│   │   ├── train.csv                      # Original training data
│   │   ├── test.csv                       # Test data
│   ├── processed/
│       ├── train_processed.csv
│       ├── test_processed.csv
│
├── outputs/
│   ├── models/                            # Saved models (e.g. .pkl, .joblib)
│   ├── reports/                           # Evaluation reports and plots
│
├── requirements.txt
├── README.md
└── .env                                   # For API keys (DagsHub, WandB)
