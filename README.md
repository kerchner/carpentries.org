## The Carpentries website

This is the repo for [The Carpentries website](https://carpentries.org).  The site is built using [The Carpentries Hugo theme](https://github.com/carpentries/carpentries-hugo-theme).  

To build this site locally, follow the instructions in the theme's repo.

Run `make serve` in your project's folder to serve the site locally.

## Organizing content 

On 18 November 2024, this site was released using Hugo as the static site generator.  This README section will be updated as we add in more information about how to use the new infrastructure.

### General content

General content is in one of the folders in the `content` folder.  These folders are organized by theme.  No new files should be created in the root of the `content` folder.

### Blog posts

**File names and location**
Blog posts go in the `content/posts/YYYY/MM` folder.  Images for the blog posts go in the corresponding `static/blog/YYYY/MM` folder. Note YYYY is the four digit year and MM is the two digit month. Be sure the file location and the blog post date as defined in the yaml metadata (see below) match up.

The file name should **not** include a date.  The file name should be entirely in lowercase.

**File metadata**

The file should begin with yaml metadata (data contained within three hyphens at the top of the file). An example is below:

```
---
layout: page
authors: ["Person One", "Person Two"]
teaser: "A short line describing the post that will display on the blog list page"
title: "Blog post main title"
date: 2024-11-18
time: "09:00:00"
tags: ["Data Carpentry", "Community"]
---
```

**Blog post tags:** Whenever possible, make sure the tags are from our [list of existing tags](https://carpentries.org/blog/posts-by-tags/).

