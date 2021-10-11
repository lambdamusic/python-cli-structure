# Python CLI structure

A reusable project structure for CLI applications built with Python.

Features

* Uses [Click](https://click.palletsprojects.com)
* Include basic [Sphinx](https://www.sphinx-doc.org/en/master/) docs structure
* Packaged with [setuptools](https://setuptools.pypa.io/en/latest/setuptools.html)


## How to use? 

Clone this project and use it as the basis for your CLI. 

EG you can have a bash scommand that helps with that:s

```bash
new_pycli () { cp -R /path/to/python-cli-structure newcliapp; rm -R newcliapp/cliapp.egg-info; rm -rf newcliapp/.git; cd newcliapp; }
```

Then you can call `new_pycli` to get a fresh CLI project structure (make sure you update the path above as per your installation).

## cliapp - first time setup

1. pick a $PROJECT_NAME

2. search for 'cliapp' with you IDE and replace with PROJECT_NAME

3. rename the top level folder 'cliapp' with PROJECT_NAME

4. Create virtual env and off you go!

```
$ mkvirtualenv $PROJECT_NAME
$ pip install --editable .
```