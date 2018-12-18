Project Goals:
- Determine key parameters/features of home rentals that dictates it's rental price in the city of San Francisco. 
- Highlight key features to inform and provide guidelines to budget-constrained renters.

Project Approach:
- Scrape data from Craigslist using BeautifulSoup4
- Perform linear regression analysis using StatsModels and Scikit-learn libraries in Python

Notes:

Craigslist is a popular website for renters as it contains a relatively large selection of listings with lower prices compared to more modern and newer apartment complexes that are professionally managed or requires management fees. Most of the listings are put up by self managing landlords or tenants looking to sublet a room. Over 3000 listings were scraped between October 6 and 7, 2018. Of the 3000 listings scraped only 763 were unique. These 763 data points were used for this analysis.

10 features were selected, with 3 being continuous, and the rest being categorical. The Target, the rental price is continuous. The linear regression model used was ordinary lease squares. Regularization, adjusting polynomials and functional forms were applied, however, non of those methods improved the model, rather they would lead to overfitting.

Results:

Mean squared error from a 5-fold cross validation resulted in a average of about $852 dollars. This is reasonable given that the average rent is about $3,638 dollars, and the data size was fairly small.
