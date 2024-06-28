# python versions and env setup
## install pyenv
1. check out the [manual](https://github.com/pyenv/pyenv?tab=readme-ov-file#unixmacos)
2. use the installation option through brew

## install pyenv-virtualenv plugin
see [here](https://github.com/pyenv/pyenv-virtualenv?tab=readme-ov-file#installing-with-homebrew-for-macos-users)
```
brew install pyenv-virtualenv
```

## pyenv usage
### list python version available for installation
```
pyenv install -l
```

### install a version of python
```
pyenv install 3.10.4
```

### list installed python versions/environments
```
pyenv versions
```

### create a new virtual environment
```
pyenv virtualenv <python_version> <environment_name>
```

### activate a venv
```
pyenv local myproject
```
to put a .python-version into the dir, or alternatively
```
pyenv activate myproject
```
