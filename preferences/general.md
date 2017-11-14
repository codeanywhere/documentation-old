---
current_menu: general
---

# General Preferences
General Preferences are devided in three groups: Workspace, File Explorer and Editor.

Using GUI Preferences, you can set your general preferences and when you are done, just choose "Save" option.

![goto](images/gui_preferences.png "gui_preferences")

If you are defining preferences using JSON you must follow the Default General Preferences syntax which you can see at the bottom of this section.

For example, if you wish to chacge a Theme, you'll see it is set to: 
```
"workspace": { 
	"theme": "monokai" 
} 
```
And now you can change it inside Preferences -> User/Project -> General, by adding code:
```
"workspace": { 
	"theme": "white" 
}
```
And by doing this, you'll override settings from Default.

All Default General Preferences:
```
{

  "workspace": {
    // should preferences be defined in JSON format
    "json_preferences": false,

    // whether to use live pair programming on shared files
    "pair_programming": false,

    // codeanywhere visual theme
    // currently available: "monokai", "monokai-retina", "dark", "white"
    "theme": "monokai",

    // editor syntax highlighting
    // currently available: "monokai", "dark", "white", "eclipse", "ambiance", "blackboard", "pastel-on-dark", "seti"
    "color_scheme": "monokai",
    
    // use sound notifications (for example on file save)
    "sounds": true,
    
    // whether to show info on how to use copy/paste in SSH terminal (for windows)
    "ssh_copy_paste_info": true,

    // whether to open SSH Terminal tabs in bottom panel (if single or row-2 layout is used)
    "open_ssh_in_bottom_panel": false
  },
 
  "fileExplorer": {
    // should file explorer be visible
    "visible": true,

    // show checkboxes for selecting files in file explorer
    "checkboxes": false,

    // open files and folders with a double click
    "dblclick": false,

    // show hidden files and folders
    "show_hidden_files": true,

    // show open files
    "show_open_files": true,

    // should horizontal scroll be enabled
    "horizontal_scroll": false,

    // should drag & drop be disabled
    "dragDrop_disabled": false
  },

  "editor": {
    // auto-close brackets and quotes while typing. By default, it'll auto-close ()[]{}''""
    "auto_close_brackets": true,

    // auto-close html tags
    "auto_close_tags": true,

    // show code completions while typing 
    "autocomplete": true,

    "bookmarks": true,

    // whether to periodically save unsaved opened tabs 
    "autosave": false,

    // whether to show colorpicker when invoked 
    "colorpicker": true,

    // auto detect indentation on file open (spaces or tabs)
    "detect_indentation": true,

    // open file with encoding
    "default_encoding": "UTF-8",

    // whether to expand emmet abbreviation when indenting (usually when tab key is pressed)
    "emmet_expand_abbreviation_on_indent": true,

    // show fold icons in gutter
    "fold_gutter": true,

    // editor font size
    "font_size": 14,

    // editor font family (if set to false, theme default will be used)
    // available options: 'Anonymous Pro', 'Droid Sans Mono', 'Inconsolata', 'Raleway', 'PT Mono', 'Source Code Pro', 'Share Tech Mono', 'Ubuntu Mono'
    "font_family": "Inconsolata",

    // the period of inactivity (in milliseconds) that will cause a new history event to be started when typing or deleting
    "history_event_delay": 250,

    // highlights occurrences of the selected text
    "highlight_selection_matches": true,

    // highlight active line in gutter
    "hover_active_line": true,

    // default indentation (can be ignored if detect_indetation is enabled)
    "indent_with_tabs": false,

    // show line numbers in gutter
    "line_numbers": true,

    // show errors and warnings in gutter
    "lint": true,

    // when enabled, causes matching brackets to be highlighted whenever the cursor is next to them
    "match_brackets": true,

    // when enabled, will cause the tags around the cursor to be highlighted
    "match_tags": true,

    // whether to show MiniMap in editor
    "minimap": true,

    // open editor in read-only mode
    "read_only": false,

    // editor scroll style
    // available options: "overlay" and "native"
    "scrollbar_style": "overlay",

    // the number of spaces a tab is considered equal to
    "tab_size": 2,

    // the maximum number of undo levels that the editor stores
    "undo_depth": 1000,

    // whether to scroll or wrap long lines
    "wrap_lines": false
  }

}
```
