
## How install my p9k-custom theme
We are going to install the following tools to help us achieve this look:

1. Install zsh
2. Install Oh-my-zsh (A Framework for managing your zsh configuration)
3. Powerlevel9k-custom (A Theme Engine for ZSH)

## Install zsh

Install zsh from repositories your distributive and verify:

```
$ sudo apt-get install zsh
$ zsh --version
```

Change the default shell from bash to zsh:

```
$ chsh -s $(which zsh)
```

Restarts your computer:
```
$ sudo shutdown -r now
```

## Installing Oh-my-zsh

Clone the repository:
```
$ git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
```

Backup your current ZSH Configuration:
```
$ cp ~/.zshrc ~/.zshrc.orig
```

Oh-my-zsh have provided us with sample .zshrc files for us to use and customise . We’ll be using one of the templates provided. Replace our ~/.zshrc with the one included in the templates.
```
$ cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
$ source ~/.zshrc
```

## Installing Powerlevel9k-custom

Oh my Zsh requires the themes to be in a specific directory ```custom/plugins/```
```
git clone git@github.com:devopscoder331/powerlevel9k-custom.git ~/.oh-my-zsh/custom/themes/powerlevel9k
```

Now select this theme in your ~/.zshrc file. Set ZSH_THEME in ~/.zshrc and save the file.
```
ZSH_THEME="powerlevel9k/powerlevel9k"
```

Now reload the shell with:
```
source ~/.zshrc
```
