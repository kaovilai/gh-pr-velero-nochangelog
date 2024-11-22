# gh-pr-velero-nochangelog

A GitHub CLI extension script that creates pull requests with the `kind/changelog-not-required` label automatically applied.

Note that this requires you to have ability to create pull requests and apply labels on PRs in the repository.

## Usage

```bash
gh pr-velero-nochangelog [additional gh pr create flags]
```

## Features

- Creates a GitHub pull request using `gh pr create`
- Automatically adds the `kind/changelog-not-required` label
- Passes through any additional flags to the underlying `gh pr create` command

## Requirements

- [GitHub CLI](https://cli.github.com/) installed and configured
- Proper repository permissions to create pull requests and apply labels

## Installation

1. Make sure you have GitHub CLI installed
2. `gh extension install kaovilai/gh-pr-velero-nochangelog`

## Development
1. `gh extension install .`
2. `gh pr-velero-nochangelog --base something`

pr should be created with label to base branch "something"
