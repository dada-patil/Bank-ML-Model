# BankInsight Streamlit app

This repository contains the Streamlit entrypoint and its model artifact.

## Run locally

```bash
python -m pip install -r requirements.txt
streamlit run LogisticModel.py
```

## Deploy on Streamlit Community Cloud

Push this directory to a GitHub repository. In Streamlit Community Cloud,
create an app with:

- **Repository:** the GitHub repository containing this directory
- **Branch:** the branch you pushed
- **Main file path:** `LogisticModel.py`

The dependency file and `logistic_model.pkl` must remain alongside the app
entrypoint. The model artifact was saved with scikit-learn 1.9.1 and pandas 3;
the requirements pin compatible major versions for loading it.
