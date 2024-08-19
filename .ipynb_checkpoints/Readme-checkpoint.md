# Classification Model to Predict outcome of Football matches

## Table of Contents
1. [Project Description](#project-description)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Results](#results)
5. [Examples](#examples)
6. [Contact Information](#contact-information)

## Project Description
In this modelling project, I built a classification model to predict the outcome of football matches. The scope includes; web scrapping to collect historic match result for the 2022/2023 and 2023/2024 Premier league season, data transformation, cleaning, encoding of character data type, exploratory analysis to identify trends/pattern and relatioships between data, and finally predictive modelling for match predictions.
The dataset consist of historic match result from the 2022/2023 and the just concluded season. key features include, team, opponent, GL, Sh, SoT,GF,GA etc.

#### Preliquisites
To succesfully run the code in the web scrapping and match prediction notebook, install the following modules
- Pandas
- numpy
- matplotlib
- seaborn
- sklearn
- beautifulsoup4

execute the below line of code in your notebook to install the latest version of the above packages.
```python
!pip install pandas numpy matplotlib seaborn sklearn bs4

```

# Usage
---

### Data Preparation
perform the following preprocessing on the dataset to make it suitable for the model and for optimum performance.

- Remove match records with missing feature values.
- Standardize team/opponent names
- Encode character features

### Running the model
split the dataset into training and test. since the data is a time series, split using dates such that training sets have later date values.

_Model selection:_ Three classification models namely; SVC-linear, SVC-rbf, and RandomForestClassifier are fitted to the training set. the best performing model(SVC-linear) is used for predictions.

### Model Evaluation
The models predictive performance on test sets is evaluated using the classification report metric. this provide a summary report contain model accuracy, f1_score, precision, and recall.

### Result
[![model_performance](model_evaluation.png)]


Goto [Model](https://github.com/Gab001-data/Football-Match-Prediction-Model/blob/main/PL_match_prediction.ipynb)

