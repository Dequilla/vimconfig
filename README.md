# My vim config

# Install
## Linux
`git clone https://github.com/Dequilla/vimconfig.git && cd vimconfig/ && chmod +x install.sh && ./install.sh`

## Windows
`git clone https://github.com/Dequilla/vimconfig.git; cd .\vimconfig\; .\win-install.ps1`


### Context Menu (right click)
- Add the following to a .reg file and run to get neovim to right-click menu on Windows.
```
Windows Registry Editor Version 5.00

;; Neovim-Qt

[HKEY_CLASSES_ROOT\*\shell\nvim-qt]
@="Edit with Neovim-Qt"
"Icon"="\"C:\\Program Files\\Neovim\\bin\\nvim-qt.exe\""

[HKEY_CLASSES_ROOT\*\shell\nvim-qt\command]
@="\"C:\\Program Files\\Neovim\\bin\\nvim-qt.exe\" \"%1\""

[HKEY_CLASSES_ROOT\Directory\shell\nvim-qt]
@="Open with Neovim-Qt"
"Icon"="\"C:\\Program Files\\Neovim\\bin\\nvim-qt.exe\""

[HKEY_CLASSES_ROOT\Directory\shell\nvim-qt\command]
@="\"C:\\Program Files\\Neovim\\bin\\nvim-qt.exe\" \"%1\""

[HKEY_CLASSES_ROOT\Directory\Background\shell\nvim-qt]
@="Open Neovim-Qt here"
"Icon"="\"C:\\Program Files\\Neovim\\bin\\nvim-qt.exe\""

[HKEY_CLASSES_ROOT\Directory\Background\shell\nvim-qt\command]
@="\"C:\\Program Files\\Neovim\\bin\\nvim-qt.exe\" \"%v\""
```
Based on [this](https://gist.github.com/JAffleck/2ba6ca0bd0d5545fd17c396357b9abf0)
