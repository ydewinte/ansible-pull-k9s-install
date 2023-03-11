# ansible-pull-k9s-install
This repo will allow you to install k9s using ansible-pull
`ansible-pull --url git@github.com:ydewinte/ansible-pull-k9s-install.git --key-file ~/.ssh/id_rsa --accept-host-key --checkout main -e “version=v0.27.3” install-k9s.yml