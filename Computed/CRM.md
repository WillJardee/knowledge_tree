---
aliases: [CRM]
tags: 
title: CRM
linter-yaml-title-alias: CRM
date created: Tuesday, January 24th 2023, 8:12:37 am
date modified: Thursday, January 26th 2023, 12:14:45 pm
---


```dataview
table phone, email, birthday, relationship, 
choice(
	regexmatch("\w+", instagram), 
	elink("https://instagram.com/@" + instagram, instagram), "\-") as instagram,
choice(
	regexmatch("\w+", instagram),
	elink("https://twitter.com/" + twitter, twitter), "\-") as twitter,
choice(
	regexmatch("\w+", instagram),
	elink("https://linkedin.com/@" + linkedin, linkedin), "\-") as linkedin, url as url
from "Databases/CRM"
where file.name != "CRM"
```
