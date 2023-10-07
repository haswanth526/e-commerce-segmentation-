

## Problem Statement

As an e-commerce platform, it is very important to profile your customers, dividing your clientele base into groups based on their needs and expectations. Grouping will help us come up with dedicated marketing strategies and will aid us in recommending products to different user bases. In this project, we are interested in analyzing the content of an E-commerce database that lists purchases made by ∼4000 customers over a period of one year (1/12/2010 to 9/12/2011). Based on this analysis, we would like to develop models to group the 4000 customers into different buckets. Such a model must take into account the similarity between the products purchased between the users (i.e. a user might purchase 2 different products which are very similar to each other), the spending patterns of a user, their meta information, etc.

## Minimum Requirements

The end objective of the participant is to come up with customer segmentations that take into account all the information that is presented in the dataset. The participant is expected to use NLP techniques to find similarity between the products.

## Project Summary:

In this project I used NLP (Natural Language Processing) techniques to extract frequent words in the 'Description' column of Products purchased and done Clustering text documents using k-means to obtain Product Categories.

Used Feature Extaction method TfidfVectorizer whch uses an in-memory vocabulary (a Python dict) to map the most frequent words to features indices and hence compute a word occurrence frequency (sparse) matrix. The word frequencies are then reweighted using the Inverse Document Frequency (IDF) vector collected feature-wise over the corpus. Performed dimensionality reduction using LSA (Latent semantic analysis) to this extracted features before fitting into K- means.

Finally with the Product Categories we clustered Customers based on thier purchases and spending pattern.


