---
title: About
permalink: /about/
---

# About

This is a starter template for a mkdocs jekyll theme, based on these two
previous beauties:

 - [alexcarpenter/material-jekyll-theme](http://alexcarpenter.github.io/material-jekyll-theme)
 - [squidfunk/mkdocs-material](https://github.com/squidfunk/mkdocs-material)

Specifically, I wanted a completely jekyll-based template that would render
markdown docs, deployed on GitHub pages, and set up with easy customization
and preview.

## Getting Started

### Get the code

You can clone the repository right to where you want to host the docs:

```bash
$ git clone https://github.com/vsoch/mkdocs-jekyll.git docs
$ cd docs
```

### Customization

#### config.yml

To edit configuration values, customize the [_config.yml](_config.yml).
Most are documented there.

### Adding pages

To add pages, write them into the [pages](pages) folder. 
You define urls based on the `permalink` attribute in your pages,
and then add them to the navigation by adding to the content of [_data/toc.myl](_data/toc.yml).

### 3. Options

Most of the configuration values in the [_config.yml](_config.yml) are self explanatory,
but we can describe a few here if it's helpful.

+ Theme
 - Green
  - Blue
  - Orange
  - Purple
  - Grey
+ Fixed Navigation
  - True
  - False

### 4. Serve

Depending on how you installed jekyll:

```bash
jekyll serve
# or
bundle exec jekyll serve
```

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
