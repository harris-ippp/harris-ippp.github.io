---
title: Introduction to Programming for Public Policy
author: James Saxon
geometry: margin=1in
documentclass: amsart
fontsize: 11pt
header-includes:
  - \input{js_header.tex}
---

* Contact: James Saxon ([jsaxon@uchicago.edu](mailto:jsaxon@uchicago.edu)), TAs (2017 TBD)
* Discussion Board: [Chalk](https://chalk.uchicago.edu/).  Please use -- we will monitor.
* Meeting Day/Time: Section 1, MW 9-10:20am; Section 2: MW 1:30-2:50
* Lab Sessions: Thursday and Friday afternoons, time TBD.

# Course Aims
The past decade has witnessed an explosion in the collection of ‘big data,’ and the sophistication and accessibility of the tools required to analyze those data.
This has spurred government agencies and policy analysts to embrace novel, data-driven approaches to policy creation and evaluation.
Yet this development remains hesitant: analysts often rely on pre-processed data for their decisions.

This is an introductory course in programming and data analysis for public policy students with no prior coding experience;
 it is the first in Harris's new data science sequence.
It is for anyone who wants to gather, explore, and share raw quantitative data – or work with others who do.
The course has three goals:

1. We will first introduce students to the basic tools required to write and share: text editors, the command line, and version control (git).
2. Students will learn to think algorithmically using self-contained problems in python: to turn a question into a python program.
   We will cover the fundamentals of the language including types, control, functions, input/output, and scripts.
   We will touch on debugging and (time-permitting) computability.
3. We will then cover tools and recipes for retrieving, cleaning, visualizing, and analyzing data. 
    * Data science libraries: manipulating data with pandas, plotting with matplotlib and plotly, and running basic statistical and geographical analysis (GIS).  The pandas structures resemble R, and are a useful groundwork for the second course in this series.
    * Relational databases (SQL): selecting and aggregating data from databases.
    * Web scraping and APIs: how to retrieve and use public data from the web.

Ultimately, students should be comfortable using what they've learned in further Harris/Chicago courses in programming, statistics, and Policy Lab -- and in research after leaving Harris.
They should be confident independently exploring new packages for further projects.
They should know enough to productively collaborate on projects with engineers, and understand the potential of such work.

Throughout we’ll emphasize good practices for collaborative code development and strive to de- mystify computers, the internet, and open source software.
Particularly after the first weeks, we’ll highlight how these skills apply to evaluating and improving policy.




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
Work will be collected through Chalk and GitHub, so get a student account [here](https://education.github.com/pack).
The first week's assignment will be graded only for completeness, and I will de-weight the lowest grade by one half.
Each subsequent assignment will be assessed on: 

* **Correctness (60%)**: Most questions will be evaluated directly on chalk.  In some cases you will have to submit plots, etc. to GitHub.
* **Style and performance (40%)**: A TA will review your code from GitHub. 
  An automatic script will collect work at 1:30am, Wednesday morning.
  _You are responsible for ensuring that your push was sucessful._
  A per-question rubric out of 4 is as follows:
    0. No apparent effort -- the code is absent or effectively incomplete.
    1. A clear start has been made but the code hangs, crashes or otherwise provides an incomplete answer.
    2. The code is largely complete but gets the wrong answer.  Readily identifiable modifications would result in a working solution.
    3. The answer is correct and the code is readable.
    4. The code is clear, the solution correct, and the commenting appropriate.  If relevant, it runs "quickly."


Since we may review challenging parts of the homeworks in class on Wednesday,
  late work submitted within one week will count for 80%; notify the TAs to 'pull' it when it is complete.
You must complete eight out of the nine assignments to pass the course.

## Final Projects (30%) 

Working in pairs, students will ask a simple policy question.
To answer it they will identify at least two disjoint data sources, merge them,
perform a simple but correct statistical analysis
and create a simple (but possibly dynamic) dashboard to illustrate this.

Please see [final](https://harris-ippp.github.io/final) for full details on the project, and due dates.

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
    * Shell: [Learning the Shell](http://linuxcommand.org/learning\_the\_shell.php), William E. Shotts, Jr, parts 2, 3, 5, and 6.
    * Python: [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) chapters 3 and 5-8.
* **[Assignments](https://github.com/harris-ippp/02-algorithmic-thinking/blob/master/README.md)**: Simple algorithmic problem solving for several [Project Euler](https://projecteuler.net/) type problems.  Drawing with turtles. 

## Week 3: Debugging, Optimizing, and Reusing.

### Input/Output and data formats.  Options.  Exceptions.

Reading from and writing to files.
CSV, JSON, pickle.
Reusable code.
Programs and arguments.  

### Debugging and profiling.  Algorithmic complexity and optimization. 

Using `pdb` and `time`.
Big-O notation.
Recursive algorithms.
Precomputation.
Asking questions.

* **Slides**: [List comprehension](https://github.com/harris-ippp/lectures/blob/master/03/list_comprehension.pdf), [file formats](https://github.com/harris-ippp/lectures/blob/master/03/files.pdf), [debugging](https://github.com/harris-ippp/lectures/blob/master/03/debugging.pdf), and [complexity](https://github.com/harris-ippp/lectures/blob/master/03/complexity.pdf).
* **Readings**: Official documentation for [input and output](https://docs.python.org/3/tutorial/inputoutput.html), [argparse](https://docs.python.org/3/library/argparse.html) and [pdb](https://docs.python.org/3/library/pdb.html).  [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) Chapter 20 on debugging and 21 on complexity.
    * Coding can be tough, and everyone needs to ask for help sometimes.  Eric Steven Raymond wrote an important (though somewhat snarky) piece on [How To Ask Questions The Smart Way](http://www.catb.org/esr/faqs/smart-questions.html#intro), to get people to respond with the answer you need.  Thinking carefully about your question will often bring you to the answer!
* **[Assignments](https://github.com/harris-ippp/03-sudoku/blob/master/README.md)**:  Solve Sudoku.  Students will work in groups of up to three to solve Sudoku.  [Assignment description](https://github.com/harris-ippp/03-sudoku/blob/master/README.md) and [repositories](https://classroom.github.com/assignment-invitations/acb6c296950cc73142b3ba923b8a35fc).

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
Overtraining. Deep and shallow learning.

### Implementation.
Creating and understanding a (very) simple multilayer perceptron

* **Readings**: [Neural Networks for Pattern Recognition](https://www.amazon.com/Networks-Pattern-Recognition-Advanced-Econometrics/dp/0198538642), Christopher Bishop (fine, this is a book); Statistical Data Analysis, Glen Cowan.  [Supervised Machine Learning: A Review of Classification Techniques](http://www.informatica.si/index.php/informatica/article/download/148/140), S. B. Kotsiantis.
* **Assignment**: None -- time for final project!

## Week 10 and Finals: Project presentations (to be finalized).



