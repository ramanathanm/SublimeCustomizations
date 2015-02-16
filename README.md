# SublimeCustomizations
All My Sublime Customizations

### Installed Packages
1. [SideBarEnhancements](https://github.com/titoBouzout/SideBarEnhancements)
2. [Auto Semi-colon](https://github.com/vivait/SublimeAutoSemiColon)
3. [Emmet](https://github.com/sergeche/emmet-sublime)

### Vintage Tweaks
1. Mac OS Vintage [key repeat](https://gist.github.com/kconragan/2510186) tweak - 
2. To support :q in the Command Pallete [Sublime 3 Unofficial-doc](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/command_palette.html)
  1. cd "Library/Application Support/Sublime Text 3/Packages/Default"
  2. edit Default.sublime-commands, add the below lines (use commas as appropriate)
  ```javascript
  { "caption": ":q Close", "command": "close" },
  { "caption": ":xa Close All", "command": "close_all" },
  { "caption": "File : Close", "command": "close" },
  { "caption": "File : Close All", "command": "close_all" },

