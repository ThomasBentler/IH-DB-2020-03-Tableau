# DATABER-20-03-Module2-Project-Tableau


## Project-Tableau- Research - New York City Restaurant Inspections

When searching for a subject and data to use for this Tableau project I stumbled on a dataset with about 400.00 entries of restaurant inspections by the local health authorities ion New York including cuisine types, adresses, dates, grading, scoring and latitudes and longitudes as geographical data, which was intriguiging to include in this project. Originally I had in mind to analyze the food services structure in New York City, yet found that such work had alreeady been done and also that by looking at the data more closely found an even more interesting aspect, which could bring real benefit to users, who want go out to a restaurant in New York City and want to also make their choice based on the best possible data on the status of the place's   food handling hygiene and safety. I found that beyond the hygiene grade provided by the health department data on Nerw York City restaurants that go deeper is not publicly available at a glance, such as actual inspection scores, number of inspections, number of violations recorded, maximum, minumum and average inspection scores hit. To visuialize these parameters per unique restaurant while mouse over on a geographic map was the idea for the solution I had in mind.


## Dataset
https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/43nn-pn8j


## Database
I downloaded the dataset csv file into MYSQL database and started to manipulate the data in such a way that in the end a final table with all parameters for Tableau would be created. These manipulations included changes in Datatype from String to Date, group bys for most recent inspections, for restaurants of specific grades as well as creation of new paramenters and aggregations of new values for scores (MIN, MAX, AVG) and COUNT for number of inspections and number of violations. Besides the grade itself, also if a restaurants grade is pending or if tzhe restaurant has just opened is of importance and needed to be reflected in the final table.


## Workflow
Once the final table was created I connected the database with Tableau and started working with the new data there. Again, the datatypes needed to be checked and column names optimized in regards to the limitations of web publication . In Tableau what I needed to create first was a central metrics list, from which the newly to be created tooltip can pull its values. The standard tooltip itself needed to be expanded and adjusted in pixel for width and height. The parameter names abbreviated due to the limitations of space available. From there everything was quite easy. Creating the geographic maps, creating filters by borough (city district) or by grading was an easy task. All in all I spent 2/3 of my time with data preparation and 1/3 with data visualization, which was a key learning for me. Everything in the data preparation stage took a minimum of twice as long as I had anticipated. In Tableau the complexity lied in pushing a maximum of parameters into a tiny tiny format,which the Tooltip by default only allows.


## Links
Repository:
https://github.com/ThomasBentler/DATABER-20-03-Module2-Project-Tableau

Tableau Public:
https://public.tableau.com/shared/WHJCXBCXQ?:display_count=y&:origin=viz_share_link

Links to Resources:
https://a816-health.nyc.gov/ABCEatsRestaurants/#/faq

Previous Data Science done with this dataset:
https://nycdatascience.com/blog/student-works/nyc-restaurants-reviews-and-inspection-scores/