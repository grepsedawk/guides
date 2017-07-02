# How To: Fork and PR code

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

## Step 4: Create new feature branch

```bash
git fetch upstream
git checkout upstream/master
git checkout -b my-branch-name
```

## Step 5: Commit

```bash
git status
git add file1 file2 file3 # or git add -p for interactive patch add
git commit
```

## Step 6: Push

For the first push:
```bash
git push --set-upstream origin my-branch-name
```

For all later pushes:
```bash
git push
```

## Step 7: Submit Pull Request

https://help.github.com/articles/creating-a-pull-request-from-a-fork/

## Step 8: Repeat

Repeat steps 4-7 for additional PRs
