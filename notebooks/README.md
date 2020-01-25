Jupyter notebooks
=================

To develop Python code interactively we will make extensive use of
[Jupyter](https://jupyter.readthedocs.io), a Python-based web app you can
install on your computer and then use to launch this collection of
**Jupyter notebooks**.

Before we begin, open your Conda Powershell or Terminal app, activate the
Conda environment, and move to your local clone of the repository:

### Mac/Linux

```bash
(base) $ conda activate black-hole-3.7
(black-hole-3.7) $ cd ~/src/black-hole-astrophysics/notebooks
```

### Windows

```bash
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
