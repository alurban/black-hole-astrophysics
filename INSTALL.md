Installation
============

Introduction
------------

**Note:** All software used for this course is open source, meaning it is
distributed free of charge and well-supported for wide use.

To study black hole dynamics, we will frequently find it useful to do
numerical simulations, which inevitably require learning to write software.
Our primary language will be Python (specifically, `python-3.7`) both because
it is relatively intuitive and because there are many, many packages and
libraries available through it. To install these packages, we will use
[Conda](https://docs.conda.io/en/latest/), a package management and
distribution service compatible with Windows, MacOS, and Linux.

Installing Miniconda
--------------------

To begin, you will need to download the (free) minimal installer for conda
called [Miniconda](https://docs.conda.io/en/latest/miniconda.html). From this
link, choose the installer that works for your operating system. In most
cases I recommend using the 64-bit installer since it offers more computing
power, but this is really up to you.

Creating the `black-hole-3.7` conda environment
-----------------------------------------------

Next, you can create what is known as a *virtual environment* to install all
the packages you will need, without interfering with anything else already
installed on your computer. Virtual environments are nice because they provide
a sandbox in which you can do absolutely anything -- if it becomes corrupted,
just nuke it from orbit and start over with ease!

Conda provides its own suite of tools to manage a special flavor of virtual
environments, called *conda environments*. In this repository, the `conda`
folder contains tools that go one step further, and automatically build an
environment for you from a pre-baked recipe:

```bash
$ cd conda/
$ ./bh-conda-env create
```

**Note:** You may need to run this with `sudo` on your computer due to user
permissions.

This command builds a recipe called `black-hole-3.7`, which you can activate
via

```bash
$ conda activate black-hole-3.7
```

"Activating" simply means you are now inside the sandbox, and have access to
all the packages and features set up there. To go back to your computer's
default (or *native*) environment, simply deactivate it:

```bash
$ conda deactivate
```

Maintaining `black-hole-3.7`
----------------------------

To check the environment after creating it:

```bash
$ ./bh-conda-env check
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

Finally, to update software package versions, change (or pull) the pinned
version in `environment.yaml` and use the `update` command:

```bash
$ ./bh-conda-env update
```

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
