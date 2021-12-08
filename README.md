# bank-data-analysis
The data was collected from UCI Machine Learning Repository but it originated from a research paper what was published on Sicence Direct. Link: https://www.sciencedirect.com/science/article/pii/S016792361400061X?via%3Dihub
One Portuguese bank’s data was observed and collected from 2008 to 2013 for the purpose of understanding telemarketing effectiveness. The period of data collection was right after The Financial Crisis in 2008-2009 so we expected to see such an effect in the dataset. The data initially included 150 features but was reduced to 22 most significant ones, which primarily related to client data, socio-economic data published by the Banco de Portugal and marketing campaign’s attributes

There is one outcome variable in the dataset which is Y - taking binary values of YES and NO in which YES represented for one customer who subscribed to the term deposit after the phone call and NO means they didn’t. While we aim to investigate the underlying clusters within the data set, we realized that the common segmentation methods (K-means, hierarchical clustering)will require a dataset with all numeric variables and that is not the case in the dataset we were working with. In fact, besides the age or duration of the call variables, the rest of the dataset variables were categorical. We realized that different clustering techniques must be implemented to achieve the goal that we aim for.

Given that the data included both categorical and numerical data, statistical techniques such as Gower Distance, the PAM (Partitioning Around Medoids) and Silhouette Width were implemented on 25% of the dataset which included these select predictor variables: age, job, marital, education, default, housing, loan, contact, duration, campaign, pdays, previous, and poutcome. As mentioned before, we noticed that the duration variable is heavily right-skewed so we made sure to transform this variable into logarithmic form while running Gower distance using Daisy package in R. The silhouette method was then applied to find the optimal number of clusters

Techniques will be used
1. Clustering with Gower distance
2. Partitioning Around Medoids (PAM) algorithm
3. Silhouette width


