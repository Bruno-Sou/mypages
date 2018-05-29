---
layout: page
title: "Page list"
permalink: /page/list/
---

## This is the list of pages available programatically


Site pages = {{ site.pages | map: "path" | join: " , " }}
