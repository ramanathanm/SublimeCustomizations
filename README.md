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
  ```

3. Escape key to close "Autocomplete" menu & entre directly in to "Normal/Escape mode" - [Reference](https://github.com/tonymagro/VintageEscape), Add the following lines to Default key bindings:
  ```javascript
  [
  	{ "keys": ["escape"], "command": "exit_auto_complete_and_insert_mode", "context":
  		[
  			{ "key": "auto_complete_visible", "operator": "equal", "operand": true }
  		]
  	},
  
  	{ "keys": ["ctrl+["], "command": "exit_auto_complete_and_insert_mode", "context":
  		[
  			{ "key": "auto_complete_visible", "operator": "equal", "operand": true }
  		]
  	}
  ]
```
  
### My Sublime Config

```javascript
{
  "font_face": "Inconsolata",
  "font_size": 12,
  "color_scheme": "Packages/Color Scheme - Default/Monokai.tmTheme",
  "color_scheme": "Packages/Tomorrow-Night.tmTheme",
  "tab_size": 2,
  "hot_exit": true,
  "file_exclude_patterns":
  [
    ".gitkeep",
    ".gitignore",
    ".bowerrc",
    ".ember-cli",
    ".jshintrc",
    ".editorconfig",
    ".travis.yml"
  ],
  "folder_exclude_patterns":
  [
    ".svn",
    ".git",
    ".hg",
    "CVS",
    "tmp",
    "node_modules",
    "bower_components",
    "dist"
  ],
  "font_size": 13,
  "ignored_packages":
  [
  ],
  "rulers":
   [
      "horizontal"
   ],
  "theme": "Soda Light.sublime-theme",
  "vintage_start_in_command_mode": true,
  "caret_style": "phase",
  "highlight_line": true,
  "fade_fold_buttons": false,
  "bold_folder_labels": true,
  "vintage_ctrl_keys": true,
  "vintage_start_in_command_mode": true,
  "find_selected_text": true,
  "highlight_modified_tabs": true
}
```
