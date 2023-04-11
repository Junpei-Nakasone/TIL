https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection
```
ssh -T git@github.com
```

This command uses the SSH protocol to connect to GitHub and performs a test to verify whether authentication is successful or not.

Specifically, the `ssh` command is used to connect to a remote host using the SSH protocol, and the `-T` option is used to prevent the SSH client from allocating a TTY(terminal) after connecting. This means that the SSH session is used only for the purpose of authentication testing and will not be connected to remote shell.
