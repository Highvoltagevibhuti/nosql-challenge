**Create NoSql database by importing establishment jason file into new uk_food database.**

Use following command inro gitbash:

mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

mongosh

use uk_food

show collections.

**Part 3: Exploratory Analysis**

1. Which establishments have a hygiene score equal to 20?

**There are 41 establishments which has hygiene score of 20. Please refere file NOSQL_Analysis_starter**

2. Which establishments in London have a RatingValue greater than or equal to 4?

Hint: The London Local Authority has a longer name than "London" so you will need to use $regex as part of your search.

**There are 34 establishments**


3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

Hint: You will need to compare the geocode to find the nearest locations. Search within 0.01 degree on either side of the latitude and longitude.

**Check jupiter notebook** 

4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

Hint: You will need to use the aggregation method to answer this.

	_id	count
0	Thanet	1130

1	Greenwich	882

2	Maidstone	713

3	Newham	711

4	Swale	686

5	Chelmsford	680

6	Medway	672

7	Bexley	607

8	Southend-On-Sea	586

9	Tendring	542
