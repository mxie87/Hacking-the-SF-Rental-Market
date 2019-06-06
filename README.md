NOTE: please use nbviewer to view jupyter notebook files if it does not load. Simply copy the link to the jupyter notebook file, go to this website: https://nbviewer.jupyter.org/ and paste into the box. 

Project Goals:
- Determine key parameters/features of home rentals that dictates it's rental price in the city of San Francisco. 
- Highlight key features to inform and provide guidelines to budget-constrained renters.

Project Approach:
- Scrape data from Craigslist using BeautifulSoup4
- Perform linear regression analysis using StatsModels and Scikit-learn libraries in Python

Notes:

Craigslist is a popular website for renters as it contains a relatively large selection of listings with lower prices compared to more modern and newer apartment complexes that are professionally managed or requires management fees. Most of the listings are put up by self managing landlords or tenants looking to sublet a room. Over 3000 listings were scraped between October 6 and 7, 2018. Of the 3000 listings scraped only 763 were unique. These 763 data points were used for this analysis.

10 features were selected, with 3 being continuous, and the rest being categorical. The target (rental price) is continuous. The linear regression model used was ordinary lease squares. Regularization, adjusting polynomials and functional forms were applied, however, non of these methods improved the model, rather they would lead to overfitting.

Results:

Root mean squared error from a 5-fold cross validation resulted in a average of about $852 dollars. This is reasonable given that the average rent is about $3,638 dollars, the adjusted R-squared is about .55, and the data set was fairly small.
