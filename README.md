# macos-ventura-setup
## System Settings
### Desktop & Dock
```
- Size -> 1/5
- Magnification -> Disable
- Automatically hide and show the Dock -> Enable
- Show recent applications in Dock -> Disable
- Hot Corners... \
  - Disable all
```
### Display
```
- Default --> More Space
- Automatically adjust brightness -> Enable
- Night Shift... \
  - Schedule -> Sunset to Sunrise
  - Turn on until sunrise -> Enable
  - Color temperature -> 1/3 below balance
```
### Touch ID & Password
```
```
### Notifications
```
- Disable all, except calender
```
### Siri & Spotlight
```
- Ask Siri -> Disable
- Spotlight -> Disable all, except Applications, System Preferences
```
### General
```
- Sharing \
  - Disable all
  - Hostname -> minhtuan1407.local
```
### Privacy & Security
```
- FileVault -> Turn On
- Screen Recording -> Add Chrome
```
### Trackpad
```
- Tracking speed -> 9/10
- Tap to click -> Enable
```
### Keyboard
```
- Key repeat rate -> 7/7
- Delay until repeat -> 5/5
```
### Accessibility
```
- Pointer Control \
  - Trackpad Options... \
    - Scroll speed -> 6/8
```
### Battery
```
- Options \
  - Wake for network access -> Only on Power Adapter
  - Optimize video streaming while on battery
```
### Control Center
```
- Battery \
  - Show Percentage -> Enable
- Keyboard Brightness \
  - Show in Control Center -> Enable
- Clock \
  - Clock Options \
  - Display time with seconds -> Enable
- Spotlight -> Don't Show in Menu Bar
```

## Finder
```
- Sidebar \
  - Favorites -> Enable all
  - Locations -> Enable all
  - Drag Library to Favorites
- Tags -> Disable all
- Advanced \
  - Showw all filename extensions -> Enable
  - Remove items from the Trash after 30 days
```

## Terminal
### Install homebrew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/minhtuan1407/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```
```
brew update
```
### Install app
```
brew install --cask \
  iterm2 \
  visual-studio-code \
  sublime-text \
  postman \
  vlc \
  zalo \
  telegram \
  evkey \
  microsoft-remote-desktop \
  the-unarchiver \
  bitwarden \
  alt-tab \
  authy \
  viber \
  zoom
```
```
brew install \
  wget \
  git \
  exa
```
### Install oh my zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
```
omz update
```
### Install zsh pluglin
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:-${ZSH:-~/.oh-my-zsh}/custom}/plugins/zsh-completions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
### Install starship
```
brew install starship
```
```
echo 'eval "$(starship init zsh)"' >> ~/.zshrc
```
### Install zoxide
```
curl -sS https://raw.githubusercontent.com/ajeetdsouza/zoxide/main/install.sh | bash
```
```
echo 'eval "$(zoxide init zsh)"' >> ~/.zshrc
```
### Install rosetta2
```
/usr/sbin/softwareupdate --install-rosetta --agree-to-license
```
### Git setup
```
git config --global user.name "minhtuan1407"
git config --global user.email "m.tuan9a2@gmail.com"
```
```
git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
```
```
git config --global init.defaultBranch main
```
### Setup hostname
```
sudo scutil --set ComputerName "minhtuan1407"
sudo scutil --set LocalHostName "minhtuan1407"
sudo scutil --set HostName "minhtuan1407"
```
### Setup system preferences
```
defaults write com.apple.screencapture type jpg
defaults write com.apple.Preview ApplePersistenceIgnoreState YES
chflags nohidden ~/Library
defaults write com.apple.finder AppleShowAllFiles YES
defaults write com.apple.finder ShowPathbar -bool true
defaults write com.apple.finder ShowStatusBar -bool true
killall Finder;
```
## Iterm2
```

```
