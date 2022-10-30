---
title: "Using Obsidian to Manage the Blog"
slug: "using-obsidian-to-manage-the-blog"
date: 2022-10-30 00:57:13-05:00
author: "Mike Pruett"
draft: false
layout: post
comments: true
tags:
- website
- hugo
- selfhosted 
categories:
- Updates
- Open Source
---

![[/uploads/Pasted image 20221030011354.png|100]]

I just recently started using [Obsidian](https://obsidian.md/) to manage my Work and Personal notes, and its pretty awesome. Obsidian is a powerful and extensible knowledge base that works on top of your local folder of plain text files.

![[/uploads/Pasted image 20221030011438.png]]

Had a random thought this evening, and wonderd if anyone had ever used Obsidian to manage their Hugo-Based Blog. Looks like there are a few, but each implementation seems to differ wildly.

So far I have done the following:
- Opened my existing git repo for the blog in Obsidian as a new Vault
- Renamed all of my Markdown files from .markdown to .md, so that Obsidian can identify them automatically.
- Created a \_templates folder the root of my repo, and configured Obsidian to use that for Template storage
- Created a **Post** Template, that includes the following front-matter
```yaml
---
title: "{{title}}"
slug: "{{title}}"
date: {{date}} {{time}}
author: "Mike Pruett"
draft: false
layout: post
comments: true
tags: []
categories: []
---
```
- Configured Obsidian to use my static/uploads folder for the Attachment Folder Path
- Configured Obsidian to use my content/posts folder for the place to store new notes

Still have some outstanding items to figure out...
- Hugo handing attachment (image) handling, as the normal way is to just use the \/uploads\/ folder
- Not sure how to traslate Obsidian Front-Matter Categories and Tags to work with Hugo

So far though, I am really impressed!
