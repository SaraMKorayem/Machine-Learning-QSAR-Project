### Machine-Learning-QSAR-Project 🔻
I created this project as a university requirement, focusing on using Quantitative Structure-Activity Relationship (QSAR) as a computational biology approach in my drug discovery journey. 

**Explanation viseo:** https://nileuniversity-my.sharepoint.com/:v:/g/personal/s_mohamed2135_nu_edu_eg/ESC4lXvkVO1Mk11SYjfoTeYBChcmPVwi4LvQPGph4GqHTw


## **QSAR Modeling of PPARγ Biological Data: Random Forest Model Deployment and pIC50 Prediction Using ChEMBL IDs and SMILES**
![image](https://github.com/SaraMKorayem/Machine-Learning-QSAR-Project/assets/169392560/8d68b628-fff7-4de1-b07c-ed4d2b187c0b)


The QSAR modeling process in this project covered the following steps:

**Data Collection and Preprocessing:** Data is collected from the ChEMBL database, focusing on the target protein PPARγ associated with diabetes. Missing data is handled by removing incomplete entries.

**Feature Engineering:** Molecular descriptors are calculated, and relevant features are selected. Bioactivity data is categorized as "active," "inactive," or "intermediate" based on IC50 values. Lipinski descriptors are computed from canonical SMILES to evaluate drug-likeness.

**Data Transformation:** IC50 values are converted to pIC50 using a custom function to ensure uniformity. Standard values are normalized to cap excessively high values, and 'intermediate' compounds are excluded.

**Exploratory Data Analysis (EDA):** Lipinski descriptors are used to explore the chemical space of 'active' and 'inactive' compounds. Visualizations and statistical tests (e.g., Mann-Whitney U test) assess the significance of differences in molecular descriptors.

**Model Development:** Molecular descriptors are calculated using the PaDEL-Descriptor tool. The data is split into training and testing sets, and a Random Forest regression model is built and evaluated using R-squared values and RMSE.

**Model Evaluation and Selection:** Various machine learning algorithms are compared using the LazyPredict library. The Random Forest model is selected based on performance metrics.

**Model Deployment:** The final model is trained, tuned using GridSearchCV, and saved using joblib and pickle libraries. The model is deployed using Streamlit.

The QSAR project report is included and contains an abstract, introduction, methodology, results, and discussion.

This project was inspired and adapted from professor Chanin Nantasenamat:   (YT) Data Professor (http://youtube.com/dataprofessor)
