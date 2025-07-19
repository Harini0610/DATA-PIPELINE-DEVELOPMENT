# DATA-PIPELINE-DEVELOPMENT

COMPANY: CODTECH IT SOLUTIONS

NAME: HARINI P

INTERN ID:CT04DH454

DOMAIN: DATA SCIENCE

DURATION: 4 WEEKS

MENTOR: NEELA SANTHOSH KUMAR

# DESCRIPTION

EDITOR USED: VISUAL STUDIOS

As part of my internship under the Data Science domain, Task 1 involved implementing data preprocessing steps on a real dataset using Python. For this, I selected the Iris dataset, which is widely used for classification tasks and contains numeric and categorical data that make it ideal for preprocessing practice. The goal of the task was to take raw data and prepare it for machine learning through cleaning, transforming, and saving the processed output into a new dataset. I began by loading the dataset using pandas, a powerful library in Python used for data manipulation. The dataset consisted of 150 records and 6 columns — namely, an ID, four numeric features (sepal and petal dimensions), and one categorical feature (species of the flower).

Next, I moved on to identifying the data types in the dataset. I used pandas' select_dtypes function to separate numerical and categorical columns. This is an important step because numerical and categorical features need to be processed differently. For example, scaling numerical values and encoding categorical values require different approaches.Then, I used scikit-learn’s Pipeline and ColumnTransformer, which are standard tools used in professional machine learning workflows. These tools allow us to chain multiple preprocessing steps together in a structured and reusable way. For the numerical columns, I applied a SimpleImputer to handle any missing values (though the dataset didn't have any in this case), using the mean strategy, and then used StandardScaler to bring all numerical values to a common scale (zero mean and unit variance). This step is essential for many machine learning algorithms that are sensitive to the range of values.

For the categorical column (Species), I applied SimpleImputer as well, but with the most frequent strategy since categorical values don’t work with mean. Then I encoded these categorical labels using OneHotEncoder, which converts them into binary columns. This helps machine learning models to treat each category as independent without introducing any order.After completing the transformation pipeline, I used the fit_transform() function to apply all preprocessing steps to the dataset. The output was a NumPy array that I converted back into a pandas DataFrame so I could view and export it. I used to_csv() to save this transformed dataset into a file called "transformed_data.csv" for further use.The final output had 8 columns, where the original numerical features were scaled and the categorical 'Species' column was expanded into three separate one-hot encoded columns. This transformed dataset is now clean, standardized, and ready to be used for training machine learning models.

To make sure everything worked, I printed the shape of the processed data, and also displayed the first few rows using .head() and the last few rows using .tail(). This helped me verify that the transformation had been applied correctly — for instance, categorical values were replaced with encoded columns and numerical values had been scaled.

This process is critical in many real-world scenarios such as preparing healthcare data (e.g., diagnosis and lab values), retail and e-commerce data (e.g., customer purchase behavior), financial data (e.g., credit scoring and fraud detection), HR datasets (e.g., attrition prediction), and IoT sensor data (e.g., fault detection in manufacturing), where ensuring high-quality, structured, and machine-readable input is crucial for effective machine learning modeling

