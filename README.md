![Alt_Text](https://github.com/KevinNourian/Podcast-Reviews/blob/main/Images/podcastreviews_logo.png)

# Introduction
“Your most unhappy customers are your greatest source of learning.” — Bill Gates

In this report, I analyzed nearly 2 million reviews by listeners of over 100,000 podcasts. Using sentiment analysis and inferential statistics, I hoped to arrive at insights that could potentially be useful to current and future podcast creators.

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
