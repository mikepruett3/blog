---
title: "{{ replace .Name "-" " " | title }}"
stub: "{{ replace .Name " " "-" | title | lower }}"
date: {{ .Date }}
author: "{{ .Site.Author.name }}"
draft: false
layout: post
comments: true
tags: []
categories: []
---

