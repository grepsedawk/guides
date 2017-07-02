# How To: Fork and Setup Remotes

## Step 1: Fork the repository

https://help.github.com/articles/fork-a-repo/

## Step 2: Clone your version of the repository

```bash
git clone git@github.com:your_username/repo_name.git
cd repo_name/
```

## Step 3: Add upstream remote

```bash
git remote add upstream git@github.com:organization_name/repo_name.git
git fetch upstream
```

