# Git shallow clone

When you use `git clone` command, you will fetch whole repository code.
If you only need latest code and don't need to get change history, you can use bellow command.(It's called shallow clone)

```bash
git clone --depth 1 git@github.com:repository-url
```

After execute shallow clone, the repository has only one latest commit.


