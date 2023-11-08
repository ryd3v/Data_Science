# Installation Guide for Data Science Environment

This guide will walk you through the installation process for the data science tools you will need throughout the
course.

## Table of Contents

- [Python Installation](#python-installation)
- [Anaconda Installation](#anaconda-installation)
- [Setting Up a Conda Environment](#setting-up-a-conda-environment)
- [Installing Jupyter Notebooks](#installing-jupyter-notebooks)
- [Common Data Science Libraries](#common-data-science-libraries)
- [Verifying the Installation](#verifying-the-installation)

## Python Installation

While Anaconda will install Python for you, it is useful to know how to install Python by itself.

1. Visit the official Python website at [python.org](https://www.python.org/downloads/).
2. Download the latest version of Python for your operating system (Windows, macOS, Linux).
3. Run the installer. Make sure to check the box that says "Add Python to PATH" during installation.

## Anaconda Installation

Anaconda is a distribution of Python that includes many of the libraries and tools you will need.

1. Go to the Anaconda download page at [anaconda.com](https://www.anaconda.com/products/distribution#download-section).
2. Select your operating system and download the Anaconda Installer for Python 3.x.
3. Run the Anaconda Installer and follow the on-screen instructions.
    - For Windows, it's recommended to check the "Add Anaconda to my PATH environment variable" option.
    - For macOS and Linux, you may need to run the installer through the terminal.

## Setting Up a Conda Environment

It's a good practice to create a separate environment for each project or course.

1. Open the Anaconda Prompt or your terminal.
2. Create a new environment with the following command:

```
conda create --name datascience python=3.8
   ```

You can replace `datascience` with any name you like and `python=3.8` with the specific version you need.

3. Activate the environment by typing:
    - On Windows: `activate datascience`
    - On macOS and Linux: `source activate datascience`

## Installing Jupyter Notebooks

With your environment activated, install Jupyter Notebook by running:

```
conda install jupyter
```

## Common Data Science Libraries

Here's how to install some common libraries that you'll use in data science:

```
conda install numpy pandas scipy scikit-learn matplotlib seaborn
```

Additional libraries can be installed similarly using

`conda install [library-name]`.

## Verifying the Installation

To verify that everything is installed correctly:

1. Launch Jupyter Notebook by typing `jupyter notebook` in your terminal or Anaconda Prompt.
2. Create a new notebook by clicking on "New" > "Python 3".
3. In the first cell of the notebook, try importing the libraries:
   ```python
   import numpy as np
   import pandas as pd
   import matplotlib.pyplot as plt
   import seaborn as sns
   import sklearn
   ```

Then execute the cell by pressing `Shift + Enter`. If no errors appear, congratulations, you've installed everything
successfully!

If you encounter any problems during installation, please consult the official documentation of the respective tool or
library, or file an issue in the course repository.
