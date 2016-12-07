---
layout: post
title: Writting an academic paper on Github Resources
---

The idea sounds a little nutty, but personally the transparency and outward accountablilty of working on a paper on github is appealing. I also just plain love writting in markdown. To that end, I am compiling a list of helpful sites/tools. You can also do the work in a private repository (if you pay) and then make it public when ready. 

1) move existing word docx to markdown. 
- [Heroku Word to Markdown Converter](https://word-to-markdown.herokuapp.com/)

- [Pandoc](http://pandoc.org/installing.html)
  ```
  $ brew install pandoc
  ```
  And from from [this tutorial](http://bob.yexley.net/generate-a-word-document-from-markdown-on-os-x/) using the command line,   from markdown to word 
  
  ```
  $ pandoc -o output.docx -f markdown -t docx markdown-file.md
  ```
  or the reverse (word to markdown) 
  ```
  pandoc -o markdown_doc.md -f docx -t markdown word_doc.docx
  ```
