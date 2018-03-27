---
title: Introduction to Programming for Public Policy
author: Eric Potash
geometry: margin=1in
documentclass: amsart
fontsize: 11pt
header-includes:
  - \input{js_header.tex}
---

* Instructor: Eric Potash ([epotash@uchicago.edu](mailto:epotash@uchicago.edu))
* TAs: [Ratul Esrar](mailto:resrar@uchicago.edu), [Muhammad Umer Naeem](mailto:umernaeem@uchicago.edu), [Darshan Sumant](mailto:darshansumant@uchicago.edu), [Nicholas Tallant](mailto:ndtallant@uchicago.edu), [Edric Tam](mailto:edrictam@uchicago.edu), [Minjia Zhu](mailto:minjiaz@uchicago.edu)
* Discussion Board: [Canvas](https://canvas.uchicago.edu/courses/15137/).  Please use -- we will monitor.
* Meeting Day/Time: Section 1, TuTh 10:30-11:50am; Section 2: TuTh 1:30-2:50pm
* Office Hours: Tu, Th 3-4pm in 217
* TA Lab Sessions in Harris room 224:
    * Mondays 10:30am (Minjia), 4:30pm (Nicholas)
    * Tuesdays 4:30pm (Edric)
    * Wednesdays 9am (Darshan), 1:30pm (Ratul), 3pm (Umer)
* TA Office Hours:
    * Mondays 11:30 (Minjia), 2pm (Edric)
    * Tuesdays 3:30-4:30pm (Nicholas)
    * Fridays 3-4pm (Umer)
    * Thursdays 3-4pm (Darshan)
    * Fridays 12-1pm in Harris 140C except 4/27/18 (Ratul)

# Course Aims
This is an introductory course in programming and data analysis for public policy students with no prior coding experience;
 it is the first in Harris's new data science sequence.
It is for anyone who wants to gather, explore, and share raw quantitative data – or work with others who do.
Students will learn:

1. Tools for writing and sharing code: text editors, the command line, and version control (git).
2. To think algorithmically, translating self-contained questions into python programs.
   We will cover the fundamentals of the language including types, control, functions, input/output, and scripts.
   We will touch on debugging and (time-permitting) computability.
3. We will then cover tools and recipes for retrieving, cleaning, visualizing, and analyzing data. 
    * Data science libraries: manipulating data with pandas, plotting with matplotlib and plotly, and running basic statistical and geographical analyses (GIS).  The pandas structures resemble R, and are a useful groundwork for the second course in this series.
    * Relational databases (SQL): selecting and aggregating data from databases.
    * Web scraping and APIs: how to retrieve and use public data from the web.

Ultimately, students should be comfortable using what they've learned in further Harris/Chicago courses in programming and statistics (incl. Policy Lab) -- and in research after leaving Harris.
They should be confident independently finding and exploring new packages for those projects.
They should know enough to productively collaborate on projects with engineers, and understand the potential of such work.

Throughout we’ll emphasize good practices for collaborative code development.
Particularly after the first weeks, we’ll highlight how these skills apply to evaluating and improving policy.


# Books and Resources
Online documentation ('docs') will provide the principal written resources for the class; sources are listed for each week.
For many code projects/'packages' and languages, these sources are literally _the_ standards that define how to use the products -- and unlike books will keep up with the packages as they evolve.
Locating these sources and using them to identify the methods or recipes you need is an important skill in coding.
The most relevant starting sites for us will be for [python 3.5](https://docs.python.org/3.5/library/index.html) and [pandas](http://pandas.pydata.org/pandas-docs/stable/).
You will also likely find the question site [Stack Overflow](http://stackoverflow.com/) very useful.


This said, two books published by O'Reilly are very good and available electronically through the UC library:
  [Think Python](https://catalog.lib.uchicago.edu/vufind/Record/9969856) (Allen Downey) and
  [Python for data analysis](https://catalog.lib.uchicago.edu/vufind/Record/9969841) (Wes McKinney).
Seeing the material multiple times will help -- so please use these resources!

# Assignments and Grading 
## Weekly assignments (80%)
Assignments will be due on Thursdays before first section (10:30am sharp) and will posted on this website at least one week in advance. Work will be collected through Chalk and GitHub, so get a student account [here](https://education.github.com/pack).

Unless otherwise noted, problem parts will be graded as follows:
* **Correctness** (3 points): Most questions will have a correct answer.
* **Style** (1 point): Code should be easy to read and well-documented. This is subjective but will be discussed through examples in class and readings.

The lowest homework grade will be dropped.

Since homework solutions will be posted and discussed in lab the following week, late homework can only be accepted until Sunday night with a 10% deduction for each late day (starting Thursdays after 10:30am). Notify the TAs to 'pull' when late homework is complete.

## Quizzes (20%)

There will be a short (about 5 minutes) quiz in lecture every week after week 1.

## Curve

We will follow the standard Harris curve: 1/8 A, 1/4 A-, 1/4 B+, 1/4 B, 1/8 B-.

## Plagiarism policy.

Writing code is substantially different from writing essays:
it is standard practice to find individual functions or google things that don't work, and copy a line or two from the manual or stack overflow.
I encourage you to discuss general strategies for solving problems with your classmates and friends.
Questions and answers on the discussion board will naturally include code.
However -- you should never ask to see another's solutions, and you absolutely should not copy code from your classmates.
No one but you should type your code.
If you find more than a single line/method, you should attribute the source in your comments.

# Setup

Part of the overhead to doing computation is getting the software running.
Students will therefore install the software required for the class on their personal laptops.
This will enable them to straightforwardly continue using the skills that they develop, when the quarter is over.

You will need the command line ([cygwin](https://www.cygwin.com/) on PCs, Terminal on Mac),
python (I will only support the [Anaconda](https://www.continuum.io/downloads) distribution), and a text editor ([Atom](https://atom.io/)).
Installation instructions are posted for [Mac](mac_install) and
[Windows](windows_install).  (If you're using Linux, you can probably figure it out yourself.)
This installation is the entire first week's homework, but it will also be used in the first week's classes!
At a minimum, you should have Atom (and cygwin, for Windows) installed *before the first class.*
We will hold multiple lab sessions in the first week to support installation of the software.
You **must** get the help you need at that point -- we won't provide this support for the entire quarter.

**Bring your laptop to every class** -- short demos will be an important part of the lectures.

# Weekly Schedule

The schedule below will be updated throughout the quarter with links to slides, homeworks, etc. Please check back often.

## Week 1: Welcome, Command line, Git

The homework assignment requires that your installation is complete. Please attend lab for help with this.
**It is absolutely required that your installation work.
You MUST come to one of the six lab sessions or office hours**
One-on-one installation tech support after the first week is at the discretion of the TAs.

1. Welcome to the course: expectations and case studies of effective use of data in transforming public policy decisions.
   Navigating the command line.
2. Writing basic scripts with an editor (Atom).  Running scripts from the command line.
   Getting basic answers to your questions, with bash.
   Uploading them with Git.

* **Slides**: To come.
* **Readings**: 
    * Git: [Hello World](https://guides.github.com/activities/hello-world/), GitHub Guides.
    * Shell: [Learning the Shell](http://linuxcommand.org/lc3_learning_the_shell.php), William E. Shotts, Jr, parts 2, 3, 5, and 6.
    * Asking for help:  Eric Steven Raymond wrote an important (though somewhat snarky) piece on [How To Ask Questions The Smart Way](http://www.catb.org/esr/faqs/smart-questions.html#intro), to get people to respond with the answer you need.  Thinking carefully about your question will often bring you to the answer!
* **Assignment**: To come.

## Week 2: Introduction to Python

1. First steps with python.
   A first shell script, reviewed.
   Syntax and semantics of the language; comments.
   Introduction of the standard data types and operations:
   `int`, `float`, `string`, `dict`, `list`, etc.
2. Basic formal logic: if, not, and, & or.
   Control statements (`if`, `else`, `break`, `continue`) and iterating with `for` and `while` loops.
   List Comprehension.

* **Slides**: To come.
* **Readings**: [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) (Downey), Chapters 1, 2, 10, and 11.  For an alternative take, consult chapters 1-5 of the official [Python Tutorial](https://docs.python.org/3/tutorial/index.html).
* **Assignment**: To come.

## Week 3: Functions, classes, and libraries; manipulating data by hand.

1. Functions: parameters, defaults, and return values.  Scope.
   Member functions, classes and libraries.
2. Reading in data.  Scripts revisited: programs, arguments, and reusable code.
3. Fixing your code: debugging and asking questions.

* **Slides**: To come.
* **Readings**: [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) chapters 3 and 5-8.
* **Assignment**: To come.

## Week 4: Scripts: Putting it Together

1. A large example: networks and inequality.
2. Complexity (time permitting): big-O notation, computability, and pre-computation.

* **Slides**: To come.
* **Readings**:
    * **Before class read: Antoni Calvó-Armengol and Matthew O. Jackson, [_The Effects of Social Networks on Employment and Inequality_](https://www.jstor.org/stable/3592937).**
    * Python: official documentation for [argparse](https://docs.python.org/3/library/argparse.html), [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) Chapter 20 on debugging and 21 on complexity.
* **Assignment** To come.

## Week 5: Pandas introduction and file formats.

Data Visualization with Python: matplotlib and pandas

1. Pandas data types.  Data frames, series.  
2. Reading basic files.  Basic exploration, slicing and plots.

* **Slides**: To come.
* **Readings**
    * Pandas: [Official Documentation](http://pandas.pydata.org/pandas-docs/stable/index.html), with [tutorials](http://pandas.pydata.org/pandas-docs/stable/tutorials.html).  I think [Greg Reda's](http://www.gregreda.com/2013/10/26/intro-to-pandas-data-structures/) is easier to understand for new users.  Once you've read that, Tom Augspurger's [Modern Pandas](https://tomaugspurger.github.io/modern-1.html) (with Jupyter notebooks) gives a bit more detail.
    * Matplotlib [Beginner's Guide](http://matplotlib.org/users/beginner.html) and [Python for Data Analysis, Ch. 8](http://www3.canisius.edu/~yany/python/Python4DataAnalysis.pdf) (McKinney).
* **Assignment**: To come.

## Week 6: Reading and Scraping Static Websites; Querying APIs

1. Reading and scraping html.  Beautiful Soup.  HTTP requests.  School data.
2. RESTful APIs and hidden APIs: Census, weather, and health.
3. The Internet and the world wide web (time-permitting).

* **Slides**: To come.
* **Readings**:
    * [The Internet, explained](http://www.vox.com/cards/the-internet) and [40 maps that explain the internet](http://www.vox.com/a/internet-maps), by Timothy B. Lee at Vox (not Tim Berners-Lee, the inventor of the web!).
    * [Beautiful Soup](http://www.crummy.com/software/BeautifulSoup/bs4/doc/).
* **Assignment**: To come.


## Week 7: Relational Databases

1. Relational databases and Structured Query Language (SQL).
   Selecting.
   Data types.
   Pandas integration.
2. Aggregation in SQL and Pandas: `group by`, `order by`, `limit`, `max`, `avg`, etc.

* **Slides**: To come.
* **Readings**: [SQL Cookbook](https://catalog.lib.uchicago.edu/vufind/Record/10176227) Chapters 1-3 and [SQLite Tutorial](http://www.sqlitetutorial.net/).  The [psycopg2 basic model usage](http://initd.org/psycopg/docs/usage.html).
* **Assignment**: To come.

## Week 8: Statistical Tools and Dashboards.
1. Scipy statistical tests.  Statsmodels -- regressions from data
2. Dashboards with Plotly.

* **Resources**: [Plotly tutorial](https://plot.ly/python/ipython-notebook-tutorial/), and [scipy](https://docs.scipy.org/doc/scipy-0.14.0/reference/stats.html) and [statsmodels](http://statsmodels.sourceforge.net/stable/) documentation.

## Week 9: Large-Scale Example -- Weather and Crime

## Week 10: Geographic Information Systems (Time Permitting)
1. Introduction to GIS in GeoPandas.  Shapefiles and data -- what's available?
   Making a map: projections and coordinate reference systems.
2. Spatial joins and aggregation.

* **Readings**: [GeoPandas](http://geopandas.org/) and the [shapely](http://toblerity.org/shapely/manual.html) users manual.

