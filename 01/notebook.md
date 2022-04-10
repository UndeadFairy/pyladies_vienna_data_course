# Jupyter Notebook intro

Jupyter Notebook is a web editor used to create complex documents,
which may include structured text and images as well
code ([not only in Python] (https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)),
graphs, mathematical formulas (LaTeX) and other interactive elements.

From another point of view, this is a very practical console for Python, where everything is
history is saved and can be returned or changed, affecting the rest
calculations.

Jupyter Notebook is suitable wherever you need to see the results immediately
your work or proceed step by step, pass someone a comprehensive program together
with visualizations and results, prepare a presentation or data analysis, etc.

## Launch

After successful installation, Jupyter Notebook can be run in an active virtual environment
with a simple command:

`` `shell
(venv) $ jupyter notebook
`` `

If this command doesn't work for you, try the following:

`` `shell
(venv) $ python -m notebook
`` `

When you start the Notebook, the web browser in which you start will also start automatically
the editor will display.

> The notebook always works in the folder in which it was started, so it is reasonable
go to the folder in which you want the resulting documents before running it
saved.

! [Notebook UI] (static / jupyter_notebook_home.png)

On the first screen you see the contents of the folder in which the Notebook is running. once
you will have some documents created, they will appear here and you will be able to return to them
and continue working.

To create a new document, click on `New`>` Python 3` at the top right.
This option selects Python 3 as the language you will use within the document.
The laptop can handle many more, so everyone will get their money's worth.

## The user interface

! [Notebook UI] (static / jupyter_notebook_new.png)

The laptop does not have a complicated interface. On the first line you will find information about the name
document and the last save, then the controls and the main menu.
A little lower then an empty cell waiting for the first content.

To the right of "Python 3" is a small but useful wheel. If at work
black, it means that Python is busy executing our commands and is
you have to wait for them to finish, or if you're wrong, for example
created an infinite loop that requires Python (or kernel) to be restarted.

## Basic use

As a first step, rename the new document. Click on the inscription on the first line
"Untitled" and choose a meaningful name.

Now try to type a command in Python in the first cell and press the keyboard key
shortcut `Shift` +` Enter`.

> An arbitrarily large piece of code can be written in one cell, even with empty lines, therefore
a keyboard shortcut must be used instead of just Enter to run it.
However, it makes more sense to divide the code into smaller parts so that it can be better controlled.

! [first command] (static / first_command.png)

You can continue in the same way. You always enter a code in a cell and then it
you run. If the cell contains any output or returns something, the result is displayed
after starting the cell just below it. However, this only applies to the output if it is on the last one
cell line, while `print` can be anywhere in the cell.

! [sample outputs] (static / outputs.png)

It works like a classic program, so it depends on the order in which the individual
cells performed. For example, you must first store some content in a variable before it can
you will be able to use. This rule is important to keep in mind because cells
v The notebook can be started independently of each other in any order. In what
The order in which they started can be determined from the numbers that occur after starting
appears in square brackets to the left of the cell. If `*` appears instead of a number after startup, it means that
Python is working and we will have to wait a while for the result.

This is what it might look like if the correct order is not followed:

! [wrong cell startup order] (static / wrong_order.png)

> Although it is not a necessity, it is customary to write documents in a notebook in order to
the cells let them run in the order in which they follow each other. Then if you send it to someone,
You will be able to easily run your code bit by bit and keep track of what's in it
going on. In addition, the main menu also has the option `Kernel`>` Restart & Run All`, which
restarts Python and then starts all cells in the document.

Notice how the cells change color. If the edge of the cell is green, it is possible
edit and use the arrows to move through the code it contains. If it's blue, it will
with arrows to move between cells. From blue to green mode
we get to the `Enter` key, or by clicking in the cell. On the contrary, from the green
to blue mode using the `Esc` key.

To control your laptop it is good to learn the keyboard shortcuts that work with it
make it easier and faster. Their list can be displayed using the `h` key.

> Keyboard shortcuts are used in blue mode, otherwise we would instead
special events wrote individual characters into cells.

Among the most important are:

