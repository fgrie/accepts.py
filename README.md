[![](https://img.shields.io/pypi/pyversions/accepts.svg?longCache=True)](https://pypi.org/pypi/accepts/)
[![](https://img.shields.io/pypi/v/accepts.svg?maxAge=3600)](https://pypi.org/pypi/accepts/)
[![Travis](https://api.travis-ci.org/looking-for-a-job/accepts.py.svg?branch=master)](https://travis-ci.org/looking-for-a-job/accepts.py/)

### Install
```bash
$ [sudo] pip install accepts
```

### Features
*	support **multiple types** argument
*	support **None** argument
*	human readable detailed exception message

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