---
current_menu: commandsandkeybindings
---

# Key Bindings

Nearly every action in Codeanywhere has a corresponding command associated with it. On top of that, every command also has a key binding that can be used to effortlessly execute the command.

Key Bindings preferences can be defined for two categories: PC and Mac.

Using GUI Preferences, you can change existing commands and when you are done, just choose "Save" option.

![goto](images/keybindings.png "keybindings")

If you are defining preferences using JSON you must follow the Default Key Bindings Preferences syntax which you can see at the bottom of this section.

For example, if you wish to change key shortcut for auto indenting, you'll see it is set to: 
```
"auto_indent": {
    "keys": ["Alt-Shift-Tab"]
}
```
And now you can change it inside Preferences -> User/Project -> Key Bindings, by adding code:
```
"auto_indent": {
    "keys": ["Alt-Shift-Tab-A"]
}
```
And by doing this, you'll override settings from Default. 

All Default Key Bindings Preferences:
```
{

  "auto_indent": {
    "keys": ["Alt-Shift-Tab"]
  },

  "beautify": {
    "keys": ["Ctrl-B"],
    "os": {
      "mac": {
        "keys": ["Cmd-B"]
      }
    }
  },

  "close_goto": {
    "keys": ["Esc"]
  },

  "close_find": {
    "keys": ["Esc"]
  },

  "duplicate_line": {
    "keys": ["Shift-Ctrl-D"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-D"]
      }
    }
  },

  "goto_line": {
    "keys": ["Ctrl-G"],
    "os": {
      "mac": {
        "keys": ["Cmd-G"]
      }
    }
  },

  "open_colorpicker": {
    "keys": ["Ctrl-Alt-K"],
    "os": {
      "mac": {
        "keys": ["Cmd-Alt-K"]
      }
    }
  },

  "open_goto": {
    "keys": ["Ctrl-P"],
    "os": {
      "mac": {
        "keys": ["Cmd-P"]
      }
    }
  },

  "open_goto_commands": {
    "keys": ["Ctrl-Shift-P"],
    "os": {
      "mac": {
        "keys": ["Cmd-Shift-P"]
      }
    }
  },

  "open_find": {
    "keys": ["Ctrl-F"],
    "os": {
      "mac": {
        "keys": ["Cmd-F"]
      }
    }
  },

  "open_replace": {
    "keys": ["Ctrl-R"],
    "os": {
      "mac": {
        "keys": ["Cmd-R"]
      }
    }
  },

  "font_size_decrease": {
    "keys": ["Shift-Ctrl-Alt-Down"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-Alt-Down"]
      }
    }
  },

  "font_size_increase": {
    "keys": ["Shift-Ctrl-Alt-Up"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-Alt-Up"]
      }
    }
  },

  "layout_single": {
    "keys": ["Alt-Shift-1"],
    "os": {
      "mac": {
        "keys": ["Alt-Cmd-1"]
      }
    }
  },

  "layout_columns_2": {
    "keys": ["Alt-Shift-2"],
    "os": {
      "mac": {
        "keys": ["Alt-Cmd-2"]
      }
    }
  },

  "layout_columns_3": {
    "keys": ["Alt-Shift-3"],
    "os": {
      "mac": {
        "keys": ["Alt-Cmd-3"]
      }
    }
  },

  "layout_columns_4": {
    "keys": ["Alt-Shift-4"],
    "os": {
      "mac": {
        "keys": ["Alt-Cmd-4"]
      }
    }
  },

  "layout_rows_2": {
    "keys": ["Alt-Shift-8"],
    "os": {
      "mac": {
        "keys": ["Alt-Shift-Cmd-2"]
      }
    }
  },

  "layout_rows_3": {
    "keys": ["Alt-Shift-9"],
    "os": {
      "mac": {
        "keys": ["Alt-Shift-Cmd-3"]
      }
    }
  },

  "layout_grid": {
    "keys": ["Alt-Shift-5"],
    "os": {
      "mac": {
        "keys": ["Alt-Cmd-5"]
      }
    }
  },

  "new_file": {
    "keys": ["Alt-N"],
    "os": {
      "mac": {
        "keys": ["Ctrl-N"]
      }
    }
  },

  "redo": {
    "keys": ["Ctrl-Y", "Ctrl-Shift-Z"],
    "os": {
      "mac": {
        "keys": ["Cmd-Y", "Cmd-Shift-Z"]
      }
    }
  },

  "save": {
    "keys": ["Ctrl-S"],
    "os": {
      "mac": {
        "keys": ["Cmd-S"]
      }
    }
  },

  "save_as": {
    "keys": ["Ctrl-Shift-S"],
    "os": {
      "mac": {
        "keys": ["Cmd-Shift-S"]
      }
    }
  },

  "save_all": {
    "keys": ["Ctrl-Alt-S"],
    "os": {
      "mac": {
        "keys": ["Cmd-Alt-S"]
      }
    }
  },


  "swap_line_down": {
    "keys": ["Ctrl-Down"],
    "os": {
      "mac": {
        "keys": ["Cmd-Ctrl-Down"]
      }
    }
  },

  "swap_line_up": {
    "keys": ["Ctrl-Up"],
    "os": {
      "mac": {
        "keys": ["Cmd-Ctrl-Up"]
      }
    }
  },

  "toggle_file_explorer": { 
    "keys": ["Alt-X"]  
  },

  "undo": {
    "keys": ["Ctrl-Z"],
    "os": {
      "mac": {
        "keys": ["Cmd-Z"]
      }
    }
  },

  "clear_bookmarks": {
    "keys": ["Shift-Ctrl-F2"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-F2"]
      }
    }
  },

  "indent": {
    "keys": ["Tab"]
  },

  "del_char_after": {
    "keys": ["Delete"],
    "os": {
      "mac": {
        "keys": ["Delete", "Ctrl-D"]
      }
    }
  },

  "del_char_before": {
    "keys": ["Backspace", "Shift-Backspace"],
    "os": {
      "mac": {
        "keys": ["Backspace", "Shift-Backspace", "Ctrl-H"]
      }
    }
  },

  "del_group_after": {
    "keys": ["Ctrl-Delete"],
    "os": {
      "mac": {
        "keys": ["Alt-Delete", "Ctrl-Alt-Backspace"]
      }
    }
  },

  "del_group_before": {
    "keys": ["Ctrl-Backspace"],
    "os": {
      "mac": {
        "keys": ["Alt-Backspace"]
      }
    }
  },

  "del_line_left": {
    "keys": ["Ctrl-K Ctrl-Backspace"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-Backspace"]
      }
    }
  },

  "del_line_right": {
    "keys": ["Ctrl-K Ctrl-K"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-K"]
      }
    }
  },

  "del_word_after": {
    "keys": ["Alt-D"],
    "os": "mac"
  },

  "del_word_before": {
    "keys": ["Alt-Backspace"],
    "os": "mac"
  },

  "del_wrapped_line_left": {
    "keys": ["Cmd-Backspace"],
    "os": "mac"
  },

  "del_wrapped_line_right": {
    "keys": ["Cmd-Delete"],
    "os": "mac"
  },

  "delete_line": {
    "keys": ["Shift-Ctrl-K"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-K"]
      }
    }
  },

  "delete_to_sublime_mark": {
    "keys": ["Ctrl-K Ctrl-W"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-W"]
      }
    }
  },

  "downcase_at_cursor": {
    "keys": ["Ctrl-K Ctrl-L"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-L"]
      }
    }
  },

  "emmet_expand_abbreviation": {
    "keys": ["Ctrl-E"],
    "os": {
      "mac": {
        "keys": ["Cmd-E"]
      }
    }
  },

  "find_all_under": {
    "keys": ["Alt-F3"]
  },

  "find_incremental": {
    "keys": ["Ctrl-I"],
    "os": {
      "mac": {
        "keys": ["Cmd-I"]
      }
    }
  },

  "find_incremental_reverse": {
    "keys": ["Shift-Ctrl-I"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-I"]
      }
    }
  },

  "find_next": {
    "keys": ["F3"],
    "os": {
      "mac": {
        "keys": ["F3"]
      }
    }
  },

  "find_prev": {
    "keys": ["Shift-F3"],
    "os": {
      "mac": {
        "keys": ["Shift-F3"]
      }
    }
  },

  "find_under": {
    "keys": ["Ctrl-F3"],
    "os": {
      "mac": {
        "keys": ["Cmd-F3"]
      }
    }
  },

  "find_under_previous": {
    "keys": ["Shift-Ctrl-F3"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-F3"]
      }
    }
  },

  "fold": {
    "keys": ["Alt-Up"]
  },

  "fold_all": {
    "keys": ["Alt-Shift-Up"]
  },

  "go_char_left": {
    "keys": ["Left"],
    "os": {
      "mac": {
        "keys": ["Left", "Ctrl-B"]
      }
    }
  },

  "go_char_right": {
    "keys": ["Right"],
    "os": {
      "mac": {
        "keys": ["Right", "Ctrl-F"]
      }
    }
  },

  "go_doc_end": {
    "keys": ["Ctrl-End"],
    "os": {
      "mac": {
        "keys": ["Cmd-Down", "Cmd-End", "Ctrl-Down"]
      }
    }
  },

  "go_doc_start": {
    "keys": ["Ctrl-Home"],
    "os": {
      "mac": {
        "keys": ["Cmd-Home", "Cmd-Up", "Ctrl-Up"]
      }
    }
  },

  "go_group_left": {
    "keys": ["Ctrl-Left"],
    "os": {
      "mac": {
        "keys": ["Alt-Left"]
      }
    }
  },

  "go_group_right": {
    "keys": ["Ctrl-Right"],
    "os": {
      "mac": {
        "keys": ["Alt-Right"]
      }
    }
  },

  "go_line_end": {
    "keys": ["Alt-Right"],
    "os": {
      "mac": {
        "keys": ["Alt-Right", "Ctrl-E"]
      }
    }
  },

  "go_line_left": {
    "keys": ["Ctrl-Left"],
    "os": {
      "mac": {
        "keys": ["Cmd-Left"]
      }
    }
  },

  "go_line_right": {
    "keys": ["Ctrl-Right"],
    "os": {
      "mac": {
        "keys": ["Cmd-Right"]
      }
    }
  },

  "go_line_start": {
    "keys": ["Alt-Left"],
    "os": {
      "mac": {
        "keys": ["Alt-Left", "Ctrl-A"]
      }
    }
  },

  "go_line_start_smart": {
    "keys": ["Home"]
  },

  "go_page_down": {
    "keys": ["PageDown"],
    "os": {
      "mac": {
        "keys": ["PageDown", "Ctrl-V"]
      }
    }
  },

  "go_page_up": {
    "keys": ["PageUp"],
    "os": {
      "mac": {
        "keys": ["PageUp", "Shift-Ctrl-V"]
      }
    }
  },

  "go_subword_left": {
    "keys": ["Alt-Left"]
  },

  "go_subword_right": {
    "keys": ["Alt-Right"]
  },

  "go_to_bracket": {
    "keys": ["Ctrl-M"],
    "os": {
      "mac": {
        "keys": ["Cmd-M"]
      }
    }
  },

  "go_word_left": {
    "keys": ["Alt-B"],
    "os": "mac"
  },

  "go_word_right": {
    "keys": ["Alt-F"],
    "os": "mac"
  },

  "unindent": {
    "keys": ["Shift-Tab"],
    "os": {
      "mac": {
        "keys": ["Shift-Tab"]
      }
    }
  },

  "insert_line_after": {
    "keys": ["Ctrl-Enter"],
    "os": {
      "mac": {
        "keys": ["Cmd-Enter"]
      }
    }
  },

  "insert_line_before": {
    "keys": ["Shift-Ctrl-Enter"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-Enter"]
      }
    }
  },

  "join_lines": {
    "keys": ["Ctrl-J"],
    "os": {
      "mac": {
        "keys": ["Cmd-J"]
      }
    }
  },

  "new_line_and_indent": {
    "keys": ["Enter"]
  },

  "next_bookmark": {
    "keys": ["F2"],
    "os": {
      "mac": {
        "keys": ["F2"]
      }
    }
  },

  "prev_bookmark": {
    "keys": ["Shift-F2"],
    "os": {
      "mac": {
        "keys": ["Shift-F2"]
      }
    }
  },

  "redo_selection": {
    "keys": ["Alt-U"],
    "os": {
      "mac": {
        "keys": ["Shift-Ctrl-U", "Shift-Cmd-U"]
      }
    }
  },

  "scroll_line_down": {
    "keys": ["Ctrl-Shift-Down"],
    "os": {
      "mac": {
        "keys": ["Cmd-Down"]
      }
    }
  },

  "scroll_line_up": {
    "keys": ["Ctrl-Shift-Up"],
    "os": {
      "mac": {
        "keys": ["Cmd-Up"]
      }
    }
  },

  "select_all": {
    "keys": ["Ctrl-A"],
    "os": {
      "mac": {
        "keys": ["Cmd-A"]
      }
    }
  },

  "select_between_brackets": {
    "keys": ["Shift-Ctrl-M"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-M"]
      }
    }
  },

  "select_bookmarks": {
    "keys": ["Alt-F2"]
  },

  "select_line": {
    "keys": ["Ctrl-L"],
    "os": {
      "mac": {
        "keys": ["Cmd-L"]
      }
    }
  },

  "select_lines_downward": {
    "keys": ["Shift-Alt-Down"],
    "os": {
      "mac": {
        "keys": ["Shift-Alt-Down"]
      }
    }
  },

  "select_lines_upward": {
    "keys": ["Shift-Alt-Up"],
    "os": {
      "mac": {
        "keys": ["Shift-Alt-Up"]
      }
    }
  },

  "select_next_occurrence": {
    "keys": ["Ctrl-D"],
    "os": {
      "mac": {
        "keys": ["Cmd-D"]
      }
    }
  },

  "select_scope": {
    "keys": ["Shift-Ctrl-Space"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-Space"]
      }
    }
  },

  "select_to_sublime_mark": {
    "keys": ["Ctrl-K Ctrl-A"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-A"]
      }
    }
  },

  "set_sublime_mark": {
    "keys": ["Ctrl-K Ctrl-Space"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-Space"]
      }
    }
  },

  "show_in_center": {
    "keys": ["Ctrl-K Ctrl-C"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-C"]
      }
    }
  },

  "show_completions": {
    "keys": ["Ctrl-Space"]
  },

  "select_next_tab": {
    "keys": ["Shift-Ctrl-Alt-Right"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-Alt-Right"]
      }
    }
  },

  "select_previous_tab": {
    "keys": ["Shift-Ctrl-Alt-Left"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-Alt-Left"]
      }
    }
  },

  "single_selection": {
    "keys": ["Esc"]
  },

  "single_selection_top": {
    "keys": ["Esc"],
    "os": {
      "mac": {
        "keys": ["Esc"]
      }
    }
  },

  "sort_lines": {
    "keys": ["F9"],
    "os": {
      "mac": {
        "keys": ["F9"]
      }
    }
  },

  "sort_lines_insensitive": {
    "keys": ["Ctrl-F9"],
    "os": {
      "mac": {
        "keys": ["Cmd-F9"]
      }
    }
  },

  "split_selection_by_line": {
    "keys": ["Shift-Ctrl-L"],
    "os": {
      "mac": {
        "keys": ["Shift-Cmd-L"]
      }
    }
  },

  "sublime_yank": {
    "keys": ["Ctrl-K Ctrl-Y"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-Y"]
      }
    }
  },

  "swap_with_sublime_mark": {
    "keys": ["Ctrl-K Ctrl-X"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-X"]
      }
    }
  },

  "toggle_bookmark": {
    "keys": ["Ctrl-F2"],
    "os": {
      "mac": {
        "keys": ["Cmd-F2"]
      }
    }
  },

  "toggle_comment": {
    "keys": ["Ctrl-/"],
    "os": {
      "mac": {
        "keys": ["Cmd-/"]
      }
    }
  },

  "toggle_overwrite": {
    "keys": ["Insert"]
  },

  "transpose_chars": {
    "keys": ["Ctrl-T"],
    "os": {
      "mac": {
        "keys": ["Cmd-T"]
      }
    }
  },

  "undo_selection": {
    "keys": ["Ctrl-U"],
    "os": {
      "mac": {
        "keys": ["Cmd-U"]
      }
    }
  },

  "unfold": {
    "keys": ["Alt-Down"]
  },

  "unfold_all": {
    "keys": ["Alt-Shift-Down"]
  },

  "upcase_at_cursor": {
    "keys": ["Ctrl-K Ctrl-U"],
    "os": {
      "mac": {
        "keys": ["Cmd-K Cmd-U"]
      }
    }
  },

  "wrap_lines": {
    "keys": ["Alt-Q"]
  }
}
```