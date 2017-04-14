# melown.github.io
Repository for Melown's open source activities web page

## Install Jekyll

This step is required only once

```
bundle install
```

## Run development server

```
bundle exec jekyll serve    # run the development server
```

Visit http://localhost:4000/ for page priview

## Write new blog post

New blog posts are stored in `./_posts/` directory. Copy one of them and adjust
to your needs.

## Add new project page

As example, you can look into `vts-browser-js`. The index file shall use
following template

```
---
layout: component
title: Project title
description: Project description, which will be displayed at home page
keywords: VTS, Melown, WebGL, ... ad yours
---

<a href="https://github.com/melown/[PLACE_PROJECT HERE]"><img style="position: absolute; top: 0; right: 0; border: 0;" src="https://camo.githubusercontent.com/652c5b9acfaddf3a9c326fa6bde407b87f7be0f4/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f6769746875622f726962626f6e732f666f726b6d655f72696768745f6f72616e67655f6666373630302e706e67" alt="Fork me on GitHub" data-canonical-src="https://s3.amazonaws.com/github/ribbons/forkme_right_orange_ff7600.png"></a>

## Documentation

* [link to project documentation](https://www.melown.com/...)

## Source code

* Source code is hosted on [GitHub](https://github.com/melown/PROJECT_NAME)

` ` `
git clone https://github.com/melown/PROJECT_NAME
` ` `

```

You should also add link to `./projects.md` file


The page will be added to front-page (homepage) automatically.

## Publish

Just `git push` to `master` branch.
