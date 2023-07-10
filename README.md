# Final-Project-Tableau

## Project/Goals

My goal for this project was to refine my skills in Tableau while honing my data analytics skills to answer questions that I have developed about the NYC airbnb data set. An additional goal was to discover useful, interesting or suprising information about NYC airbnb's

## Process

1) I created a jupyter notebook to allow me to take an easier look at the airbnb data set and make small adjustments if needed
   * I checked the type of each column in the data set
   * I also checked the null count for each column
   * I used imputation to add the mean rating to the null values in the ratings column

2. I used Tabluau to perform some exploratory data analysis on the data set and create some preliminary visuals to help me understand the data in the airbnb data set
   * Analyzed the average reviews and median price for each neighbourhood, property type and room type
     * I chose median price because it is more robust and resistant to price outliers
     * I chose average reviews because there was few outliers in the data set
3. I developed questions based on a bang for your buck basis which I calculated using a weighted avergae
   * The bang for your buck formula is as follows: (0.4 * {[Normalized Median Price]} + 0.3 * {AVG([Review Scores Rating])} + 0.1 * [Normalized Beds] + 0.2 * [Assign Numeric to Room] + 0.1 * [Number Of Reviews] + 0.4 * [Neighbourhood As Numeric])
   * I chose to use a bang for your buck methodology to try and better encompass the decision making process someone goes through when selecting an airbnb for their accomodations
   * The questions I chose:
     1) What neighbourhood, property type and room type have the best bang for your buck
     2) How has the average bang for your buck evolved over time
     3) Has there been noticable changes in bang for your buck growth in the different neighbourhoods
     4) What will Bang for your buck in NYC look like in 3 years
     5) Can the bang for your buck methodology be used to classify the data and what does that tell us about the data itself?

## Results

1. Question 1:
   * Neighbourhood: Manhattan
   * Property Type:
   * Room Type:
2. Question 2:
   * Average bang for your buck has decreased over time from a peak of 34.5 in March 2009 to 27.7 in August 2015
3. Question 3:
   * The compounded growth rate in bang for your buck as converged toward zero, this suggests that as time has gone on the average bang for your buck accross neighbourhoods has stabalized.  However the year to year percent change in bang for your buck is still quite volitile. Additionally, the linear regression model I ran on bang for your buck over time has a negative slope which further emphasizes the decrease in bang for your buck over time.
4. Question 4:
   * According to the multiplicitive forecasting model, bang for your buck will continue to deacrease for airbnb's in NYC which suggests that there will be further price increases relative to the quality of the accomodations that are provided
5. Question 5:
   * Classification of bang for your buck relative to the median price isolates the data into 4 clusters which classify the data based on the price and quality of the accomodation
   * Classification of bang for your buck relative to the average review isolates the data into 3 clusters based on the reviews of the airbnbs
   * Clustering the data in this way helps us analyze how bang for your buck is affected by price and reviews which can help us to better understand the decision making process in selecting and airbnb in NYC

## Challenges

One of the main challenges I faced was creating visualizations that were both pleasing to look at and informative and organizing them in a way that made sense in a dashboard. I wanted to 

## Future Goals

Further refine my bang for your buck calculation to create more variation in its results, run a linear regression model on what affects the bang for your buck the most, in the hopes of better understanding how people might make a decision on selecting their accomodations. Id also like to find a way to add proximity to POI's to improve the data.
