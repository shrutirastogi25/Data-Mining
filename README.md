# **Data Mining**
## B.Sc (hons) Computer Science, University of Delhi
### Practical Guidelines

#### Section 1: Preprocessing
**1.** Create a file "people.txt" with the following data:
_Age   agegroup    height    status    yearsmarried
21      adult      6.0      single        -1
2       child       3       married        0
18      adult      5.7      married        20
221    elderly      5       widowed        2
34      child      -7       married        3_
i. Read the data from the file "people.txt".
ii. Create a ruleset E that contain rules to check for the following conditions:
1. The age should be greater than years married.
2. The age should be in the range 0-150.
3. The status should be widowed, married or single.
4. If age is less than 18 the age group should be child, if age is between 18 and 65, the age group should be adult, if age is more than 65, the agegroup ahould be elderly.
iii. Check whether ruleset E is vio;ated by the data in the file "people.txt".
iv. Summarize the result obtained in part (iii).
v. Visualize the result obtained in part (iii).

**2.** Perform the folllowing preprocessing tasks on the _dirty_iris_ dataset:
i. Calculate the number and percentage of observations that are complete.
ii. Replace all the special values in data with NA.
iii. Define these rules in a seperate text file and read them.
  (Use editfile function in R (package editrules). Use similar function in Python).
  -Species should be one of the following values: setosa,versicolor or virginica.
  -All measured numerical properties of an iris should be positive.
  -The petal length of an iris is at least 2 times its petal width.
  -The septal length of an iris cannot exceed 30 cm.
  -The sepals of an iris are longer than its petals.
iv. Determine how often each rule is broken (violatedEdits). Also summarize and plot the result.
v. Find outliers in septal length using boxplot and boxplot.stats.
[a link](https://raw.githubusercontent.com/edwindj/datacleaning/master/data/dirty_iris.csv)

**3.** Load the data from _wine_ dataset. Check whether all attributes are standardized or not (mean is 0 and standard deviation is 1). If not, standardize the attributes. Do the same with _Iris_ dataset.
[a link](http://archive.ics.uci.edu/ml/datasets/Wine)

---

#### Section 2: Data Mining Techniques
Run the following algorithms on 2 real datasets and use appropriate evaluation measures to compute correctness of obtained patterns:
**4.** Run _Apriori algorithm_ to find frequent itemsets and association rules
  4.1 Use minimum support as 50% and minimum confidence as 75%.
  4.2 Use minimum support as 60% and minimum confidencce as 60%
  
**5.** Use _Naive bayes, K-nearest and Decision tree_ classification algorithms and build classifiers. Divide the data set into training and test set. Compare the accuracy of the different classifiers under the following situations:
  5.1 a. Training set=75% Test set=25%
      b. Training set=66.6% (2/3rd of total), Test set=33.3%
  5.2 Trainign set is chosen by:
      i. Hold out method
      ii. Random subsampling
      iii. Cross-Validation
  Compare the accuracy of the classifiers obtained.
  5.3 Data is scaled to standard format.
  
**6.** Use _Simple Kmeans, DBScan, Hierarchical clustering_ algorithms for clustering. Compare the performance of clusters by changing the parameters involved in the algorithms.

---
