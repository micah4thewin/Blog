# GitHub CLI

## Installation

* Download and install GitHub CLI: https://cli.github.com/

## Authentication

* Authenticate with your GitHub account: `gh auth login`
* Log out from your GitHub account: `gh auth logout`

## Repository Management

* Clone a repository: `gh repo clone [owner/repo]`
* Create a new repository: `gh repo create [name]`
* View the current repository: `gh repo view [--web]`

## Issues

* List issues: `gh issue list`
* Create a new issue: `gh issue create`
* View an issue: `gh issue view [issue_number]`
* Close an issue: `gh issue close [issue_number]`
* Reopen an issue: `gh issue reopen [issue_number]`

## Pull Requests

* List pull requests: `gh pr list`
* Create a new pull request: `gh pr create`
* View a pull request: `gh pr view [pr_number]`
* Merge a pull request: `gh pr merge [pr_number]`
* Close a pull request: `gh pr close [pr_number]`
* Checkout a pull request branch: `gh pr checkout [pr_number]`

## Gists

* Create a new gist: `gh gist create [file1] [file2] ...`
* List gists: `gh gist list`
* View a gist: `gh gist view [gist_id]`

## Aliases

* List aliases: `gh alias list`
* Set a new alias: `gh alias set [alias_name] [command]`
* Remove an alias: `gh alias rm [alias_name]`

## Help

* Show help: `gh help`
* Show help for a specific command: `gh [command] --help`
