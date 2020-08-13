+++
title = "Configuration"
weight = 010400
chapter = false
pre = "<b>d. </b>"
disableToc = false
+++

### Hugo configuration

The [Hugo global configuration](https://gohugo.io/overview/configuration/) is the basis to customize your template. There are two methods to define the configuration:

1. [A single configuration file](https://gohugo.io/getting-started/configuration/#configuration-file)
2. [A configuration directory](https://gohugo.io/getting-started/configuration/#configuration-directory)

{{% notice info %}}
The template uses the **[directory configuration](https://gohugo.io/getting-started/configuration/#configuration-directory)** method for customizing it.
{{% /notice %}}

### Global site parameters

On top of [Hugo global configuration](https://gohugo.io/overview/configuration/), you can define the following parameters in `config/_default/params.toml` file.

{{% notice info %}}
The values here are the defaults configured.
{{% /notice %}}

```toml
# Prefix URL to edit current page. Will display an "Edit this page" button on top right hand corner of every page.
# Useful to give opportunity to people to create merge request for your doc.
# See the config.toml file from this documentation site to have an example.
editURL = ""
# Author of the site, will be used in meta information
author = ""
# Description of the site, will be used in meta information
description = ""
# Shows a checkmark for visited pages on the menu
showVisitedLinks = false
# Disable search function. It will hide search bar
disableSearch = false
# Javascript and CSS cache are automatically busted when new version of site is generated.
# Set this to true to disable this behavior (some proxies don't handle well this optimization)
disableAssetsBusting = false
# Set this to true to disable copy-to-clipboard button for inline code.
disableInlineCopyToClipBoard = false
# A title for shortcuts in menu is set by default. Set this to true to disable it.
disableShortcutsTitle = false
# When using mulitlingual website, disable the switch language button.
disableLanguageSwitchingButton = false
# Hide breadcrumbs in the header and only show the current page title
disableBreadcrumb = true
# Hide Next and Previous page buttons normally displayed full height beside content
disableNextPrev = true
# Order sections in menu by "weight" or "title". Default to "weight"
ordersectionsby = "weight"
# Change default color scheme with a variant one. Can be "red", "blue", "green".
themeVariant = ""
# Provide a list of custom css files to load relative from the `static/` folder in the site root.
custom_css = ["css/foo.css", "css/bar.css"]
```