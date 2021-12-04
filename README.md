# bank-data-analysis
The data was collected from UCI Machine Learning Repository but it originated from a research paper what was published on Sicence Direct. Link: https://www.sciencedirect.com/science/article/pii/S016792361400061X?via%3Dihub
One Portuguese bank’s data was observed and collected from 2008 to 2013 for the purpose of understanding telemarketing effectiveness. The period of data collection was right after The Financial Crisis in 2008-2009 so we expected to see such an effect in the dataset. The data initially included 150 features but was reduced to 22 most significant ones, which primarily related to client data, socio-economic data published by the Banco de Portugal and marketing campaign’s attributes

There is one outcome variable in the dataset which is Y - taking binary values of YES and NO in which YES represented for one customer who subscribed to the term deposit after the phone call and NO means they didn’t. We will focus on analyzing the effectiveness of the marketing campaign so this will be the only outcome variable. However, there’s a lot of variables that were included in the dataset including bank client data, related with the last contact of the current campaign, other attributes of the marketing campaign and social and economic context attributes. We plan to include all of the variables in the dataset in our LASSO model to do variable selection before we actually build the prediction model.  

Techniques will be used
1. Hierachical Clustering
2. Regularization - LASSO
3. Multilinear regression
