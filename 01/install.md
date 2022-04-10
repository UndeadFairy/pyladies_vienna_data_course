# Installation

Installing everything you need is not complicated and only takes a moment. If during it
after all, something goes wrong, ask Slack or someone more experienced for advice.

The next steps are to have Python 3.6, 3.7 or 3.8 installed and working.
If not, one of the following three alternative paths should easily lead you to such a situation:

- If you have updated Windows 10, the easiest way is to use the installation from [Microsoft Store] (https://www.microsoft.com/store/productId/9MSSZTT1N39L).

- General installation instructions are available [in the beginner's course] (https://naucse.python.cz/course/pyladies/sessions/install/). When you choose the installer, reach for it with the latest version (at the beginning of the 3.8.8 course), ideally in the 64-bit version.

- You can use the [miniconda] distribution (https://docs.conda.io/en/latest/miniconda.html), there are usually no problems with it. People in the field of data science (including some authors of these materials) like to use it - while preparing to work with "pure" Python, they simplify the installation of some (especially computational) libraries that depend on external binary packages. The command `conda` is used for creating virtual environments and installation, see [documentation] (https://docs.conda.io/projects/conda/en/latest/user-guide/index.html).

## Directory, creation and activation of a virtual environment

First, prepare a directory for storing files (for example `pydata`) and create one in it
virtual environment.

If you don't know how to do this, the complete instructions are the same as for installing Python
in [beginner course materials] (https://naucse.python.cz/2019/pyladies-ostrava-podzim/beginners/venv-setup/).

Each time you run the command line, you will need to activate the virtual environment so that
they could work with the libraries and tools installed in it.

## Installing libraries

At the command prompt with the virtual environment active, enter the following command:

`` `shell
(venv) $ python -m pip install jupyter pandas matplotlib requests seaborn scipy scikit-learn sqlalchemy plotly xlrd openpyxl
`` `

This command installs the following libraries (and some other dependencies) in the virtual environment:

* Jupyter - web interface for interactive and reproducible work with Python
* Matplotlib - one of the most famous libraries for creating graphs
* Openpyxl - library for loading and writing .xlsx files
* Pandas - for working with tabular data
* Plotly - a library for creating interactive graphs
* Requests - a library for working with HTTP (web and API) requests
* Scikit-learn - a collection of the best known algorithms for machine learning
* SciPy - Swiss Army Knife for Scientific Computations and Advanced Mathematics
* Seaborn - extension for Matplotlib, which can create more advanced graphs
* Sqlalchemy - A library for unified, high-level access to databases
* Xlrd - library for loading .xls / .xlsx files

If any of the steps fail, or you just don't know the advice, ask Slack in the `# counseling` channel, ideally before the course starts.

In the next chapter, we'll look at how to start Jupyter and how to work with it.
