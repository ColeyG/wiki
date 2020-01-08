# SSH Keygen

- `ssh-keygen -t rsa` Create a key (on the local machine)
- `ssh-copy-id -i ~/.ssh/<KEYNAME>.pub user@host` Send the key to the remote host
