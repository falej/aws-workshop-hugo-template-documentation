+++
title = "Multilingual and i18n"
weight = 010500
chapter = false
pre = "<b>e. </b>"
disableToc = false
+++

The template is fully compatible with [Hugo multilingual mode](https://gohugo.io/content-management/multilingual/)

It provides:

- Translation strings for default values
- Automatic menu generation from multilingual content
- In-browser language switching

### Basic configuration

All configuration regarding languages is defined in `config/_default/languages.toml` file. By default, the template is configured to support **English** language only. The following is the default configuration you will find in the file:

```toml
[en]
languageName = "English"
contentDir = "content/en"
title = "AWS Workshop"
weight = 1
```

The `contentDir` parameter, helps you to define the location where all your content in that specific language will be.

For example, if you want to configure **English** and **Spanish** languages, the configuration in `config/_default/languages.toml` file should be:

```toml
[en]
languageName = "English"
contentDir = "content/en"
title = "AWS Workshop"
weight = 1

[es]
languageName = "Español"
contentDir = "content/es"
title = "Taller de AWS"
weight = 2
```

### Default content language

When working with multiple languages, you can define which language will be the default rendered in your website. You can modify the `defaultContentLanguage` parameter in `config/_default/config.toml` file.

```toml
defaultContentLanguage = "en"
```

### Overwrite translation strings

Translations strings are used for common default values used in the theme (*Edit this page* button, *Search placeholder* and so on). By default, translations are available in english only but you may use another language or want to override default values.

To override these values, create a new file in your local `i18n` folder `i18n/<idlanguage>.toml` and inspire yourself from the theme `themes/learn/i18n/<idlanguage>.toml`
