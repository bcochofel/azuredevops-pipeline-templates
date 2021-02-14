# Azure Pipeline templates

Several templates that can be used to keep your pipelines as code [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).

## semver-annotated-tag.yml

Uses GitVersion template to calculate semantic version and create Git Annotated Tag.

### Parameters

| name | type | description | default | required |
| ---- | ---- | ----------- | ------- | -------- |
| pool | object | Agent pool | vmImage ubuntu-18.04 | no |
| version | string | GitVersion version to use | "5.x" | no |
| debug | boolean | Whether or not to show all variables for GitVersion | false | no |

This template configures git user.email and user.name using some environment variables from the Agent:

* BUILD_REQUESTEDFOREMAIL
* BUILD_REQUESTEDFOR
