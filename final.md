# Final Projects (30%) 

Working in pairs, students will ask a simple policy question.
To answer it they will identify at least two disjoint data sources, merge them,
perform a simple but correct statistical analysis
and create a simple (but possibly dynamic) dashboard to illustrate this.

## Due Dates

By **November 1**, students should form groups and propose the analysis and project.
The proposal should identify a question and data sources that help them to address it (with links).
It should specify a 'baseline' functionality, describe several extensions, and include a link to the code repository.
(For an example, see [this proposal](http://cfss.uchicago.edu/ACS_final.html) from an earlier version of this class.)

By midnight **December 1st**, all code must be definitively checked in.
A README should detail the sources, describe problems encountered and solutions,
and provide clear instructions for launching the analysis and accessing the output.

During the finals period, we will have 2-hour palooza, in which groups will demonstrate their functioning dashboard
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

* Scope (20%): how many of the extensions did the group complete?  How much does the application do?
* Correctness (25%): is the baseline functionality fully delivered, bug-free?
* Style (25%): are the front-end and code both manageable?
* Performance (15%): is the site 'snappy?'
* Documentation (15%): is the class presentation engaging and interesting?  Does the README actually make it possible to understand how to find your data and run your site?

