---
title: "First Post"
date: 2022-02-11T00:49:22+08:00
draft: false
image: hugo-logo-wide.svg
tags:
        - hugo
        - stack
categories:
        - 文档
---

How I created this post:

First install hugo on your system

Choose a folder to run this command
```sh
hugo new site blog
```

`cd` into your site folder,
init a `git` repo,
and add a theme.

The theme I used is called [Stack](https://github.com/CaiJimmy/hugo-theme-stack).

```sh
cd blog
git init
git clone https://github.com/CaiJimmy/hugo-theme-stack/ themes/hugo-theme-stack
git submodule add https://github.com/CaiJimmy/hugo-theme-stack/ themes/hugo-theme-stack
```

Delete `config.toml`.

Copy the `config.yaml` file in `exampleSite/` folder

```sh
rm config.toml
cp themes/hugo-theme-stack/exampleSite/config.yaml ./
```

Add this post

```sh
hugo new post/first-post/index.md
```

Copy `archives` and `search` from `exampleSite/content/page/`

Start locally with Draft on.
```
hugo serve -D
```
