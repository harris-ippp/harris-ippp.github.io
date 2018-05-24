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
    * Wednesdays 9am (Darshan), 1:30pm (Ratul - moved to Lecture Hall), 3pm (Umer)
* TA Office Hours:
    * Mondays 11:30 - 12:30 (Minjia - in Room 224), 2pm (Edric - in the Harris Cafe) 
    * Tuesdays 2:50 - 3:50 pm (Nicholas - Harris Cafe)
    * Fridays 3-4pm in Harris Cafe (Umer)
    * Thursdays 3-4pm in 140A (Darshan)
    * Fridays 12-1pm in Harris 140A except 4/27/18 (Ratul)

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

* **Slides**: [Introduction and Command Line](https://github.com/harris-ippp/lectures-s18/raw/master/01/01.pdf), [Git](https://github.com/harris-ippp/lectures-s18/raw/master/01/01_git.pdf), [Python](https://github.com/harris-ippp/lectures-s18/raw/master/01/01_python.pdf)
* **Readings**: 
    * Git: [Hello World](https://guides.github.com/activities/hello-world/), GitHub Guides.
    * Shell: [Learning the Shell](http://linuxcommand.org/lc3_learning_the_shell.php), William E. Shotts, Jr, parts 2, 3, 5, and 6.
    * Asking for help:  Eric Steven Raymond wrote an important (though somewhat snarky) piece on [How To Ask Questions The Smart Way](http://www.catb.org/esr/faqs/smart-questions.html#intro), to get people to respond with the answer you need.  Thinking carefully about your question will often bring you to the answer!
* **Assignment**: [README](https://github.com/harris-ippp/s18-a01/blob/master/README.md) and [Checkout](https://classroom.github.com/a/l08HbtXA)

## Week 2: Introduction to Python

1. First steps with python.
   A first shell script, reviewed.
   Syntax and semantics of the language; comments.
   Introduction of the standard data types and operations:
   `int`, `float`, `string`, `dict`, `list`, etc.
2. Basic formal logic: if, not, and, & or.
   Control statements (`if`, `else`, `break`, `continue`) and iterating with `for` and `while` loops.
   List Comprehension.

* **Slides**: [Python](https://github.com/harris-ippp/lectures-s18/raw/master/02/02.pdf), [Iteration and Algorithms](https://github.com/harris-ippp/lectures-s18/raw/master/02/02b.pdf)
* **Readings**: [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) (Downey), Chapters 1, 2, 10, and 11.  For an alternative take, consult chapters 1-5 of the official [Python Tutorial](https://docs.python.org/3/tutorial/index.html).
* **Assignment**: [README](https://github.com/harris-ippp/s18-a02/blob/master/README.md), [Checkout](https://classroom.github.com/a/ea-FaLox)

## Week 3: Functions, classes, and libraries; manipulating data by hand.

1. Functions: parameters, defaults, and return values.  Scope.
   Member functions, classes and libraries.
2. Reading in data.  Scripts revisited: programs, arguments, and reusable code.
3. Fixing your code: debugging and asking questions.

* **Slides**: [Lists, Strings, and Dictionaries](https://github.com/harris-ippp/lectures-s18/raw/master/03/03.pdf)
* **Readings**: [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) chapters 3 and 5-8.
* **Assignment**: [README](https://github.com/harris-ippp/s18-a03), [Checkout](https://classroom.github.com/a/pwUy3T_U)

## Week 4: Scripts: Putting it Together

A large example: the hospital-resident matching problem

* **Slides**: [Matching](https://github.com/harris-ippp/lectures-s18/raw/master/04/04.pdf), [Sets](https://github.com/harris-ippp/lectures-s18/raw/master/04/04_set.pdf), [Simulation and Plotting](https://github.com/harris-ippp/lectures-s18/raw/master/04/04_simulation.pdf)
* **Code**: [match.py](https://gist.github.com/potash/0473ae32439ff20c46c4c926253ad7de)
* **Readings**:
    * **Before class read: D. Gale and L.S. Shapely [_College Admissions and the Stability of Marriage_](https://www.jstor.org/stable/2312726).**
    * Python: official documentation for [argparse](https://docs.python.org/3/library/argparse.html), [Think Python](http://proquestcombo.safaribooksonline.com.proxy.uchicago.edu/book/programming/python/9781449332006) Chapter 20 on debugging and 21 on complexity.
* **Assignment** [README](https://github.com/harris-ippp/s18-a04/), [Checkout](https://classroom.github.com/a/wYaRwnC9)

## Week 5: Pandas introduction and file formats.

Data Visualization with Python: matplotlib and pandas

1. Pandas data types.  Data frames, series.  
2. Reading basic files.  Basic exploration, slicing and plots.

* **Slides**: [NumPy and Pandas Introduction](https://github.com/harris-ippp/lectures-s18/raw/master/05/05.pdf), [More Pandas](https://github.com/harris-ippp/lectures-s18/raw/master/05/05b.pdf)
* **Readings**
    * Pandas: [Official Documentation](http://pandas.pydata.org/pandas-docs/stable/index.html), with [tutorials](http://pandas.pydata.org/pandas-docs/stable/tutorials.html).  I think [Greg Reda's](http://www.gregreda.com/2013/10/26/intro-to-pandas-data-structures/) is easier to understand for new users.  Once you've read that, Tom Augspurger's [Modern Pandas](https://tomaugspurger.github.io/modern-1.html) (with Jupyter notebooks) gives a bit more detail.
    * Matplotlib [Beginner's Guide](http://matplotlib.org/users/beginner.html) and [Python for Data Analysis, Ch. 8](http://www3.canisius.edu/~yany/python/Python4DataAnalysis.pdf) (McKinney).
* **Assignment** [README](https://github.com/harris-ippp/s18-a05/), [Checkout](https://classroom.github.com/a/RzGTN6cJ)

## Week 6: More Pandas Operations
1. Merging and transforming data
2. Aggregating and summarizing data using groupby
3. Running regressions using statsmodels

* **Slides**: [Pandas Merge, Transformation, and Time Series](https://github.com/harris-ippp/lectures-s18/raw/master/06/06.pdf), [Pandas Group Aggregation and Transformation](https://github.com/harris-ippp/lectures-s18/raw/master/06/06b.pdf), [Pandas Addendum](https://github.com/harris-ippp/lectures-s18/raw/master/06/06c.pdf)
* **Assignment**: [README](https://github.com/harris-ippp/s18-a06/), [Checkout](https://classroom.github.com/a/_G0JiJfQ)

## Week 7: Reading and Scraping Static Websites

1. The Internet and the world wide web.
2. Reading and scraping html.  Beautiful Soup.  HTTP requests.

* **Slides**: [The Web and Scraping](https://github.com/harris-ippp/lectures-s18/raw/master/07/07.pdf), [Scraping](https://github.com/harris-ippp/lectures-s18/raw/master/07/07b.pdf)
* **Readings**:
    * [The Internet, explained](http://www.vox.com/cards/the-internet) and [40 maps that explain the internet](http://www.vox.com/a/internet-maps), by Timothy B. Lee at Vox (not Tim Berners-Lee, the inventor of the web!).
    * [Beautiful Soup](http://www.crummy.com/software/BeautifulSoup/bs4/doc/).
* **Assignment**: [README](https://github.com/harris-ippp/s18-a07), [Checkout](https://classroom.github.com/a/HH-0wNfq)

## Week 8: APIs; Statistical Tools and Visualizations
1. RESTful APIs and hidden APIs: Census, weather, and health.
2. Scipy statistical tests.  Statsmodels -- regressions from data
3. Seaborn

* **Slides**: [APIs](https://github.com/harris-ippp/lectures-s18/raw/master/08/08.pdf),[Visualization and Regression](https://github.com/harris-ippp/lectures-s18/raw/master/08/08b.pdf)
* **Resources**: [Plotly tutorial](https://plot.ly/python/ipython-notebook-tutorial/), and [scipy](https://docs.scipy.org/doc/scipy-0.14.0/reference/stats.html) and [statsmodels](http://statsmodels.sourceforge.net/stable/) documentation.
* **Assignment**: [README](https://github.com/harris-ippp/s18-a08/), [Checkout](https://classroom.github.com/a/k4nitW64)


## Week 9: Relational Databases

1. Relational databases and Structured Query Language (SQL).
   Selecting.
   Data types.
   Pandas integration.
2. Aggregation in SQL and Pandas: `group by`, `order by`, `limit`, `max`, `avg`, etc.

* **Slides**: [Relational Databases and SQL](https://github.com/harris-ippp/lectures-s18/raw/master/09/09.pdf), [More SQL and Python Integration](https://github.com/harris-ippp/lectures-s18/raw/master/09/09b.pdf)
* **Readings**: [SQL Cookbook](https://catalog.lib.uchicago.edu/vufind/Record/10176227) Chapters 1-3 and [SQLite Tutorial](http://www.sqlitetutorial.net/).  The [psycopg2 basic model usage](http://initd.org/psycopg/docs/usage.html).
* **Assignment**: To come.

## Week 10: Intro to Geographic Information Systems
1. Introduction to GIS in QGIS.  Shapefiles and data -- what's available?
   Making a map: projections and coordinate reference systems.
2. Spatial joins and aggregation.
* **Slides**: To come.
* **Readings**: To come.
