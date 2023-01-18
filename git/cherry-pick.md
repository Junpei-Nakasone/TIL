If you added the latest commit on branch-a and want to add that commit to branch-b, you can use `cherry-pick` command.

git checkout branch-b
git pull
git cherry-pick commit_hash_id
git push origin branch-b

Difference of `git rebase` and `git cherry-pick`

`git rebase branch-b` will add all commit on branch-a to branch-b.

`git cherry-pick` will add only specified commit on branch-a to branch-b.
