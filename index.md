---
title: Introduction to Programming for Public Policy
author: James Saxon (jsaxon@uchicago.edu)
---

* Contact: James Saxon (jsaxon@uchicago.edu)
* Discussion Board: [Piazza](https://piazza.com/uchicago/fall2016/ppha30550) – please use!
* Meeting Day/Time: Section 1, MW 9-10:20am; Section 2: MW 1:30-2:50
* Office Hours: Friday afternoon, TBD.

# Course Aims
The past five to ten years have witnessed an explosion in both the collection of ‘big data,’ and the sophistication and accessibility of the tools required to analyze that data. This has spurred government agencies and policy analysts to develop novel, data-driven approaches to policy creation and evaluation.

This is an introductory course in programming and data analysis for public policy students with no prior coding experience. It is for anyone who wants to gather, explore, and share quantitative data – or work with others who do. The course has three goals:

1. Early on, students will learn to think algorithmically using self-contained problems in python.
2. We will then cover tools and recipes for retrieving, cleaning, visualizing, and analyzing data. This will include:
     * The command line. It is the ‘standard’ interface to computers for programmers. We’ll cover how to navigate it and use its many tools.
     * Coding in python: fundamentals of the language including types, control, functions and classes, input/output, complexity theory, debugging. Students will learn to turn a question into a python program.
     * Fundamentals of data science libraries (toolkits) including pandas and geopandas, plotting with matplotlib and seaborn, and basic analysis with scikit-learn.
     * Basics of relational databases – one of the most powerful ways of storing, accumulating, combining, and accessing data.
     * Basic web development: simple websites and an introduction to dynamic sites.
     * Creating datasets and accessing available data: scraping web data and using APIs.
     * Geographic Information Systems (GIS): representing your data in beautiful maps.
     * Large projects depend on many people working together on the same code. Version control (now git) makes this possible. Students will use it to submit all work, and to collaborate on several assignments.
3. Ultimately, students should be comfortable applying skills for research at Harris and beyond, and confident independently exploring new packages for further projects. They should know enough to work with and direct engineers for the projects that they need, and they should understand the potential of such work.

Throughout we’ll emphasize good practices for collaborative code development and strive to de- mystify computers, the internet, and open source software. Particularly after the first weeks, we’ll highlight how these skills apply to evaluating and improving policy.




# Books and Resources
Online documentation ('docs') will provide the principal written resources for the class; sources are listed for each week.
For many code projects/'packages' and languages, these sources are literally _the_ standards that define how to use the products -- and unlike books will keep up with the packages as they evolve.
Locating these sources and using them to identify the methods or recipes you need is an important skill in coding.

This said, several of the O'Reilly books are very good and also happen to be available electronically through the UC library:
  [Think Python](https://catalog.lib.uchicago.edu/vufind/Record/9969856) (Allen Downey),
  [Python for data analysis](https://catalog.lib.uchicago.edu/vufind/Record/9969841) (Wes McKinney), and the
  [SQL cookbook](https://catalog.lib.uchicago.edu/vufind/Record/10176227) (Anthony Molinaro).
Seeing the material multiple times will help -- so please use these resources!!

# Assignments and Grading 
## Weekly assignments (70%)
Assignments will be posted on the class GitHub site at least one week before they are due.
I will de-weight the lowest grade by one half.
The first week's assignment will be graded only for completeness.
Each subsequent assignment will be assessed on: 
* Correctness (60%): does it give the 'right' answer and behave 'correctly' (no crashing or hanging)?
* Style (30%): is the code commented and organized in a reasonable way?  Is the output visually appealing and clear?  Do all plot axes have meaningful, readable labels with units?
* Performance (10%): does it execute in a reasonable amount of time?
Since the parts of an assignment may be cumulative, it is _strongly_ advised to review and start the assignments early, so you can get help through Piazza or at office hours if you get stuck.  Assignments will be collected through GitHub, so get a student account [here](https://education.github.com/pack).

An automatic script will collect work at 1:30am, Wednesday morning.
Since we may review challenging parts of the homeworks in class on Wednesday, 
  late work will be penalized 20%; notify the instructor to 'pull' it when it is complete.  

## Final Projects (30%) 
Working in groups of two or three, students will create a small web application to interactively present data that they have gathered.
Students will choose a subject and propose the functionality to me by November 9.
That proposal should identify data sources, specify a 'baseline' functionality, and describe several extensions.
(You can consider, for instance [this proposal](http://cfss.uchicago.edu/ACS_final.html) from an earlier version of this class.)

### Due Date

Each group will make a five minute presentation of their work (+ 2 minutes for questions) -- the question they sought to ask, the data, the structure of their code and challenges, and basic functionality of their site -- on **November 30**.  Of course, you're welcome to form groups between the two sections, but I do want all group members to participate in the presentation.  Please arrange yourself to attend one of the sessions; I will send a sign-up, to make sure we don't load too heavily to one class.

By midnight **December 2nd**, all code must be definitively checked in, with a README for launching and using the site, mirroring the class presentation (questions, data sources, code structure, site layout).  Please send me a link to your code repositories well in advance.

### The baseline
* Your app must include data from at least two sources, which you will specify to me by Wednesday November 9.  I am much more interested in projects that start from some sort of a "question" and that take the merge seriously.  It is not enough to plot dots representing one type of incident on a choropleth map from another source.
  * Scour the web for city, state, federal, and foreign data portals, BLS, Census, Twitter, or any NGOs that you know.  I'd love to learn about new datasets! 
* You _may_ merge the data once and save it as CSV file (`df.to_csv()`).  Alternatively, if it is feasible and fast, you can use only the existing sources (no cached data).  
* Write at least one function that use the data to make plots or maps.  Varying the inputs (for instance, the variable or the sample) should give me diverse outputs.  In other words: there should be some sort of changeable parameters/selection/menu.
* Integrate that function into a lightweight web application, in Django.  I should be able to navigate around and see a set of nice-looking plots through matplotlib or seaborn.
* The website should look nice.

### Suggested extensions
* I would like you to build a sqlite database from the two sources, and load your data from SQL in your functions.
* The more I can vary your input, the better.  The more meaningful your plots, the better.
* If you want to do some real statistics or analysis, I'd love to see it.
* Depending on what data you use (if this is meaningful), apply a machine-learning method from sci-kit learn, to predict an outcome from inputs.

### Grading
The grading rubric will be modified to benefit ambitious projects:
* Scope (20%): how many of the extensions did the group complete?  How much does the application do?
* Correctness (25%): is the baseline functionality fully delivered, bug-free?
* Style (25%): are the front-end and code both manageable?
* Performance (15%): is the site 'snappy?'
* Documentation (15%): is the class presentation engaging and interesting?  Does the README actually make it possible to understand how to find your data and run your site?

# Where to Work / How to Compute

Part of the overhead to doing computation is getting the software running.
Students are therefore encouraged to install the software required for the class on their personal laptops.
This will enable them to straightforwardly continue using the skills that they develop, when the quarter is over.

Python will be the primary language of instruction for the course.
There are many ways of installing and running it, but I suggest
  [Anaconda](https://www.continuum.io/downloads).
A small program may be scaffolded up on many others, 
  and depend on their being in the correct place with the correct versions in order to function.
(These are called _dependencies_.)
For moderately recent computers, Anaconda handles all of this.
Anaconda installs to a single folder, so you can easily remove it at the end of the course, if so desired.

If you have any concerns about this, talk to me.
If we end up having any trouble with Anaconda, 
   I'll provide an Ubuntu Linux distribution through Docker.

**Bring your laptop to every class** -- short demos will be an important part of the lectures.

# Schedule

## Week 1: Welcome to the Course -- and to the Command line!

### Welcome to the Course.  Command line and version control.  
Case studies of effective use of data in transforming public policy decisions.
Welcome to the command line and to version control.

### First Steps with Python: Data Types and Operations
A first shell script.
Syntax and semantics of the language; comments.
Introduction of the standard data types and operations.

* **Slides**: [Command line](https://github.com/harris-ippp/lectures/blob/master/01/01a_welcome.pdf), [Git](https://github.com/harris-ippp/lectures/blob/master/01/01b_git.pdf), [Python starter/scripts](https://github.com/harris-ippp/lectures/blob/master/01/01b_python.pdf), [Simple Program Notebook](https://github.com/harris-ippp/lectures/blob/master/01/Simple%20Program.ipynb), [Variables and Types Notebook](https://github.com/harris-ippp/lectures/blob/master/01/Variables%20and%20Types.ipynb).
* **Readings**: 
   * Data and Technology in Government: [Innovative State](https://smile.amazon.com/Innovative-State-Aneesh-Chopra/dp/0802121349/) (Aneesh Chopra), and [The Responsive City](https://smile.amazon.com/Responsive-City-Communities-Data-Smart-Governance-ebook/dp/B00MQTIA3M/) (Stephen Goldsmith and Susan Crawford).
   * Python: [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) (Downey), Chapters 1, 2, 10, and 11.  For an alternative take, consult chapters 1-5 of the official [Python Tutorial](https://docs.python.org/3/tutorial/index.html).
   * Git: [Hello World](https://guides.github.com/activities/hello-world/), GitHub Guides.
* **[Assignment](https://classroom.github.com/assignment-invitations/8cfa1521ab98e0dfb7341771721f793b)**:  Command line fu: crime and salary data from Chicago.  Create a [student GitHub account](https://education.github.com/pack), and upload the first week's work.

## Week 2: Python functions, classes, and style.

### Python Introduction Continued: Control Statements and iterating

### Functions, classes, and modules.

* **Slides**: [Control Statements](https://github.com/harris-ippp/lectures/blob/master/02/Control.ipynb), [Functions, Classes and Modules](https://github.com/harris-ippp/lectures/blob/master/02/Functions%2C%20Classes%2C%20and%20Modules.ipynb).
* **Readings**: 
   * Vim: [A vim Tutorial and Primer](https://danielmiessler.com/study/vim/), Daniel Miessler.  % \note{haven't found a great reference}.
   * Shell: [Learning the Shell](http://linuxcommand.org/learning\_the\_shell.php), William E. Shotts, Jr, parts 2, 3, 5, and 6.
   * Python: [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) chapters 3 and 5-8.
* **[Assignments](https://github.com/harris-ippp/02-algorithmic-thinking/blob/master/README.md)**: Simple algorithmic problem solving for several [Project Euler](https://projecteuler.net/) type problems.  Drawing with turtles. 

## Week 3: Debugging, Optimizing, and Reusing.

### Input/Output and data formats.  Options.  Exceptions.
Reading from and writing to files.  CSV, JSON, pickle.
Reusable code.  
Programs and arguments.  

### Debugging and profiling.  Algorithmic complexity and optimization. 
Using `pdb` and `time`.
Big O notation.
Recursive algorithms.
Precomputation.
Asking questions.

* **Slides**: [List comprehension](https://github.com/harris-ippp/lectures/blob/master/03/list_comprehension.pdf), [file formats](https://github.com/harris-ippp/lectures/blob/master/03/files.pdf), [debugging](https://github.com/harris-ippp/lectures/blob/master/03/debugging.pdf), and [complexity](https://github.com/harris-ippp/lectures/blob/master/03/complexity.pdf).
* **Readings**: Official documentation for [input and output](https://docs.python.org/3/tutorial/inputoutput.html), [argparse](https://docs.python.org/3/library/argparse.html) and [pdb](https://docs.python.org/3/library/pdb.html).  [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) Chapter 20 on debugging and 21 on complexity.
   * Coding can be tough, and everyone needs to ask for help sometimes.  Eric Steven Raymond wrote an important (though somewhat snarky) piece on [How To Ask Questions The Smart Way](http://www.catb.org/esr/faqs/smart-questions.html#intro), to get people to respond with the answer you need.  Thinking carefully about your question will often bring you to the answer!
* **[Assignments](https://github.com/harris-ippp/03-sudoku/blob/master/README.md)**:  Solve Sudoku.  Students will work in groups of up to three to solve Sudoku.  (Assignment description)[https://github.com/harris-ippp/03-sudoku/blob/master/README.md] and (repositories)[https://classroom.github.com/assignment-invitations/acb6c296950cc73142b3ba923b8a35fc].

## Week 4: Data Visualization with Python: matplotlib and pandas

### Pandas.
Data imports, slicing, merging, and exploration.

### Plotting and data analysis.
The matplotlib, seaborn, and statsmodels libraries

* **Slides**: [Introduction to Pandas](https://github.com/harris-ippp/lectures/blob/master/04/Introduction%20to%20Pandas.ipynb), [Worked Examples](https://github.com/harris-ippp/lectures/blob/master/04/Examples%2C%20and%20Some%20More%20Features.ipynb).
* **Readings**
   * _matplotlib_: [Beginner's Guide](http://matplotlib.org/users/beginner.html) and [Plotting and Visualization](http://nbviewer.jupyter.org/github/jrjohansson/numerical-python-book-code/blob/master/ch04-code-listing.ipynb), Robert Johansson.
   * _pandas_: Reference for the [Official Documentation](http://pandas.pydata.org/pandas-docs/stable/index.html), with [tutorials](http://pandas.pydata.org/pandas-docs/stable/tutorials.html).  I think [Greg Reda's](http://www.gregreda.com/2013/10/26/intro-to-pandas-data-structures/) is easier to understand for new users.  Once you've read that, Tom Augspurger's [Modern Pandas](https://tomaugspurger.github.io/modern-1.html) (with Jupyter notebooks) gives a bit more detail.
   * _matplotlib_: [Beginner's Guide](http://matplotlib.org/users/beginner.html) and [Plotting and Visualization](http://nbviewer.jupyter.org/github/jrjohansson/numerical-python-book-code/blob/master/ch04-code-listing.ipynb), Robert Johansson.
   * _seaborn_: [tutorial](https://stanford.edu/~mwaskom/software/seaborn/tutorial/distributions.html).
* **[Assignments](https://github.com/harris-ippp/04-pandas/blob/master/README.md)**: Pandas and python.  Problem statement [here](https://github.com/harris-ippp/04-pandas/blob/master/README.md).

## Week 5: Relational Databases

### Relational Databases
What is Structured Query Language (SQL)?  Motivations, use cases.
Data types.  Creating, selecting, updating, dropping, and joining in SQLite.
Database design: primary keys, triggers, and uniqueness and redundancy.
Precomputation revisited.

### Creating and Querying a Simple Database
Importing data.  Aggregation with group; ordering and limiting.  Python interface: `sqlite3`.

* **Slides**: [SQL](https://github.com/harris-ippp/lectures/blob/master/05/sql.pdf), see also the [examples](https://github.com/harris-ippp/lectures/tree/master/05/ex) directory.
* **Readings**: [SQL Cookbook](https://catalog.lib.uchicago.edu/vufind/Record/10176227) Chapters 1-3 and [SQLite Tutorial](http://www.sqlitetutorial.net/).  The [psycopg2 basic model usage](http://initd.org/psycopg/docs/usage.html) and [sqlalchemy](http://docs.sqlalchemy.org/en/latest/orm/tutorial.html) tutorial.
* **[Assignments](https://github.com/harris-ippp/05-sql/blob/master/README.md)**: query data on the American Time Use Survey.  Create a salaries database.  Plot through pandas.

## Week 6: Static Websites and Web Scraping

### The interwebs: pipes and tubes.
The Internet and the world wide web.
Servers and the cloud; Apache, nginx, etc.
The HTTP protocol (there are others)!
Cascading style sheets.

### RESTful APIs, Scraping.

* **Slides**: [The Internet, the Web, and HTML](https://github.com/harris-ippp/lectures/blob/master/06/web_html.pdf), [APIs and Scraping](https://github.com/harris-ippp/lectures/blob/master/06/resources.pdf).
* **Readings**:
   * [The Internet, explained](http://www.vox.com/cards/the-internet) and [40 maps that explain the internet](http://www.vox.com/a/internet-maps), by Timothy B. Lee at Vox (not Tim Berners-Lee, the inventor of the web!).
   * See the w3schools references for [html](http://www.w3schools.com/html/default.asp), [css](http://www.w3schools.com/css/default.asp}{CSS}, and [bootstrap](http://www.w3schools.com/bootstrap/).
   * [Beautiful Soup](http://www.crummy.com/software/BeautifulSoup/bs4/doc/).
* **[Assignments](https://github.com/harris-ippp/06-web/blob/master/README.md)**: Create a simple but professional personal website with at least three sections, and post it to [home.uchicago.edu](http://home.uchicago.edu) (or wherever).  Assemble data from the Virginia elections site.

## Week 7: Dynamic Websites

### Dynamic websites and Django
Dynamic versus static sites: python WSGI, php, cgi, and javascript.
Setting up the test server, and getting your files from week 7 in place.
Simple templates and responses.

### Django: Responding to Queries
Models.  
Get and post revisited.
Incorporating other python modules, and displaying plots.

* **Readings**: The [Django Tutorial](https://docs.djangoproject.com/en/1.9/intro/) and [Using Web Frameworks for Scientific Applications](http://hplgit.github.io/web4sciapps/doc/pub/web4sa_plain_all.html#wf:vib:django), Hans Petter Langtangen.
* **Assignments**: Create a django application to (a) load your website from last week, (b) perform a simple calculation, and (c) present a configurable scatter plot using the SQLite database created in week 5.

## Week 8: Geographic Information Systems

### Introduction to GIS
Shapefiles and data -- what's available?
Working with the QGIS GUI: importing, merging, filtering, and clipping vector layers.
Projections and coordinate reference systems.
Postgres and merging.

### GeoPandas, shapely, and folium: scripting and interactive plotting.

* **Readings**: 
   * QGIS: [QGIS Basics For Journalists](https://multimedia.journalism.berkeley.edu/tutorials/qgis-basics-journalists/), Len De Groot; and the [QGIS Tutorial](http://www.qgistutorials.com/en/index.html).
   * Python GIS: [GeoPandas](http://geopandas.org/) and the [shapely](http://toblerity.org/shapely/manual.html) users manual.
* **Assignment**: make an attractive map for one field profiled by tract for the entire US.  Make a PDF.  Detailed tutorial provided.

## Week 9: Maximizing the Power of Your Data: Multivariate Discrimination

### Theory and context.
Understanding errors versus optimizing results, and their interplay.
Multilayer perceptrons, decision trees, and likelihoods.
Overtraining.
Deep and shallow learning.
### Implementation.
Creating and understanding a (very) simple multilayer perceptron

* **Readings**: [Neural Networks for Pattern Recognition](https://www.amazon.com/Networks-Pattern-Recognition-Advanced-Econometrics/dp/0198538642), Christopher Bishop (fine, this is a book); Statistical Data Analysis, Glen Cowan.  [Supervised Machine Learning: A Review of Classification Techniques](http://www.informatica.si/index.php/informatica/article/download/148/140), S. B. Kotsiantis.
* **Assignment**: None -- time for final project!

## Week 10 and Finals: Project presentations (to be finalized).
