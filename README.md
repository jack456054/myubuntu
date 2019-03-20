# Install Zsh and Oh-My-Zsh on Ubuntu

## Install Zsh on Ubuntu:
```
$ sudo apt install zsh
```

## Install Oh-My-Zsh via wget:
```
$ sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

## Change the following line in ~/.zshrc file:
```
ZSH_THEME="agnoster"
```

## Install powerline font:
```
$ sudo apt-get install fonts-powerline
```

## Install more powerline font:
```
$ git clone https://github.com/powerline/fonts.git
$ ./fonts/install.sh
```
Note: Change font in the terminal setting.


## Install autosuggestions:
```
$ git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## Install syntax-highlighting:
```
$ git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

## Update plugins in .zshrc file:
```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```
Note: zsh-syntax-highlighting must be the last one.

## Source the .zshrc file:
```
$ source ~/.zshrc
```

## Change default shell to Zsh:
```
$ chsh -s $(which zsh)
```
Note: Need to log out and log into activate.
