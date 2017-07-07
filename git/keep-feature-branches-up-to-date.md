# How To: Keep Feature Branches Up To Date

If commits come into `upstream/master` after you [branch off](create-a-pr.md#step-2-create-new-feature-branch), you will need to keep your branch up to date with `upstream/master` before you PR. To do this, I recommend the slightly more challenging, yet more simple `rebase` method.

## Step 1: Ensure you're on the correct branch

```bash
git status
# check current branch, is it correct? If not:
git checkout my-feature-branch
```

## Step 2: Rebase!

Rebase is a utility that takes the master branch and "replays your work over it". It is the cleanest way to update your code with the latest master.

```bash
git rebase -i upstream/master
# You will be brought to an editor. You simply need to exit and save.
# If you stop at a commit, it's probably a merge conflict. This will be a somewhat rare occurrence.
# If it happens, you can try to resolve it with `git mergetool`.
# if you stop at a commit, it's probably a merge conflict. You can try to resolve with:
# Once it says your rebase is successful, VERIFY everything looks good, then force push like so:
git push -f # note: THIS DESTROYS OLD DATA ON GITHUB AND PUSHES YOUR LOCAL BRANCH UP FORCEFULLY
```
