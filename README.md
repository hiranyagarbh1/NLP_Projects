**Project Overview:**
This project focuses on hierarchical text classification using Amazon product reviews. The goal is to classify reviews into three hierarchical categories: cat1, cat2, and cat3. We have implemented two different solutions to achieve this:

**Multiple Machine Learning Classifiers:** This approach involves predicting each category separately using distinct machine learning models.
**HiClass Library with SVM Classifier:** This method leverages the HiClass library combined with a Support Vector Machine (SVM) to predict all three hierarchical categories simultaneously.

**Dataset:**
The dataset used in this project consists of Amazon product reviews. Each review is labeled with three hierarchical categories: cat1, cat2, and cat3. These categories represent a multi-level classification problem where each level is dependent on the previous one.

**Solutions:**

**Solution 1: Multiple ML Classifiers**

In this approach, we have implemented separate classifiers for each hierarchical category:

Category 1 (cat1): A machine learning classifier is trained to predict the primary category.
Category 2 (cat2): A different classifier is trained to predict the secondary category, taking into account the predictions from cat1.
Category 3 (cat3): Another classifier is used to predict the tertiary category, based on the predictions from cat1 and cat2.
This method ensures that each level of the hierarchy is predicted independently, allowing for flexibility and potentially higher accuracy at each stage.

**Solution 2: HiClass Library + SVM Classifier**

In the second approach, we use the HiClass library, which is designed specifically for hierarchical classification tasks. Combined with a Support Vector Machine (SVM) classifier, this method predicts all three hierarchical categories in a single step. This integrated approach can efficiently handle the dependencies between the categories and provide a cohesive prediction for the entire hierarchy.

**Implementation Details:**
Environment: Both solutions are implemented in Jupyter Notebooks for ease of experimentation and visualization.
Libraries Used: We utilized various Python libraries, including scikit-learn for the ML classifiers and the HiClass library for hierarchical classification. Additional libraries such as pandas, numpy, and matplotlib were used for data manipulation and visualization.

**Conclusion:**
This project demonstrates two distinct methods for hierarchical text classification on a dataset of Amazon product reviews. By comparing the performance and efficiency of the multiple ML classifiers and the HiClass + SVM approach, we aim to provide insights into the best practices for hierarchical text classification tasks.
