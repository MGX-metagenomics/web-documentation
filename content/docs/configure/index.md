---
title: 'Configuration'
date: .Date
draft: false
weight: 100
summary: Syntax highlighting and menus can be configured via `config.toml`.
---

## Syntax Highlighting

Whisper uses the in-built code highlighting that ships with hugo. https://gohugo.io/content-management/syntax-highlighting/

You can insert code snippets in any markdown file by using standard code fences syntax ie:

````
```
insert code here
```
````

You can specify the langauge by adding a declaration after the backticks

````
```javascript
insert code here
```
````

### Pygments Options

The following code highlighting options are configured in the `config.toml`

```toml
pygmentsCodeFences = true
pygmentsCodefencesGuessSyntax = true
pygmentsUseClasses = true
```

## Main menu

Configure the main menu by editing the `config.toml`

```toml
[[menu.main]]
name = "Home"
url = "/"
weight = 1

[[menu.main]]
name = "Docs"
url = "/docs/"
weight = 2
```
