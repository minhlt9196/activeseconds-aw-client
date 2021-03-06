aw-client
=========

[![GitHub Actions badge](https://github.com/ActivityWatch/aw-client/workflows/Build/badge.svg)](https://github.com/ActivityWatch/aw-client/actions)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Typechecking: Mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)


[**Documentation**](https://activitywatch.readthedocs.io/en/latest/)

Client library for ActivityWatch in Python.

Please see the documentation for usage and examples.


## How to install

To install the latest git version directly from github without cloning, run
`pip install git+https://github.com/minhlt9196/aw-client.git`

To install from a cloned version, cd into the directory and run
`poetry install` to install inside an virtualenv. If you want to install it
system-wide it can be installed with `pip install .`, but that has the issue
that it might not get the exact version of the dependencies due to not reading
the poetry.lock file.


## Examples

The `examples/` directory contains a couple of example scripts, including:

 - `time_spent_today.py` - fetches all non-afk events and sums their duration to get the total active time for the day.
 - `merge_buckets.py` - merges two buckets with non-intersecting events by moving all events from one into the other.
 - `redact_sensitive.py` - redact sensitive events.
