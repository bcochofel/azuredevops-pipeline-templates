# Templates for some tools

## GitVersion

GitVersion template.

### GitVersion parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| version | string | GitVersion version to use | "5.x" | no |
| debug | boolean | Whether or not to show all variables for GitVersion | false | no |

## git-chglog

git-chglog template.

The message used to commit has the `[skip ci]` option to avoid trigerring a CI build.
See [this](https://docs.microsoft.com/en-us/azure/devops/pipelines/scripts/git-commands?view=azure-devops&tabs=yaml)
for moe info.

### git-chglog parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| install | boolean | Whether or not to install git-chglog | true | no |
| version | string | git-chglog version to install | "0.10.0" | no |
| useNextTag | boolean | Whether or not to use --nex-tag | false | no |
| nextTag | string | --next-tag argument (retrieve from GitVersion) | "" | no |

## References

* [Azure DevOps GitTools bundle](https://marketplace.visualstudio.com/items?itemName=gittools.gittools)
* [pre-commit](https://pre-commit.com/)
* [CHANGELOG Generator](https://github.com/git-chglog/git-chglog)
