# ansible-pull-k9s-install
This repo will allow you to install k9s using ansible-pull, one command, no fuss anymore...

Prerequisites:
* Ansible is installed on the machine
* The key on the machine you try to deploy it on needs to have it's public key in a git user (doesn't matter which one)

Example on how to use it:

```
# Example 1: No key (auto selection of ~/.ssh/id_rsa) and use group_vars value (latest version)

ansible-pull --url git@github.com/ydewinte/ansible-pull-k9s-install.git --accept-host-key install-k9s.yml

# Example 2: Specific key and version v0.27.2

ansible-pull --url git@github.com/ydewinte/ansible-pull-k9s-install.git --key-file /specific/private/key --accept-host-key --checkout main -e “version=v0.27.2” install-k9s.yml
```
