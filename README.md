# My dotfiles

## 0.Generate SSH keys

Check out [Generating a new SSH key and adding it to the ssh-agent](https://help.github.com/enterprise/2.15/user/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

## Steps

```
❯ mkdir ~/.ssh
❯ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
❯ bash
❯ eval "$(ssh-agent -s)"
❯ fish
❯ ssh-add ~/.ssh/id_rsa
❯ sudo apt-get install xclip
❯ xclip -sel clip < ~/.ssh/id_rsa.pub
```

Finaly, we need to perform these steps --> [Add the SSH key to your GitHub Account](https://help.github.com/enterprise/2.15/user/articles/adding-a-new-ssh-key-to-your-github-account)

## 1. How to install

Follow these steps

```
❯ cd ~/projects
❯ git clone git@github.com:MattCo23/dotfiles.git
❯ cd dotfiles
❯ cp ./gitconfig ~/.gitconfig
```
