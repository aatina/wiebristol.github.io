# Contributing

## Introduction

Contributing to the Women in Engineering website has never been easier! It's a simple four stage process. For those already familiar with Github, here's what you need to do. (For those not familiar, keep reading and we'll explain in more detail).

***Note:** You only need to do steps 1 and 2 the first time you wish to create or edit the website. If you've forked already/before skip to step 3.*

1. Create a Github account
2. Fork the website repository
3. Create or edit the page or blog post you wished to edit
    - Or if you're feeling daring, edit the website's design! You might want to talk to our webmaster first though - Ed Nutting.
4. Submit a pull request (for your changes to be integrated into the main website)
    - All changes are reviewed by our webmaster. We endeavour to have good changes merged within 48 hours.
    - ***Note:** You only need to submit a new pull request if your previous one has been merged or closed.*

## 1. Creating a Github account

### 1. Go to Github

Head over to the [Github home page](https://github.com) and click the shiny, green sign up button.

### 2. Sign up

Go ahead, fill in your details! We suggest you use your university email (and you might even want to consider applying for the free student account). Make sure you use a sensible username and remember that your profile will be publicly visible (picture, username and any changes you make to the website - even if they aren't merged with the main website!).

### 3. Confirm your email address

Github will send you a confirmation email to verify your email address. You'll need to complete the verification before you can proceed.


## 2. Forking the website repository

### What is a fork?

A fork is just a copy of the original repository (and a repository is essentially just a sophisticated folder for a project). Your copy allows you to make changes piece by piece, track everything and try things out without affecting the main website. Once you're happy with your changes then you can use a pull request (described later) to request the changes be merged with the main website.

### Why do I need to fork?

We don't grant people direct access to the main website repository. There are two reasons for this:

1. Github teams (which is what gives multiple people direct access) isn't free and is a hassle to manage (more hassle than just using forks/pull requests).
2. Forks (i.e. personal copies) allow you to experiment with changes without accidentally breaking the live website. A pull request then allows our committee to check changes (for spelling, grammar, spam, etc.) before they go live on the website. Usually, changes will be fairly straightforward so they will be merged within 48 hours.

### 1. Go to the website repository

Head to the [WiE repository](https://github.com/wiebristol/wiebristol.github.io). Given you're viewing this document, you've probably already found the repository (good work!)

### 2. Click fork

In the top-right corner of the page you'll see a button called `Fork` - click it. This will create a new fork just for you and then take you to the page for that fork. In future, this is where you will need to go to edit stuff. You only need to fork once!

### 3. Your fork is a copy. You'll often need to update your copy...

Changes come in from lots of different forks. This will mean that your copy will become out of date quite rapidly when compared to the main website. Before you work on any changes, you should check whether you need to update your fork. Github will tell you when your fork is "out of date" or "behind" the main website. If this is the case, you'll need to merge down from the main repository to yours. This will mean creating a pull request to go from the main website to your fork. This is doing the opposite of the pull request process that will be explained later - so you can just reverse the process when needed.


## 3. Create or edit a page or blog post

### a. Creating a page

Creating a page shouldn't happen very often. Mostly, you'll want to add content to an existing page or write a blog post. Some pages, you won't want to appear in the main menu bar - i.e. they'll only be linked to from within one of the main pages. We'll explain how to create these two types of page now.

#### Create a file for the page

First, you'll need to create a new file for the page. Create a file named `MyPageName.md` in the root folder (`/`) of the website. Then put in one of the templates from below.

#### Template for pages in the main menu bar

```
---
layout: page
title: Page Title
permalink: /page-title-no-spaces/
excerpt: Brief (max. 20 word) description of the page.
---
```

#### Template for other pages

```
---
layout: page
permalink: /path/to/page/no/spaces/
excerpt: Brief (max. 20 word) description of the page.
---
```

### b. Creating a blog post

Creating a blog post is similar to creating a page, except that it goes in a different folder and has a special name format. To create a blog post, create a file with the following name in the `_posts` folder:

`YEAR-MONTH-DATE-Post-Title-No-Spaces.md`

For example, a post titled *Contributing to the website* written on the *1st of March 2016* would have the following file name:

`2016-03-01-Contributing-to-the-website.md`

Then copy/paste the following template into the file.

#### Template for blog posts

```
---
layout: post
title: Post Title
date: YEAR-MONTH-DATE HOUR:MINUTE:00 +0100
categories: post categories space separated e.g. equality sponsorship events
---
```

### c. Writing / editing a page or blog post

Almost all posts and pages are written ***Markdown*** syntax. (Some pages include some HTML but your probably won't need it.) Markdown is a really simple and fast way to write nicely formatted articles. There are great tutorials available online. We recommend [this one](http://www.markdowntutorial.com).

We also have some specific guidelines for pages and posts. There are a few things to be aware of, which are:

1. Links to pages within the website need to be created as follows:
   ```
   [Link Text]({{ "path/to/page/" | prepend: site.base_url }})
   ```
2. Links to posts within the blog need to be created as follows:
   ```
   [Link Text]({{ post_url 2010-07-21-name-of-post }})
   ```
3. To create a heading and (optionally) strapline, use the following in the YAML (the stuff within the `---` at the start of the file):
   ```
   headline: Women in Engineering Society
   strapline: The story so far
   ```
4. To create a full-width image at the top of a page (after the heading/strapline), use the following in the YAML (the stuff within the `---` at the start of the file):
   ```
   image: "iwd2016.png"
   ```
   *Note: The image must be in the `images` folder.*

### d. Useful resources

[This site](https://daringfireball.net/projects/markdown/syntax) has a great summary of all the Markdown features and how to use them. If you find a feature which doesn't work, let us know (using the Issue Tracker) and we'll try to get it fixed.

## 4. Submit a pull request

1. Go to your fork of the website repository
2. Click `Create Pull Request`
3. Check the merge setup matches the following:
   Left: WieBristol:master
   Right: YourFork:master

   (Or, if you are trying to update your fork with changes from the main website, select the above options the opposite way round.)
4. Click submit
5. Write a useful message explaining your changes
6. Click submit
7. Respond to any comments / change requests
   ***Note:** If you make more edits to your repository while a pull request exists, those changes will automatically be included in the pull request.*
8. Wait for your changes to be merged
9. See your changes on the website!


## 5. What do I do next time I want to make an edit?

Head to your fork, check whether you need to update the fork (if so, create a pull request from the main website to your fork - the opposite of the above described process), merge that pull request (hopefully you won't have merge conflicts - if you do, either read up on how to use Git to resolve them or get in touch with us!), then go ahead and edit or create a file as described above.


## 6. Adding images or other files

Images should go in the `images` folder. To include them in a page, use the following:

```
{% include image image="image-name.ext" alt="Four to six word image description" %}
```

*Note: This is not the same as standard markdown syntax for images!*

If you want the image to appear in the full width of the page, use the following:

```
{% include image image="image-name.ext" alt="Four to six word image description" full_width=true %}
```

Files should go in a subdirectory of the `files` folder (which, at the time of writing, doesn't exist). To include a link to a file in a page, use the following:

```
{% include file file="file-name.ext" text="Link text to appear in page" %}
```
