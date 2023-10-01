# Final-Project-Statistical-Modelling-with-Python

## Project/Goals

In this project, I am completing all the questions in Assignment.md file by filling out the notebooks in the 'notebooks' folder, and storing any data into the 'data' folder. 
My goals include getting data from various different website APIs and transforming this data into dataframes and then performing various tasks with the data including visualizing and creating a model.

## Process
- Send an API request to citybikes API to get all bike stations in Toronto, and store results into a dataframe.
- Send an API request to Foursquare API and yelp API for places in each stations lattitude/longitude. Parse through response and store details into a dataframe.
- Explore data from both API results using visualizations.
- Merged Yelp results with citybikes results into one table.
- Stored the merged tables into an SQLite database
- Attempting to create a simple linear regression model

## Results
Got 705 bike stations for Toronto, ON. Got 500 places for the top 50 of the bike station locations through Foursquare API and 1000 from Yelp API. 
Found that Yelp API provided better results as there were more characteristics for each place and more places were returned for each location, thus joined yelp results table with city bikes table for the 'joining_data' notebook in this project.
After viewing the ratings and creating some visualizations, I was able to see that yelp API results have better overall rating then Foursquare API. Got the top 10 rated places from each API response.
Created a simple linear regression model where the dependent variable is 'rating' for the POIs (Places of Interests) and the indepedent variable is the number of bikes in each location. After viewing the outputs of the model,
The R-squared value is 0.003 which means the model is capable of explaining only o.3% of the patterns in the data. Also got valuable information from the 'coef' and 'p>|t| results. From the output, it looks like the independent variable (free_bikes)
does not impact the rating value.


## Challenges 
This project involved a lot of problem solving and applying various techniques to achieve different results. The most time consuming thing for me was making API requests to different website APIs to get data and then parse the data and transform it into a dataframe. 

## Future Goals
Create more visualizations and explore more characteristics of the places returned from each API request. Check more relationships between different variables by creating more models. Take a closer look at the data and understand it better.  
