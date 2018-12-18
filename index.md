---
layout: sidenav
---
# NSW Government github pages template

### Background
This repo is a theme so that NSW Government designers to create prototype digital products (static or transactional) which are displayed using github pages.

### How to use
First, we need to import [use-NSW-jekyll](https://github.com/tjharrop/use-NSW-jekyll) to a repo in your own account.
1. Sign in to github.com
2. Click + in the top right
3. Select 'import repository'
4. Paste `https://github.com/tjharrop/use-NSW-jekyll.git` in to the old repo URL
5. Name your project
6. Click 'Begin import'

Your repo is ready to go!

Now we tell github pages to host the prototype
1. Open `github.com/your-username/your-new-repository` (the one you just created)
2. Click settings
3. Scroll down to github pages
4. Select the master branch as the source (in the drop-down) and click save. It'll take about 10 minutes to build. The URL will be shown to you

Change settings so it all works
1. In github, or an editor, edit the `_config.yml` file. Change the `baseurl:` to `/your-repo-name`
2. Change `title:` and `description:` to match your project

### Your website is ready to go!

**Editing the nav**

Your navigation is generated from a file in your repository. It's in `_data` and it's called `navs.yml`

It uses the YAML format - there are editors out there to help

**Creating pages**

If you create a file, it will adopt the template. If you create a directory and call the page 'index.md' for markup or 'index.html' if you prefer HTML, it will show by default.

**Other options**

There are 3 templates, which you can change using the 'layout' option in the page settings
- default - no side nav
- sidenav - contains a side-nav
- accordion - contains a side nav which shows/hides

You can set the site 'stage' (such as alpa/prototype/beta) in the `_config.yml` file

### Tech
[NSW-uikit-starter](https://github.com/tjharrop/nsw-uikit-starter) is a fork of the DTA's [Uikit Starter](https://github.com/govau/uikit-starter) which, instead of being static HTML files, generates a NSW-branded theme for Jekyll, the Ruby on Rails static site builder used by github pages.

The whole Jekyll theme is available in [NSW-jekyll-theme](https://github.com/tjharrop/NSW-jekyll-theme).

You can use NSW-jekyll-theme without forking it, by referencing it as a remote theme.

This package is a demo of that, which you can import and modify.
