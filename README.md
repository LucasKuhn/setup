# New Mac Setup for a Web Developer
Setup of essential tools to install after formatting your mac 

# Basic things tutorial
- Install [HomeBrew](https://brew.sh) first, then use homebrew to install everything else.
```
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
``` 

- [Iterm2](https://iterm2.com) for a better terminal
```
brew cask install iterm2
``` 

- [Rectangle](https://rectangleapp.com) for window management ( I use the spectacle settings )
``` 
brew cask install spectacle
```

- [1Password](https://1password.com) for password management 
```bash
brew cask install 1password
```

- [VSCode](https://code.visualstudio.com) as an editor
``` 
brew cask install visual-studio-code
``` 

- [Atom](https://atom.io/) another editor 
``` 
brew cask install atom 
``` 

# Make your terminal pretty 
- Install [Oh My Zsh](https://ohmyz.sh)
``` 
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
``` 

- Set a theme for Oh My Zsh ( I use theunraveler )
``` 
open ~/.zshrc
ZSH_THEME="theunraveler"
``` 

- [Optional] Set a color theme for iTerm ( I love the one by [Clovis](http://www.clovis.pro), instruction below )
``` 
  Download the .itermcolors file from:   https://github.com/Clovis-team/clovis-open-code-extracts/tree/master/utils
  Preferences -> Profile -> Colors -> Import 
```

- Setup [ZSH suggestions](https://github.com/zsh-users/zsh-autosuggestions)
```
brew install zsh-autosuggestions
``` 

- Setup [ZSH Syntax highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
``` 
brew install zsh-syntax-highlighting
``` 

- Remember to use the included iTerm2 history-autocomplete: 
```
cmd + ;
```

- Improve iTerm window looks
```
Settings -> Appearance -> Theme: Minimal 
``` 

- Improve iTerm word travel 
``` 
Settings -> Profile -> Keys
```
- Then setup the following
```
" ⌥ + ← " - Travel back a word - Send text with Vim characters: \033b
" ⌥ + → " - Travel forward a word - Send text with Vim characters: \033f
" ⌥ + del " - Delete a word - Send hex code: 0x1B 0x08
" ⌘ + del " - Delete line - Send hex code: 0x15
```

- Change the font to Menlo (available by default)
```
Preferences -> Profile -> Text -> Font: Menlo
``` 

- Or install a custom font. I like Hack Font from [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts#option-4-homebrew-fonts)
``` 
brew tap homebrew/cask-fonts
brew cask install font-hack-nerd-font
brew untap homebrew/cask-fonts
``` 

- Other worthy mention fonts:
```
- Fira Code 
- Source Code Pro
- Cascadia 
```

Remove the `last login` line on top of iterm:
``` 
cd ~ ; touch .hushlogin
``` 

# Ruby Enviroment 

I recently started using `ruby-install` and `chruby` instead of `rbenv`.
It's a lightweight solution and seems simpler to use:
```
brew install ruby-install
brew install chruby
``` 

Then install the latest stable ruby: 
``` 
ruby-install ruby 
``` 

And enable chruby to set that version as default, and change the version according to .ruby-version file on a folder. 
To do so, append to your .zshrc:
```
source /usr/local/opt/chruby/share/chruby/chruby.sh
source /usr/local/opt/chruby/share/chruby/auto.sh
chruby ruby-2.7.2 # <- Your installed version here
```



# Sources
General setup and terminal:
- (I like this) https://medium.com/@Clovis_app/configuration-of-a-beautiful-efficient-terminal-and-prompt-on-osx-in-7-minutes-827c29391961
- https://medium.com/better-programming/setting-up-your-mac-for-web-development-in-2020-659f5588b883#3ead
- https://dev.to/v3frankie/setup-your-mac-for-development-2020-edition-1c8a
- https://github.com/bootcoder/ENV_Scratch_Setup#dotfiles

Ruby env:
- https://stackoverflow.com/questions/51126403/you-dont-have-write-permissions-for-the-library-ruby-gems-2-3-0-directory-ma
- https://stevemarshall.com/journal/why-i-use-chruby/
- https://www.moncefbelyamani.com/the-definitive-guide-to-installing-ruby-gems-on-a-mac/
- https://github.com/monfresh/install-ruby-on-macos
