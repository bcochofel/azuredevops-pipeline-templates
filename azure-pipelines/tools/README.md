# Templates for some tools

## GitVersion

GitVersion template has 2 optional parameters:

* version: Version to install (default 5.x)
* debug: Whether or not to print all variables (default false)

## pre-commit

pre-commit template has 3 optional parameters:

* pool: Agent Pool object (default vmImage ubuntu-18.04)
* python_version: Python version to use (default 3.9)
* install: Whether or not to install pre-commit (default true)

## References

* [Azure DevOps GitTools bundle](https://marketplace.visualstudio.com/items?itemName=gittools.gittools)
* [pre-commit](https://pre-commit.com/)
* [CHANGELOG Generator](https://github.com/git-chglog/git-chglog)
