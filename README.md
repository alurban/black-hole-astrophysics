PHYS 290: Black Hole Astrophysics
=================================

Welcome, black hole mechanics!

This repository hosts software and related materials for PHYS 290: Black Hole
Astrophysics, a Special Topics course offered in spring 2020 at Allegheny
College.

Contents
--------

This repository contains the following materials:

* [Course website](https://alurban.github.io/black-hole-astrophysics/)
* [Installation guide](INSTALL.md) for the `black-hole-3.7` conda environment
* A library of [Jupyter notebooks](notebooks/) with worked examples

Installing Git
--------------

[Git](https://git-scm.com) is a widely-used version control system that allows
large groups of people to easily share and distribute software. In this course
I will use Git to post (and occasionally fix) interactive software tutorials
for students, which simulate orbits around black holes and dig into various
data analysis and signal processing techniques.

In general, Git often comes pre-installed on Mac and Linux systems, but not
on Windows. For Windows users, Git can be installed (for free) by following
[this link](https://git-scm.com/downloads) and selecting the best graphical
installer for your operating system.

**Note for Mac users:** if Git is installed on your system but doesn't work
straight away, you may need to re-install `xcode` tools:

```
xcode-select --install
```

This is annoying, but harmless, as the tools are open-source (i.e., free) and
should take only a few minutes to install.

Access
------

To clone this repository, open an app called Terminal (on Mac or Linux) or
Git Shell (on Windows) and do the following:

```
mkdir -p ~/src
cd ~/src/
git clone https://github.com/alurban/black-hole-astrophysics.git
```

Alternatively, you can download a ZIP-compressed version using the "clone or
download" button at the top of this page. This will work from any system, but
you won't be able to inherit any changes or updates.

Pulling updates
---------------

**Disclaimer:** you will be able to track upstream changes and work from
this clone, but you **will not** be able to push changes back to `master`
unless I grant you permissions. Please [email me](mailto:aurban1@lsu.edu) if
you would like to discuss setting up push privileges.

Git allows users to access the full history of edits to files in this
repository. The primary branch of that history, by convention, is referred to
as `master`. This is analogous to music production, where audio engineers
keep a running copy of progress on a song called the *master copy*.

Whenever I post updates, fixes, or new software notebooks, you can pull them
down to your laptop by opening Terminal (on Mac or Linux) or Git Shell (on
Windows) and doing the following:

```
cd ~/src/black-hole-astrophysics
git pull
```

**Note:** this assumes you've checked out the `master` branch, which is almost
certainly the case. If you want to be more careful you can instead use a
slightly longer command:

```
git pull --rebase origin master
```

You may occasionally need to stash any local changes before pulling, in which
case you can do:

```
git stash
```

I recommend copying any changed files to a separate location beforehand, so
that you don't lose them in the stash.

This barely scratches the surface of what you can do with Git. For more
information, consider visiting the extensive [online documentation]().

Other resources
---------------

### At Allegheny College

* [Pelletier Library](https://sites.allegheny.edu/lits/library/)
* [Dean of Students office](https://sites.allegheny.edu/deanofstudents/)
* [The Writing Center](https://sites.allegheny.edu/learningcommons/writing/)
* [Learning Commons](https://sites.allegheny.edu/learningcommons/)
* [Student resources](https://sites.allegheny.edu/resources/student-services/)
* [Counseling Center](https://sites.allegheny.edu/counseling/) (a 24-hour
  crisis line may be reached at +1 814-332-2105)

### Data science and signal processing

* A neat [Python tutorial](https://www.learnpython.org) with focus on data
  science
* [Stackoverflow](http://stackoverflow.com), a vast font of wisdom for coding
  and debugging
* A collection of [tutorials](https://losc.ligo.org/tutorials/) centered on
  gravitational wave signal processing

### My work experience

* [LIGO Livingston Observatory](http://ligo.caltech.edu/LA)
* Online version of my [curriculum vitae](http://alurban.github.io/)

### Misc.

**Pro tip:** if your eyes hurt after staring at a computer screen all day,
consider using software that adjusts your monitor's color filter to reflect
indoor vs. outdoor lighting conditions, such as
[f.lux](https://justgetflux.com).

Finally, if you're feeling overwhelmed, take a break from science with
[this random cute animal generator](https://attackofthecute.com/random.php)!

Legalese
--------

Software and materials in this repository are provided under the terms of the
[MIT License](LICENSE). Strictly speaking, you are free to modify, distribute,
and use this software for any purpose (with appropriate citation) with the
understanding that it comes "as-is" and has no warranty.
