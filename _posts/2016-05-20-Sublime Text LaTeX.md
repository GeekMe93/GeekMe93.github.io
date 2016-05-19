---
layout: post
title: Taming your Sublime Text 3 for LaTeXing
categories: [tutorial]
tags: [Sublime Text, LaTeX, tutorial]
---

Although it is 3:00 AM Singapore time, I still decide to write something because I just lost my sleep. After finishing the workflow article, I want to give more detail about how I integrate Sublime Text 3  and MacTeX as my favorite documentation system.

Sublime Text 3 is a beast for writing LaTeX code. It provide me customized function for building my work. Some awesome features I frequently used are listed as:

> 1. Some great packages via package control;
> 2. Key-binding features;
> 3. Customized LaTeX snippets;

### Fantastic packages for LaTeXing

Here I make a list of packages with short discretions to make your typing easy:

- [Packages control](https://packagecontrol.io/installation): this is the first package you must have.
- [LaTeXtools](https://github.com/SublimeText/LaTeXTools): your best friend for LaTeX in Sublime Text.
- [LaTeX-cwl](https://github.com/LaTeXing/LaTeX-cwl): for the autocompletion of LaTeX commands.
- [LaTeXTab](CSV/Excel to LaTeX Table): greater helper for CSV/Excel to LaTeX Table

Technically speaking, with these for packages, I will get a quick workflow on write your own documents. Actually, I always use some academic tables in your notes or reports. I modified LaTeXTab packages a little bit for better indentation and academic use.

### Key-binding to boost your productivity

I will use one example to illustrate how key-binding can be useful. One scenario for users is that I use subscripts and superscripts a lot. Every time in the math mode, I want a auto-completion function of `{}` when typing `_` or `^`. Then I use the following code to build the key-binding:

```
[
    { "keys": ["_"], "command": "insert_snippet", "args": {"contents": "_{$1}$0"},                          
    "context":  
        [
            { "key": "selector", "operator": "equal", "operand": "text.tex.latex string.other.math"},
            { "key": "setting.auto_match_enabled", "operator": "equal", "operand": true },
            { "key": "selection_empty", "operator": "equal", "operand": true, "match_all": true }
        ]
    }
]
```

From: <a>http://tex.stackexchange.com/questions/140169/sublime-text-snippets-just-for-latex/140222#140222</a>

### LaTeX snippets: this is super good

Accumulated snippets for you code according to your personal habits will become a great treasure for you. The more snippets you write, the faster for you to write. My snippets will be divided into:

> 1. Element snippets: a collection of complex formulas functions; 
> 2. Structure snippets: comments, customized figure and table, templates snippets;
> 3. Auxiliary snippets: helping sheet snippet when forgetting something syntax and notation;

There are a lot of features I still need time add expand my list in this article. 