# ansible-pull-k9s-install
This repo will allow you to install k9s using ansible-pull

Example on how to use it:

```
ansible-pull --url git@github.com:ydewinte/ansible-pull-k9s-install.git --key-file ~/.ssh/id_rsa --accept-host-key --checkout main -e “version=v0.27.3” install-k9s.yml
```

Currently You will need to fork and change the value in the group_vars for the version or use the extra_vars parameter (-e) to provide the exact version you want, it is planned to make it pull the latest by default and specific when provided with the version variable via the parameter