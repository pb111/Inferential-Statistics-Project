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

## 2. Sample vs Population

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


===============================================================================

## 3. Sampling distributions


-	A sampling distribution is a probability distribution of a test statistic which is obtained through a large number of samples drawn from a population.
-	As we increase the sample size, sample mean approach towards normal distribution around the population mean. 
-	The variability of the sample mean decreases as the sample size increases.
-	As the sample size increases, the sampling distribution curve follows a normal distribution curve.
-	The shape of the sampling distribution does not reveal anything about the shape of the population.
-	Sampling distribution helps to estimate the population statistic. This will be explained by `Central Limit Theorem`.


===============================================================================

## 4. Central Limit Theorem

-	Central Limit Theorem is one of the most important theorems in probability theory and statistics.
-	It states that, under certain conditions, the sum of a large number of random variables is approximately normal.
-	A version of the Central Limit Theorem applies to i.i.d. (Independent Identically Distributed) random variables.
-	Suppose that X1, X2, …, Xn are i.i.d random variables with 
expected values , E[Xi] = µ < ∞    and   variance , Var[Xi] = σ2  < ∞
-	Then the sample mean has mean µ and variance σ2/n.

### Assumptions underlying Central Limit Theorem

There are several assumptions behind the Central Limit Theorem. These are as follows:-

1.	The dataset must follow the randomization condition. It must be sampled randomly.
2.	Samples drawn should be independent of each other.
3.	Sample size should not be more than 10% of the population size when sampling is done without replacement.
4.	The sample size should be large enough. In general, a sample size of 30 is considered sufficient when the population is symmetric.


### Important points about Central Limit Theorem

There are several important points that we need to keep in mind regarding Central Limit Theorem. These points are as follows:-

1.	CLT is applicable irrespective of the type of the distribution of the population. 
2.	So, given a dataset with unknown distribution, the sample mean will approximate the normal distribution.
3.	The greater the sample size the lower the standard error. So, the greater the accuracy in determining the population mean from the sample mean.

===============================================================================





