
You can check all shells which can be login shell on your computer by displaying `/etc/shells`.

```bash
cat /etc/shells
# List of acceptable shells for chpass(1).
# Ftpd will not allow users to connect who are not using
# one of these shells.

/bin/bash
/bin/csh
/bin/dash
/bin/ksh
/bin/sh
/bin/tcsh
/bin/zsh
```

If fish is not on `/etc/shells` you can add fish.

Check fish's path.

```bash
which fish
/usr/local/bin/fish
```

add fish to `/etc/shells`.

```bash
suto vi /etc/shells
Password:
```

Confirm that fish is on `/etc/shells`.

```bash
cat /etc/shells
# List of acceptable shells for chpass(1).
# Ftpd will not allow users to connect who are not using
# one of these shells.

/bin/bash
/bin/csh
/bin/dash
/bin/ksh
/bin/sh
/bin/tcsh
/bin/zsh
/usr/local/bin/fish
```

Change the login shell to fish.

```bash
chsh -s /usr/local/bin/fish
```
