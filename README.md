# New Mac Setup
Setup of essential tools to install after formatting my mac

# Mac Tools

- **Spectacle** : Managing windows 👓
- **iTerm2** : Better terminal 
- **HomeBrew** : For installing stuff
- [Atom](https://atom.io/) — My editor of choice ``` brew cask install atom ```
- Packages:
- Highlight Selected

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

- Setup [ZSH suggestions](https://github.com/zsh-users/zsh-autosuggestions)
```
brew install zsh-autosuggestions
``` 

- Setup [ZSH Syntax highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
``` 
brew install zsh-syntax-highlighting
``` 


- [Cascaria Font ( patched from Nerd Fonts)](https://github.com/ryanoasis/nerd-fonts/blob/master/patched-fonts/CascadiaCode/complete/Caskaydia%20Cove%20Regular%20Nerd%20Font%20Complete.ttf)

# Make the terminal pretty
- [I like this](https://medium.com/@Clovis_app/configuration-of-a-beautiful-efficient-terminal-and-prompt-on-osx-in-7-minutes-827c29391961)
- [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts#option-4-homebrew-fonts)
