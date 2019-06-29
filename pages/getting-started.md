---
title: Getting Started
permalink: /getting-started/
tags: 
 - jekyll
 - github
 - github-pages
---

# Getting Started

## Install Dependencies

Initially (on OS X), you will need to setup [Brew](http://brew.sh/) which is a package manager for OS X and [Git](https://git-scm.com/). To install Brew and Git, run the following commands:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install git
```

If you are on Debian/Ubuntu, then you can easily install git with `apt-get`

```bash
apt-get update && apt-get install -y git
```

### Install Jekyll

You can also install Jekyll with brew.

```bash
$ brew install ruby
$ gem install jekyll
$ gem install bundler
$ bundle install
```

On Ubuntu I do a different method:

```bash
git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL
rbenv install 2.3.1
rbenv global 2.3.1
gem install bundler
rbenv rehash
ruby -v

# Rails
curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
sudo apt-get install -y nodejs
gem install rails -v 4.2.6
rbenv rehash

# Jekyll
gem install jekyll
gem install github-pages
gem install jekyll-sass-converter

rbenv rehash
```

## Get the code

You should first fork the repository to your GitHub organization or username,
and then clone it.

```bash
$ git clone https://github.com/<username</mkdocs-jekyll.git docs
$ cd docs
```

You can clone the repository right to where you want to host the docs:

```bash
$ git clone https://github.com/<username>/mkdocs-jekyll.git docs
$ cd docs
```

## Customization

### config.yml

To edit configuration values, customize the [_config.yml](_config.yml).
Most are documented there, and please [open an issue](https://www.github.com/{{ site.github_user }}/{{ site.github_user }}/issues) if you have questions.

### Adding pages

To add pages, write them into the [pages](pages) folder. 
You define urls based on the `permalink` attribute in your pages,
and then add them to the navigation by adding to the content of [_data/toc.yml](_data/toc.yml).

### Tags

If you include tags on a page, by default they won't link to anything. However,
if you define a `tag_search_endpoint` url in your configuration file, by clicking
the tag, the user will be taken to this page to search for it. As an example,
we define the current search endpoint to be Ask Cyberinfrastructure, and
page tags link to a search on it:

```
tag_search_endpoint: https://ask.cyberinfrastructure.org/search?q=
```

The tags appear at the bottom of the page for you to click, as on this page.

### Alerts

{% include alert.html type="info" title="What is an alert?" content="An alert is a box that can stand out to indicate important information. You can choose from levels success, warning, danger, info, and primary. This example is an info box, and the code for it looks like this:" %}

```
{%raw%}{% include alert.html type="info" title="What is an alert?" content="An alert is a box that can stand out to indicate important information. You can choose from levels success, warning, danger, info, and primary. This example is an info box, and the code for it looks like this:" %}
{%endraw%}
```

Just for fun, here are all the types:

{% include alert.html type="warning" content="This is a warning" %}
{% include alert.html type="danger" content="This alerts danger!" %}
{% include alert.html type="success" content="This alerts success" %}


## Serve

Depending on how you installed jekyll:

```bash
jekyll serve
# or
bundle exec jekyll serve
```
