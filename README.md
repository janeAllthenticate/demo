# demo
Demo Allthenticate Capabilities

```
git config --global gpg.format ssh
git config --global commit.gpgsign true
git config --global user.signingkey $(allthenticate-get-key)
```

Set ssh agent to use allthenticate agent
```
# zsh
echo "export SSH_AUTH_SOCK=$HOME/.ssh/allthenticate-agent.sock" >> ~/.zshenv
# bash
echo "export SSH_AUTH_SOCK=$HOME/.ssh/allthenticate-agent.sock" >> ~/.bashrc
```
