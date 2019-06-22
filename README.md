# Inferential Statistics with Python Project

**Inferential Statistics** is the process of drawing inferences about the population from the sample data. Inferential Statistics is used to draw inferences from the data that are not immediately available. In this project, I have discussed the inferential statistical concepts and their practical applications. In particular, I have discussed `Central Limit Theorem`, `t- test`, `ANOVA` , `Chi-square goodness of fit test` and `Correlation coefficient`.


===============================================================================

## Table of Contents


1.	Introduction to inferential statistics
2.	Sample vs Population
3.	Sampling distributions
4.	Central Limit Theorem
5.	t test
6.	Different types of t test
7.	ANOVA
8.	Chi-square goodness of fit test
9.	Regression and ANOVA
10.	Coefficient of Determination (R-Square)
11.	Correlation coefficient
12.	References


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

## 5. t-Test

-	In statistics, a t-test is a type of inferential statistic. 
-	The t-test is a statistical hypothesis test in which the test statistic follows a Student’s t-distribution under the null hypothesis. 
-	It is used to determine if there is a significant difference between the means of two groups. 
-	It is most likely used when the dataset follow a normal distribution and may have unknown variances.
-	A t-test is used as a hypothesis testing tool, which allows testing of an assumption applicable to a population.


### t-Test Assumptions

There are several assumptions regarding the t-Test. These are as follows:-

1.	The sample mean X̅ follows a normal distribution with mean μ and variance σ2/n, where μ and σ are the mean and standard deviation of the population and n is the sample size.
2.	The square of the standard error of the mean, s2 follows a χ2 distribution with n-1 degrees of freedom.
3.	The second assumption is that the data is collected from a representative and randomly selected portion of the total population.
4.	The sample size used should be reasonably large enough. A large sample size means the distribution of results should approach a normal bell-shaped curve.
5.	The final assumption is the homogeneity of variance. Homogeneous or equal variance exists when the standard deviations of samples are approximately equal.


### Steps to perform a t-Test

-	A t-Test allows us to compare the average values of the two data sets and determine if they came from the same population. 
-	Basically, there are four steps involved in performing a t-Test. These are as follows:-


#### 1. Define a problem statement

-	The first step is to define a problem statement.
-	In the problem statement, we set up the null hypothesis (Ho) by assuming that the two sample means from each of the two data sets are equal.


#### 2. Calculate a t-statistic

-	The second step in conducting a t-Test is to calculate a t-statistic value. 
-	The calculation of a t-statistic requires three key data values.
-	They include the difference between the mean values from each data set (difference in means), the standard deviation of each group and the number of data values in each group.


#### 3. Compare the t-statistic value with t-distribution values

-	The outcome of the t-test yields a t-statistic value.
-	This t-statistic value is then compared against a value obtained from a critical value table (called the T-Distribution Table).
-	This comparison helps us to conclude whether the difference between means occurred by chance or whether the data sets really have intrinsic differences.
-	The t-Test questions whether the difference between groups represents a true difference in the study or if it is just a meaningless statistical difference.


#### 4. Interpret the result

-	The t-distribution table is available in one-tail and two-tail formats.
-	The one-tail format is used in those cases where the t-statistic have a fixed value with a clear direction (positive or negative).
-	The two-tail format is used in cases where the t-statistic falls in a bounded range.
-	The t-test produces two values as its output – t-value and degrees of freedom.
-	Higher values of the t-value, also called t-score, indicate that a large difference exists between the two sample sets. So, a large t-score indicates that the groups are different.
-	The smaller the t-value, the more similarity exists between the two sample sets. A small t-score indicates that the groups are similar.


#### Decision criteria

-	Alternatively, once the t-value and degrees of freedom are determined, a p-value can be found using the table of values from Student’s t-distribution. 
-	If the calculated p-value is below the threshold value for statistical significance, then we reject the null hypothesis in favour of the alternative hypothesis.


## Types of t-Test

There are three different types of t-test that can be performed depending on the data and requirement. These are 1-sample, 2-sample and Paired t-test. Their description are as follows:-


### 1. One-sample t-test

-	One-sample t-tests are appropriate when a sample is being compared to the population from a hypothesis. 
-	The population parameters are known in advance or are calculated from the population data.
 
