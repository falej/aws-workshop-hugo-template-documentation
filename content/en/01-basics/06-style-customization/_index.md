+++
title = "Style customization"
weight = 010600
chapter = false
pre = "<b>f. </b>"
disableToc = false
+++

## Change the logo

To change the default template logo, go to `layouts/partials` and modify the `logo.html` file. Write any HTML you want. You could use an `img` HTML tag and reference an image created under the *static* folder, or you could paste a SVG definition.

{{% notice note %}}
The size of the logo will adapt automatically.
{{% /notice %}}

## Change the favicon

If your favicon is a `png`, just drop off your image in your local `static/images/` folder and name it `favicon.png`.

If you need to change this default behavior, create a new file in `layouts/partials/` named `favicon.html`. Then write something like this:

```html
<link rel="shortcut icon" href="/images/favicon.png" type="image/x-icon" />
```

## Change default colors

#### Native color scheme variants

Hugo theme **Learn** let you choose between 3 native color scheme variants (**red**, **blue**, **green**). To change the theme variant to any of the native color schemes, modify the following parameter in `config/_default/params.toml`:

```toml
# Change default color scheme with a variant one. Can be "red", "blue", "green" or "aws".
themeVariant = "red"
```
#### Custom color scheme variants

To create a custom color scheme variants, it is necessary to create a new CSS file in your local `static/css` directory, prefixed by `theme`.

By default, the template uses a **custom** variant for AWS. It can be found in `static/css/theme-aws.css` and you are free to make any changes you want.

{{% notice warning %}}
We don't recommend to change the default `theme-aws.css` file. Instead make a copy of it and do any modification in the new file, but keep in mind that the AWS custom variant color scheme was designed following the AWS brand guidelines and we encourage you to align your modifications to them.
{{% /notice %}}
