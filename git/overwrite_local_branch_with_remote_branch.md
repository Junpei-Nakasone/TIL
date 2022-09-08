If you added commit which is not need to push remote branch and want to sync your local branch with your remote branch, you can use below.

```bash
git fetch
git checkout branch_1
git reset --hard origin/branch_1
```
