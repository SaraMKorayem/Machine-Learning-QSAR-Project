# Machine-Learning-QSAR-Project 🔻
I created this project as a university requirement, focusing on using Quantitative Structure-Activity Relationship (QSAR) as a computational biology approach in my drug discovery journey. 
https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.technologynetworks.com%2Fdrug-discovery%2Farticles%2Fscreening-strategies-used-in-drug-discovery-353812&psig=AOvVaw0qUTaT3HQpNhkgz8qOU-AF&ust=1717512221514000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCPj_juHVv4YDFQAAAAAdAAAAABAE 

The QSAR modeling process in this project covered several steps:

Data Collection and Preprocessing: Data is collected from the ChEMBL database, focusing on the target protein PPARγ associated with diabetes. Missing data is handled by removing incomplete entries.

Feature Engineering: Molecular descriptors are calculated, and relevant features are selected. Bioactivity data is categorized as "active," "inactive," or "intermediate" based on IC50 values. Lipinski descriptors are computed from canonical SMILES to evaluate drug-likeness.

Data Transformation: IC50 values are converted to pIC50 using a custom function to ensure uniformity. Standard values are normalized to cap excessively high values, and 'intermediate' compounds are excluded.

Exploratory Data Analysis (EDA): Lipinski descriptors are used to explore the chemical space of 'active' and 'inactive' compounds. Visualizations and statistical tests (e.g., Mann-Whitney U test) assess the significance of differences in molecular descriptors.

Model Development: Molecular descriptors are calculated using the PaDEL-Descriptor tool. The data is split into training and testing sets, and a Random Forest regression model is built and evaluated using R-squared values and RMSE.

Model Evaluation and Selection: Various machine learning algorithms are compared using the LazyPredict library. The Random Forest model is selected based on performance metrics.

Model Deployment: The final model is trained, tuned using GridSearchCV, and saved using joblib and pickle libraries. The model is deployed using Streamlit.

Report to this project is included: containing an abstract, introduction, methodology, results, and conclusion.

This project was inspired and adapted from professor Chanin Nantasenamat:   (YT) Data Professor (http://youtube.com/dataprofessor)
