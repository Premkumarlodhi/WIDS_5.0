# WIDS_5.0
1. Project Overview
In this project, I aimed to build a robust, reproducible, and scalable machine learning pipeline. The core objective was not just to achieve high accuracy on a dataset, but to follow industry-standard MLOps practices, including modular code structure, data validation, and model tracking.

2. Data Acquisition and Exploratory Data Analysis (EDA)
I began by analyzing the dataset to understand its underlying structure. My EDA phase involved:

Statistical Profiling: I calculated mean, median, and variance to identify data distributions.

Visualization: I used heatmaps for correlation analysis and distribution plots to identify skewness in the features.

Insight Generation: I discovered significant class imbalances and identified key features that had the highest predictive power for the target variable.

3. Data Preprocessing and Feature Engineering
To prepare the data for training, I implemented a modular preprocessing pipeline:

Handling Missing Values: I used median imputation for numerical features and mode imputation for categorical ones to ensure no data loss.

Encoding: I applied one-hot encoding for categorical variables with low cardinality and label encoding where appropriate.

Scaling: I used standard scaling to normalize numerical features, ensuring that the model is not biased toward features with larger magnitudes.

Feature Selection: I dropped redundant columns and utilized PCA for dimensionality reduction where features were highly collinear.

4. Model Selection and Training
I experimented with several algorithms to find the best fit for this problem:

Baseline Models: I started with Linear/Logistic Regression and Decision Trees to establish a performance baseline.

Ensemble Methods: I implemented Random Forest and Gradient Boosting (XGBoost/LightGBM) which significantly improved the results.

Hyperparameter Tuning: I utilized GridSearchCV and RandomizedSearchCV to optimize parameters such as learning rate, tree depth, and estimators.

5. Model Evaluation
I evaluated my models using multiple metrics to ensure a holistic view of performance:

Accuracy & F1-Score: Crucial for understanding the balance between precision and recall.

Confusion Matrix: Used to identify specific classes where the model was struggling.

ROC-AUC Curve: I plotted this to evaluate the model's ability to distinguish between classes.

6. MLOps Integration and Deployment
The final stage of my project involved transitioning from a notebook to a production-ready script:

Modularization: I refactored the code into distinct modules for data ingestion, transformation, and model training.

Logging and Exception Handling: I integrated custom logging to track the execution flow and added robust error handling.

Pipeline Automation: I ensured the entire process from raw data to model prediction can be executed as a single pipeline.

7. Conclusion
Through this project, I successfully built an end-to-end ML system. I learned the importance of data quality, the nuances of model tuning, and the necessity of writing clean, modular code. All tasks outlined in the WiDS 5.0 curriculum have been completed and are documented in my GitHub repository
