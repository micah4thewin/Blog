## Authentication

* Authenticate with your GitHub account:
```bash
gh auth login
```
* Log out from your GitHub account:
```bash
gh auth logout
```

## Repository Management

* Clone a repository:
```bash
gh repo clone [owner/repo]
```
* Create a new repository:
```bash
gh repo create [name]
```
* View the current repository:
```bash
gh repo view [--web]
```

## Issues

* List issues:
```bash
gh issue list
```
* Create a new issue:
```bash
gh issue create
```
* View an issue:
```bash
gh issue view [issue_number]
```
* Close an issue:
```bash
gh issue close [issue_number]
```
* Reopen an issue:
```bash
gh issue reopen [issue_number]
```

## Pull Requests

* List pull requests:
```bash
gh pr list
```
* Create a new pull request:
```bash
gh pr create
```
* View a pull request:
```bash
gh pr view [pr_number]
```
* Merge a pull request:
```bash
gh pr merge [pr_number]
```
* Close a pull request:
```bash
gh pr close [pr_number]
```
* Checkout a pull request branch:
```bash
gh pr checkout [pr_number]
```

## Gists

* Create a new gist:
```bash
gh gist create [file1] [file2] ...
```
* List gists:
```bash
gh gist list
```
* View a gist:
```bash
gh gist view [gist_id]
```

## Aliases

* List aliases:
```bash
gh alias list
```
* Set a new alias:
```bash
gh alias set [alias_name] [command]
```
* Remove an alias:
```bash
gh alias rm [alias_name]
```

## Help

* Show help:
```bash
gh help
```
* Show help for a specific command:
```bash
gh [command] --help
```
