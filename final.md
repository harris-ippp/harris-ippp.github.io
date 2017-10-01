# Final Projects (25%) 

Working in pairs, students will ask a simple policy question.
To answer it they will identify at least two disjoint data sources, merge them,
perform a simple but correct statistical analysis
and create a simple (but possibly dynamic) dashboard to illustrate this.

## Due Dates

By **October 31**, students should form groups and propose the analysis and project.
The proposal should identify a question and data sources that help them to address it (with links).
A number of data sources are listed below, for inspiration.
It should specify a 'baseline' functionality, describe several extensions, and include a link to the code repository.

By midnight **December 1st**, all code must be definitively checked in.
A README should detail the sources, describe problems encountered and solutions,
and provide clear instructions for launching the analysis and accessing the output.

During the finals period (December 4, 1:30-3:30), we will have 2-hour palooza,
  in which groups will demonstrate their functioning dashboard
  for others in the class and for the professor and TAs.

## Baseline

You are aiming for something like our week 9 example on weather and crime.
You can see a straightforward writeup of this work, here:

https://harris-ippp.github.io/weather

* Your work must* include data from at least two sources, specified in your proposal.
  I am much more interested in projects that start from some sort of a "question" and that take the data merge seriously.
  This is not a statistics class, and I'm not looking for iron-clad causality.  But neither am I interested in a scatter plot of two random variables.
  * It is not enough to plot dots representing one type of incident on a choropleth map from another source, or plot school quality against crime rates.
  * *I will make an exception for the two source rule, if one or more of the parameters require significant cleaning.  For example, fertility histories in the NLSY are very, very messy.  So too, are some state election returns.  But this is the exception, and you must discuss this with me before your proposal.
* Produce plots and tables and develop a sensible model with statsmodels.  Give that model a workout.
* Describe what you have done in a clean and presentable notebook (or website), preferably with some degree of manipulability.
* Document your technical work in the README file.

## Suggested extensions

