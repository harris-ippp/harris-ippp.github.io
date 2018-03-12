# Mac Install Instructions

### Terminal
You will need to have a **Terminal** set up on your computer.  If you're running a Mac, it _is_ installed.  Just Spotlight search for 'Terminal.'  Easy!

### Python 
Download the **Python 3.6, 64-bit [Anaconda](https://www.continuum.io/downloads)**, and install it on your computer.
* The Graphical User Interface (GUI) installer is easier -- please use it.
* It may ask for your business email -- you can ignore it.)
* If the installer asks whether or not it can edit your .bashrc, the answer is _yes_.
* When the install is complete, open Terminal and type `python`, then hit `<Enter>`.  It should read `Python 3.5.2 |Anaconda...` a new command prompt.  You can test it out (`1 + 1`, then `<Enter>`) and quit (`quit()` or `ctrl+D` on a Mac).
  
You're done with the python part! 

### Atom Text Editor
I encourage you to use [**Atom**](https://atom.io/) as a text editor; it provides syntax highlighting that you will find useful.  The [Download](https://atom.io/) and installation should be trivial.  If you want, you can delete it when you're done.
* Installing a "de-linter" to find bugs in your code will help a lot.  Go to settings (⌘,) and click on "Install."  Then search for "linter-pylint" and install it with all of the dependencies that come up.  Now whenever you save a python file, it will (partially!!) check your work!
* As an alternative, you may sometimes wantto use Jupyter notebooks or Spyder.  Both of these come with your Anaconda installation.
* Atom requires OS X 10.8 or later.  For 10.6 or 10.7, try Sublime or TextWrangler ([4.5.12](http://www.barebones.com/support/textwrangler/updates.html)).

### GitHub 
Create a [**student GitHub account**](https://education.github.com/pack), or just a standard GitHub account.  You will use this account to push (submit) all of your work.  Download and install [git](https://git-scm.com/downloads).
* If your OS is more than five years old (10.7 or 10.8), you may need to get your git from [Sourceforge](https://sourceforge.net/p/git-osx-installer/activity/?page=0&limit=100#57cc86a334309d5c609e9fc8); search for version git-2.3.5-intel-universal-snow-leopard.dmg.  If you did the Window Cygwin setup, it should have included git.

* Tell GitHub who you are, by executing the running the following commands, with appropriate substitutions from the command line (Terminal):
  ```
  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"
  ```

