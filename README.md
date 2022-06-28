# ssh-env
Easy way to switch between multiple SSH keys (mostly for git)

Include `ssh-env` in your bash profile config (~/.profile,  ~/.bash_profile, or ~/.bashrc) by adding:

```
 # SSH Default key
 export SSH_DEFAULT=~/.ssh/id_ed25519
 . ~/bin/ssh-env
```

After that you can use it with: `ssh-switch <key name>`

By default it will load the key set in `SSH_DEFAULT` at the shell initialization. 

Other commands are: 
 * `ssh-unset` will unset the env variables being set to the default key 
 * `ssh-list` will list all of the keys in your .ssh directory
 * `ssh-which` shows the current ssh key being set
