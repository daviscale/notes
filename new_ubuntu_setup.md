# Setting up a new Ubuntu instance

## Automated Software Installations

Run these commands to install software:

```bash
sudo apt-get update
sudo apt-get install neovim
sudo apt install openjdk-14-jre-headless
sudo apt-get install silversearcher-ag
sudo apt-get install tmux
```

## SBT

- Download the latest version of [sbt](https://www.scala-sbt.org/). 
- Extract the ZIP file. 
- Move the folder to /var/lib
- Make a link with `sudo ln -s /var/lib/sbt/bin/sbt /usr/local/bin`

## SSH

Generate a new ssh key with:

```bash
ssh-keygen
# follow the prompts

# Start the OpenSSH auth agent and add your newly created identity
eval `ssh-agent -s`
ssh-add
```

## nvim

Complete nvim setup found at https://github.com/daviscale/vimrc

## Git

Tell Git who you are:

```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

Tell Git you want to use nvim:

```bash
git config --global core.editor "nvim"
```
