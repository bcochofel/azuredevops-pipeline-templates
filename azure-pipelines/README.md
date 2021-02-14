# Azure Pipeline templates

Several templates that can be used to keep your pipelines as code [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).

## pre-commit

pre-commit template.

### pre-commit parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| pool | object | Agent pool | vmImage ubuntu-18.04 | no |
| debug | boolean | Set pipeline to debug | false | no |
| python_version | string | Python version to use | "3.9" | no |
| install | boolean | Whether or not to install pre-commit | true | no |

## semver-annotated-tag.yml

Uses GitVersion template to calculate semantic version and create Git Annotated Tag.

### semver-annotated-tag parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| pool | object | Agent pool | vmImage ubuntu-18.04 | no |
| debug | boolean | Set pipeline to debug | false | no |

This template configures git user.email and user.name using some environment variables from the Agent:

* BUILD_REQUESTEDFOREMAIL
* BUILD_REQUESTEDFOR

## changelog.yml

Uses git-chglog to generate `CHANGELOG.md` file using the
[conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) messages.

### changelog parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| pool | object | Agent pool | vmImage ubuntu-18.04 | no |
| debug | boolean | Set pipeline to debug | false | no |
| install | boolean | Whether or not to install git-chglog | true | no |
