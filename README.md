# Installing usable bash autocomplete shell on Ubuntu 16.10 / 17.04

## 1. Step install zsh:

```
~> sudo apt-get install zsh
~> sudo apt-get install git-core
~> wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh
~> chsh -s `which zsh`
~> sudo shutdown -r 0
```

## 2. Step edit ~/.zshrc

```
~> gedit .zshrc

   Change following lines :
   ------------------------
   ZSH_THEME="fishy"
   plugins=(git cp command-not-found git-extras gnu-utils history pip python ruby screen svn)

   Uncomment :
   -----------
   DISABLE_AUTO_UPDATE="true"

   Add to end  :
   -------------
   source $HOME/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh
```

## 3. Download and install zsh-autosuggestions

```
~> cd ~
~> mkdir .zsh
~> cd .zsh
~> git clone https://github.com/zsh-users/zsh-autosuggestions
```

## 4. Done !


