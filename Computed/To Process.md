---
aliases: [To Process]
tags: []
title: To Process
date created: Tuesday, December 13th 2022, 2:33:51 pm
date modified: Friday, January 27th 2023, 11:40:35 am
linter-yaml-title-alias: To Process
---

```dataview
list
from "Inbox" OR "Readwise" OR "Readwise-Example"
where contains(file.tags, "#to-process")
```
