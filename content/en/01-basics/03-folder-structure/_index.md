+++
title = "Folder structure"
weight = 010300
chapter = false
pre = "<b>c. </b>"
disableToc = false
+++

The following is a high-level overview of each of the directories:

### Dir \<archetypes\>

You can create new content files in Hugo using the `hugo new` command. By default, Hugo will create new content files with at least `date`, `title` (inferred from the file name), and `draft = true`. This saves time and promotes consistency for sites using multiple content types. You can create your own [archetypes](https://gohugo.io/content-management/archetypes/) with custom preconfigured front matter fields as well.

### Dir \<config\>

Hugo ships with a large number of [configuration directives](https://gohugo.io/getting-started/configuration/#all-variables-yaml). The config directory is where those directives are stored as JSON, YAML, or TOML files. Every root setting object can stand as its own file and structured by environments. Projects with minimal settings and no need for environment awareness can use a single `config.toml` file at its root.

### Dir \<content\>

All content for your website will live inside this directory. Each top-level folder in Hugo is considered a [content section](https://gohugo.io/content-management/sections/). For example, if your site has three main sections — `blog`, `articles`, and `tutorials` — you will have three directories at `content/blog`, `content/articles`, and `content/tutorials`. Hugo uses sections to assign default [content types](https://gohugo.io/content-management/types/).

### Dir \<data\>

This directory is used to store configuration files that can be used by Hugo when generating your website. You can write these files in YAML, JSON, or TOML format. In addition to the files you add to this folder, you can also create [data templates](https://gohugo.io/templates/data-templates/) that pull from dynamic content.

### Dir \<i18n\>

Hugo uses [go-i18n](https://github.com/nicksnyder/go-i18n) to support string translations.

Translations are collected from the `themes/<THEME>/i18n/` folder (built into the theme), as well as translations present in `i18n/` at the root of your project. In the `i18n`, the translations will be merged and take precedence over what is in the theme folder. Language files should be named according to [RFC 5646](https://tools.ietf.org/html/rfc5646) with names such as `en-US.toml`, `fr.toml`, etc.

### Dir \<layouts\>

Stores templates in the form of `.html` files that specify how views of your content will be rendered into a static website. Templates include [list pages](https://gohugo.io/templates/list/), your [homepage](https://gohugo.io/templates/homepage/), [taxonomy templates](https://gohugo.io/templates/taxonomy-templates/), [partials](https://gohugo.io/templates/partials/), [single page templates](https://gohugo.io/templates/single-page-templates/), and more.

### Dir \<static\>

Stores all the static content: images, CSS, JavaScript, etc. When Hugo builds your site, all assets inside your static directory are copied over as-is.

### Dir \<themes\>

If you decide to use a theme with your website, all of the files for the theme will go in here. Generally, unless you know what you’re doing, you don’t wanna mess with the files in this folder.
