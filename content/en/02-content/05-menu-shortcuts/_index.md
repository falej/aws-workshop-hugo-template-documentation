+++
title = "Menu shortcuts"
weight = 020500
chapter = false
pre = "<b>e. </b>"
disableToc = false
+++

You can define additional menu entries or shortcuts in the navigation menu without any link to content.

## Basic configuration

In `config/_default/` directory add a `menus.toml` file and add a `[[shortcuts]]` entry for each link your want to add.

Example from the current website:

```toml
[[shortcuts]]
name = "<i class='fas fa-bookmark'></i> Hugo Documentation"
identifier = "hugodoc"
url = "https://gohugo.io"
weight = 100100

[[shortcuts]]
name = "<i class='fas fa-bookmark'></i> Theme Learn Documentation"
url = "https://learn.netlify.app"
weight = 100200
```

## Configuration for Multilingual mode

When using a multilingual website, you can set different menus for each language. In `config/_default/` directory add a `menus.<id-language>.toml` for each language setup in your project.

For example, if you want to support English (en) and Spanish (es), you will have to have two menu files:

```toml
# config/_default/menus.en.toml
[[shortcuts]]
name = "<i class='fas fa-bookmark'></i> Hugo Documentation"
identifier = "hugodoc"
url = "https://gohugo.io"
weight = 100100

[[shortcuts]]
name = "<i class='fas fa-bookmark'></i> Theme Learn Documentation"
url = "https://learn.netlify.app"
weight = 100200
```

```toml
# config/_default/menus.es.toml
[[shortcuts]]
name = "<i class='fas fa-bookmark'></i> Hugo Documentación"
identifier = "hugodoc"
url = "https://gohugo.io"
weight = 100100

[[shortcuts]]
name = "<i class='fas fa-bookmark'></i> Theme Learn Documentación"
url = "https://learn.netlify.app"
weight = 100200
```

Read more about [hugo menu](https://gohugo.io/extras/menus/) and [hugo multilingual menus](https://gohugo.io/content-management/multilingual/#menus)
