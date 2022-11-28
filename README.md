![Alt_Text](https://github.com/KevinNourian/Podcast-Reviews/blob/main/Images/podcast-icon-g36b926a37_1280.png)

# Introduction
“Your most unhappy customers are your greatest source of learning.” — Bill Gates

Text mining is the process of deriving insights from unstructured text.

Sentiment analysis is a type of text mining that attempts to understand the emotions expressed in the text through NLP (Natural Language Processing) and ML (machine learning). Based on this information, organizations can position their products or services differently, change their target audience, allocate resources in other ways, or initiate further actions as they deem necessary.

What are the qualities of a good podcast?
Many qualities would make a good podcast. Below are 5 important ones according to some industry analysts:

1. Focus on a central idea
1. Authenticity
2. Knowledge of the subject matter
3. High-quality production
4. Engaging material

Inferential Statistics: Since it is not always practical or even possible to survey an entire population, we study samples of the population to arrive at conclusions about the population. Inferential statistics is the branch of statistics that attempts to arrive at such conclusions. In the case of sentiment analysis, we use inferential statistics to try to infer from the sample data what the population might think or feel.

Confidence Interval: A confidence interval is a tool that shows how certain we are that a population parameter lies within a set of measures arrived at by our sampling methods.

Standard Error: The standard error tells us how far the sample statistic (like the sample mean) deviates from the actual measure (like the population mean).

Hypothesis Testing: A hypothesis is an idea that can be tested. Hypothesis testing is a method that uses inferential statistics to evaluate two mutually exclusive statements about a population and determine which statement is best supported by the sample data. One statement is called the null hypothesis. The other is called the alternative hypothesis.

Null Hypothesis: The null hypothesis is a statement about a population based on our current knowledge. If we accept the null hypothesis, we accept that any observation contrary to it, happened by chance alone and the change that we may be considering will not have the effect we are seeking. Accepting the null hypothesis will lead to no change in opinions or actions.

Alternative Hypothesis: The alternative hypothesis is the opposite of the null hypothesis. It states that our observations regarding the results of the change or innovation did not occur by chance. Accepting the alternative hypothesis may lead to changes in opinions or actions.

Test Statistic: A test statistic contains information about the data that is relevant for deciding whether to reject the null hypothesis. Common test statistics include T-Test, Z-Test, Anova, and Chi-square.

T-Test: A t-test is commonly used when we want to know if a measurement in a sample (like the sample mean) is significantly different from the same measurement in another sample. To use the t-test, the data points must be independent of each other. They must be numerical and generated from random sampling. We must also know the variance of the measurement in each sample. Ideally, the data follow a normal distribution. There are different types of t-tests. For this report, I used the independent two-sample t-test.

Z-Test: A z-test is commonly used when we want to know if a measurement in a sample (like the sample mean) is significantly different from the same measurement in a population (like the population mean). To use the z-test, the data points must be independent of each other. They must be numerical and generated from random sampling. We must also know the standard deviation and mean of the population. Ideally, the data follow a normal distribution.

Type I Error: Type I error occurs when we reject the null hypothesis when it is true.

Type II Error: Type II error occurs when we accept the null hypothesis but it is false.

Level of Significance (α): Since 100% accuracy is not possible for accepting or rejecting the null hypothesis, we select a level of significance, which is the probability of rejecting the null hypothesis when it is true. The level of significance is the probability of making a Type I error. For example, to have a 95% confidence that we are not making a type I error, we set α as .05. This means that there is a 5% probability that we will make a type I error and reject a true null hypothesis.

P-Value: The p-values evaluate how well the sample data support the null hypothesis. Given that the null hypothesis is true, a p-value is the probability of getting the results we obtained from the sample data by random chance alone. We can determine the p-value through t-tests and z-tests.

High P-Value means that our data are likely if the null hypothesis is true. You accept the null hypothesis.
Low P-Values mean that our data are unlikely if the null hypothesis is true. You reject the null hypothesis.

Logistic Regression: Logistic Regression is an algorithm, that classifies categorical outcomes. Logistic Regression is not to be confused with Linear Regression, where the outcome is numerical and continuous. In logistic regression, the maximum likelihood estimate identifies the maximum probability of producing an outcome.

What does this report cover?
In this report, I analyzed nearly two million reviews by listeners of over 100,000 podcasts. Using sentiment analysis and inferential statistics, I arrived at insights that could potentially be useful to current and future podcast creators.

# Goal
To provide usable information for creating good podcasts or improving the quality of existing ones.

# Technical Requirements

1. Download the data.
2. Load data using SQLite and Pandas.
3. Perform exploratory data analysis.
4. Provide clear explanations.
5. Provide suggestions about how the analysis can be improved.

# Datasets

I used 3 databases from Kaggle's Mental Health in the Tech Industry and concentrated on tech industry workers who work for tech companies:

> **Categories**: Contain PodcastID and the associated category of the podcast. <BR>
> **Podcasts**: Contains PodcastID and title of the podcast. It also includes other information that I did not use. <BR>
> **Reviews**: Contains a column called, "Content" with the review written by the listener, ID of the reviewer and the PodcastID. It also includes other information that I did not use. <BR>
> **Runs**: I did not use any information from this table.

The total number of participants in my analysis is 1.9 million.
