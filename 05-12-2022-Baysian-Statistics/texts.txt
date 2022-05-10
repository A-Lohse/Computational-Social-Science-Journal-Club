# Setting Up Your Environment

We'll be using PYMC3/PYMC4 for this session. I would strongly recommend using Anaconda Virtual Environments for this.
If you are not familiar with Anaconda, feel free to reach out and we can meet up some time and I can help you set it up :)


## Windows

[Installation Guide](https://github.com/pymc-devs/pymc/wiki/Installation-Guide-%28Windows%29)

## Mac OS

For me installing PyMC3 on Mac did not workout (apparently there was some bug - at least there have been a couple of threads in the PYMC forum created on this topic within just the last couple of days without good answers).
So I installed the Beta Version of PyMC4 which works nicely.
```git clone https://github.com/pymc-devs/pymc.git
cd pymc
conda env create -f ./conda-envs/environment-dev-py39.yml
conda activate pymc-dev-py39
pip install .``

You can also find the official installation guide here:
https://github.com/pymc-devs/pymc/wiki/Installation-Guide-(MacOS)


Information on the differnce between v3 and v4:
https://www.pymc-labs.io/blog-posts/the-quickest-migration-guide-ever-from-pymc3-to-pymc-v40/

## Other Packages

Apart from PYMC3 we will need a couple of other packages - please make sure to have them installed in your newly created conda environment:

```
import numpy as np
import pandas as pd
import scipy.stats as stats

# Exploratory Analysis fo Bayesian Models
import arviz as az

# Probabilistic Programming Language
import pymc as pm
import aesara

# Plottiing
import matplotlib.pyplot as plt
```

# Literature
(in order of importance to follow the session)

- [Evidence of bias in the Eurovision song contest: modelling the votes using Bayesian hierarchical models](https://www.tandfonline.com/doi/pdf/10.1080/02664763.2014.909792?needAccess=true)
- [Differential impact of government lockdown policies on reducing air pollution levels and related mortality in Europe](https://www.nature.com/articles/s41598-021-04277-6)
- [Spatial survival modelling of business re-opening after Katrina: Survival modelling compared to spatial probit modelling of re-opening within 3, 6 or 12 months](https://journals.sagepub.com/doi/pdf/10.1177/1471082X20967158)



# Datasets

For the survival analysis example (if we get that far) we are using this datset here:
https://r-data.pmagunia.com/dataset/r-dataset-package-hsaur-mastectomy


# Resources
Not necessary for our session - just resources I found helpful and maybe you might find them helpful too?

### PYMC
*Attention: Some of these use PyMC whereas others use PyMC3 -> there are quite some differences between the versions*
- [Estimating Probabilities with Bayesian Modelling in Python](https://towardsdatascience.com/estimating-probabilities-with-bayesian-modeling-in-python-7144be007815) - Good introducory article
- [A Modern Introduction to Probabilistic Programming with PyMC](https://austinrochford.com/posts/intro-prob-prog-pymc.html#A-Bayesian-analysis-of-Lego-set-prices)
- [Logistic Regression with PyMC](https://docs.pymc.io/en/v3/pymc-examples/examples/generalized_linear_models/GLM-logistic.html)
- [Bayesian Modelling in Python](https://bayesiancomputationbook.com/welcome.html?utm_campaign=Data_Elixir&utm_source=Data_Elixir_370)
-  [Bayesian Methods for Hackers](https://github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers)
- [Introduction to Computational Statistics with PyMC3](https://sjster.github.io/introduction_to_computational_statistics/docs/Production/PyMC3.html)

### Bayesian Statistics
- [Statistical Rethinking](https://github.com/rmcelreath/stat_rethinking_2022?utm_campaign=Data_Elixir&utm_source=Data_Elixir_370#statistical-rethinking-2022-edition) - including very nice youtube lectures
- [Bayesian Optimization Book](https://bayesoptbook.com//?utm_source=hackernewsletter&utm_medium=email&utm_term=books)

### Bayesian Modelling in R
- [Statistical Rethinking - How to in R](https://bookdown.org/content/4857/small-worlds-and-large-worlds.html#building-a-model)
- [Spatial and Spatio-temporal BayesianModels with R-INLA]([[Spatial and Spatio%E2%80%90temporal Bayesian Models with R%E2%80%90INLA - 2015 - Blangiardo.pdf]]) (Includes a nice (programming language agnostic) Introduction to Bayesian Methods & an introduction to R)