-	In testing the null hypothesis (Ho) that the population mean is equal to a specified value μ0, we use the t-statistic given by

![t-statistic](https://github.com/pb111/Inferential-Statistics-Project/blob/master/Images/t-statistic.png)

-	x̅ is the sample mean. 
-	s is the sample standard deviation of the sample and n is the sample size. 
-	The degrees of freedom used in this test are n − 1. 
-	The parent population does not need to be normally distributed, but the distribution of the population of sample means x̅ is assumed to be normal. 
-	By the central limit theorem, if the observations are independent and the second moment exists, then t will be approximately normal N(0,1).


### 2. Independent two-sample t-test

-	Two-sample t-tests are appropriate for comparing two samples. 
-	These tests are typically experimental and evaluate samples from a controlled experiment.
-	The two-sample t-test takes sample data from two groups and calculates the t-value.
-	The 2-sample t-test requires independent groups for each sample.
-	In this case, the t-statistic used is given by the following formula. 


![Two-sample t-test](https://github.com/pb111/Inferential-Statistics-Project/blob/master/Images/2-sample%20t-test.png)


-	where the symbols have their usual meanings.


### 3. Paired t-test

-	This test is used when the samples are dependent. 
-	It is used when there is only one sample that has been tested twice (repeated measures) or when there are two samples that have been matched or "paired".
-	The test statistic used in this case is given by

![Paired t-test](https://github.com/pb111/Inferential-Statistics-Project/blob/master/Images/Paired%20t-test.png)

-	The symbols have their usual meanings.
-	The degree of freedom used is n − 1, where n represents the number of pairs.


===============================================================================

## 6. ANOVA

-	ANOVA is an acronym for **Analysis of Variance**.
-	It can be used in cases where we want to compare the means of more than two groups.
-	The ANOVA test allows a comparison of more than two groups to determine whether a relationship exists between them.
-	The result of the ANOVA formula, the F-statistic (also called F-ratio) allows for the analysis of multiple groups of data to determine the variability between samples and within samples.
-	The null hypothesis (Ho) is that there is no real difference exists between the tested groups. So, the result of the ANOVA’s F-ratio statistic will be close to 1.


### Formula for ANOVA

-	The Formula for ANOVA is given by the following formula-

# D-Formula for ANOVA

-	F=ANOVA coefficient
-	MST=Mean sum of squares due to treatment
-	MSE=Mean sum of squares due to error


### Assumptions used in ANOVA

There are four basic assumptions used in ANOVA. They are given below:-

1.	The expected values of the errors are zero.
2.	The variances of all errors are equal to each other.
3.	The errors are independent.
4.	They are normally distributed.


There are various types of ANOVA test used in practice. These are as follows:-


### 1. One way ANOVA

-	When we are comparing more than three groups based on one factor variable, then it is said to be **One way ANOVA**.
-	The null hypothesis (Ho) for the test is that the means of the groups are equal.
-	Therefore, a significant result means that the two means are unequal.


### Limitations of one-way ANOVA

-	A one way ANOVA test will tell us that at least two groups were different from each other.
-	But, it won’t tell us what groups were different.
-	If the test returns a significant f-statistic, we may need to run another test like Least Significant Difference to examine which groups had a difference in means.


### 2. Two way ANOVA
-	A two way ANOVA is just the extension of the one way ANOVA.
-	When we have more than one factor variable, then it is said to be **Two way ANOVA**.
-	It is utilized to observe the interaction between the two factors and tests the effect of two factors at the same time.


## Key terms and concepts


### Sum of square between groups

-	For the sum of the square between groups, we calculate the individual means of each group.
-	Then we take the difference between data points from the individual mean for each group. 
-	Finally, we will take the sum of the square of difference for all the individual groups.


### Sum of squares within group

-	In order to get the sum of squares within a group, we calculate the grand mean for all groups and then take the deviation from the individual group.
-	The sum of all groups will be done after the square of the deviation.


### F-ratio

-	To calculate the F-ratio, the sum of the squares between groups will be divided by the sum of the square within a group.


### Degree of freedom

-	To calculate the degree of freedom between the sums of the squares group, we will subtract one from the number of groups. 
-	The sum of the square within the group’s degree of freedom will be calculated by subtracting the number of groups from the total observation.

===============================================================================
