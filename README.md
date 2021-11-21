# Python Template

This is a template for python projects using python 3.6 and later.

## How to use

To create a repository using this template with github cli:

```
$ gh repo create --template bebleo/python-template
```

Or, create the repository on [github.com] using bebleo/python-template as a
template.

Once the repository has been completed then edit and commit:

1. `setup.cfg`, putting your own values in for author, author email, project
   name, description, and version.
2. `LICENSE` update the copyright name with an appropriate vaslue.
2. Rename the project folder to match the name. From inside the repository
   run `mv ./package_name ./{{ project.name }}` substituting
   the name of your package for "{{ project.name }}".

## About the template

This template is opinionanted and uses `tox` out of the box to run tests with
Python 3.6 to Python 3.10. We use `flake8` and `isort` for linting. To install
these:

```
$ python -m pip install --user -e .[dev]
```

Static type checking is handled using `mypy`, but this is not currently
installed for local use.
