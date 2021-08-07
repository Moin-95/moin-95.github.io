# Python

## Local setup

Install [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv)
```sh
brew install pyenv-virtualenv

echo 'eval "$(pyenv init --path)"' >> ~/.zprofile
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.zshrc
```

> `pyenv-virtualenv` uses `python -m venv` (Python 3.3+) if it is available and the `virtualenv` command if not.

Install [Python 3]()
```sh
# list possible python versions
pyenv install --list
# install a python version
pyenv install 3.9.5

# create a new virtualenv
pyenv virtualenv 3.9.5 python3
# activate a virtualenv
pyenv activate python3
# deactivate a virtualenv
pyenv deactivate

# path to python executable
pyenv which python
# list available virtualenvs
pyenv virtualenvs

# delete existing virtualenv
pyenv uninstall python3
```

## Containerized Python development

- [Docker blog post series](https://www.docker.com/blog/tag/python-env-series/)