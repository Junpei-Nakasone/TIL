# Git config

Git has a tool `git config` which controls configurations for how git works.

`git config` can be found in below three different places.

1. `/etc/gitconifg` file. That has configuration values for all users and all repositories on the system. If you specify `--system` option for `git config` command, the command read/write to this file.

2. The next place Git looks is the `~/.gitconfig` or `~/.config/git/config` file. That has configuration values for specific user. If you specify `--global` option for `git config` command, the command read/write to this file.

3. Finally, Git looks for `config` file on your current repository's git directory(which means `.git/config`). That has configuration values for specific repository.

Each of these levels (system, global, local) overwrites values in the previous level, so values in `.git/config` overwrites those in `[path]/etc/gitconfig`.
