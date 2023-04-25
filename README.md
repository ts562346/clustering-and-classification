# clustering-and-classification

Used the Iris dataset for clustering and classification. Created the following methods to implement clustering feature:

findNearestCentroids(X, centroids):
       inputs:  'X':          pandas df      A complete pandas dataframe of observations data.
                'centroids':  pandas df      A dataframe holding the K centroids (there are K rows), 
                                             with the same column types as X.   
       output:  'assign':     list of ints   A mapping of the data in X with the centroids in 'centroids'
                                             i.e., if row 42 in 'X' is closest to row 3 in 'centroids', 
                                                   then element 42 in 'assign' is '3'.

findCentroids( X, idx, k):
       inputs:  'X':          pandas df      A complete pandas dataframe of observations data.
                'assign':     list of ints   The same list of ints as the output of 'findNearestCentroids'
                'k':          integer        The hyper-parameter 'k'
       output:  'centroids':  pandas df      A dataframe holding the K centroids (there are K rows), 
                                             with the same column types as X.  

my_kmeans( X, k, max_iter):            
       inputs:  'X':          pandas df      A complete pandas dataframe of observations data.
                'k':          integer        The hyper-parameter 'k'
                'max_iter':   integer        The hyper-parameter setting the maximum number of iterations to make
       output:  'centroids':  pandas df      A dataframe holding the K centroids (there are K rows), 
                                             with the same column types as X. 
                'assign':     list of ints   A mapping of the data in X with the centroids in 'centroids'
                                             i.e., if row 42 in 'X' is closest to row 3 in 'centroids', 
                                                   then element 42 in 'assign' is '3'.            
  
  
These methods were then used to cluster the iris dataset for different values of k.

For classification, Naive Bayes, Support Vector Machine and the MLP Classifier (a simple neural network) was used on the Iris and Deli dataset (a total of 6 models).

The models were trained and tested on, there is a detailed analysis of each model in the notebook.
