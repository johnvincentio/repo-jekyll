# Jekyll

[Home](https://jekyllrb.com/)

## Note

To start jekyll server:

```
cd demosite
bundle exec jekyll serve
```

From browser

```
http://localhost:4000/
```

Deploy to web server:

```
demosite/_site
```

## Install
sudo gem install jekyll bundler

## Create New Project

```
cd cms/repo-jekyll/udemy-jekyll
jekyll new demosite
```

```
To run the server:
cd demosite
bundle exec jekyll serve

which creates the folder:
_site

from browser:
http://localhost:4000/
```

## Theme

```
cd demosite
edit _config.yml
notice:
theme: minima

```

Where is the theme?

```
cd demosite
bundle show minima

/Library/Ruby/Gems/2.0.0/gems/minima-2.1.0
```

Remove

```
rm about.md index.md
cd _posts
rm *.markdown
```

Configure

```
config.yml:
delete:
theme: minima

Gemfile:
delete:
gem "minima", "~> 2.0"
```

Remove dependencies:

```
bundle
```

Add folders:

```
cd demosite
_includes
_layouts
```

Copy template:

```
copy folders within template to demosite
```

## Create Default Layout

```
in _layouts
create default.html
```


Yaml front matter, top of the file.

Top of each html file.


Build includes

## Posts

Each post is a file in _posts. For example:

2016-01-19-benefits-of-static-website-generators.md

Url:
http://local:4000/jekyll/2016/01/19/benefits-of-static-website-generators.html

_config.yml
set permalink to improve the urls.

http://localhost:4000/jekyll/benefits-of-static-website-generators.html

Note that jekyll come from the category front yaml of the MD file.

Default path to the post is:
category/name/year/month/day/title.html









