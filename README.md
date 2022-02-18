# Big_Data_Analysis

## Overview
Amazon has thousands of reviews some are naturally generated and some are given by people who are paid to review the product. This poses one large question; do paid reviews contain bias towards products? To analize this I will be gathering data from vines aws bucket, and comparing non vine reviews with vine reviews.

## Analysis 
The results from my first attempt of this analysis I had gathered the data from the aws bucket and then cleaned it. and stored it into a database with the amazon_review_etl. Then I went forward with the analysis process inside of amazon reviews analysis. 

With the first set of reviews I analized I had noticed there were plenty of Non-Vine reviews to account for a moderately acurate study but there were not nearly enough vine reviews for it to be reliable. This is still the code left in the repository with the results displayed below.

**---------------------------------------------------------- <br>
4 for Vine Reviews <br>
1004 for non-Vine Reviews <br>
---------------------------------------------------------- <br>
Vine Reviews had 1 five star review <br>
Non Vine Reviews had 495 fine star review <br>
---------------------------------------------------------- <br>
25.0 percent of Vine reviews were 5 star <br>
49.30278884462152 percent of Non Vine reviews were 5 star <br>
----------------------------------------------------------** <br>

To get more accurate and useable analysis I went forward with reviewing another dataset. Since vine has all of its datasets formatted the same I was able to simply replace the URL at the Load Amazon Data Into Spark section. In doing this I ran all the cells once again and got much more useable results to provide a better basis for theories. 

**---------------------------------------------------------- <br>
272 for Vine Reviews <br>
30456 for non-Vine Reviews <br>
---------------------------------------------------------- <br>
Vine Reviews had 150 five star review <br>
Non Vine Reviews had 14163 five star review <br>
---------------------------------------------------------- <br>
55.14705882352941 percent of Vine reviews were 5 star <br>
46.50315208825847 percent of Non Vine reviews were 5 star <br>
----------------------------------------------------------** <br>

As you see its very important to have a larger sample size for this sort of study because the results from these two products was so drastically different. 


## Results 

For the results I had three main goals 
- Get the total number of reviews from each source
- Get the total number of five star reviews from each source
- Get the percent of five star reviews fro each source.

**---------------------------------------------------------- <br>
272 for Vine Reviews <br>
30456 for non-Vine Reviews <br>
---------------------------------------------------------- <br>
Vine Reviews had 150 five star review <br>
Non Vine Reviews had 14163 five star review <br>
---------------------------------------------------------- <br>
55.14705882352941 percent of Vine reviews were 5 star <br>
46.50315208825847 percent of Non Vine reviews were 5 star <br>
----------------------------------------------------------** <br>

The second set of data shown above has a good amount of reviews from each source so it should be good to draw conclusions and one thing to notice is that vine has a much higher probability of getting a 5 star review beating non vine reviews b 9%.

Another number that would be good to use for insight is the average number of stars for vine and non vine reviews. This would help show if there is a potential different distrubution for each, because with just these statics there could be different situations where one source --vine or not vine-- could have a high quantity of 4 star reviews that werent considered in the bias for the product. 
