https://man.openbsd.org/ssh-keygen.1#R
```bash
ssh-keygen -R example.com
```

### ssh-keygen — OpenSSH authentication key utility

### -R hostname
Removes all keys belonging to the specified hostname(with optional port number) from a known_hosts file. This option is useful to delete hashed hosts.
