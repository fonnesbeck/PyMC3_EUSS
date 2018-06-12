# Tutorial: Probabilistic Programming with Python

**EU Summer School, June 26, 2018**

[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/fonnesbeck/PyMC3_EUSS)


This intermediate-level course will provide students with hands-on experience applying practical Bayesian statistical modeling methods on real data. PyMC3 is a high-level Python library for building statistical models using probabilistic programming, and fitting them using modern Bayesian computational methods. I will provide an introduction to Bayesian inference and prediction, followed by a tutorial on probabilistic programming with PyMC3, including the use of Markov chain Monte Carlo (MCMC) and Variational Inference (VI), using real-world datasets. The last part of the course will focus on modeling strategies and how to avoid various pitfalls when applying Bayesian statistics to your own work. The course will assume familiarity with Python and with basic statistics (e.g. probability), but does not require previous experience with Bayesian methods or probabilistic programming.

## Syllabus

### Introduction to PyMC3

* Variable types
* Probability models
* Simple case studies

### Markov Chain Monte Carlo

* Metropolis sampling
* Gradient-based sampling methods

### Approximation Methods

* MAP
* Variational inference
* ADVI

### Model Building with PyMC3

* Specifying priors and likelihoods
* Deterministic variables
* Factor potentials
* Custom variables
* Step methods
* Generalized linear models
* Missing Data

### Model Checking and Output Processing

* Storage backends
* Convergence diagnostics
* Goodness of fit
* Plotting and summarization


## Software Installation

Running PyMC3 requires a working Python3 interpreter, preferably Python 3.6. A complete Python installation for Mac OSX, Linux and Windows can most easily be obtained by downloading and installing the free [`Anaconda Python Distribution`](https://www.continuum.io/downloads) by ContinuumIO. 

`PyMC3` can be installed using `conda`, a package management tool that is bundled with Anaconda. PyMC3 also depends on several third-party Python packages which will be automatically installed when installing via `conda`. The four required dependencies are: `Theano`, `NumPy`, `SciPy`, `Matplotlib`, and `joblib`. To take full advantage of PyMC3, the optional dependencies `seaborn`, `pandas` and `Patsy` should also be installed. You can install PyMC3 and its dependencies by cloning this repository:

```
git clone https://github.com/fonnesbeck/PyMC3_EUSS.git
```

Then move into the directory created by the clone, and install the required packages using `conda`:

```bash
cd PyMC3_EUSS
conda env create -f environment.yml
```

This will create a *virtual environment* called `pymc_tutorial` that includes the dependencies for PyMC3 that is completely separate from any other Python installations you may have on your machine. To activate this environment to run the course materials, you can run the following command from the terminal:

```bash
source activate pymc_tutorial
```

**If you would rather not install the software yourself, you can use the MyBinder.org link at the top of the page to run the course materials on a remote server**
