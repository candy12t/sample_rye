# sample-rye

try [rye](https://github.com/mitsuhiko/rye)

## rye

```sh
# init project
$ rye init sample && cd sample
$ tree
.
├── README.md
├── pyproject.toml
└── src
    └── sample_rye
        └── __init__.py

# specify python version
$ rye pin 3.11

# add module
$ rye add flask
$ rye add --dev pytest # only development

# install
$ rye sync # create file `requirements-dev.lock`, `requirements.lock`
$ tree
.
├── README.md
├── pyproject.toml
├── requirements-dev.lock
├── requirements.lock
└── src
    └── sample_rye
        └── __init__.py

# run pytest
$ rye run pytest

# build
$ rye build
```
