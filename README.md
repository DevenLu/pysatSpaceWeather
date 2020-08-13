# pysatSpaceWeather: pysat support for Space Weather Indices
[![Build Status](https://travis-ci.org/pysat/pysatSpaceWeather.svg?branch=main)](https://travis-ci.org/pysat/pysatSpaceWeather)
[![Coverage Status](https://coveralls.io/repos/github/pysat/pysatSpaceWeather/badge.svg?branch=main)](https://coveralls.io/github/pysat/pysatSpaceWeather?branch=main)

# Installation

Currently, the main way to get pysatSpaceWeather is through github.

```
git clone https://github.com/pysat/pysatSpaceWeather.git
```

Change directories into the repository folder and run the setup.py file.  For
a local install use the "--user" flag after "install".

```
cd pysatSpaceWeather/
python setup.py install
```

Note: pre-1.0.0 version
------------------
pysatSpaceWeather is currently in an initial development phase.  Much of the API is being built off of the upcoming pysat 3.0.0 software in order to streamline the usage and test coverage.  This version of pysat is planned for release later this year.  Currently, you can access the develop version of this through github:
```
git clone https://github.com/pysat/pysat.git
cd pysat
git checkout develop-3
python setup.py install
```
It should be noted that this is a working branch and is subject to change.

# Using with pysat

The instrument modules are portable and designed to be run like any pysat instrument.

```
import pysat
from pysatSpaceWeather.instruments import sw_dst

ivm = pysat.Instrument(inst_module=sw_dst)
```
