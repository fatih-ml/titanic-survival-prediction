# Titanic Survival Prediction: A Comprehensive Exploration

The sinking of the Titanic remains one of the most tragic events in maritime history, claiming the lives of many passengers in a heartbreaking manner. This project delves into the infamous Titanic dataset, available on Kaggle, to predict survival outcomes using various machine learning models. The dataset, derived from this historic catastrophe, not only provides a real-world context for analysis but also serves as a valuable resource for data science enthusiasts and students seeking a comprehensive guide.

## **Project Overview**  
Motivated by the project's prominence within the data science community and the rich dataset derived from a well-documented historical event, this endeavor aims to create a detailed guideline for both personal use and as a resource for aspiring data scientists. The journey encompasses initial data exploration, meticulous data preprocessing, insightful exploratory data analysis, model building, feature selection, and hyperparameter tuning.  

## **Outline of the Study**  
* Introduction
* Initial Data Exploration
* Data Preprocessing  
* Exploratory Data Analysis and Visualizations  
* Model Building and Feature Selection  
* Hyperparameter Tuning  

## **Data Preprocessing and Feature Engineering**  
The data preprocessing phase involved not only combining train and test datasets but also addressing missing values and performing extensive feature engineering. Beyond extracting titles from names, 'Family' and 'IsAlone' features were created, capturing the nuanced dynamics of passenger relationships. Despite concerted efforts on names, tickets, and cabins, only title extraction significantly contributed to the models. Additionally, binning age and fare variables proved pivotal, not only enhancing model performance but also mitigating issues of overfitting.

## **Exploratory Data Analysis and Key Findings**  
The exploratory data analysis (EDA) extended beyond surface-level examination, employing nested pivots and nuanced questioning to extract deeper insights. Beyond the well-established impact of gender on survival rates, the analysis revealed surprising correlations, such as the lack of correlation between age and survival—a phenomenon elucidated by gender-based disparities. Further revelations included the substantial influence of passenger class, ticket fares, and the emergence of titles as critical factors. Notably, the exploration uncovered intricate patterns related to age, gender, and survival, highlighting the complexity of the dataset.

## **Key Findings from EDA:**  
- Gender has the highes correlation with survival rate
- Age has a farily low correlation with survival rate since the gender effect eliminates the age-survival correlation
- Females have almost 4 times higher possibility to survive than males
- 1st class travellers are 3 times high possible to survive than 3rd class passengers
- As the fare increase, survival rate increases as well. After 40 dollars, survival possibility surpass the death possibility
- Child survival rates are almost identical no matter the genders
- Males having special titles such as Colonel, Sir etc have almost 70% higher survival rates.

## **Classification Models, Feature Selection, and Key Findings**  
The classification model phase embraced a diverse set, including Random Forest Classifier, Logistic Regression, XGBoost Classifier and 5 other models more. Different pipelines have been created for different model types and accuracy scores observed for evaluating the model performances. Cross validation and learning curves utilized for model performances on both training and test sets, moreover feature importances are analyzed and feature selection implemented. It is found that Sex, Fare, Pclass, Title (newly created) and Family (newly created) are the most important features effecting the survival rate of passengers. Therefore we excluded other features and observed a fair increase in model performance while we decrease the complexity and dimensionality. Eventually XGBoost outperformed other models, and chosen as the final model.

## **Challenges and Future Improvements**  
Challenges encountered included intricate feature extraction, potential overfitting, and the critical task of feature selection. Future improvements may involve delving deeper into feature engineering, especially on surnames, ticket numbers, and cabins. Additionally, the exploration of more sophisticated models, potentially including neural networks or complex layered approaches, could further enhance predictive accuracy and robustness.

## **Contact**  
For questions, collaborations, or further discussions, feel free to reach out on [Linkedin](https://www.linkedin.com/in/fatih-calik-469961237/), [Github](https://github.com/fatih-ml) or [Kaggle](https://www.kaggle.com/fatihkgg)

## **Dataset**  
Also, you can reach the famous Kaggle titanic competition and original dataset on [this link](https://www.kaggle.com/c/titanic)
