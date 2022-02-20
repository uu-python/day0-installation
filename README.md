# Installation instructions for the course

Use these instructions to install Git, Shell, Python and associated libraries
(numpy and friends) on Windows, macOS and Linux.


## Windows

#### Shell and Git
Install [git for windows](https://git-scm.com/download/win). This provides both git and a bash shell for basic commands.

#### Python
We recommend using [Anaconda](https://www.anaconda.com/products/individual) to install Python, for simplicity.
You can also use [Miniconda](https://docs.conda.io/en/latest/miniconda.html#windows-installers) if you feel confortable.

To make `conda` available from within the `Git Bash` open `Git Bash` and then run the following:

	$ echo ". ${HOME}/anaconda3/etc/profile.d/conda.sh" >> ${HOME}/.bash_profile

Now restart `Git Bash`. You should now be able to simply run `conda activate` to make Python available from within `Git Bash`.


## macOS

#### Shell
macOS system come with a shell, so there's no need to install one.
You access the shell from the `Terminal` (found in `/Applications/Utilities`). This [video](https://www.youtube.com/watch?v=9LQhwETCdwY) shows this.

#### Git
If git is not already installed you can install it together with the XCode Command Line Tools like:

	$ sudo xcode-select --install

or using [homebrew](https://brew.sh/):

	$ brew install git

#### Python
We recommend using [Anaconda](https://www.anaconda.com/products/individual) to install Python, for simplicity.
You can also use [Miniconda](https://docs.conda.io/en/latest/miniconda.html#macos-installers) if you feel confortable.

## Linux

#### Shell
Linux system come with a shell, so there's no need to install one.

#### Git
To install Git use the package manager of your distribution.

For Debian/Ubuntu run:

	$ sudo apt-get install git

For Fedora:

	$ sudo dnf install git

#### Python
We recommend using [Anaconda](https://www.anaconda.com/products/individual) to install Python, for simplicity.
You can also use [Miniconda](https://docs.conda.io/en/latest/miniconda.html#linux-installers) if you feel confortable.


### Anaconda vs Miniconda

Anaconda installs not only Python but also a large number of packages including everything we need for this course (and much more).
Miniconda installs a minimal `conda` environment. You will then have to manually install the following packages:
- numpy
- scipy
- matplotlib
- jupyter

You can do this with:

	conda install numpy scipy matplotlib jupyter


