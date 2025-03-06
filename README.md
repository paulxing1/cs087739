java c Assignment 3 Note 1: for answers with Python, display both codes and results clearly. Note 2: for answers with manual calculation, please display all calculation steps clearly. Question 1. [30 points @ 6 points each] A firm collected 5 training instances with 2 features X1  and X2  and their types.

Instance X1 X2 Type 1 12.1 11.7 + 2 7.9 2.1 × 3 7.8 8.4 + 4 7.3 6.9 × 5 11.2 8.9 +

(a)   Use  Python  to  plot  the  5  instances  with X1  on  the x-axis  and X2   on  the y-axis. Visualize instances with different color according to their Type values. With a new instance (i.e., Instance 6) with (X1, X2) = (6.5, 2. 1), please complete tasks below with either Python or manual calculation. Round all results to 4 decimal places. (b)   Calculate the Euclidean distance between the new instance and each of the 5 training instances using both X1  and X2 . (c)   Calculate their Cosine distance as well. (d)   What  is the predicted  Type value for the new instance using 3-NN algorithm and majority vote (based on cosine distance)? (e)   What’s  the predicted  Type  value  for the new instance using 3-NN algorithm and weighted  voting  (based  on  cosine  distance  computed  at  step  (c))?  What  is  the estimated class probability for it? Please report the results in one or two tables. For example, answers for Q1(b) -(c) can be organized as below: Instance X1 X2 Type (b) Euclidean Distance (c) Cosine Distance 1 12.1 11.7 +

… … … …

6 6.5 2.1

Question 2. [30 points] A firm collected 6 instances with 2 features X1 and X2.

Instance X1 X2 1 1 4 2 1 3 3 0 5 4 5 2 5 6 3 6 4 0

With instance 1 and 4 selected as the initial centroids, we’d like to simulate the k-means algorithm to separate all instances into two clusters (k  = 2).  Please complete below tasks with either Python or manual calculation, round results to 2 decimal places. (a)    [5 points] Compute Euclidean distance from each instance to the two centroids. (b)   [5 points] Assign instances to the two clusters by finding their closest centroids. (c)    [5 points] Compute the clustering quality with SSE  = ∑i(k)= 1 ∑p∈ci  d(p, mi )2 . (Note: d(p, mi ) is Euclidean Distance between instance p  its centroid mi.) (d)   [5 points] Compute the mean feature values for instances in the two clusters respectively, in the format of (X1, X2 ). (e)    [10 points] Update the two cluster centroids with the mean feature values calculated in step (d), then repeat step (a) – (d) once. Will the clustering result (i.e., cluster allocation) change?  Any improvement in SSE? Please report the代 写Assignment 3 Foundations in Big Data Analytics: Concepts and TechniquesPython 代做程序编程语言 results in one or two tables. For example, answers for Q2(a)-(d) can be reported in below table. Instance X1 X2 (a) Distance to Instance 1 (a) Distance to Instance 4 (b) Cluster Label (d) Updated Centroid 1 1 4

2 1 3

… … …

6 4 0

(c) SSE: Question 3. [24 points] A bank trained a classification model to predict the likelihood of default for each customer.  There are 1000 customers in the database: the “No Default” cases take up 80% of the data while the “Default” cases take up 20%. Applying this  classifier on this dataset yields below confusion matrix.

Predicted Class Default No Default Actual Class Default 150 50 No Default 100 700 As the average lending amount is $100 and interest rate is 10%, the cost-benefit matrix (negative numbers means cost) is:

Predicted Class Default No Default Actual Class Default 0 -$100 No Default 0 $10 (a)    [4  points]  Which  group  (“Default”  or  “No  Default”)  will  you  consider  as  the positive class? (b)   [8 points @ 2 points each] Calculate the followings score for this model: (i)    Accuracy (ii)   True positive rate (Sensitivity) (iii)  True negative rate (Specificity) (iv)  Precision (for the positive class only) (c)    [4 points] Calculate the expected value (per person) for this model. (d)   [4 points] Assume we aim to target the same proportion of customers as in the first table, with only positive predictions will be targeted.   Write  down  the confusion matrix for a random classifier. (e)    [4 points] Calculate the overall expected value (per person) for the random classifier in step (d). Question  4.  [16  points]  Two  classifiers  (Model  A  and  B)  are  used  to  predict  the probability of increase in the Fed Funds rate (i.e., increase vs. no increase), with each quarter considered as an instance. The predicted increase probabilities over the past 6 quarters (instances) are displayed in the following table: Quarter Actual Model A Model B 1 1 0.43 0.63 2 1 0.52 0.53 3 1 0.85 0.56 4 1 0.69 0.71 5 0 0.03 0.18 6 0 0.31 0.76 Please visualize below points with either Python or manually. (a)    [12 points] Plot the ROC curve for the 2 classifiers and the random classifier. Please calculate the TP and FP rates with the following cutoff values: [0, 0.2, 0.4, 0.5, 0.6, 0.8, 1]. (Note: you may need to calculate the TP and FPrates for each cut-offmanually. The visualization can be done with either manually or with Python. ) (b)   [4 points] Which model is better? Why?

   加QQ codinghelp Email: cscholary@gmail.com
