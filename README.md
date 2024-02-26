# nosql-challenge
Module 12 Challenge - UWA Data Analytics Bootcamp

Before using the code in the 'Main' folder of this repository, load the 'establishments.json' file into MongoDB using this query (executed in a terminal with the directory set to the json containing folder):
mongoimport --db uk_food --collection establishments --drop --file establishments.json --jsonArray

The "Main" folder contains 'NoSQL_setup_starter.ipynb' and 'NoSQL_analysis_starter.ipynb'. 'NoSQL_setup_starter.ipynb' loads, cleans and modulates the data loaded into MongoDB from the 'establishments.json' file.

'NoSQL_analysis_starter.ipynb' runs multiple queries that answer the following questions:

1. Which establishments have a hygiene score equal to 20?
41 establishments have a hygiene score of 20.

2. Which establishments in London have a RatingValue greater than or equal to 4?
33 establishments in London have a RatingValue greater than or equal to 4.

3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
The top 5 establishments sorted by lowest hygiene score are: "Volunteer", "Plumstead Manor Nursery", "Atlantic Fish Bar", "Iceland", and "Howe and Co Fish and Chips - Van 17".

4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
_id	count
Thanet	1130
Greenwich	882
Maidstone	713
Newham	711
Swale	686
Chelmsford	680
Medway	672
Bexley	607
Southend-On-Sea	586
Tendring	542