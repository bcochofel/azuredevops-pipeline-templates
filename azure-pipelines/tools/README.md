# Templates for some tools

## GitVersion

GitVersion template.

### GitVersion parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| version | string | GitVersion version to use | "5.x" | no |
| debug | boolean | Whether or not to show all variables for GitVersion | false | no |

## pre-commit

pre-commit template.

### pre-commit parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| pool | object | Agent pool | vmImage ubuntu-18.04 | no |
| python_version | string | Python version to use | "3.9" | no |
| install | boolean | Whether or not to install pre-commit | true | no |

## git-chglog

git-chglog template.

### git-chglog parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| install | boolean | Whether or not to install git-chglog | true | no |
| version | string | git-chglog version to install | "0.10.0" | no |

## References

* [Azure DevOps GitTools bundle](https://marketplace.visualstudio.com/items?itemName=gittools.gittools)
* [pre-commit](https://pre-commit.com/)
* [CHANGELOG Generator](https://github.com/git-chglog/git-chglog)
