# Setting up a new Ubuntu instance

## Automated Software Installations

Run these commands to install software:

```bash
sudo apt-get update
sudo apt-get install neovim
sudo apt-get install silversearcher-ag
sudo apt-get install tmux
```

## SSH

Generate a new ssh key with:

```bash
ssh-keygen -t ed25519 -C "your@example.com"
# follow the prompts

# Start the OpenSSH auth agent and add your newly created identity
eval `ssh-agent -s`
ssh-add
```

## nvim

Complete nvim setup found at https://github.com/daviscale/vimrc

## Git

Tell git who you are:

```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

Tell git you want to use nvim:

```bash
git config --global core.editor "nvim"
```

Tell git you want to update the default branch name to `main`:

```bash
git config --global init.defaultBranch main
```

## zsh

Follow instructions here to install zsh and make it the default shell:

https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH

Install oh my zsh:

https://ohmyz.sh/#install

Install your personal .zshrc file.
