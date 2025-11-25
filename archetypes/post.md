---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
authors: ["ZDevilInside"]   # or leave ["author"] if you want to fill manually
categories: ["Aviation"]    # default category, adjust as needed
tags: ["tag"]               # starter tag
description: "Write a short description here."
draft: true
image: "thumbnail.jpg"      # filename of bundled image (placed next to index.md)
slug: "{{ .Name }}"         # ensures clean URL based on folder name
summary: "Optional summary for list pages."
---
