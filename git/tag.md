# git tag

You can see the existing tags in Git by typing `git tag`.

```bash
$ git tag
v1.0
v1.1
```

You can also see the tags with particular pattern match.
If you want to search v2.1 series You can run below.

```bash
$ git tag -l "v2.1*"
v2.1.0
v2.1.1
v2.2.2
```

When you want to tag to any commit, you can run below.

```bash
$ git tag <tag_name> <commit> # tag to specified commit
$ git tag <tag_name> # tag to latest commit on current branch
```
