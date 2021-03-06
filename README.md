# test-suites

[![Build Status](https://travis-ci.org/intropro/test-suites.svg?branch=master)](https://travis-ci.org/intropro/test-suites)
[![codecov](https://codecov.io/gh/intropro/test-suites/branch/master/graph/badge.svg)](https://codecov.io/gh/intropro/test-suites)


The tool for executing test cases based on pytest framework

The main goal of the project that there is no need to install any python dependencies to use it. Only one file `test-suites` is needed to be copied to local machine or remote server. The test-suites already contains all required libraries for writing test cases.

Includes:
- pytest
- argparse
- plumbum
- py
- PyYAML

## How to install

Just copy test-suites binary from GitHub Releases to your local machine or remote machine where test cases shall executed

## Test case example

Please follow the instruction from pytest documentation how to write the test cases.http://doc.pytest.org/en/latest/contents.html

The simple example:

```python
def test_example():
    assert True
```

## How to use

```sh
$ test-suites
============================= test session starts ==============================
platform linux2 -- Python 2.7.12, pytest-3.0.3, py-1.4.31, pluggy-0.4.0
rootdir: /repo, inifile:
plugins: cov-2.4.0
collected 2 items

tests/test_example.py .
tests/test_yaml.py .

---------- coverage: platform linux2, python 2.7.12-final-0 ----------
Name                     Stmts   Miss  Cover   Missing
------------------------------------------------------
testsuites/__init__.py       6      0   100%
testsuites/__main__.py       3      3     0%   2-6
testsuites/main.py          10     10     0%   2-15
------------------------------------------------------
TOTAL                       19     13    32%

=========================== 2 passed in 1.08 seconds ===========================
```
The command line interface for test-suites is the same as for pytest, http://doc.pytest.org/en/latest/usage.html

## Versions

- pytest, v3.0.2
- argparse, v1.4.0
- plumbum,v1.6.2
- py,v1.3dev
- PyYAML, v3.12

## License

The package contains several components with own license

- pytest is Copyright Holger Krekel and others, 2004-2016. Distributed under the terms of the MIT license, pytest is free and open source software.
- argparse is (c) 2006-2009 Steven J. Bethard <steven.bethard@gmail.com>. The argparse module was contributed to Python as of Python 2.7 and thus was licensed under the Python license. Same license applies to all files in the argparse package project.
- plumbum, is (c) Tomer Filiba <tomerfiliba@gmail.com>, MIT license.
- py is (c) Holger Krekel and others, 2004-2015, MIT license
- pyyaml is Copyright Kirill Simonov, Distributed under the terms of the MIT license, YAML parser and emitter for Python
