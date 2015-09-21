---
layout: post
title: Simplify Writing with Markdown
tags: [markdown]
---


It occurred to me recently that I use ***markdown*** to simplify most of my writing/publishing workflows, so I thought it would be a good idea to share a quick tutorial for others who might be interested. 

![Markdown]({{ site.baseurl }}/images/2015-09-21-markdown.png)

<br>

<i class="fa fa-hand-o-right"></i> ***Before I begin though, a quick introduction...***


### What is markdown? 

[Markdown](https://daringfireball.net/projects/markdown/) is a [plain text markup format](https://en.wikipedia.org/wiki/Markup_language) created by [John Gruber](https://daringfireball.net/)</a>.

Markdown converts easily to formatted [HTML](https://en.wikipedia.org/wiki/HTML) which makes it a great tool for writing and publishing.

In addition to the original version, there are several markdown variations:

* [MultiMarkdown (MMD)](https://github.com/fletcher/MultiMarkdown/wiki/MultiMarkdown-Syntax-Guide)
* [Github Flavored Markdown (GFM)](https://help.github.com/articles/github-flavored-markdown/)

### What are the benefits of markdown?

* It's ***easy*** to learn
* It ***significantly speeds up*** writing/publishing workflows
* It can be created, edited and stored on a variety of platforms and devices because it's ***just plain text***
* An increasing number of writing tools and services support it as a ***primary format***

### Markdown workflow examples? 

I use markdown to:

* Write all posts for this blog
* Create, send and reuse emails from [Google Docs](https://www.google.com/docs/about/) with my [TSMarkMail Google Doc Add-on]({{ site.baseurl }}/2015/03/27/tsmarkmail-overview/)
* Initiate many of my [Drafts app workflows]({{ site.baseurl}}/2015/09/03/ios-automation-with-drafts/)
* Initiate many of my [Workflow app workflows]({{ site.baseurl}}/2015/04/06/ios-automation-with-workflow/)
* Write documentation for my [Github projects](https://github.com/techstreams)
* Write ebooks and documentation with [Gitbook](https://www.gitbook.com/)

<i class="fa fa-sticky-note"></i> *I plan to share some of my favorite writing/publishing workflow details in upcoming posts.*

<br>

<i class="fa fa-hand-o-right"></i> ***Now for the tutorial...***

In the interest of time, I'll only be highlighting markdown elements I use most frequently:

* Paragraph 
* Text Emphasis
* Headings
* Blockquote
* List
* Horizontal Rule
* Link
* Image
* Table 
* Code


<br>

---

<br>


## Paragraph

* Begin markdown paragraph text at the left margin.

* Separate paragraphs from other markdown elements *(including other paragraphs)* with one or more blank lines.

* *Lines of text within a paragraph are continuous. To separate lines within the same paragraph, add __two space characters__ to the end of the previous line.*

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_paragraph.md %}

<br>

---

<br>

## Text Emphasis

* Markdown text emphasis can be inserted *inline* and does not need to begin at the left margin.

* Create emphasis by surrounding text with special symbols.

* To display text as **Bold**, surround text in:
  * two consecutive asterisks `**`
  * two consecutive underscores `__`


* To display text as *Italics*, surround text in:
  * a single asterisk `*`
  * a single underscore `_`

* To display text in ***Bold Italics***, surround text in:
  * three consecutive astersks `***`
  * three consecutive underscores `___`

* To display text as ~~Strikethrough~~, surround text in:
  * two consecutive tildas `~~`

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_text_emphasis.md %}

<br>

---

<br>

## Headings

* There are **six levels** of headings possible in markdown. 

* Begin markdown headings at the left margin.

* Create a heading by entering the `#` symbol followed by a space character and the heading text. 

* Enter the number of `#` symbols per heading level.

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_headings.md %}

<br>

---

<br>

## Blockquote

* Begin markdown blockquotes at the left margin.

* Create a blockquote by entering a `>` symbol followed by a space character and the blockquote text. 

* Blockquotes can also be nested by entering consecutive `>` symbols.

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_blockquote.md %}

<br>

---

<br>

## List

Markdown supplies both ***Ordered*** and ***Unordered*** lists.

* **Ordered List:**

  * Begin a markdown list item at the left margin.

  * Enter the list item number followed by a `.` symbol followed by a space character and the item text. 

  * *Each list item can also be numbered with `1.`and the correct list number will be displayed.* 

  * Lists can be ***nested*** by including a ***two space character indention***.

* **Unordered List:**

  * Begin a markdown list item at the left margin.

  * Type a `*`, `-` or `+` symbol followed by a space character and the item text. 

  * Lists can be ***nested*** by including a ***two space character indention***.

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_list.md %}

<br>

---

<br>

## Horizontal Rule

* Begin a markdown horizontal rule at the left margin.

* Create a horizontal rule (line break) by entering:
  * three consecutive underscores `___`
  * three consecutive dashes `---`
  * three consecutive asterisks `***`

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_horizontal_rule.md %}


<br>

---

<br>

## Link

* Markdown links can be inserted *inline* in text and do not need to begin at the left margin.

* Add links by entering ***link text*** enclosed in `[]` symbols followed by the ***full link url*** enclosed in `()` symbols.

  * Example: `[Link Text](http://someurl)`

  * Example *with link title*: `[Link Text](http://someurl "Link Title")`

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_link.md %}

<br>

---

<br>

## Image

* Markdown images can be inserted *inline* in text and do not need to begin at the left margin.

* Add images by entering a `!` symbol followed by the ***image alt text*** enclosed in `[]` symbols followed by the ***full url of the image*** enclosed in `()` symbols.

  * Example: `![Image Alt Text](http://someimageurl)`

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_image.md %}

<br>

---

<br>

## Table

* Begin a markdown table at the left margin.

* Tables can be created by adding pipe dividers (`|` symbol) between each ***table cell***.

  * **Table Header vs Table Body** - separate the table *header row* from *table body rows* by adding a row of cells containing dashes

  * **Text Alignment Within Table Column** - include colon `:` symbols within the dash row to define *left-aligned, right-aligned, or center-aligned* text in table body cells

  * **Inline Markdown** - table cell text can include *inline markdown*  such as Links and Text Empahsis *(see corresponding elements above)*

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_table.md %}


<br>

---

<br>


## Code

* Code snippets can be included in markdown.
  * **Inline Code** - wrap inline code with backtick <code>`</code> symbols
  * **Indented Code** - indent code blocks with ***4 space characters***
  * **Fenced Code Blocks** - wrap code with backtick <code>```</code> symbols to create a ***multi-line block of code***

<br>

{% gist techstreams/2240e7de0840bc8ec218 md_code.md %}







