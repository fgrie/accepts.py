[![](https://img.shields.io/pypi/pyversions/accepts.svg?maxAge=86400)](https://pypi.org/pypi/accepts/)
[![](https://img.shields.io/pypi/v/accepts.svg?maxAge=86400)](https://pypi.org/pypi/accepts/)
[![](https://img.shields.io/badge/libraries.io-accepts-green.svg?maxAge=86400)](https://libraries.io/pypi/accepts)

[![CodeFactor](https://www.codefactor.io/repository/github/looking-for-a-job/accepts.py/badge)](https://www.codefactor.io/repository/github/looking-for-a-job/accepts.py)
[![CodeClimate](https://codeclimate.com/github/looking-for-a-job/accepts.py/badges/gpa.svg)](https://codeclimate.com/github/looking-for-a-job/accepts.py)
[![Scrutinizer](https://scrutinizer-ci.com/g/looking-for-a-job/accepts.py/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/looking-for-a-job/accepts.py/)
[![BetterCodeHub](https://bettercodehub.com/edge/badge/looking-for-a-job/accepts.py?branch=master)](https://bettercodehub.com/results/looking-for-a-job/accepts.py)
[![Sonarcloud](https://sonarcloud.io/api/project_badges/measure?project=accepts.py&metric=code_smells)](https://sonarcloud.io/dashboard?id=accepts.py)

[![Codecov](https://codecov.io/gh/looking-for-a-job/accepts.py/branch/master/graph/badge.svg)](https://codecov.io/gh/looking-for-a-job/accepts.py)
[![CircleCI](https://circleci.com/gh/looking-for-a-job/accepts.py/tree/master.svg?style=svg)](https://circleci.com/gh/looking-for-a-job/accepts.py/tree/master)
[![Scrutinizer](https://scrutinizer-ci.com/g/looking-for-a-job/accepts.py/badges/build.png?b=master)](https://scrutinizer-ci.com/g/looking-for-a-job/accepts.py/)
[![Semaphore CI](https://semaphoreci.com/api/v1/looking-for-a-job/accepts-py/branches/master/shields_badge.svg)](https://semaphoreci.com/looking-for-a-job/accepts-py)
[![Travis](https://api.travis-ci.org/looking-for-a-job/accepts.py.svg?branch=master)](https://travis-ci.org/looking-for-a-job/accepts.py/)

### Install

```bash
$ [sudo] pip install accepts
```

### Features

*	support **multiple types** argument
*	support **None** argument
*	human readable detailed exception message

### Usage

```python
>>> from accepts import accepts

>>> @accepts(arg1type,arg2type,...)
```

### Examples

```python
>>> @accepts(int)
def inc(value):
	return value+1

>>> inc(1) # ok
>>> inc(1.5) # exception
TypeError: ....

# multiple types
>>> @accepts((int,float))

# None
>>> @accepts((int,float,type(None)))
```

### Sources

+   [`accepts.accepts(*types)`](https://github.com/looking-for-a-job/accepts.py/blob/master/accepts/__init__.py)