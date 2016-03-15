# Hugo Phlat Theme

A flat bootstrap theme for the Hugo static website engine.

## Installation

Use an existing Hugo project or create a fresh one before trying to install this theme.  Within the Hugo project, execute the following command from your Command Prompt (Windows) or Terminal (Mac and Linux):

```
mkdir themes
cd themes
git clone https://github.com/nraboy/hugo-phlat-theme
```

See the [official Hugo themes documentation](http://gohugo.io/themes/installing) for more info.

## Usage

This theme expects the standard Hugo site layout.

```
.
└── content
    ├── post
    |   ├── post1.md
    |   └── post2.md
    ├── page
    |   ├── about.md
    |   ├── contact.md
```

Run `hugo --theme=hugo-phlat-theme` to generate your site!

## Configuration

This theme relies heavily on a well crafted `config.toml` file.  Here are the required parameters:

```toml
baseurl = "http://replace-this-with-your-hugo-site.com/"
languageCode = "en-us"
title = "Own the Web"

[permalinks]
    post = "/:year/:month/:slug/"
    page = "/:slug/"

[taxonomies]
    tag = "tags"
    category = "categories"
```

Everything that comes next is optional:

```toml
[[menu.header]]
    name = "Home"
    weight = 1
    url = "/"

[[menu.header]]
    name = "Resources"
    weight = 2
    url = "/resources/"

[[menu.header]]
    name = "Contact"
    weight = 3
    url = "/contact/"

[[menu.footer]]
    name = "Privacy Policy"
    weight = 1
    url = "/privacy-policy/"

[[menu.footer]]
    name = "Sponsors"
    weight = 2
    url = "/sponsors/"

[params]
    google_analytics = "UA-XXXXXXX-YY"
    google_adsense = "ca-pub-XXXXXXXX"
    disqus = "site_name_here"
    twitter = "https://www.twitter.com/nraboy"
    googleplus = ""
    linkedin = ""
    youtube = ""
    paypal = ""
```

## About the Author

If you like this theme let me know!  You can reach me easiest on Twitter at [@nraboy](https://www.twitter.com).
