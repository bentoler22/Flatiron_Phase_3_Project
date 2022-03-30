#  Diabetes Classification for County Health Department
<img src="./images/diabetes.jpeg" alt="Drawing" style="width: 900px;height:300px;float: left;"/>

**Author:** Benjamin Toler

## Overview
This project uses machine learning classification algorithms to predict whether a person has diabetes, as well as determine what are some of the most important features related to diabetes. A XGBoost model built using CDC survey data from 2015 predicts whether a person has diabetes with a 76% accuracy and 80% recall. The model determined general health, blood pressure, and BMI to be the most important features in predicting diabetes. This information can be used to inform guidance for future public health efforts.

## Business Problem
The local health department wants to address the prevalence of diabetes in their community. A classification model for diabetes can predict which people are at risk as well as identify key risk factors that can be addressed with targeted health interventions.

## Data
This project uses 2015 survey data from the CDC's Behavioral Risk Factor Surveillance System. The dataset contains information about the health and lifestyle of 72,692 people. The target variable in this dataset is a binary with values of 1 meaning a person is pre-diabetic or diabetic and 0 meaning they are not pre-diabetic or diabetic. The datset used is balanced.

<img src="balanced_data.png" width="240" height="240" align="center"/>

## Method
The analysis uses classification algorithms to predict a binary diabetes variable. Iterating through multiple classification algorithms, XGBoost was determined to be the optimal model based on accuracy and recall scores.

## Results
The final XGBoost model has a 76% accuracy and 80% recall.

The final model included 27 predictor variables. Of those, general health, high blood pressure, and BMI were the three most significant predictors of diabetes.

![feature_importance](./images/feature_importance.png)

## Conclusions
- **Provide the survey online for community members to complete:** For those whom the model predicts to be pre-diabetic or diabetic, a recommendation to see a doctor for further testing should be given.
- **Educate the community of the link between general health and diabetes:** Some people may be under the assumption that diabetes is solely determined by genetics and are therefore not a risk if they do not have a family history of the disease. Increasing awareness that diabetes is linked with general health can help prevent the development of the disease.
- **Provide specific dietary and lifestyle steps the community can take to reduce blood pressure and lose weight:** high blood pressure and high BMI are key risk factors in diabetes. Knowing how to lower these to metrics is essential to reducing their prevalence in the community.
- **Invest in programs that increase access to healthier foods:** In addition to providing health advice, ensuring access to resources for the community to follow such advice is critical.

## Next Steps
- **Search for additional survey data to be included in the model to improve accuracy and recall:** the current model incorrectly classifies 24% of survey responses
- **Conduct analysis of how different diets impact diabetes:** the current features included in the model are primarily about general health conditions. Specific information about what types of foods are correlated with diabetes can be beneficial in preventing disease.
- **Analyze the relationship between environmental factors and diabetes:** this model includes primarily health and lifestyle factors. Environmental factors such as housing or pollution levels may also be indicators of diabetes.

## For More Information

See the full analysis in the [Jupyter Notebook](./Diabetes_Classification.ipynb) or review this [presentation](./presentation.pdf).

For additional info, contact Benjamin Toler at [bentoler22@gmail.com](mailto:alison.bentoler22@gmail.com)


## Repository Structure

```
├── data
├── images
├── .gitignore
└── Diabetes_Classification.ipynb
├── README.md
├── presentation.pdf
