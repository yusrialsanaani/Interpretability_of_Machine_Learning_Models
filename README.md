# Machine Learning Models Interpretability

The **objective** of this project is to introduce the explainable AI methods such as **SHAP** and **LIME**. These methods allow to explain and interpret the predictions of machine learning models, hence providing insight into the criteria behind predictions of machine learning models.

The main **Importance of Interpretability** is to allow us to perform error analysis and building a trust.
- Perform Error Analysis: allows to work specifically on weak points and to counteract them when training a model.
- Building a trust: many machine learning applications require trust in them so that the application can help with making a decision. Knowing the reasons for a prediction makes the decision to trust the application easier.

## Dataset
The dataset used in this project is Parkinsons Data Set taken from https://archive.ics.uci.edu/ml/datasets/parkinsons.
- This dataset is based on voice measures in frequency. 
- It was produced and released by the University of Oxford, available in the UCI ML Repository. 
- The dataset consists of 22 features and 1 result column of the diagnosis. 
- There are a total of 195 rows. Moreover, the dataset has been created from a measure of dysphonia and pitch period entropy.

## Interpretability Workflow
The general workflow of Interpretability is shown in the figure below.
The normal flow is to train a model with data and get predictions, then define an explainer and ingest both the data and the trained model to to it.
The defined explainer can provide Global or local interpretability.
- Global interpretability: This reflects the general behavior of the features in the model and allow us to understand which are the features that most impact the final output and of how much.
- Local interpretability: This shows the specific behavior of the features in a single model prediction, allowing us to understand all their single impacts on the final output. 

**LIME** is an example of explainers that provide **Local Interpretability**, while **SHAP** is an example of explainers that provide both **Local and Global Interpretabilities**.

SHAP explainers depends on Shap values. Shap values calculated based on the impact and contribution of each feature toward the prediction.
SHAP provides interpretabilities using different ways through different plots. Each plot will represent the impact, contribution of features in different ways providing both local and global  


![image](https://user-images.githubusercontent.com/89004966/166139032-41fec0c1-996c-40ad-bcef-48fa9cbd10bc.png)

![image](https://user-images.githubusercontent.com/89004966/166139599-8f9596be-0656-4abd-b6d3-7e41bcb61719.png)



