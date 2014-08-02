# Hyde

Hyde is a two-column [Sculpin](https://sculpin.io) theme that pairs a prominent sidebar with uncomplicated content. It's based on the Jekyll theme [Poole](http://getpoole.com), the Jekyll butler.

![Hyde screenshot](screenshot.png/)


## Contents

- [Usage](#usage)
- [Options](#options)
  - [Sidebar menu](#sidebar-menu)
  - [Sticky sidebar content](#sticky-sidebar-content)
  - [Themes](#themes)
  - [Reverse layout](#reverse-layout)
- [Development](#development)
- [Author](#author)
- [License](#license)


## Usage

Hyde is a theme built on top of [sculpin](https://sculpin.io), which provides a fully furnished sculpin setup—just download and start the sculpin server. See [Sculpin getting started guide](https://sculpin.io/getstarted/) for how to install and use Sculpin.


## Options

Hyde includes some customizable options, typically applied via classes on the `<body>` element.


### Sidebar menu

Create a list of nav links in the sidebar template by assigning a hyperlink.

**Why require a specific layout?** Sculpin will return *all* pages, including the `atom.xml`, and with an alphabetical sort order. To ensure the first link is *Home*, we exclude the `index.html` page from this list by specifying the `default` layout.


### Sticky sidebar content

By default Hyde ships with a sidebar that affixes it's content to the bottom of the sidebar. You can optionally disabled this by removing the `.sidebar-sticky` class from the sidebar's `.container`. Sidebar content will then normally flow from top to bottom.

```html
<!-- Default sidebar -->
<div class="sidebar">
  <div class="container sidebar-sticky">
    ...
  </div>
</div>

<!-- Modified sidebar -->
<div class="sidebar">
  <div class="container">
    ...
  </div>
</div>
```


### Themes

Hyde ships with eight optional themes based on the [base16 color scheme](https://github.com/chriskempson/base16). Apply a theme to change the color scheme (mostly applies to sidebar and links).

There are eight themes available at this time.

To use a theme, add anyone of the available theme classes to the `<body>` element in the `default.html` layout, like so:

```html
<body class="theme-base-08">
  ...
</body>
```

To create your own theme, look to the Themes section of included CSS file. Copy any existing theme (they're only a few lines of CSS), rename it, and change the provided colors.

### Reverse layout

Hyde's page orientation can be reversed with a single class.

```html
<body class="layout-reverse">
  ...
</body>
```

## Author

**Kirk Dawson**
- <https://github.com/kdawson133>
- <https://twitter.com/kirk133>

Based on The Hyde Theme for Jekyll by [@mdo](https://twitter.com/mdo)

## License

Open sourced under the [MIT license](LICENSE.md).
