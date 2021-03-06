Jupyter notebooks
=================

To develop Python code interactively we will make extensive use of
[Jupyter](https://jupyter.readthedocs.io), a Python-based web application that
launches a collection of **Jupyter notebooks**. Note, the Jupyter software
package is already installed as part of the `black-hole-3.7` Conda environment.

Before using Jupyter, open your Conda Powershell or Terminal app, activate the
Conda environment, and move to your local clone of this repository:

### Mac/Linux

```bash
(base) $ conda activate black-hole-3.7
(black-hole-3.7) $ cd ~/src/black-hole-astrophysics/notebooks
```

### Windows

```powershell
(base) C:\Users\myname>conda activate black-hole-3.7
(black-hole-3.7) C:\Users\myname>cd ~\src\black-hole-astrophysics\notebooks
```

## Using Jupyter

To launch a Jupyter server on your computer, on either Mac/Linux or Windows,
execute the following:

```bash
jupyter notebook
```

This will open the `notebooks/` folder in Jupyter. To open a specific
notebook, e.g. `classical-orbits.ipynb`, you can do

```bash
jupyter notebook classical-orbits.ipynb
```

The notebook itself will have a standard file menu allowing you to save, quit,
and do various other actions. If you ever need to kill the server from your
Powershell or Terminal window, you can do that by hitting `CTRL`+`C`.

The blocks of code within a Jupyter notebook are called *cells*. To run these,
either use the menu at the top of the page (the button that says `Run` or the
dropdown menu `Cell`) or on your keyboard hit `SHIFT`+`RETURN` or
`SHIFT`+`ENTER`. These cells are meant to be run in sequential order, so if
you go back and make a change to a previous cell, in general you should re-run
the later cells as well.
