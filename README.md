# Breast-cancer_prediction_model
The primary objective of this project is to build and compare multiple machine learning models to predict the diagnosis of breast cancer (malignant or benign) based on a dataset of various cell characteristics.
This project is about building a computer model to predict whether a breast cancer tumor is benign (non-cancerous) or malignant (cancerous). The process is broken down into several easy-to-understand steps:

### 1. **Getting the Data** 
First, the project uses a dataset from a file called **"Breast_cancer_dataset.csv"**. This file is like a big spreadsheet containing information about different tumors. For each tumor, there are 33 pieces of information, such as its size, texture, and other physical characteristics. The most important piece of information is the "diagnosis," which tells us if the tumor is malignant (M) or benign (B).

---

### 2. **Cleaning and Preparing the Data** 
Before the computer can learn from the data, it needs to be cleaned up.
* **Removing Unnecessary Information:** Some columns, like a patient ID number ("id") and an empty column ("Unnamed: 32"), aren't useful for making a prediction, so they are removed.
* **Making Words into Numbers:** The "diagnosis" column has words like 'M' and 'B'. The computer needs numbers, so these are converted into `1` (for malignant) and `0` (for benign).
* **Separating the Data:** The data is then split into two groups: the **features** (all the tumor characteristics) and the **target** (the diagnosis we want to predict).
* **Training vs. Testing:** The data is further split into a **training set** (80% of the data) and a **testing set** (20% of the data). The training set is used to teach the models, and the testing set is used to see how well they perform on new, unseen data.
* **Scaling the Data:** To ensure all the features are on a similar scale, the numbers are adjusted using a process called **StandardScaler**. This helps the models work better.

---

### 3. **Training the Models** 
In this step, different machine learning models—think of them as different types of students—are taught to find patterns in the training data to connect the tumor features to the correct diagnosis. The project uses several types of models:
* Logistic Regression
* Decision Tree
* Random Forest
* Gaussian Naive Bayes
* Support Vector Machine (SVM)
* K-Nearest Neighbors
* XGBoost

---

### 4. **Evaluating the Results** 
Once all the models have been trained, they are tested on the data they haven't seen before (the testing set). The goal is to see how many times each model correctly predicts whether a tumor is benign or malignant.

The results show how accurate each model is at making predictions. For example, some models were over **95% accurate**, which means they correctly predicted the diagnosis for 95 out of every 100 tumors in the test set.

---

### 5. **Comparing the Models** 🏆
Finally, a bar chart is created to show the accuracy of all the models in one place. This makes it easy to compare them and see which one is the "best student" for this particular task. The best performing models in this project were the Decision Tree, Random Forest, and XGBoost classifiers, all with an accuracy of over 95%.
