# iTerm2 + Oh My Zsh + Dracula + PowerLevel10k

Refs:\
(1) https://dev.to/ibrahim_s/iterm2-oh-my-zsh-dracula-theme-plugins-2f9e

(2) https://dev.to/abdfnx/oh-my-zsh-powerlevel10k-cool-terminal-1no0

<br>

## Setup Zsh and Git
```
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
$ brew install zsh
$ brew install git
```

<br>

## Install iTerm2
```
$ sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
You can set iTerm2 as default terminal by clicking `iTerm2 > Make iTerm2 Default Term`.

<br>

## Install Dracula theme
```
$ git clone https://github.com/dracula/iterm.git
```

<br>

## Activate theme
(1) Go to `iTerm2 > Preferences > Profiles > Color Tab`\
(2) Open the `Color Presets...` by drop-down at the bottom right conner of the window\
(3) Select `Import...` from the list\
(4) Select `Dracula.itermcolors` file (Normally, this file located at `$HOME` directory of your computer)\
(5) Select the `Dracula` from `Color Presets...`\
(6) You can also install plugins, browse plugins at https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins\
(7) Run the `$ source ~/.zshrc` command to apply the changes

<br>

## PowerLevel10k setup
Powerlevel10k is a theme for Zsh. It emphasizes speed, flexibility and out-of-the-box experience.
Ref: https://github.com/romkatv/powerlevel10k

(1) Install recommended font at https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k \
(2) Install Powerlevel10k 
```
$ git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
Then you need to enable the Powerlevel10k theme by changing the value of ZSH_THEME to following in `~/.zshrc` file :
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```
(3) Open new terminal\
(4) Setup configuration wizard by type `p10k configure`

<br>

## Recommended plugin for terminal
[`exa`](https://the.exa.website/) is a modern replacement for `ls`
```
$ brew install exa
```