Ekta Patel 27754515  
Tanu Patel 40077670  
Bryan Staniszewski 27486294  
Ricky Jr Mungcal 40179696  

# Project Summary

The National 2009 H1N1 Flu Survey conducted in the United States provided valuable data regarding individuals' vaccination patterns and their socio-demographic backgrounds, opinions, and health behaviors. This project aims to leverage this dataset to predict individuals' likelihood of receiving H1N1 and seasonal flu vaccines based on various attributes they shared during the survey.

## Research Questions:

1. Can we predict individuals' vaccination status based on their socio-demographic characteristics, opinions, and health behaviors?
2. Do higher income individuals tend to receive vaccinations more than lower income individuals?
3. Are individuals with higher education levels more inclined to get vaccinated?
4. What is the proportion of the population vaccinated against H1N1 compared to seasonal flu?

## Dataset Characteristics:

The dataset includes responses from the National 2009 H1N1 Flu Survey, covering information on individuals' vaccination status, socio-economic background, opinions, and health behaviors. It consists of both categorical and numerical features, covering a wide range of variables related to the survey questions. 


Some attributes include: 

- h1n1_concern: float64
- h1n1_knowledge: float64
- behavioral_antiviral_meds: float64
- behavioral_avoidance: float64
- behavioral_face_mask: float64
- behavioral_wash_hands: float64
- behavioral_large_gatherings: float64
- behavioral_outside_home: float64
- behavioral_touch_face: float64
- doctor_recc_h1n1: float64
- doctor_recc_seasonal: float64
- chronic_med_condition: float64
- child_under_6_months: float64
- health_worker: float64
- health_insurance: float64
- opinion_h1n1_vacc_effective: float64
- opinion_h1n1_risk: float64
- opinion_h1n1_sick_from_vacc: float64
- opinion_seas_vacc_effective: float64
- opinion_seas_risk: float64
- opinion_seas_sick_from_vacc: float64
- age_group: object
- education: object
- race: object
- sex: object
- income_poverty: object
- marital_status: object
- rent_or_own: object
- employment_status: object


The complete dataset can be found [here](https://www.drivendata.org/competitions/66/flu-shot-learning/).

## Project Objectives:

1. Preprocess the data to handle missing values, encode categorical variables, and prepare it for model training.
2. Conduct data visualizations aligned with the research questions to gain insights into the relationships between variables.
3. Build classification models to predict vaccination patterns and compare their performance.

## Model Evaluation:

### Class of Models:
- **Supervised learning:** Since we are dealing with a dataset where instances are given with known labels and we are trying to predict on unknown labels, using this class of models allows for better and more accurate prediction results.
### Algorithms:

- **K Nearest Neighbors**: This is a versatile algorithm that is used for prediction by classifying data points on the similarity of their neighbors. It is a lazy learning algorithm since it stores the entire training dataset and only computes prediction when needed which makes it suitable for handling noisy and linear data without making assumptions about the data structure.
- **Random Forest (RF)**: This algorithm constructs multiple decision trees by utilizing random subsets of both data and features. These trees collectively contribute to the final prediction by each casting a vote for a particular class. The class receiving the most votes is then chosen to be the predicted class, providing a conclusive outcome. By employing this method, RF decreases the chances of overfitting and enhances the model's accuracy at the same time.

### Evaluation Metrics:

- **Accuracy, precision, and F1-score**: Assess the models' predictive performance.
- **ROC Curve**: Analyze the trade-off between true positive rate and false positive rate.
- **Business Metrics**: Measure the practical utility of the models, such as revenue growth and operational efficiency improvements.

## Modeling Approach:

The project employs supervised learning techniques as the dataset contains labeled instances (vaccination status) along with features. Random Forest and K-nearest neighbors algorithms are selected for their effectiveness in handling classification tasks. Random Forest mitigates overfitting issues by combining multiple decision trees, while K-nearest neighbors makes predictions based on the majority class among the k nearest neighbors.

## Conclusion:

This project aims to provide insights into the factors influencing individuals' vaccination behaviors and develop predictive models to aid future public health efforts. By carrying out analytic techniques and evaluating model performance, the project seeks to contribute to the understanding and prevention of influenza outbreaks.


