# Hate Speech Detection in the Polish Language Using Machine Learning and Deep Learning Approaches

---

## Project Description

Project carried out as part of a master's thesis at Wrocław University of Science and Technology.

In the age of social media, hate speech is becoming an increasingly visible and dangerous issue. Online platforms are flooded with hateful content that negatively impacts users, making it crucial to develop effective detection methods. This project focuses on comparing various machine learning and deep learning techniques, including state-of-the-art transformer models, to evaluate their effectiveness in detecting hate speech in Polish.

The study utilizes two datasets collected from social media platforms—Wykop and Twitter—and further validates the models on a proprietary dataset featuring challenging classification cases such as sarcasm, irony, and harsh language. A significant part of the research analyzes how different data preprocessing strategies affect the models’ performance.

The experiments lead to insights and recommendations on selecting optimal approaches for hate speech detection, contributing to a better understanding of the complexities involved in classifying hate speech, especially in nuanced or contextually difficult texts.

---

## Repository Structure

This repository contains three main folders: `code_notebooks`, `experiment_results`, and `resources`.

### 1. `code_notebooks`

This folder includes all the notebooks in `.ipynb` format used during the master's thesis. Below is a description of the main files and subfolders:

- **Description_extreme/twitter/wykop_dataset.ipynb**  
  Detailed analysis of datasets (Wykop, Twitter, extreme dataset) – number of samples, class distribution, basic statistics, and visualizations.

- **DL_algorithm_LSTM_twitter/wykop.ipynb**  
  Training and testing process of the LSTM model on Twitter and Wykop datasets, including result plots and saving the trained model.

- **Eval_HerBERT/LSTM/ML/RoBERTa_algorithm_extreme.ipynb**  
  Evaluation of the best models on the proprietary challenging cases dataset, which includes sarcasm, youth slang, and hidden discrimination.

- **HerBERT-BASE-CASED_twitter/wykop.ipynb**  
  Training and testing of the HerBERT-BASE-CASED transformer model on Twitter and Wykop datasets, with result visualization and model saving.

- **ML_algorithms_KNN_twitter/wykop.ipynb**  
  Training and testing of the classical KNN model on Twitter and Wykop datasets, including plots and model saving.

- **ML_algorithms_RF_twitter.ipynb**  
  Training and testing of the Random Forest (RF) model on Twitter and Wykop datasets, with result visualization and model saving.

- **ML_algorithms_SVM_twitter.ipynb**  
  Training and testing of the Support Vector Machine (SVM) model on Twitter and Wykop datasets, including plots and model saving.

- **ML_algorithms_XGB_twitter.ipynb**  
  Training and testing of the XGBoost (XGB) model on Twitter and Wykop datasets, along with result visualization and model saving.

- **Preprocessing_extreme/wykop/twitter_dataset.ipynb**  
  Detailed presentation of the data preprocessing process divided into three variants for extreme, Wykop, and Twitter datasets.

- **XML-ROBERTA-BASE_twitter.ipynb**  
  Training and testing of the XLM-RoBERTa model on Twitter and Wykop datasets, including result plots and model saving.

- **Distribution_shift.ipynb**  
  The distribution shift between Wykop/Twitter and the extreme dataset was analyzed using Jensen-Shannon and Kullback-Leibler divergences on word and label distributions, as well as semantic differences assessed with Maximum Mean Discrepancy and visualized via PCA and t-SNE on Sentence-BERT embeddings.

---

### 2. `experiment_results`

This folder contains the results of all experiments conducted using the notebooks from the `code_notebooks` folder. The results are organized in subfolders named after the respective notebooks. Here you can find metric files, plots, saved models, and other output data from the experiments.

---

### 3. `resources`

This folder includes files necessary for the proper functioning of notebooks and data analysis processes:

- **BAN-PL.csv** – Wykop dataset used in the experiments.  
- **extreme_examples.csv** – Proprietary dataset of challenging, contextually complex cases for evaluation.  
- **polish** – Custom file containing a list of Polish stopwords.  
- **polish_vulgarisms_extended.txt** – File with an extended list of vulgarisms, used for censoring during preprocessing.  
- **v1_test.csv** – Twitter test dataset.  
- **v1_training.csv** – Twitter training dataset.

---

Each folder and file has been carefully prepared to enable full reproducibility of the results and further development of hate speech detection methods in the Polish language.
