---
layout: post
title: Create Impressive PDFs With iOS Automation
tags: [drafts, workflow, markdown]
---

I love iOS automation.  There are so many amazing possiblities.  

In a [previous post](http://techstreams.github.io/2015/10/01/create-impressive-google-docs-on-the-go/), I detailed an ***Impressive Google Docs*** workflow I created using [Drafts](http://agiletortoise.com/drafts/), [Markdown](https://daringfireball.net/projects/markdown/) and [Google Fonts](https://www.google.com/fonts#AboutPlace:about).

<blockquote class="twitter-tweet" lang="en"><p lang="en" dir="ltr">Clever, flexible Google Doc action (with good write up) from <a href="https://twitter.com/techstreams">@techstreams</a>: <a href="http://t.co/b42FNKIgvP">http://t.co/b42FNKIgvP</a></p>&mdash; Drafts (@draftsapp) <a href="https://twitter.com/draftsapp/status/649912882247827456">October 2, 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>

Combining a modified version of this [original Drafts action](http://drafts4-actions.agiletortoise.com/a/19v) with an *action extention workflow* developed with the [Workflow](https://workflow.is/) app, I'm now able to create **Impressive PDFs**.  

Interested?  Read on. 

---

### How To Create Impressive PDFs 

> ... *with Drafts, Markdown, Google Fonts and Workflow*

<br>

![]({{site.baseurl}}/images/2015-11-13-impressive-pdf.png)

<br>


**STEP 1**

Install the following apps on your iOS mobile device:

* [Drafts](https://itunes.apple.com/us/app/drafts-4-quickly-capture-notes/id905337691?mt=8)
* [Workflow](https://itunes.apple.com/us/app/workflow-powerful-automation/id915249334?mt=8)

<i class="fa fa-hand-o-right"></i> *For more on __Drafts__ see [iOS Automation with Drafts](http://techstreams.github.io/2015/09/03/ios-automation-with-drafts/).*

<i class="fa fa-hand-o-right"></i> *For more on __Workflow__ see [iOS Automation with Workflow](http://techstreams.github.io/2015/04/06/ios-automation-with-workflow/).*

`~~~`

**STEP 2**

After app installation:

* Install the **[Impressive PDFs Drafts Action](https://drafts4-actions.agiletortoise.com/a/1a1)** from the *[Drafts Action Directory](https://drafts4-actions.agiletortoise.com)*
* Install the **[HTML to PDF](https://workflow.is/workflows/35d87231e09f4a6f9d11bdca0a2510b7)** workflow

<i class="fa fa-exclamation-triangle"></i> *Ensure that there are no other workflows with the name __HTML to PDF__ resident within the [Workflow](https://workflow.is/)  app or you may encounter an issue.*



`~~~`

**STEP 3**

Enter document content into **Drafts** using markdown. 

Looking for an example?  Try this markdown:

```
# Test PDF

---

It's easy to create ***Impressive PDFs*** with:

* Drafts
* Markdown
* Google Fonts
* Workflow

---

### Try A Table

| Column 1 | Column 2 |
| :------: | :------: |
| One      | Two      |
| Three    | Four     |


```

<i class="fa fa-hand-o-right"></i> *For an introductory markdown tutorial, see [Simplify Writing with Markdown](http://techstreams.github.io/2015/09/21/simplify-writing-with-markdown/).*

<i class="fa fa-hand-o-right"></i> *For more on editing in Drafts, see the [Basics of Navigating Drafts](https://agiletortoise.zendesk.com/hc/en-us/articles/203530077-Basics-Navigating-Drafts).*

<i class="fa fa-hand-o-right"></i> *If you need better document element separation/spacing, use the `<br>` line break tag between elements when creating your markdown content. To assist, I’ve created a convenient `<br>` [Drafts Key](https://agiletortoise.zendesk.com/hc/en-us/articles/202865034-Using-the-Enhanced-Keyboard) which can be installed from __[here](http://drafts4-actions.agiletortoise.com/k/19h)__.*




`~~~`

**STEP 4**

In **Drafts**, run the installed **[Impressive PDFs Drafts Action]()** on the completed markdown content.

<i class="fa fa-hand-o-right"></i> *See the [Basics of Navigating Drafts](https://agiletortoise.zendesk.com/hc/en-us/articles/203530077-Basics-Navigating-Drafts) for more information on running Drafts Actions.*

![]({{site.baseurl}}/images/2015-11-13-drafts-action.png)

<br>

When the action runs, you'll be prompted for ***three*** items:

**1) [Google Font](https://www.google.com/fonts) to use for document styling**

> Enter the desired [Google Font](https://www.google.com/fonts) name or leave the default _[Roboto](https://www.google.com/fonts/specimen/Roboto)_ font.

> In addition to *[Roboto](https://www.google.com/fonts/specimen/Roboto)*, here are a few of my other favorite fonts:

> * *[Muli](https://www.google.com/fonts/specimen/Muli)*
> * *[Lobster](https://www.google.com/fonts/specimen/Lobster)*
> * *[Indie Flower](https://www.google.com/fonts/specimen/Indie+Flower)*
> * *[Architects Daughter](https://www.google.com/fonts/specimen/Architects+Daughter)*

> <i class="fa fa-exclamation-triangle"></i> *Not all Google Fonts may be supported.*

> <i class="fa fa-exclamation-triangle"></i> *Google Font thickness, slant and width are not supported by this action.*

**2) Document headings color**

> Enter the name of a color *(e.g., red)* or an [html color hex code](http://www.w3schools.com/html/html_colors.asp) *(e.g., #FF0000 for red)*.   ***Leave #000000 for the default color black.*** 

> <i class="fa fa-hand-o-right"></i> *Document headings are created with markdown.  See the [Simplify Writing with Markdown](http://techstreams.github.io/2015/09/21/simplify-writing-with-markdown/) post for additional information.*


**3) Document body text color**

> Enter the name of a color *(e.g., red)* or an [html color hex code](http://www.w3schools.com/html/html_colors.asp) *(e.g., #FF0000 for red)*.   ***Leave #000000 for the default color black.*** 


After completing each prompt:

* Press the **OK** button to continue  
* Press the **Cancel** button to exit and return to **Drafts**


`~~~`

**STEP 5**

The **[Impressive PDFs Drafts Action](https://drafts4-actions.agiletortoise.com/a/1a1)** will now ***automatically*** pass the document content to the **[HTML to PDF](https://workflow.is/workflows/35d87231e09f4a6f9d11bdca0a2510b7)** workflow to create the PDF.

![]({{site.baseurl}}/images/2015-11-13-workflow.png)

<br>

When the workflow runs:

**1) A _Preview_ will display once PDF generation is complete**

> Click the **Done** link in the top left corner to continue.

**2) You will be prompted for a name for the generated PDF**

> Enter a new name or leave the *default* value.

> Press **OK** to continue.  Press **Cancel** to exit the workflow and return to **Drafts**.

**3) An _Action_ prompt will display**

> * *__Share:__ select to share PDF (e.g., email, message, ...)*
> * *__Open In App:__ select to open PDF in another app (e.g., [Google Drive](https://itunes.apple.com/us/app/google-drive-free-online-storage/id507874739?mt=8), [Evernote](https://itunes.apple.com/us/app/evernote/id281796108?mt=8), [Dropbox](https://itunes.apple.com/us/app/dropbox/id327630330?mt=8), [iBooks](http://www.apple.com/ibooks/), ...)*
> * *__Cancel:__ cancel workflow*

You will be returned to **Drafts** once the workflow is complete.









