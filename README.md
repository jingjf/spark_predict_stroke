# spark_predict_stroke

Here, we use PySpark to implement machine learning to predict whether a patient would have stroke or not.

Firstly, exploratory data analysis (EDA) is performed. As we can see the dataset is significantly imbalanced.

Secondly, data cleaning and feature creation is assembled into the Pipeline in PySpark, which is one of the biggest advantages of Spark framework.

Thirdly, hyperparameter tuning and feature selection is performed. Specifically, Elastic Net method is used to find the optimal parameters. The final result uses a Ridge penalty.

At last, the Propensity Mathcing is used to test the causality of features and stroke. Eg, there is no causality between the marriage status and the probability of stroke.
