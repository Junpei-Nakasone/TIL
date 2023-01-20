`ssh-keygen` generates, manages and converts authentication keys for ssh. `ssh-keygen` can create RSA keys for use by SSH protocol version 1 and RSA or DSA keys for use by SSH protocol version2.The type of key to be generated is specified with the -t option. If invoked without any arguments, ssh-keygen will generate an RSA key for use in SSH protocol 2 connections.

example:
```bash
ssh-keygen -t rsa -f example-ssh-key -N ''
```

### Options
- -t type:
Specifies the type of key to create. The possible values are "rsa1" for protocol version 1 and "rsa" or "dsa" for protocol version 2.

- -f filename:
Specifies the filename of the key file.

- -N new_passphrase:
Provides the new passphrase.
