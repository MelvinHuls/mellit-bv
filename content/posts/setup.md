---
title: Setup Mellit.dev
linkTitle: setupSite
description: A description of how this site was setup.
date: 2024-02-11T14:30:00+01:00
summary: Want to find out how this site was set up? Read this post to find out.
---

A collection of resources used to build this site. Combined with some tips that might save time.

## Hugo

First make a small project with: [link](https://gohugo.io/getting-started/quick-start/)

Do note that this demo makes posts, which are available in https://localhost:1313/posts. The homepage will be empty, don't let this confuse you.

The homepage itself can be configured in the hugo.toml (config.toml). [Spectral](https://github.com/sbruder/spectral/blob/master/exampleSite/config.toml) has a good example.

### Customize themes
For css/scss you can just make a file and reference it in your hugo.toml (config.toml). I had to overwrite the stylesheets.html file of the theme I'm using to make this work.
Also: it needs to be in a list, even if you have 1 file.

For specific files they should not be edited directly in the themes dir. But you can add files to your project and they have priority. See [link](https://gohugobrasil.netlify.app/themes/customizing/)

The theme uses [fontawesome](https://fontawesome.com/icons), so you can add/override icons using these.

## Domain setup
For hosting github pages is being used.

### Google domains
Hosting config for Google domains can be configured as follows: [link](https://medium.com/8px-magazine/hosting-a-website-for-free-get-started-with-google-domains-github-pages-980986550958)

Note: when configuring the 'A Record' the '@' should just be empty.

This blogpost is however incomplete and after completing it you should follow: [link](https://gohugo.io/hosting-and-deployment/hosting-on-github/)


## Extra notes

Top level headers are ignored. A &lt;h1&gt;&lt;/h1&gt; tag in html and a # in markdown will be ignored. ## and &lt;h2&gt;&lt;/h2&gt; work.


## Example

If you need a more hands-on example. The code for this site can be found in my GitHub repo: [link](https://github.com/MelvinHuls/mellit-bv)