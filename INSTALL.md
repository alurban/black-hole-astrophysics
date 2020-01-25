Installation
============

Introduction
------------

**Note:** All software used for this course is open source, meaning it is
distributed free of charge and is well-supported for wide use.

To study black hole dynamics, we will frequently find it useful to do
numerical simulations, which inevitably require learning to write software.
Our primary language will be Python (specifically, `python-3.7`) both because
it is relatively intuitive and because there are many, many packages and
libraries available through it. To install these packages, we will use
[Conda](https://docs.conda.io/en/latest/), a package management and
distribution service compatible with Windows, MacOS, and Linux.

Installing Miniconda
--------------------

To begin, you will need to download the (free) minimal installer for Conda
called [Miniconda](https://docs.conda.io/en/latest/miniconda.html). From this
link, choose the installer that works for your operating system. In most
cases I recommend using the 64-bit installer since it offers more computing
power, but this is really up to you.

Creating the `black-hole-3.7` Conda environment
-----------------------------------------------

Next, you can create what is known as a *virtual environment* to install all
the packages you will need, without interfering with anything else already
installed on your computer. Virtual environments are nice because they provide
a sandbox in which you can do absolutely anything &mdash; if it becomes
corrupted, just nuke it from orbit and start over with ease!

Conda provides its own suite of tools to manage a special flavor of virtual
environments, called *Conda environments*. Here you'll find instructions for
setting this up on your own computer.

### Mac/Linux

In this repository, the `conda` folder contains tools that automatically build
an environment for you from a pre-baked recipe that I maintain. Simply launch
your Terminal app, go to your local clone of the git repository, and do:

```bash
cd conda/
./bh-conda-env create
```

This may take several minutes to finish, but you'll be given a status bar       
along the way.

**Note:** You may need to run this with `sudo` on your computer due to user
permissions.

### Windows

The script provided here won't work on Windows systems, but fear not, because
you can still do the same basic function. From the Start menu, open your
Conda Powershell app and do the following:

```powershell
conda create -n black-hole-3.7 python=3.7
```

This will create a Conda environment called `black-hole-3.7` that has version
3.7 of Python baked-in. Next, install a few packages into this environment:

```powershell
conda install -n black-hole-3.7 -c conda-forge ipython=7.11.1 jupyter=1.0.0 gwpy=1.0.1
```

This may take several minutes to finish, but you'll be given a status bar
along the way.

### Activating and deactivating

The commands above build an environment called `black-hole-3.7`, which you can
activate from your Powershell or Terminal app via

```bash
conda activate black-hole-3.7
```

"Activating" simply means you are now inside the sandbox, and have access to
all the packages and features set up there. To go back to your computer's
default (or *native*) environment, simply deactivate it:

```bash
conda deactivate
```

Maintaining `black-hole-3.7`
----------------------------

To check the environment after creating it, from a Mac or Linux machine:

```bash
./bh-conda-env check
```

On a Windows machine, you can instead run

```powershell
conda info --all
```

This will list out the packages and environment variables contained within
`black-hole-3.7`, which should include the following variables:

```bash
GWPY_RCPARAMS
GWPY_USETEX
MATPLOTLIBRC
XDG_DATA_HOME
```

Please [email me](mailto:aurban1@lsu.edu) to discuss what these variables do
and how to change them.

### Extra functionality (Mac/Linux)

When in doubt, the help documentation is also informative:

```bash
$ ./bh-conda-env --help
usage: bh-conda-env [-h] {create|check|update}

Create or update the conda environment for
Black Hole Astrophysics

positional arguments:
  action		conda action to perform, must be one
			of 'create', 'check', or 'update'

optional arguments:
  -h, --help		show this help message and exit
```
