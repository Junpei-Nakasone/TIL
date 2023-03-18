```bash
git config --get remote.origin.url

git@github.com:Junpei-Nakasone/til.git
```

```bash
git remote show origin

* remote origin
  Fetch URL: git@github.com:Junpei-Nakasone/til.git
  Push  URL: git@github.com:Junpei-Nakasone/til.git
  HEAD branch: main
  Remote branches:
    develop   tracked
    feature-a tracked
    main      tracked
  Local branch configured for 'git pull':
    main merges with remote main
  Local refs configured for 'git push':
    develop pushes to develop (fast-forwardable)
    main    pushes to main    (up to date)
```

```bash
cat .git/config

[core]
        repositoryformatversion = 0
        filemode = true
        bare = false
        logallrefupdates = true
        ignorecase = true
        precomposeunicode = true
[remote "origin"]
        url = git@github.com:Junpei-Nakasone/til.git
        fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
        remote = origin
        merge = refs/heads/main
```

```bash
git remote -v

origin  git@github.com:Junpei-Nakasone/til.git (fetch)
origin  git@github.com:Junpei-Nakasone/til.git (push)
```
