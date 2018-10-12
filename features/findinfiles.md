---
current_menu: findinfiles
---

# Find in Files

Find in files is a quick way to see if a certain string or pattern appears across many files. 

This feature works for containers and SSH connections.

To initiate Find in Files, go to the Find menu, then Find in Files or use the keyboard shortcut (Cmd/Ctrl + Shift + F).

![fif](images/fif.png "findinfiles")

Find in Files can also be initiated using File Explorer by opening context menu for a directory:

![fifcontext](images/fifcontext.png "findinfiles context menu")

When this is done, a find bar will show up:

![fifbar](images/fifbar.png "findinfiles bar")


## Find
To start a search, type the search term or string into the "Find" text box and click Find or press Enter. A window will open below the find panel that will show all occurrences of the search terms. To go to the file where the search term occurs, simply click the search result text.

## Path
If you want to narrow down your search, you can specify a path to a directory you are interested in.

## Exclude
Exclude field can be used for skiping any file with a name suffix that matches the pattern [_glob_](https://en.wikipedia.org/wiki/Glob_(programming)), using wildcard matching.

## Search Modifiers
Regular Expressions - Turning this on allows for use of regular expressions which are complex but can help match very specific patterns of strings

Match Case - If the search will be case sensitive or not