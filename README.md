# set-up-repo

[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/suzuki-shunsuke/set-up-repo)

A tiny script to configure GitHub Repositories.

[setup](setup)

## What the script does

Configure repository settings:

- Disable Projects and Wiki
- Disable merge commits and rebase merging (only squash merging is allowed)
- Enable auto-merge
- Delete head branches on merge
- Allow updating branches

Enable security features:

- Immutable releases
- Dependabot alerts
- Private vulnerability reporting

Create repository rulesets:

- `main`: Protect the default branch (forbid deletion and force push, require pull requests)
- `require_sign`: Require signed commits on all branches
- `forbid_tag_change`: Forbid updating and deleting tags, and require signed tags
- `forbid_tag_creation`: Allow only repository admins to create tags

## How To Use

```sh
setup <repository full name>
```

e.g.

```sh
setup suzuki-shunsuke/setup-up-repo
```
