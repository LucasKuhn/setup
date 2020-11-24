# New Mac Setup
Setup of essential tools to install after formatting my mac

# Tutorial
1. Install [HomeBrew](https://brew.sh) first, then use homebrew to install everything else.
```
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
``` 

- [Iterm2](https://iterm2.com)
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

- VSCode 
``` 
brew cask install visual-studio-code
``` 

- [Atom](https://atom.io/)
``` 
brew cask install atom 
``` 

- Atom 
```
brew cask install atom
``` 

# Make Terminal Pretty
- [Oh My Zsh](https://ohmyz.sh)
``` 
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
``` 

- Set a theme ( I use theunraveler )
``` 
open ~/.zshrc
ZSH_THEME="theunraveler"
``` 

- Set the awesome color scheme by the [Clovis](http://www.clovis.pro) team
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

- Use the included history-autocomplete: `cmd + ;` 

- Improve iTerm looks
```
Settings -> Appearance -> Theme: Minimal 
``` 

- Improve iTerm word travel 
``` 
Settings -> Profile -> Keys
```
`option + <-` - Travel back a word - Send text with Vim characters: \033b
`option + ->` - Travel forward a word - Send text with Vim characters: \033f
`option + del` - Delete a word - Send hex code: 0x1B 0x08
`cmd + del` - Delete line - Send hex code: 

- Change the font to Menlo (available by default)
```
Preferences -> Profile -> Text -> Font: Menlo
``` 

- But I prefer Install Hack Font from [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts#option-4-homebrew-fonts)
``` 
brew tap homebrew/cask-fonts
brew cask install font-hack-nerd-font
``` 

Worthy mention fonts:
- Fira Code 
- Source Code Pro
- Cascadia 


# Sources
- [I like this](https://medium.com/@Clovis_app/configuration-of-a-beautiful-efficient-terminal-and-prompt-on-osx-in-7-minutes-827c29391961)
- https://medium.com/better-programming/setting-up-your-mac-for-web-development-in-2020-659f5588b883#3ead
- https://dev.to/v3frankie/setup-your-mac-for-development-2020-edition-1c8a
