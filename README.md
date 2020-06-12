# eCommerce A/B Testing Project

Run an A/B test to determine if there is a significant difference in purchases between shoppers who remove items from their cart and shoppers who do not remove items from their cart.

People behave differently in different environments. Unlike when shoppers have carts the grociery store, adding an item to an online shopping cart does not nesscitiate the shopper remove items they no longer wish to purchase, or reach the checkout line at all. As the online shopping community continues to grow it becomes increasingly important for marketers to understand consumer behavior in the online environment. This study aims to shed light on such behavior for an eCommerce cosmetics shop. 

 
<img src="Images/cosmetics_banner.jpg"></img>

# DATA:

Events history for a eCommerce cosmetics shop
- November and October 2019
- 9 variables
- Over 4 million rows
- from Kaggle (https://www.kaggle.com/mkechinov/ecommerce-events-history-in-cosmetics-shop)

# Question:
How do we tell when a person is considering making a purchase in an online environment?

# Theory:

# Hypothesis:

Ho: Adding products to a cart and removing products from a cart equally indicate a purchase.

Ha: Removing products from a cart better indicates a purchase than adding products to a cart.


# DATA ANALYSIS:

# 1. Data Preparation:
In this step I prepare the data for analysis.

# 2. Exploratory Analysis:
In this step I explore the shape of the data. 

# 3. A/B Test:
In this step I conduct an A/B test to evaluate the hypotheses. 



# A/B Test Results :
- Statistically different
- Visually different
- Reject the Null

<img src="Images/clustering_by_genre.png" width="650" height="500"></img>

<img src="Images/clustering_by_KMeans.png" width="650" height="500"></img>

### Conclusion: Removing items from a cart better indicate a purchase than adding items to a cart.

- Numeric comparison

<img src="Images/cluster_centers.png"></img>

    * KMeans cluster 0: High energy, high danceability, high valence
    * KMeans cluster 1: High energy, high danceability, low valence
    * KMeans cluster 2: High instrumentalness
    * KMeans cluster 3: Low liveness, low energy, high danceability
   
### Conclusion: Some clusters closely represent genres i.e. rock and cluster 0, while others do not seem to represent any one particular genre but songs with similar metrics within them.

# Next Steps :
- Design a pop-up that incentivizes people to follow through with a purchase/ buy more
   * i.e. spend $5 more and get free shipping
- Implement it at the time someone removes an item from their cart 
- Run more A/B tests to determine if it helps increase sales
   
# Limitations :
- Assumptions
  * I assume each remove_from_cart instance is an intentional act of the user 
