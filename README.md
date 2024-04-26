# ML-classification-SVM-kNN-Trees
This project focuses on predicting the risk of diabetes from health and lifestyle data, which can prove to be a beneficial feature, for example, for a wellness app that provides personalized health tips.    
As many people don't perform regular doctor check-ups, helping individuals at risk to become aware of their potential condition encourages timely intervention, promoting early lifestyle changes and healthcare consultations.     

For the task, I use a [Kaggle-availlable](https://www.kaggle.com/datasets/tigganeha4/diabetes-dataset-2019) diabetes dataset, which doesn't contain any advanced medical info that wellness-app users may not possess (insulin or glucose blood levels) and instead resembles a typical questionnaire.      

* In the initial exploratory analysis phase, distributions, summary statistics, and feature relationships with the target variable are examined.     
* Pre-processing involves data cleaning and ordinal/binary feature encoding.     
* My classifiers of choice in this experiment are **SVM, kNN, and Decision Trees**. Their performance is compared through an implementation of **nested cross-validation**.      
  * Prior to the hyperparameter tuning within the nested CV, I also generally explore the influence of each model's associated hyperparameters to establish a more reasonable grid.     
* As the dataset was heavily imbalanced, I'm addressing it using Synthetic Minority Oversampling Technique (SMOTE) as well as "stratified" strategies. 

The Decision Trees model demonstrated the best performance with a balanced accuracy of 94% and an F1 score of 93%, while also being the most computationally efficient.
