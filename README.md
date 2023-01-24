# Amazon Vine Analysis

## Overview of the analysis

For this project I collaborated as a data analyst with Big Market, a company that manages and analyses big data for large companies like $ellby.

Our client $ellby, is an eCommerce platform that's about to launch a large product catalog on a retail website, but needs help comparing how their product reviews compared to the competition are selling and they'd also like to enroll in a program that offers free products to selected reviewers, but first they need to know if this idea will benefit them and if it is worth the investment.

For this analysis, we're going to use AWS, the platform where we're going to create a database and a bucket that will be linked to a server in pgAdmin so that we'll be able to read and analyse our large csv file.

Let's go shopping!! 🛍️

## Results

The first part of our analysis consisted of creating a vine table where we filtered the most important columns to get our results (review_id, star_rating, helpful_votes, total_votes, vine,verified_purchase). 

<img width="746" alt="Screenshot 2023-01-23 at 23 11 41" src="https://user-images.githubusercontent.com/112814924/214214222-7905f443-4cea-4314-9d29-0e7cb7ca58d0.png">

Then, we split the results of the vine program into two data frames: paid reviews and unpaid reviews. Here are the results of our data frames.

<img width="696" alt="Screenshot 2023-01-23 at 23 12 13" src="https://user-images.githubusercontent.com/112814924/214214292-e085a306-d961-4dfb-97ac-3c7d9f7e12e2.png"> 

<img width="715" alt="Screenshot 2023-01-23 at 23 12 26" src="https://user-images.githubusercontent.com/112814924/214214323-913f78e8-48f2-4bd7-9e6a-2325af495a96.png">

To further this analysis, we calculated the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for all Vine and non-Vine reviews.

### - How many Vine reviews and non-Vine reviews were there?

Our results show that in total there are 21 vine reviews and 7,689 non-Vine reviews.

<img width="307" alt="Screenshot 2023-01-23 at 23 12 58" src="https://user-images.githubusercontent.com/112814924/214214352-3409b28f-25fc-4f14-8b96-d19d5cd1d597.png"> 

<img width="339" alt="Screenshot 2023-01-23 at 23 13 41" src="https://user-images.githubusercontent.com/112814924/214214410-ff89afe7-bfd5-40d8-b329-da608a6a233c.png">

### - How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

We can see from the results that 11 vine reviews were 5-star and 4,444 non-Vine reviews were 5-star.

<img width="539" alt="Screenshot 2023-01-23 at 23 13 10" src="https://user-images.githubusercontent.com/112814924/214214496-cd1c11d7-2fb0-48b0-85b0-f0f0d1fe0130.png"> 

<img width="567" alt="Screenshot 2023-01-23 at 23 14 03" src="https://user-images.githubusercontent.com/112814924/214214505-560b8bdd-a191-4ca7-9530-de79df849bf1.png">

### - What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

This is a very interesting result. The percentage of 5-star Vine reviews was 52% and the percentage of non-Vine 5-star reviews was 57%, meaning that from this specific dataset there was a higher percentage of reviewers that are not part of the vine program.

<img width="616" alt="Screenshot 2023-01-23 at 23 13 28" src="https://user-images.githubusercontent.com/112814924/214214534-8da63cb4-4cff-40ea-ba5d-de46d99c030c.png"> 

<img width="635" alt="Screenshot 2023-01-23 at 23 14 13" src="https://user-images.githubusercontent.com/112814924/214214542-ef781ce7-2683-4088-a26c-e2deb85e6e38.png">

## Summary 

The vine program is based on detailed, honest and unbiased opinions. Our dataset showed that this is a valuable program because although some customers were paid to leave their reviews, the results did not show a higher percentage of 5-star ratings compared to non-paid reviewers. 

This means that as a seller through the Amazon Vine program, you cannot buy 5-star reviews, which makes Amazon's review system very trustworthy.

For that reason, our results mean that enrolling in a program that offers free products for reviews may not be the strategy that $ellby should focus on, instead they may consider focusing on the quality, durability and price of the products that will be part of the catalog. This will allow all consumers to leave a real opinion about these products.

One additional analysis I would suggest $ellby is to look at the non-5-star reviews and see if the results skew more towards 1-star or 4-star reviews, to learn about consumer preferences.

### Resources

Platform: AWS

Open Source: PySPark

SQL, Google Colab
