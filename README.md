# Amazon Vine Analysis

## Overview of the analysis

For this project I collaborated as a data analyst with Big Market, a company that manages and analyses big data for large companies like $ellby.

Our client $ellby, is an eCommerce platform that's about to launch a large product catalog on a retail website, but needs help comparing how their product reviews compared to the competition are selling and they'd also like to enroll in a program that offers free products to selected reviewers, but first they need to know if this idea will benefit them and if it is worth the investment.

For this analysis, we're going to use AWS, where we're going to create a database and a bucket that will be linked to a server in pgAdmin so that we'll be able to read and analyse our large csv file.

## Results

The first part of our analysis consisted of creating a vine table where we filtered the most important columns to calculate our results (review_id, star_rating, helpful_votes, total_votes, vine,verified_purchase). Then, we spplited the results of the vine program inot two dataframes: paid reviews and unpaid reviews. Here are the results of our dataframes.

images

To further this analysis, we calculated the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for all Vine and non-Vine reviews.

### - How many Vine reviews and non-Vine reviews were there?

Our results show that in total there are 21 vine reviews and 7689 non-Vine reviews.

images

### - How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

We can see from the results that 11 vine reviews were 5 stars and 4444 non reviews were 5 stars.

images

### - What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

This is a very intersting result. The percentage of 5 stars Vine reviews was 52% and the percentage of 5 stars non-Vine reviews was 57%, which means that from this specific dataset there was a higher percentage from non-Vine reviewers.

images

## Summary 

Using bulleted lists and images of DataFrames as support, address the following questions:

the vine program is based on detailed, honest and unbiased opinion. The dataset showed that is a valuable program because even though some customers were paid, the reuslts didn't show a higher percentage of 5 star raitings compared to the unpaid reviewers.

Meaning, that as a seller through the amazon vine program you cannot buy 5 star raitings which makes amazon review systme, reliable.

An additional analysis that I would suggest doing is looking at the non 5 star reviews and analyse if the results lean towards 1 stars or 4 stars reviews.


### Resources

Server: AWS

SQL, PySpark