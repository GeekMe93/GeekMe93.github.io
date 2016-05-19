---
layout: post               
title: Jekyll Set-up on Mac        
categories: [tutorial]
tags: [jekyll, website, github-pages]

---


I spent nearly week to set up my own website based on Jekyll and github 
pages. In this process, I gained a general idea of the structure of  website set-up. This is a really interesting. I once considered writing my own website based on some commercialized templates. But the low degree of customization forced me to give up the "relying on other person" idea. Thanks to github and Jekyll, all this came true!
 

## Fork or Create

You could choose to fork, but I would like to create a new repo.

- following [instructions](https://pages.github.com) in github to create your repo;
- Save your repo into Github Desktop
- commit and sync to post

## The structure of Jekyll

- `_config.yml`: configuration of you pages;
- `_layout`: folders for you templates;
- `_includes`: small pieces of html which can be included into other files via **liquid tag**;
- `_posts`: where you posts should lie in;
- `css, js`: style sheet and how your web behave;

## Set up the local Jekyll environment

> 1. install Xcode, the newest version;
> 2. install Xcode developer command lines; Open your terminal, type: xcode-select --install
> 3. Install the github-pages; gem install github-pages
> 4. Install bundler; gem install bundler
> 5. change directory to your local github repository; bundle install
Here, some bundle has been installed in installing github-pages, only a few of them will be updated according to you Gemfile in your repository;

## You are free to website now

> `bundle exec jekyll serve`

> `jekyll serve --watch --baseurl ""`