* `h` displays help
* `a` inserts a new cell above the current one
* `b` inserts a cell below the current one
* `x` extracts the cell
* `c` copies the cell
* `v` inserts a kick or cut cell below the current one
* `Shift` +` v` pastes the copied or cut cell above the current one
* `Ctrl` +` s` saves the document
* `m` switches a cell from python code to text

** The most important keyboard shortcut ** is the first - `h` - with its help
you will get to the list of everyone else very quickly.

## Content types

The basic cell type is a code cell that can do everything from Python
you already know.

! [Python examples] (static / python_example.png)

### Text

By pressing the `m` key (in blue mode) we can switch the cell from python mode
code to text mode, which allows us to enrich documents with a lot of different content.
We know that the cell is in text mode by the fact that it will no longer be blue to the left of it
`In []`. While for cells with Python we get the result after running the program
prints below the cell, the text cell is only rendered as text when started.

### Markdown

An ordinary text would not be so interesting in itself and will not contribute to clarity
more than just a comment. Therefore, we have the ability to format it and to some extent
so adjust its appearance, but mainly its structure. Used for formatting
Markdown language (https://en.wikipedia.org/wiki/Markdown). Markdown
allows you to format text using plain characters.

For example:

* Text beginning with `#` will automatically become the first heading when the cell is started
levels. `##` then they do the second level, etc.
* If we introduce the text with asterisks - `* for example *` - it will be written * in italics *.
A pair of asterisks on each side will then make the text ** bold **.
* When several lines start with an asterisk, they become a bulleted list.
When we use numbers at the beginning, the list will be numbered.
* Links look like this: `[link text] (path or URL)` - to square
the text of the link is written in parentheses at the beginning and the path to the destination in parentheses
or URL.
* Images look almost the same as links, only they have at the beginning before the first
exclamation mark: `! [python logo] (static / python_logo.png)`

Simply formatted text in this way could look like this:

! [markdown source] (static / markdown_source.png)

The result of such formatting can then look like, for example, cell startup
thus:

! [markdown] (static / markdown.png)

### Mathematical formulas

If you know the notation of mathematical formulas that is used in LaTeX, you can
use it in text on laptop as well. Just start and end the latex formula
using `$` (or `$$`).

Examples of several entries:

! [latex examples] (static / latex_examples.png)

If you need formulas and this notation is new to you, there is no need to learn
everything about LaTeX, you just need simple rules for writing math
formulas. For example, [this help] (https://cs.wikipedia.org/wiki/N%C3%A1pov%C4%9Bda:Matematick%C3%A9_vzorce) from Czech wikipedia will help you.

## Other useful features

The notebook has a number of conveniences that make it easier for us to work with it.

### Help

When you type a question mark after the name of a function (instead of parentheses) or a module
(eg: `print?`), a help will appear after running such a cell. That's extra
displayed outside the main document, so it does not interfere with further work and may remain
open longer.

Shorter help (so-called documentation string) can be displayed while writing code using
keyboard shortcuts `Shift` +` Tab`. This displays the documentation string of the function
in a small bubble near the active cell.

### Special commands

Commands beginning with a percent sign have a special meaning in a laptop. For example
`% time` can measure and display how long it took to execute the code written on the line immediately following this command.

Special commands starting with two percent (eg: `%% time`) then have an effect on the whole
cell instead of one row.

A list of all special commands can be obtained with `% lsmagic`.

### Command line commands

It is also very easy to run commands from the command line in laptop cells.
Instead of running Python, just start with a command line
(eg: `! whoami`)

## Continued

The notebook can do a lot of that and it will also write materials for it
the following chapters, which will allow us to put the theory into practice
examples also with graphs and pictures and those interested to try out with experiments.

> All lesson source codes and prepared data are available in
[GIT repositories] (https://github.com/PyDataCZ/naucse.python.cz/tree/master/lessons/pydata).
From here it is possible to download notebooks of individual lessons and experiment as you wish.

However, the development of classic applications and in general for projects with a more complex structure is still
better divide the code into modules and edit it in a suitable text editor.
It is common practice to first quickly assemble a functional in an interactive laptop environment
prototype and then transform it into a classic application.
