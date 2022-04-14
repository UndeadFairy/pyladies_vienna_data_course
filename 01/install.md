# Installation

Installing everything you need is not complicated and should only take a moment. If you exceprience any trouble during installation, ask mentors directly or via Slack any time later. 

First step is to have Python installed. Check if your version is higher than Python 3.6. If not, or you do not have python installed, please follow instructions [in beginners course](https://pyladiesvienna.pythonanywhere.com/2022/pyladies-en-vienna-2022-data-science/beginners-en/install_vienna/)


## Directory, creation and activation of a virtual environment

First, prepare a directory for this whole course and storing files you will need
(for example `pydata` or anything else) and create a virtual environment inside.

If you don't know how to do this step, the complete instructions can be found [here](virtual_environment.md).

### What is a virtual environment? 

A virtual environment is an isolated Python environment where a project's dependencies are installed in a different directory from those installed in the system's default Python path (and other virtual environments). This way packages you install in PyData course environment will not affect other parts of your work.

Each time you want to use command line for PyData course, you will need to activate the virtual environment so that you can easily work with with the libraries and tools installed in it.


## Installing libraries

At the command prompt with the virtual environment active, enter the following command:

```shell
(venv) $ python -m pip install jupyter jupyterlab pandas matplotlib requests seaborn scipy scikit-learn sqlalchemy plotly xlrd openpyxl
```

This command installs the following libraries (and some other dependencies) in the virtual environment:

* Jupyter - web interface for interactive and reproducible work with Python
* jupyterlab - much nicer and more modern web interface for interactive and reproducible work with Python - that one we will mainly use.
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

If any of the steps fail, or you just don't know the solution, ask mentors or anytime later via Slack in your course channel. 

In the next chapter, we'll look at how to start Jupyter lab and how to work in it.
