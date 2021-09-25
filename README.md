# Network-Intrusion-Detection-

Objective
Analyse the data set for Network Intrusion Detection, investigate and evaluate the result and predict the overall performance.
Processes Steps
1.) Data was read using SKLEARN library and it was read as a data frame from the given CSV file.
2.) Columns were read using info command.
The data has 40 columns, with 22544 entries.
3.) Pre-processing
a. The categorical data was converted to numerical data
b. Data was cleaned and records containing null was removed.
The columns – “src_bytes, dst_bytes, count & srv_count” had null values, Total reecords with null values – 15,
After dropping the null values, the data has 40 columns with 22529 reccords.
c. The columns were divided into dependent & independent variables.
The column “class” was taken as dependent variable & the others were taken as independent variables.
d. The data was standardised to have zero mean and unit variance.
4.) Feature Engineering
a. Correlation among different columns were computed and visualised
b. Columns with high correlation among themselves (> 70%) was removed.
The following variables has high correlation:
'dst_host_rerror_rate', 'dst_host_same_srv_rate', 'dst_host_serror_rate', 'dst_host_srv_count', 'dst_host_srv_rerror_rate', 'dst_host_srv_serror_rate', 'num_root', 'rerror_rate',
'same_srv_rate', 'srv_rerror_rate', 'srv_serror_rate'
5.) Data Preparation:
a. Data was split for training & testing in the ratio of 0.7 & 0.3 respectively
6.) Different algorithms were used to train the model
a. KNeighborClassifiaer
b. Gaussiaon Naïve Bayes Model
c. Decision Trees
d. Logistic regression
7.) The models were trained with cross validation (cv = 10)
8.) For each of the models, Accuracy, Mean Score, Confusion Matrix & classification results were observed.
