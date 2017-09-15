# Final Projects (30%) 

Working in pairs, students will ask a simple policy question.
To answer it they will identify at least two disjoint data sources, merge them,
perform a simple but correct statistical analysis
and create a simple (but possibly dynamic) dashboard to illustrate this.

## Due Dates

By **October 31**, students should form groups and propose the analysis and project.
The proposal should identify a question and data sources that help them to address it (with links).
It should specify a 'baseline' functionality, describe several extensions, and include a link to the code repository.
(For an example, see [this proposal](http://cfss.uchicago.edu/ACS_final.html) from an earlier version of this class.)

By midnight **December 1st**, all code must be definitively checked in.
A README should detail the sources, describe problems encountered and solutions,
and provide clear instructions for launching the analysis and accessing the output.

During the finals period (December 4, 1:30-3:30), we will have 2-hour palooza,
  in which groups will demonstrate their functioning dashboard
  for others in the class and for the professor and TAs.

## Baseline

* Your dashboard must include data from at least two sources, specified in your proposal.
  I am much more interested in projects that start from some sort of a "question" and that take the merge seriously.
  It is not enough to plot dots representing one type of incident on a choropleth map from another source.
    * Scour the web for city, state, federal, and foreign data portals, BLS, Census, Twitter, or any NGOs that you know.  I'd love to learn about new datasets!
* You _may_ merge the data once and save it as CSV file (`df.to_csv()`).
  Alternatively, if it is feasible and fast, you can use only the existing sources (no cached data).
* Write at least one function that use the data to make plots or maps.  Varying the inputs (for instance, the variable or the sample) should give me diverse outputs.  In other words: there should be some sort of changeable parameters/selection/menu.

## Suggested extensions

* Build a sqlite database from the two sources, and load your data from SQL in your functions.
* The more I can vary your input, the better.  The more meaningful your plots, the better.
* If you want to do some real statistics or analysis, I'd love to see it.
* Depending on what data you use (if this is meaningful), apply a machine-learning method from sci-kit learn, to predict an outcome from inputs.

## Grading
The grading rubric will be modified to benefit ambitious projects:

* Proposal and Interest (20%): does the proposal represent a serious effort to find data and ask or explore an interesting policy question with those data?  It is understood that this is a proposal and not a finished product.  But if you are unsure if you can do a project with a dataset, please ask me or the TAs for input.  You must look at the data, to understand what it can do.  The proposal must be on-time.
* Correctness (20%): is the baseline analysis delivered bug-free with thought for the statistics?
* Scope (20%): how much do you try to do?  You will get points for correct and meaningful: plots, tables, maps, manipulable data (drop-down, etc.), hosting the website online, etc.
* Style (20%): are the front-end and code both navigable?
* Documentation (20%): is the presentation in the data palooza functional and engaging?  Does the README actually make it possible to understand how to find your data and run your site? 

## Datasets for Inspiration

Please go hunting for dataset that interest you.
In the past, students have come up with really great datasets from their home countries.
My suggestions below are super US-centric ones that I've used recently.
But I particularly enjoy seeing foreign datasets.  

* US Census APIs and Geographies
  * [American Community Survey](https://www.census.gov/data/developers/data-sets/acs-5year.html) 5-year estimates.  This is my go-to for demographic data at very good granularity
  * [Decennial Census](https://www.census.gov/data/developers/data-sets/decennial-census.html) is somewhat more precise for ethnic/racial and breakdowns, but the data are less rich.
  * [Health Insurance Statistics](https://www.census.gov/data/developers/data-sets/Health-Insurance-Statistics.html)
  * [City SDK](https://uscensusbureau.github.io/citysdk/) -- from what I can tell, a slightly less-good version of the Census API.
  * Also Check out [TIGER](https://www.census.gov/geo/maps-data/data/tiger.html) for mapping.
* Bureau of Labor Statistics: [main page](https://www.bls.gov/data/) and [python example](https://www.bls.gov/developers/api_python.htm).  Let me know if you use this, and I have examples...
  * [American Time Use Survey](https://www.bls.gov/tus/) -- we used it in class.
* Weather Underground [historical data](https://www.wunderground.com/weather/api/d/docs?d=data/history) has a fantastic, free API for current and historical data.
* City Data portals:
  - [Chicago](): Crime, DIVVY, Grocery Stores
City portals  Chicago, NYC, etc.
  - DIVVY
Illinois Schools
World Health health-data.org
Twitter
Elections v. demographics
  - Louisiana, North Carolina, Virginia, Minnesota, Wisconsin
Stocks

World Bank Development Indicators: 
https://datahelpdesk.worldbank.org/knowledgebase/topics/125589
IPUMS

google map APIs -- elevations, travel time

migration

FBI UCT
https://crime-data-explorer.fr.cloud.gov/api

NLSY

WHO Global Health Observatory http://apps.who.int/gho/data/node.home

Education
https://collegescorecard.ed.gov/data/
https://nces.ed.gov/surveys/hsls09/
https://nces.ed.gov/ccd/
Drop-out rates : https://nces.ed.gov/ccd/drpcompstatelvl.asp

National Assessment of Educational Progress
https://nces.ed.gov/nationsreportcard/naepdata/

Migration -- LODES, etc

