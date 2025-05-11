# SSH

## Security Key

* Generate SSH key: `ssh-keygen -t ed25519-sk -O resident -O verify-required -O application=ssh:trentshailer.com -C ssh:trentshailer.com`
* Retrieve SSH key: `sudo ssh-keygen -K`

## `config`

```
Host server
	HostName 127.0.0.1
	IdentityFile ~/.ssh/id_ed25519_sk_desktop
	User username
Host github.com
	IdentityFile ~/.ssh/id_ed25519_sk_desktop
```
