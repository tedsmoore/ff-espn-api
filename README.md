[![Build Status](https://travis-ci.org/cwendt94/ff-espn-api.svg?branch=master)](https://travis-ci.org/cwendt94/ff-espn-api) [![codecov](https://codecov.io/gh/cwendt94/ff-espn-api/branch/master/graphs/badge.svg)](https://codecov.io/gh/cwendt94/ff-espn-api) [![Join the chat at https://gitter.im/ff-espn-api/community](https://badges.gitter.im/ff-espn-api/community.svg)](https://gitter.im/ff-espn-api/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![PyPI version](https://badge.fury.io/py/ff-espn-api.svg)](https://badge.fury.io/py/ff-espn-api)

# ff-espn-api

This package uses ESPN's Fantasy Football API to extract data from any public or private league. I am currently using this package for my leagues personal website and I plan to keep updating and adding features.

Please feel free to make suggestions, bug reports, and pull request for features or fixes!

This package was inspired and based off of [rbarton65/espnff](https://github.com/rbarton65/espnff).

## Installing
With Git:
```
git clone https://github.com/cwendt94/ff-espn-api
cd ff-espn-api
python3 setup.py install
```
With pip:
```
pip install ff_espn_api
```

## Usage
[For usage and API details head over to the Wiki!](https://github.com/cwendt94/ff-espn-api/wiki)

### Run Tests
```
python3 setup.py nosetests
```

## Issue Reporting
If you find a bug follow the steps below for reporting.

1. Open a [new issue](https://github.com/cwendt94/ff-espn-api/issues) with a brief description of the bug for the title

2. Run the application in debug mode to view ESPN API request's and response's
    ```python
    from ff_espn_api import League
    league = League(league_id=1245, year=2019, debug=True)
    ```
    The application will print all requests and the response from ESPN's API in the console. I would suggest piping the console output to a text file as it will be a lot of data.

3. Find the last log before the crash and copy it in the issue descrption with the line number of the crash or possible bug.

4. Submit the new issue!

I will try to comment on the issue as soon as possible with my thoughts and possible fix!