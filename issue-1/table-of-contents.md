---
layout: issue-1
title: Table of Contents
---
{% for page_name in site.data.issue_1 %}
  {% assign list_page = site.pages | where: "name", page_name | first %}
  * [{{list_page.title}}]({{list_page.url | relative_url}}) by {{list_page.author}}
{% endfor %}
