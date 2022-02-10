---
layout: post
title:  "Using Jekyll and GitHub to build a blog!"
date:   2022-02-04 15:15:39 -0500
categories: blog jekyll
---

Wanting to create my own blog for a long time, I recently came accross many personal websites and blogs hosted on GitHub (username.github.io). After reading a bit, I realized that this is quite easy. I followed the steps given below.

1. It is best to follow the official instructions on the [github page](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll).
2. While testing the site locally, `bundle exec jekyll serve` gave an error. I had to run `bundle add webrick` to make this work. This is because the latest ruby doesn't come bundled with *webrick*.
3. If it runs properly, make changes to the _config.yml and about.markdown file and run again.
4. Upload to github.

This will set up a basic blog site which can be modified as per your liking.

Cheers!