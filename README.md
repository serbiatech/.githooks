# GitHooks - Collection of Git hooks
This repository is created with idea to be used as submodule for other repositories.
After installation every time when git commands are run this hooks will be triggered.

## Adding .githooks submodule to the existing repository
Hooks can be added to the existing repository with commands
```bash
git submodule add git@github.com:serbiatech/.githooks.git
git submodule init
```
## Updating .githooks submodule
After adding submodule or cloning repository that already have submodule we can install/update submodule with command
```bash
git submodule foreach git pull origin main
```

## Linking git hooks with client
We can link git hooks with command
```bash
sh .githooks/git-link-hooks
```

## Unlinking git hooks from client
We can unlink git hooks with command
```bash
sh .githooks/git-unlink-hooks
```
