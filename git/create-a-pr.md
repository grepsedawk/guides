# How To: Create a PR

## Step 1: Ensure your repo/remotes are set up properly

You can find a guide here:

https://github.com/pachonk/guides/blob/master/git/fork-and-setup-remotes.md

## Step 2: Create new feature branch

```bash
git fetch upstream
git checkout upstream/master
git checkout -b my-branch-name
```

## Stepi 3: Commit

```bash
git status
git add file1 file2 file3 # or git add -p for interactive patch add
git commit
```

## Step 4: Push

For the first push:
```bash
git push --set-upstream origin my-branch-name
```

For all later pushes:
```bash
git push
```

## Step 5: Submit Pull Request

https://help.github.com/articles/creating-a-pull-request-from-a-fork/

## Step 6: Repeat

Repeat steps 2-5 for additional PRs

