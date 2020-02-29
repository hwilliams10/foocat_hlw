## foocat_hlw 

![](https://github.com/hwilliams10/foocat_hlw/workflows/build/badge.svg) [![codecov](https://codecov.io/gh/hwilliams10/foocat_hlw/branch/master/graph/badge.svg)](https://codecov.io/gh/hwilliams10/foocat_hlw) ![Release](https://github.com/hwilliams10/foocat_hlw/workflows/Release/badge.svg)

[![Documentation Status](https://readthedocs.org/projects/foocat_hlw/badge/?version=latest)](https://foocat_hlw.readthedocs.io/en/latest/?badge=latest)

Python package that eases the pain concatenating Pandas categoricals!

### Installation:

```
pip install -i https://test.pypi.org/simple/ foocat_hlw
```

### Features
- `catbind` combines two categorical variables

### Dependencies

- python = "^3.7"
- pandas = "^1.0.1"

### Usage

Example:
```
 >>> from foocat_hlw import foocat_hlw
 >>> a = pd.Categorical(["character", "hits", "your", "eyeballs"])
 >>> b = pd.Categorical(["but", "integer", "where it", "counts"])
 >>> foocat_hlw.catbind(a, b)
    [character, hits, your, eyeballs, but, integer, where it, counts]
    Categories (8, object): [but, character, counts,
    eyeballs, hits, integer, where it, your]
 ```

### Documentation
The official documentation is hosted on Read the Docs: <https://foocat_hlw.readthedocs.io/en/latest/>

### Credits
This package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
