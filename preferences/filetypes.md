---
current_menu: filetypes
---

# FileTypes

For syntax highlighting and language support, Codeanywhere uses [Codemirror](https://codemirror.net/). CodeMirror supports over two dozen different modules, and any changes made to CodeMirror are reflected back into Codeanywhere.
By default, files are highlighted based on their file extension. You can still add new extensions in User or Project preferences and override the ones from General preferences 

Using GUI Preferences, you can change existing filetype exentions or add a new one using option menu and when you are done, just choose "Save" option.

![goto](images/filetypes.png "filetypes")


If you are defining preferences using JSON you must follow the Default FileTypes Preferences syntax which you can see at the bottom of this section.

For example, if you wish to add new extension for HTML mode, you'll see it is set to: 
```
"HTML": { 
  "extension": ["html", "htm"]
}
```
And now you can add CTP extension inside Preferences -> User/Project -> File Types, by adding code:
```
"HTML": { 
  "extension": ["html", "htm", "CTP"]
}
```
And by doing this, you'll override settings from Default.

All Default FileTypes Preferences:
```
{
  "APL": {
    "extension": ["dyalog", "apl"]
  },
  "PGP": {
    "extension": ["pgp"]
  },
  "ASN.1": {
    "extension": ["asn", "asn1"]
  },
  "Asterisk": {
    "extension": []
  },
  "Brainfuck": {
    "extension": ["b", "bf"]
  },
  "C": {
    "extension": ["c", "h"]
  },
  "C++": {
    "extension": ["cpp", "c++", "cc", "cxx", "hpp", "h++", "hh", "hxx"]
  },
  "Cobol": {
    "extension": ["cob", "cpy"]
  },
  "C#": {
    "extension": ["cs"]
  },
  "Clojure": {
    "extension": ["clj"]
  },
  "CMake": {
    "extension": ["cmake", "cmake.in"]
  },
  "CoffeeScript": {
    "extension": ["coffee"]
  },
  "Common Lisp": {
    "extension": ["cl", "lisp", "el"]
  },
  "Cypher": {
    "extension": ["cyp", "cypher"]
  },
  "Cython": {
    "extension": ["pyx", "pxd", "pxi"]
  },
  "CSS": {
    "extension": ["css"]
  },
  "CQL": {
    "extension": ["cql"]
  },
  "D": {
    "extension": ["d"]
  },
  "Dart": {
    "extension": ["dart"]
  },
  "diff": {
    "extension": ["diff", "patch"]
  },
  "Django": {
    "extension": []
  },
  "Dockerfile": {
    "extension": []
  },
  "DTD": {
    "extension": ["dtd"]
  },
  "Dylan": {
    "extension": ["dylan", "dyl", "intr"]
  },
  "EBNF": {
    "extension": []
  },
  "ECL": {
    "extension": ["ecl"]
  },
  "Eiffel": {
    "extension": ["e"]
  },
  "Elm": {
    "extension": ["elm"]
  },
  "Embedded Javascript": {
    "extension": ["ejs"]
  },
  "Embedded Ruby": {
    "extension": ["erb"]
  },
  "Erlang": {
    "extension": ["erl"]
  },
  "Factor": {
    "extension": ["factor"]
  },
  "Forth": {
    "extension": ["forth", "fth", "4th"]
  },
  "Fortran": {
    "extension": ["f", "for", "f77", "f90"]
  },
  "F#": {
    "extension": ["fs"]
  },
  "Gas": {
    "extension": ["s"]
  },
  "Gherkin": {
    "extension": ["feature"]
  },
  "GitHub Flavored Markdown": {
    "extension": []
  },
  "Go": {
    "extension": ["go"]
  },
  "Groovy": {
    "extension": ["groovy"]
  },
  "HAML": {
    "extension": ["haml"]
  },
  "Haskell": {
    "extension": ["hs"]
  },
  "Haxe": {
    "extension": ["hx"]
  },
  "HXML": {
    "extension": ["hxml"]
  },
  "ASP.NET": {
    "extension": ["aspx"]
  },
  "HTML": {
    "extension": ["html", "htm"]
  },
  "HTTP": {
    "extension": []
  },
  "IDL": {
    "extension": ["pro"]
  },
  "Jade": {
    "extension": ["jade"]
  },
  "Java": {
    "extension": ["java"]
  },
  "Java Server Pages": {
    "extension": ["jsp"]
  },
  "JavaScript": {
    "extension": ["js"]
  },
  "JSON": {
    "extension": ["json", "map"]
  },
  "JSON-LD": {
    "extension": ["jsonld"]
  },
  "Jinja2": {
    "extension": []
  },
  "Julia": {
    "extension": ["jl"]
  },
  "Kotlin": {
    "extension": ["kt"]
  },
  "LESS": {
    "extension": ["less"]
  },
  "LiveScript": {
    "extension": ["ls"]
  },
  "Lua": {
    "extension": ["lua"]
  },
  "Markdown": {
    "extension": ["markdown", "md", "mkd"]
  },
  "mIRC": {
    "extension": []
  },
  "MariaDB SQL": {
    "extension": []
  },
  "Mathematica": {
    "extension": ["m", "nb"]
  },
  "Modelica": {
    "extension": ["mo"]
  },
  "MUMPS": {
    "extension": []
  },
  "MS SQL": {
    "extension": []
  },
  "MySQL": {
    "extension": []
  },
  "Nginx": {
    "extension": []
  },
  "NTriples": {
    "extension": ["nt"]
  },
  "Objective C": {
    "extension": ["m", "mm"]
  },
  "OCaml": {
    "extension": ["ml", "mli", "mll", "mly"]
  },
  "Octave": {
    "extension": ["m"]
  },
  "Pascal": {
    "extension": ["p", "pas"]
  },
  "PEG.js": {
    "extension": ["jsonld"]
  },
  "Perl": {
    "extension": ["pl", "pm"]
  },
  "PHP": {
    "extension": ["php", "php3", "php4", "php5", "phtml", "ctp"]
  },
  "Pig": {
    "extension": ["pig"]
  },
  "Plain Text": {
    "extension": ["txt", "text", "conf", "def", "list", "log"]
  },
  "PLSQL": {
    "extension": ["pls"]
  },
  "Properties files": {
    "extension": ["properties", "ini", "in"]
  },
  "Python": {
    "extension": ["py", "pyw"]
  },
  "Puppet": {
    "extension": ["pp"]
  },
  "Q": {
    "extension": ["q"]
  },
  "R": {
    "extension": ["r"]
  },
  "reStructuredText": {
    "extension": ["rst"]
  },
  "RPM Changes": {
    "extension": []
  },
  "RPM Spec": {
    "extension": ["spec"]
  },
  "Ruby": {
    "extension": ["rb"]
  },
  "Rust": {
    "extension": ["rs"]
  },
  "Sass": {
    "extension": ["sass"]
  },
  "Scala": {
    "extension": ["scala"]
  },
  "Scheme": {
    "extension": ["scm", "ss"]
  },
  "SCSS": {
    "extension": ["scss"]
  },
  "Shell": {
    "extension": ["sh", "ksh", "bash"]
  },
  "Sieve": {
    "extension": ["siv", "sieve"]
  },
  "Slim": {
    "extension": ["slim"]
  },
  "Smalltalk": {
    "extension": ["st"]
  },
  "Smarty": {
    "extension": ["tpl"]
  },
  "Solr": {
    "extension": []
  },
  "Soy": {
    "extension": ["soy"]
  },
  "SPARQL": {
    "extension": ["rq", "sparql"]
  },
  "Spreadsheet": {
    "extension": []
  },
  "SQL": {
    "extension": ["sql"]
  },
  "Swift": {
    "extension": ["swift"]
  },
  "MariaDB": {
    "extension": []
  },
  "sTeX": {
    "extension": []
  },
  "LaTeX": {
    "extension": ["text", "ltx"]
  },
  "SystemVerilog": {
    "extension": ["v"]
  },
  "Tcl": {
    "extension": ["tcl"]
  },
  "Textile": {
    "extension": ["textile"]
  },
  "TiddlyWiki ": {
    "extension": []
  },
  "Tiki wiki": {
    "extension": []
  },
  "TOML": {
    "extension": ["toml"]
  },
  "Tornado": {
    "extension": []
  },
  "troff": {
    "extension": []
  },
  "TTCN": {
    "extension": ["ttcn", "ttcn3", "ttcnpp"]
  },
  "TTCN_CFG": {
    "extension": ["cfg"]
  },
  "Turtle": {
    "extension": ["ttl"]
  },
  "TypeScript": {
    "extension": ["ts"]
  },
  "Twig": {
    "extension": []
  },
  "VB.NET": {
    "extension": ["vb"]
  },
  "VBScript": {
    "extension": ["vbs"]
  },
  "Velocity": {
    "extension": ["vtl"]
  },
  "Verilog": {
    "extension": ["v"]
  },
  "XML": {
    "extension": ["xml", "xsl", "xsd"]
  },
  "XQuery": {
    "extension": ["xy", "xquery"]
  },
  "YAML": {
    "extension": ["yaml", "yml"]
  },
  "Z80": {
    "extension": ["z80"]
  }
}
```
