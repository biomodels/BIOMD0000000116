# BIOMD0000000116: Model_0

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000116.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000116.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000116 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


This model encoded according to the paper _Cross-talk and decision making in
MAP kinase pathways._ Supplementary Figure 2 has been reproduced by
COPASI4.0.20 (development) using parameter scan method. You probably need to
uncheck "always use initial conditions" in copasi when you simulate for the
second run in order to get the figure. S1 scale from 0 to 12. Keep in mind
that the y axis is the fractions of excited X3 and Y3, meaning that X3P and
Y3P are normalized by total concentration X3T and Y3T.

The results from modeling the pathway in Supplementary Figure1a, including
both activation and inhibition. According to the paper, the value of ka and kd
should in the orange region (ka belongs [0,1], kd belongs [1,10]) so assigned
ka=0, kd=1.

The author made the simplifying assumption that the interactions between the
pathways are symmetric. Thus the k12xy=k12yx=ka, k33xy=k33yx=kd.

  

To the extent possible under law, all copyright and related or neighbouring
rights to this encoded model have been dedicated to the public domain
worldwide. Please refer to [CC0 Public Domain
Dedication](http://creativecommons.org/publicdomain/zero/1.0/) for more
information.

In summary, you are entitled to use this encoded model in absolutely any
manner you deem suitable, verbatim, or with modification, alone or embedded it
in a larger context, redistribute it, commercially or not, in a restricted way
or not.

  

To cite BioModels Database, please use: [Li C, Donizelli M, Rodriguez N,
Dharuri H, Endler L, Chelliah V, Li L, He E, Henry A, Stefan MI, Snoep JL,
Hucka M, Le Novère N, Laibe C (2010) BioModels Database: An enhanced, curated
and annotated resource for published quantitative kinetic models. BMC Syst
Biol., 4:92.](http://www.ncbi.nlm.nih.gov/pubmed/20587024)


