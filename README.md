# Amazon_Vine_Analysis


## Overview

This analysis was performed to assess the written reviews by members of the paid Amazon Vine program. This program is a service that allows manufacturers and publishers to receive reviews for their products. The way it functions is that companies will pay a fee to Amazon and provide products to these members, who will be required to publish a review.

The analysis is to look if there is any bias between reviews made by these members vs the reviews of people that are not part of the program. The assessment was done to a dataset focused on videogames that can be found in the following link. (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)


## Results

To understand how the reviews were made it was proposed three questions:
* How many Vine reviews and non-Vine reviews were there?
* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

With help of Google Collaboratory and Pyspark the data set was polished and recorded the following answers to the questions asked:

*** DataFrame

<img width="990" alt="Screen Shot 2022-10-19 at 19 44 04" src="https://user-images.githubusercontent.com/104656920/196830467-b3780ef4-1d38-4e2e-9b23-4370cd2095e6.png">



1. *How many Vine reviews and non-Vine reviews were there?*


<img width="1395" alt="Screen Shot 2022-10-19 at 19 42 27" src="https://user-images.githubusercontent.com/104656920/196830356-07aaf3af-8d48-421c-b055-4319e05abf95.png">

  * Total Vine Reviews: 90
  * Total non-Vine Reviews: 37,831
  
 
2. *How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?*

<img width="638" alt="Screen Shot 2022-10-19 at 19 46 39" src="https://user-images.githubusercontent.com/104656920/196830708-13d75b80-5726-4b92-9cca-a02e72430547.png">

  * Total 5 stars Reviews: 14,748
  * Total 5 stars Vine Reviews: 44
  * Total 5 stars non-Vine Reviews: 14,704

3. *What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?*

<img width="632" alt="Screen Shot 2022-10-19 at 19 49 57" src="https://user-images.githubusercontent.com/104656920/196831214-58138fe3-3e67-473f-92fb-839ac2936c51.png">

* Vine reviews 5 stars percentage: 48.89%
* non-Vine reviews 5 stars percentage: 38.88%




## Summary 

After reviewing the dataset, we can see that members of the Vine program actually have a positive bias towards the products comparing to the customers that are not part of the program, because the Vine reviews have a 10% more probability to be reviewed with a five star rating.

If needed it could done another assessment with the dataset given by looking for bias but with another perspective, looking into poor reviews of the products. To see if it is likely that Vine members review a product with low star count(0,1,2).




