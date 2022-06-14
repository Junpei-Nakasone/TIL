# Symbolic link

Symbolic link is a link that is stored at one location on your machine and points to another location on the same machine.

Symbolic link is often shortened to `symlink`.

### how to make symbolic link

you can make symbolic link like below.

```bash
ls -s destination location
```

For example, if you move your .bashrc from HOME directory to dotfiles directory, you can make symbolic link with below command.

```bash
ls -s dotfiles/.bashrc ~/.bashrc
```