* I recognize that not all data sources are equally easy to use.  I will reward efforts to use datasets that are take a bit of work.  For instance, lining up two 20-line excel spreadsheets... not that impressive.
* Build a sqlite database from the two sources, and load your data from SQL in your functions.
* Mapping the data... more points for "[very complex](http://saxon.harris.uchicago.edu/~jsaxon/migration/migration.html)") maps.
* Build a website, and put it online as you did in Week 6.  You are welcome to use html as in HW6, or Jekyll themes on GitHub to do this, as I do for the class websites.  More points for your own, navigable HTML or Jekyll; less points for copying your jupyter notebook.
* Depending on what data you use (if this is meaningful), apply a machine-learning method from sci-kit learn, to predict an outcome from inputs.  See [slides](https://github.com/harris-ippp/lectures/blob/master/old/nn/nn.pdf) from last year's class.  (This is fire -- be careful with this stuff in the real world.)
* Build interactive functions or a dashboard as in our Thanksgiving lectures.
* Use a machine learning model (sci-kit learn), to predict one outcome from inputs.  But you must be careful that the predictor makes sense.

## Grading
The grading rubric will be modified to benefit ambitious projects:

* Proposal and Interest (20%): does the proposal represent a serious effort to find data and ask or explore an interesting policy question with those data?  It is understood that this is a proposal and not a finished product.  But if you are unsure if you can do a project with a dataset, please ask me or the TAs for input.  You must look at the data, to understand what it can do.  The proposal must be on-time.
* Correctness (20%): is the baseline analysis delivered bug-free with thought for the statistics?
* Scope (20%): how much do you try to do?  You will get points for correct and meaningful: plots, tables, maps, manipulable data (drop-down, etc.), hosting the website online, etc. -- see "extensions."
* Style (20%): are the front-end and code both navigable?  Is the code well-commented?  Does its division among files make sense?  Do all plots have appropriate legends and labels?  
* Documentation (20%): is the presentation in the data palooza functional and engaging?  Does the README actually make it possible to understand how to find your data and run your site?  Is your code well-commented?

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
  * [Migration flows](https://www.census.gov/data/developers/data-sets/acs-migration-flows.html)
  * Commuting patterns: [LODES](https://lehd.ces.census.gov/data/)
  * Also Check out [TIGER](https://www.census.gov/geo/maps-data/data/tiger.html) for mapping.
* [National Longitudinal Survey of Youth](https://www.nlsinfo.org/content/cohorts) -- one of the great datasets of all time, but it can be a lot to bite off.
* [Integrated Public Use MicroSamples](https://usa.ipums.org/usa/) -- standardizes data across many Censuses and the ACS.  Great for time series or old data.
* Bureau of Labor Statistics: [main page](https://www.bls.gov/data/) and [python example](https://www.bls.gov/developers/api_python.htm).  Let me know if you use this, and I have examples...
  * [American Time Use Survey](https://www.bls.gov/tus/) -- we used it in class.
* City Data portals (I looked at a bunch of crime, whence the slant... but it's legitimately one of the more interesting datasets that they release)
  * [Chicago](https://data.cityofchicago.org/): [Salaries](https://data.cityofchicago.org/Administration-Finance/Budget-2017-Budget-Ordinance-Positions-and-Salarie/x94i-grxu), [Crime](https://data.cityofchicago.org/view/5cd6-ry5g), [DIVVY trips](https://data.cityofchicago.org/Transportation/Divvy-Trips-Dashboard/u94x-unre), [Grocery Stores/Food Deserts](https://data.cityofchicago.org/Community-Economic-Development/Grocery-Stores-2013/53t8-wyrc/data), [CTA Ridership](https://data.cityofchicago.org/Transportation/CTA-Ridership-L-Station-Entries-Monthly-Day-Type-A/t2rn-p8d7/data)
  * [New York](https://data.cityofnewyork.us/browse?provenance=official&sortBy=most_accessed&utf8=%E2%9C%93): e.g., [Crime](https://data.cityofnewyork.us/Public-Safety/NYPD-7-Major-Felony-Incidents/hyij-8hr7), 
  * [Philadelphia](https://www.opendataphilly.org/dataset): [Crime](https://www.opendataphilly.org/dataset/crime-incidents), [Traffic Cameras](https://www.opendataphilly.org/dataset/red-light-cameras), [School Survey](https://data.cityofnewyork.us/Education/NYC-School-Survey/kwk4-6u9e)
  * [San Francisco](https://datasf.org/opendata/): [Crime](https://data.sfgov.org/Public-Safety/Police-Department-Incidents/tmnf-yvry)
  * [Boston](https://data.boston.gov/): [Crime](https://data.boston.gov/dataset/crime-incident-reports-july-2012-august-2015-source-legacy-system)
* [FBI Unified Crime Reports](https://crime-data-explorer.fr.cloud.gov/api) ... to complete the crime spree
* [National Center for Education Statistics](https://nces.ed.gov/) and its [DataLab](https://nces.ed.gov/datalab/)
  * [CollegeScorecard](https://collegescorecard.ed.gov/data/) (not an API, but the superficial information is trivially extractable)
  * [Common Core Data](https://nces.ed.gov/ccd/)
  * [High School Longitudinal Study](https://nces.ed.gov/surveys/hsls09/)
  * [Drop out rates](https://nces.ed.gov/ccd/drpcompstatelvl.asp)
  * [National Assessment of Educational Progress](https://nces.ed.gov/nationsreportcard/naepdata/)
  * [International Dat Explorer](https://nces.ed.gov/surveys/pisa/idepisa/report.aspx)
  * Also... [used.gov](https://usedgov.github.io/)
* Illinois [Report Card](https://illinoisreportcard.com/) doesn't have an API, but it's very scrap-able.
* Institute for Health Metrics and Evaluation: http://healthdata.org
  * It's not an API, but with a little bit of work, you can pull all their data right out.
* [World Bank Development Indicators](https://datahelpdesk.worldbank.org/knowledgebase/topics/125589)
* [WHO Global Health Observatory](http://apps.who.int/gho/data/node.home)
* Voting -- State Election Returns (this is an area I know very well -- ask if you're interested)
  * It's very easy to find good [county-level election returns](https://github.com/tonmcg/County_Level_Election_Results_12-16) for national elections.  Precinct-level is harder.
  * Louisiana [Official](https://voterportal.sos.la.gov/Graphical), but json [backend](https://voterportal.sos.la.gov/ElectionResults/ElectionResults/Data?blob=20161108/VotesRaceByPrecinct/Votes_53898_01.htm), and [maps](http://house.louisiana.gov/H_Redistricting2011/default_LouisianaPrecinctShapefiles.htm) available.
  * North Carolina [returns](http://er.ncsbe.gov/downloads.html?election_dt=11/08/2016)  and [maps](http://dl.ncsbe.gov/index.html?prefix=PrecinctMaps/)
  * Virginia [returns](http://historical.elections.virginia.gov/elections/search/year_from:1924/year_to:2016/office_id:1/stage:General) and [maps](https://github.com/vapublicaccessproject/va-precinct-maps-2016)  (Actually, I've fixed those maps...)
  * [Minnesota](https://gisdata.mn.gov/dataset/bdry-electionresults-2012-2020) 
  * [Wisconsin](http://data-ltsb.opendata.arcgis.com/datasets/e702e29dbdf74d3b8b153c06fac2c721_0)
  * Ask if you want more -- these are a pain to work with.  But you can get TN, MD, TX, FL, etc.
* Stocks: These are constantly breaking (Google and Yahoo just did).  But check out [Bloomberg](https://www.bloomberg.com/professional/support/api-library) and you can look around for a way to hack google finance.  As Harris students, you also have access to the Bloomberg terminal in the basement...
* Twitter has one of _the_ great [APIs](https://dev.twitter.com/rest/public)
* [google maps](https://developers.google.com/maps/documentation/) -- they have APIs for elevations (biking!?), travel times (isolation?), distances, geolocation, etc.
* Weather Underground has a [fantastic, free API](https://www.wunderground.com/weather/api/d/docs?d=data/history) for current and historical weather data.

