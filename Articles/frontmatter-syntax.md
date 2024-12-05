# Why syntax is important in Markdown files on adonisjs 6 (saut de ligne)

## Today I Discovered How a Simple Syntax Error Like Line Breaks in a .md File Can Break a Website

While working on our AdonisJS 6 project, we had to use a front matter block containing a title and a summary. However, when trying to display our pages, we encountered the following error:

**can not read a block mapping entry; a multiline key may not be an implicit key at line 6, column 1: ^**


After spending significant time debugging the routes and HTML pages, I realized that the problem was caused by line breaks in the front matter of our Markdown files. This subtle issue completely prevented the website from functioning as expected.

### Correct syntax 
```
---
title: Another awesome movie
summary: Reprehenderit eiusmod in deserunt quis adipisicing deserunt eu qui nisi. Aliquip est Lorem quis adipisicing et voluptate proident dolore id occaecat ut ex commodo aliquip.
---
```
### Incorrect syntax 
```
---
title: Another awesome movie
summary: Reprehenderit eiusmod in deserunt quis adipisicing deserunt 
eu qui nisi. Aliquip est Lorem quis adipisicing 
et voluptate proident dolore id occaecat      ut ex commodo aliquip.
---
```

If you want to include line breaks in your summary or any multi-line text, you can:

- The | character allows you to write multi-line text as-is, preserving all line breaks in the output.
- The > character allows multi-line text where line breaks in the source file are replaced by spaces in the output.

### In conclusion, if you focus on the syntax, you will save time. 