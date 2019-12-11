
# Practice on Git

## Table of Contents

* [Fork](#fork)
* [gitignore](#gitignore)  

<a name="fork"/>

## Fork

A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project. [Learn more](https://help.github.com/en/articles/fork-a-repo)

<img src="/docs/images/git-fork.png" alt="alt text" width="100%" />

### Keeping a fork up to date

#### 1. Clone your fork:

```
git clone git@github.com:YOUR-USERNAME/YOUR-FORKED-REPO.git
```

##### 2. Add remote from original repository in your forked repository: 
```
cd into/cloned/fork-repo
git remote add upstream git://github.com/ORIGINAL-DEV-USERNAME
REPO-YOU-FORKED-FROM.git
git fetch upstream
```

##### 3. Updating your fork from original repo to keep up with their changes:

```
git pull upstream master
```

### How can I change the author name

```
$ git filter-branch --env-filter '
WRONG_EMAIL="wrong@example.com"
NEW_NAME="New Name Value"
NEW_EMAIL="correct@example.com"

if [ "$GIT_COMMITTER_EMAIL" = "$WRONG_EMAIL" ]
then
    export GIT_COMMITTER_NAME="$NEW_NAME"
    export GIT_COMMITTER_EMAIL="$NEW_EMAIL"
fi
if [ "$GIT_AUTHOR_EMAIL" = "$WRONG_EMAIL" ]
then
    export GIT_AUTHOR_NAME="$NEW_NAME"
    export GIT_AUTHOR_EMAIL="$NEW_EMAIL"
fi
' --tag-name-filter cat -- --branches --tags
```

<a name="gitignore"/>

## gitignore

To find best gitignore configure: [https://www.gitignore.io/](https://www.gitignore.io/)

#### Example:

System:
```
# System
.DS_Store
```

IDE:

```
# IDE config
/.idea
/.vscode
```
Terraform:

```
# Ignore Terraform default files
.terraform/
/.terraform/
*.local.auto.tfvars
```

Node:

```
### Node ###
# Logs
logs
*.log
npm-debug.log*
yarn-debug.log*
yarn-error.log*
lerna-debug.log*

# Dependency directories
node_modules/
jspm_packages/
```
