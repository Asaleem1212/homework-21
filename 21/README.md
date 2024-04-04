# Alphabet Soup Funding Application Prediction Model

## Overview

This project aims to leverage deep learning techniques to predict the success of funding applications submitted to Alphabet Soup, a philanthropic organization. The objective is to optimize the decision-making process, enabling Alphabet Soup to allocate resources effectively to projects with the highest likelihood of impact.

## Dataset

The dataset contains several features related to the funding applications, including the type of application, affiliation, classification, use case, organization status, income amount, special considerations, and the amount requested.

## Analysis Process

### Data Preprocessing
- **Target Variable:** `IS_SUCCESSFUL` indicates whether the funding was successful.
- **Features:** Included variables such as `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`.
- **Removed Variables:** Identification details `EIN` and `NAME` were removed as they do not contribute to the prediction model.

### Model Architecture
- **Layers:** The model comprises an input layer, three hidden layers (with 4, 8, and 16 neurons, respectively), and an output layer.
- **Activation Functions:** ReLU for hidden layers and Sigmoid for the output layer.

### Training and Evaluation
- The model was trained over 100 epochs with a validation split to mitigate overfitting.
- Final model accuracy on test data: ~73%.

## Results

The deep learning model showed a promising start in predicting the success of funding applications, achieving an accuracy of approximately 73%. Steps were taken to refine and optimize the model, including adjusting neuron counts, layer numbers, and preprocessing techniques.

## Summary and Recommendations

The model's performance indicates a solid foundation with room for further improvement. We recommend exploring a Random Forest Classifier as an alternative, due to its robustness in handling various data types and less susceptibility to overfitting. This approach could also provide insights into the most influential features for funding success.

## Future Work

- Implement a Random Forest Classifier to compare performance with the deep learning model.
- Conduct feature importance analysis to identify key predictors of application success.
- Explore additional data preprocessing and feature engineering techniques to enhance model performance.
