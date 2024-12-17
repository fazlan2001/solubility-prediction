# Molecular Solubility Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on predicting molecular solubility (logS) using machine learning models. The dataset contains molecular descriptors, including molecular weight, partition coefficient (LogP), number of rotatable bonds, and aromatic proportions, with the target variable being the logarithm of solubility (logS).

The project explores multiple machine learning algorithms, evaluates their performance, and visualizes key insights.

## Dataset

  - Source: [Delaney Solubility Dataset](https://raw.githubusercontent.com/dataprofessor/data/refs/heads/master/delaney_solubility_with_descriptors.csv)
  - The [Delaney Solubility Dataset](https://raw.githubusercontent.com/dataprofessor/data/refs/heads/master/delaney_solubility_with_descriptors.csv) contains chemical descriptors and solubility measurements for various compounds. The dataset includes the following columns:
      - MolLogP: Logarithm of the partition coefficient.
      - MolWt: Molecular weight of the molecule.
      - NumRotatableBonds: Number of rotatable bonds in the molecule.
      - AromaticProportion: Proportion of aromatic atoms.
      - logS: Target variable - logarithm of solubility.
  - Size: 1144 rows × 5 columns

#### This dataset is used to predict the solubility of chemical compounds based on these descriptors.

### Sample Data 

![image](https://github.com/user-attachments/assets/6ef9b382-b0e4-4e14-8a41-7e9223f6ee08)


## Goals and Objective

  1. Data Analysis: Perform Exploratory Data Analysis (EDA) to identify relationships between features and solubility.

  2. Machine Learning Models: Train and evaluate the following models:
      - Random Forest Regressor

  3. Model Evaluation: Assess models using:
       - Root Mean Squared Error (RMSE)
       - Mean Absolute Error (MAE)
       - R² Score
    


  ## ⚙️ Steps to Run the Project

  ### Option 1: Run on Google Colab

   1. Open Google Colab.
   2. Upload the MLCW.ipynb notebook file.
   3. Install dependencies by running:
        - !pip install -q scikit-learn pandas matplotlib seaborn
   4. Run the notebook.
   5. The dataset is automatically fetched using this code:
        - import pandas as pd
        - url = 'https://raw.githubusercontent.com/dataprofessor/data/refs/heads/master/delaney_solubility_with_descriptors.csv'
        - dataset = pd.read_csv(url)


  ### Option 2: Run Locally

   1. Clone the Repository:
        - git clone https://github.com/fazlan2001/solubility-prediction.git
        - cd solubility-prediction
          
   2. Install Dependencies:
        - pip install -r requirements.txt
          
   3. Run the Notebook:
        - Launch Jupyter Notebook and open MLCW.ipynb:
            - jupyter notebook MLCW.ipynb
         


## 📊 Visualizations

  1. Feature Correlation Heatmap
  2. box Plots before Outliers and after handling outliers (e.g., MolWt vs. logS, MolLogP vs. logS)
  3. Model Performance Comparison using bar plots for RMSE, MAE, and R².

## 🔮 Future Work

  - Hyperparameter Tuning for models to further improve accuracy.
  - Feature Engineering: Add more molecular descriptors to enrich the dataset.
  - Model Deployment: Use Flask/Streamlit to create a simple app for solubility prediction.


## 📝 License
   - This project is licensed under the MIT License.


## 🤝 Acknowledgments

  - Dataset: Delaney Solubility Dataset by Data Professor.
  - Tools: scikit-learn, pandas, matplotlib.

## 📬 Contact
  - For questions, reach me at [fazlanfowmy@gmail.com].



