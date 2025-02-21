---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
# layout: default
layout: list
title: Home
---

## Welcome to My Site

This is a test page for the "News" section.

{% for item in site.data.content %}
  <h2>{{ item.title }}</h2>
  <p>{{ item.excerpt }}</p>
  <a href="#">더보기</a>
{% endfor %}
