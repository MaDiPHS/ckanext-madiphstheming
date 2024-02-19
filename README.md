[![Tests](https://github.com/treinar/ckanext-madiphstheming/workflows/Tests/badge.svg?branch=main)](https://github.com/treinar/ckanext-madiphstheming/actions)

<img src="README_images/MaDiPHS_logo.png" style="height: 200px; padding-bottom: 50px;"/>

# ckanext-madiphstheming

This extension contains the UI modifications for [https://ckan.madiphs.org](https://ckan.madiphs.org)


## Requirements

Compatibility with core CKAN versions:

| CKAN version    | Compatible?   |
| --------------- | ------------- |
| 2.9 and earlier | not tested    |
| 2.10            | yes    |


## Installation

**TODO:** Add any additional install steps to the list below.
   For example installing any non-Python dependencies or adding any required
   config settings.

To install ckanext-madiphstheming:

1. Activate your CKAN virtual environment, for example:

     . /usr/lib/ckan/default/bin/activate

2. Clone the source and install it on the virtualenv

    git clone https://github.com/treinar/ckanext-madiphstheming.git
    cd ckanext-madiphstheming
    pip install -e .
	pip install -r requirements.txt

3. Add `madiphstheming` to the `ckan.plugins` setting in your CKAN
   config file (by default the config file is located at
   `/etc/ckan/default/ckan.ini`).

4. Restart CKAN. For example if you've deployed CKAN with nginx on Ubuntu:

     sudo systemctl reload nginx


## Config settings

None at present

## Developer installation

To install ckanext-madiphstheming for development, activate your CKAN virtualenv and
do:

    git clone https://github.com/treinar/ckanext-madiphstheming.git
    cd ckanext-madiphstheming
    python setup.py develop
    pip install -r dev-requirements.txt


## Tests

**Currently (2024-02-19) the tests are failing**

To run the tests, do:

    pytest --ckan-ini=test.ini


## License

[AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
