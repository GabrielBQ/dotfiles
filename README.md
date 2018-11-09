# My DotFiles

## 0. Generate `SSH` keys

Follow this steps

Check out [Generating a new SSH key and adding it to the ssh-agent](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

### Steps

```sh
❯ ssh-keygen -t rsa -b 4096 -C "gabrielbarreiroquintans@gmail.com"
❯ bash
❯eval "$(ssh-agent -s)"
❯fish
❯ssh-add ~/.ssh/id_rsa
```

Then, enter to [Add the SSH key to your GitHub account.](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account)

and

```
❯sudo apt-get install xclip
❯xclip -sel clip < ~/.ssh/id_rsa.pub
```

Finally, go to setting on your profile of [GitHub](https://github.com/GabrielBQ), to the `SSH` and `GPG` keys and create a new SSH key (like SSH @ObradoiroTeo),
on the description, use paste.

## How to install

```sh
❯ cd ~/projects
❯ git clone git@github.com:GabrielBQ/dotfiles.git
❯ cd dotfiles
❯ cp ./gitconfig  ~/.gitconfig
```
