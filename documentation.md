---
layout: page
title: Documentation
author: Mackenzie Brooks
---

## Contents
{:.no_toc}

* ToC
{:toc}

---

For Ed documentation, see [GitHub](https://github.com/elotroalex/ed/blob/master/documentation.md).

## Why

Why write in this format for this type of site? Why not Wordpress or DSpace or ArchivesSpace? 

Writing in plain text is a preservation strategy. Have you ever had trouble opening an old Word document or other strange file format? Software companies often create their own file formats for use in their applications. If the company goes away, the file format can too. 

Plain text documents contain the text and nothing else. There is no styling or formatting stored in the file. Plain text files don't take up much space and load quickly on phones or weak internet connection. For more, see [Minimal Computing](http://go-dh.github.io/mincomp/).

Applications like Wordpress and ArchivesSpace are powerful, but they are overkill for a website that just wants to provide a clean, reading interface for documents. We use the static site generator [Jekyll](http://jekyllrb.com/) to create Transcriptions @ W&L. Ed is a Jekyll theme for minimal editions. Check out ["How (and Why) to Generate a Static Website Using Jekyll"](http://chronicle.com/blogs/profhacker/jekyll1/60913) of ["Sustainable Authorship in Plain Text using Pandoc and Markdown"](http://programminghistorian.org/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown) for more justification.

---

## Markdown 
Markdown is a syntax for writing plain text documents. Markdown allows you to add basic style and formatting to text that will be published on the web. Think about Markdown as a short-hand for writing, not as something to be read. 

[Markdown Guidelines](https://daringfireball.net/projects/markdown/)

~~~ markdown
# This is a level one heading 
## This a level two heading

*this is italics*
**this is bold**

* list 1
* list 2
* list 3

> this is a
> blockquote
> see? 

*** is a horizontal line
~~~

Ed uses a specifc style of Markdown called [Kramdown](http://kramdown.gettalong.org/syntax.html) to handle footnotes.  

## Transcription Style Guide
What elements will we need to cover?
* Dates
* Corrections
* Text outside of text block

---

## Metadata
Each transcription begins with a block of metadata in a format called YAML - YAML Ain't Markup Language. We can add more metadata categories if need be. 

* Layout - determines the genre/format of the text. 
* Title - title of the text
* Author - author of the text
* Editor - person(s) who transcribed the text
* Rights - statement on intellectual property rights
* Source - institution, collection, record group or collection number
* Categories - select a category from a controlled list
* Publication date - we might want to distinguish between date of creation, date of publication, and date of transcription 

~~~ yaml
---
layout: page
title: "Diary of Frank Smith Reader"
author: Frank Smith Reader
editor: Mackenzie Brooks
rights: Public Domain
source: Washington and Lee Special Collections and Archives
categories: civilwardiaries
publication-date: 2016
---
~~~

---

## Footnotes

Footnotes are possible in the following format:

~~~ markdown

- O Captain! my Captain! rise up and hear the bells; 
- Rise up—for you the flag is flung—for you the bugle[^fn2] trills,

...

[^fn2]: The bugle is a small trumpet implicated in the military industrial complex.
~~~

These footnotes can be placed anywhere, but they will always be generated at the bottom of the document. To have a multi-paragraph footnote you need to start the footnote text on the next line after the footnote anchor and indent it:

---


## Blockquotes

Blockquotes are possible in the following format:

~~~ markdown
> This is to certify that I, the undersigned, have given the bearer, my servant, full liberty to go to Baltimore, and spend the Easter holidays.
>
> Written with mine own hand, &c., 1835.  
> WILLIAM HAMILTON,
~~~

To use a line break in block elements add two spaces after the end of the line where you want the break. You can't see them after `&c., 1835.` but they are there.

