---
current_menu: snippets
---

# Snippets

Snippets are smart templates that will insert text for you and adapt it to their context. They allow you to generate commonly used code syntax from a shortcut as soon as possible. This way, you can quickly re-use any code! 

### Creating Snippets

Using GUI Preferences, you can remove existing snippets or add a new one using option menu and when you are done, just choose "Save" option.

![goto](images/snippets.png "snippets")

You can define your snippets for specific languages in User or Project Preferences in a JSON format as well. 

Here is an example for "For Loop" snippet for JavaScript:

```
   "For Loop": {
    "prefix": "for",
    "body": [
      "for (var ${1:index} = 0; ${1:index} < ${2:array}.length; ${1:index}++) {",
      "\tvar ${3:element} = ${2:array}[${1:index}];",
      "\t$4",
      "}"
    ],
    "scope": {
      "mode": ["JavaScript"]
    },
    "description": "For Loop snippet"
  },
```

In the example above:

  - *For Loop* is the snippet name
  - *prefix* defines a prefix used for listing a Snippet. In this example, just enter the Tab key after typing "for" and you'll see your Snippet content.
  - *body* is the Snippet content.
  - *scope* containes *mode* of your Snippet. In this case it is JavaScript mode.
  - *description* explains data in a Snippet.
  

You can use $id and ${id:label} for variables since variables with the same name are connected. 
Since the syntax is like this: ${id:label}, each acts as a default value for a tab stop. With the help of field markers, you can cycle through positions within the snippet by pressing the Tab key.


Identical field markers mirror each other: when you edit the first one, the rest will be populated with the same value in real time.
By expanding the field syntax a little bit, you can define default values for a field. Placeholders are useful when there’s a general case for your snippet but you still want to keep its customization convenient.

In order to edit Snippet file go to Preferences -> User/Project -> Snippets

For example, in order to change For Loop defined in Default Preferences, go to Preferences -> User/Project -> Snippets and type:

```
   "For Loop": {
    "prefix": "for",
    "body": [
      "for (var ${2:index} = 0; ${2:index} < ${1:array}.length; ${2:index}++) {",
      "\tvar ${3:element} = ${1:array}[${2:index}];",
      "\t$4",
      "}"
    ],
    "scope": {
      "mode": ["JavaScript"]
    },
    "description": "For Loop snippet"
  },
```

This will change your For Loop for javascript to start defining array and then index.

All Default Snippets Preferences:
```
{
  "Anonymous function": {
    "prefix": "fn",
    "body": [
      "function() {",
      "\t$1",
      "}"
    ],
    "scope": {
      "mode": ["JavaScript"]
    },
    "description": "Anonymous function snippet"
  },
  
  "console.log": {
    "prefix": "log",
    "body": [
      "console.log($1)$2"
    ],
    "scope": {
      "mode": ["JavaScript"]
    },
    "description": "console.log snippet"
  },
  
  "For Loop": {
    "prefix": "for",
    "body": [
      "for (var ${1:index} = 0; ${1:index} < ${2:array}.length; ${1:index}++) {",
      "\tvar ${3:element} = ${2:array}[${1:index}];",
      "\t$4",
      "}"
    ],
    "scope": {
      "mode": ["JavaScript"]
    },
    "description": "For Loop snippet"
  },
  
  "if/else": {
    "prefix": "ife",
    "body": [
      "if ($1) {",
      "\t$2",
      "} else {",
      "\t$3",
      "}"
    ],
    "scope": {
      "mode": ["JavaScript"]
    },
    "description": "if/else condition snippet"
  },
  
  "While Loop": {
    "prefix": "while",
    "body": [
      "while (${1:expression}) {",
      "\t$2",
      "}"
    ],
    "scope": {
      "mode": ["JavaScript"]
    },
    "description": "While Loop snippet"
  }
}
```