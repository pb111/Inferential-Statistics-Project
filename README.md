# Inferential Statistics with Python Project

**Inferential Statistics** is the process of drawing inferences about the population from the sample data. Inferential Statistics is used to draw inferences from the data that are not immediately available. In this project, I have discussed the inferential statistical concepts and their practical applications. In particular, I have discussed `Central Limit Theorem`, `Hypothesis Testing`, `Types of errors in hypothesis testing`, `z  test`, `t  test`, `ANOVA` , `Chi-square goodness of fit test` and `Correlation coefficient`.


===============================================================================

## Table of Contents


1.	Introduction to inferential statistics
2.	Sample vs Population
3.	Sampling distributions
4.	Central Limit Theorem
5.	Confidence intervals
6.	Hypothesis testing
    -	Null hypothesis
    -	Alternate hypothesis
7.	Types of errors in hypothesis testing
    -	Type I error
    -	Type II error
8.	z test
9.	t test
10.	Different types of t test
11.	ANOVA
12.	Chi-square goodness of fit test
13.	Regression and ANOVA
14.	Coefficient of Determination (R-Square)
15.	Correlation coefficient
16.	References



===============================================================================

## 1. Introduction to Inferential Statistics


Inferential statistics is the branch of statistics that allows us to draw inferences about the population data from the sample data. Inferential statistics help us to conclude whether a sample is significantly different from the population. They help us to find if one model is significantly better than the other. They help us to conduct hypothesis testing.


There are a number of techniques to draw inferences from the sample data. The most important ones are `hypothesis testing`, `z test`,
`t test`, `ANOVA` and `Chi-square goodness of fit test`. In this project, I will discuss these techniques. At first, I will start the discussion by discussing sample and population.


===============================================================================

## 2. Sample and Population

I will start the discussion of population and sample as follows.


### Population

-	A population is a collection of all of the items in the dataset.
-	They are usually denoted with an upper case letter N.
-	The numbers we obtain by using a population are called **parameters**.
-	Populations are hard to define and hard to observe in real life. 
-	Conducting a census on population is an impractical approach because it requires time and financial resources.


### Sample

-	A sample is a subset of the population.
-	They are usually denoted with a lower case letter n.
-	The numbers we obtain by using a sample are called **statistics**.
-	A sample is much easier to gather. They are less time-consuming and cheaper. Time and resources are the main reasons we prefer analysing samples rather populations.
-	They have two key characteristics - **randomness** and **representativeness**.
-	**Randomness** means a random sample is collected when each member of the sample is chosen from the population strictly by chance.
-	**Representativeness** means a representative sample is a subset of the population that accurately reflects the members of the entire population.
-	Sampling is much more practical but it is prone to sampling error.
-	A sample non-representative of the population introduce **bias**. The method chosen for such sampling is called **sampling bias**.
-	`Convenience bias`, `judgement bias`, `size bias` and  `response bias` are main types of sampling bias. 
-	The best technique for reducing bias in sampling is **randomization**. 
-	`Simple random sampling` is the simplest of randomization techniques. 
-	`Cluster sampling` and `stratified sampling` are other systematic sampling techniques.


