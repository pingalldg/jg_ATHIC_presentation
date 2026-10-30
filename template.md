[//]: # "Template file used to generate reveal.js style presentations written in Markdown using Pandoc, with some examples!"
[//]: # "Last revised 05.11.2021"


[//]: # "A YAML metadata block is used to specify title/author/etc..."

---
title: Your main title
subtitle: Your subtitle
author: Your name here
date: manually specified date
---

[//]: # "Begin presentation"

# This will spawn a parent slide
- This is a bullet point  
Text can also be placed without a bullet point

## This will spawn a child slide downwards from the nearest parent
1. This 
2. List
3. Is
4. Ordered

## This will spawn another child, in downwards from the previous child
[//]: # "GitHub-flavoured Markdown is supported"
A | Simple | Table
- | ------ | -----
1 | Hello | World!

# This will spawn a new parent slide, rightward to the previous parent/child

[//]: # "End presentation"