---
layout: default
---

## Setup

## Downloading the data

The easiest way is to go to the github page and clone the repository OR click the green "Clone or Download" button and "Download Zip".

### Python
<a href="https://www.anaconda.com/download/">Anaconda</a>,
an all-in-one installer, is recommended.

Regardless of how you choose to install it,
<strong>please make sure you install Python version 3.x</strong>
(e.g., 3.7 is fine).

When using the IPython notebook, a programming environment
that runs in a web browser, you will need a reasonably
up-to-date browser. The current versions of the Chrome, Safari and
Firefox browsers are all
<a href="http://ipython.org/ipython-doc/2/install/install.html#browser-compatibility">supported</a>
(some older browsers, including Internet Explorer version 9
and below, are not).

#### Windows
<a href="https://www.youtube.com/watch?v=xxQ0mzZ8UvA">Video Tutorial</a>
<ol>
<li>Open <a href="https://www.anaconda.com/download/">http://continuum.io/downloads</a> with your web browser.</li>
<li>Download the Python 3 installer for Windows.</li>
<li>Install Python 3 using all of the defaults for installation <em>except</em> make sure to check <strong>Make Anaconda the default Python</strong>.</li>
</ol>

#### Mac OS X
<a href="https://www.youtube.com/watch?v=TcSAln46u9U">Video Tutorial</a>
<ol>
<li>Open <a href="http://continuum.io/downloads">http://continuum.io/downloads</a> with your web browser.</li>
<li>Download the Python 3 installer for OS X.</li>
<li>Install Python 3 using all of the defaults for installation.</li>
</ol>

#### Linux
<ol>
<li>Open <a href="http://continuum.io/downloads">http://continuum.io/downloads</a> with your web browser.</li>
<li>Download the Python 3 installer for Linux.<br>
(Installation requires using the shell. If you aren't
comfortable doing the installation yourself
stop here and request help at the workshop.)
</li>
<li>
Open a terminal window.
</li>
<li>
Type <pre>bash Anaconda3-</pre> and then press
tab. The name of the file you just downloaded should
appear. If it does not, navigate to the folder where you
downloaded the file, for example with:
<pre>cd Downloads</pre>
Then, try again.
</li>
<li>
Press enter. You will follow the text-only prompts. To move through
the text, press the space key. Type <code>yes</code> and
press enter to approve the license. Press enter to approve the
default location for the files. Type <code>yes</code> and
press enter to prepend Anaconda to your <code>PATH</code>
(this makes the Anaconda distribution the default Python).
</li>
<li>
Close the terminal window.
</ol>

### Testing If Anaconda was installed


1. Open up the Anaconda Command Prompt
2. Type "ipython" into the prompt
3. You should see Python open up with Python 3.7.x and using the Anaconda distribution
4. Type "quit()" to exit
5. Type "jupyer notebook" to launch the notebook (this may take a while if it is the first time you are launching it)
6. Note the URL (with the token), paste it into your browser
7. Close the anaconda prompt when you're done

### Installing Packages

To install the packages needed for the class you can follow the instructions below:

1. Open your Anaconda Command prompt (Windows)
2. Run the following lines of code
    - note that ctrl+v may not paste in windows,
	  you can paste by pressing shift + insert,
	  or by clicking the icon to the top left of the Anaconda Command promt then edit then paste

If you are just following along with the class, you may only need to run the following command:

Anaconda has everything you need for the class.
However,  f you installed miniconda, instead of Anaconda,
you would need to run the following commands to make sure you have everything.

``` bash
conda install xlwt openpyxl seaborn statsmodels scikit-learn regex odo numba
conda install -c conda-forge feather-format wget
pip install lifelines pandas-datareader
```
