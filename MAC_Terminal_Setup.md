# Setup Your Mac Terminal

## Install Homebrew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Add Homebrew To Path
```
  echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/[username]/.zprofile
  eval "$(/opt/homebrew/bin/brew shellenv)"
```

## Install iTerm2
``` 
brew install --cask iterm2
```

## Install Git
```
brew install git
```

## Install Oh My Zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```


## Install PowerLevel10K Theme for Oh My Zsh
```
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
Now that it’s installed, open the ”~/.zshrc” file with your preferred editor and change the value of “ZSH_THEME” as shown below:

```
 ZSH_THEME="powerlevel10k/powerlevel10k"
```

To reflect this change on your terminal, restart it or run this command:

```
	source ~/.zshrc
 ```

## Install Meslo Nerd Font
Install the font by pressing “y” and then quit iTerm2.

## Update VSCode Terminal Font (Optional)
Open settings.json and add this line:
```
"terminal.integrated.fontFamily": "MesloLGS NF"
```

## Configure PowerLevel10K
Restart iTerm2. You should now be seeing the PowerLevel10K configuration process. If you don’t, run the following:
```
p10k configure
```
## Increase Terminal Font Size
	• Open iTerm2 preferences
	• Go to Profiles > Text
	• I increase my font size to about 20px


## Install ZSH Plugins

### Install z-sh autosuggestions :
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

### Install zsh-syntax-highlighting:
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

Open the ”~/.zshrc” file in your desired editor and modify the plugins line to what you see below.
```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting web-search)
```

### Load these new plugins by running:
```
source ~/.zshrc
```

