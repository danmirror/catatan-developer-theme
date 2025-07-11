## Catatan Developer Themes
> themes ini hanya boleh di gunakan oleh developer dari catatan developer.

## instalation
- create site baru jika belum ada
```
$ hugo new site catatan-developer
```
- gunakan submodule untuk theme atau extract manual dan taruh di dalam folder themes
```
$ git submodule add https://github.com/danmirror/catatan-developer-theme.git themes/catatan-developer-theme
```
- copy paste code ini ke hugo.toml

```
baseURL = "https://catatandeveloper.id/"
languageCode = 'en-us'
title = 'Catatan Developer'
theme = "catatan-developer-theme"

[params]
    logo = "images/logo_144.png"

[pagination]
    disableAliases = false
    pagerSize = 6
    path = 'page'

[markup]
    [markup.highlight]
        codeFences = true
        guessSyntax = true
        hl_Lines = ""
        lineNos = false
        noClasses = true
        style = "base16-snazzy"
    
    unsafe = true
[outputs]
home = ["HTML", "JSON"]
```

## run code
```
$ hugo serve --minify
```



## tree
```
├── archetypes/
│   └── default.md
├── content/
│   ├── about/_index.md
│   ├── author/danuandrean/_index.md
│   ├── issue/development-issue/_index.md
│   ├── tutorial/development/_index.md
│   ├── tutorial_cpp_1.md
│   └── tutorial_cpp_2.md
├── static/images/
│   ├── arduino/
│   ├── cpp/
│   └── logo.png
├── themes/
│   └── catatan-developer-theme/
├── hugo.toml

```


