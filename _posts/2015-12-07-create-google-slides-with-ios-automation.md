---
layout: post
title: Create Google Slides With iOS Automation
tags: [drafts, workflow, markdown, google-slides]
---

In the [last post](http://techstreams.github.io/2015/12/02/mind-maps-to-google-slides/) I describe how I create ***[Google Slides](https://www.google.com/slides/about/)*** with one of my favorite [mind mapping](https://en.wikipedia.org/wiki/Mind_map) apps.   In this post, I share two other methods I use to automate presentation creation from my plain text ***[markdown](http://daringfireball.net/projects/markdown/)*** notes.

*  **[Drafts](http://agiletortoise.com/drafts/)** &nbsp; <i class="fa fa-plus"></i> &nbsp;  **[makeSlides](http://toketaware.com/makeslides/)** &nbsp;  <i class="fa fa-arrow-right"></i>&nbsp;   **[Google Slides](https://www.google.com/slides/about/)**

* **[Workflow](https://workflow.is/)** &nbsp;  <i class="fa fa-plus"></i> &nbsp;  **[makeSlides](http://toketaware.com/makeslides/)** &nbsp;  <i class="fa fa-arrow-right"></i> &nbsp;  **[Google Slides](https://www.google.com/slides/about/)**

---


### Overview

The core of my plain text presentation workflow is **[makeSlides](http://toketaware.com/makeslides/)** which can be *[installed](https://itunes.apple.com/us/app/makeslides/id596053822?mt=8)* from the App Store.

> *makeSlides will convert [Markdown](http://daringfireball.net/projects/markdown/), [OPML](http://en.wikipedia.org/wiki/OPML) and Plain Text files into Microsoft PowerPoint format files*

I use *[markdown](http://daringfireball.net/projects/markdown/)* ... so just need to follow a few simple **[makeSlides](http://toketaware.com/makeslides/)** rules when creating my presentation content.

<i class="fa fa-hand-o-right"></i> *For an introductory markdown tutorial, see [Simplify Writing with Markdown](http://techstreams.github.io/2015/09/21/simplify-writing-with-markdown/).*

***makeSlides Markdown Rules:***

> * ***Level 1*** text will become a ***Title Slide***
> * ***Level 2*** text will become the title of a ***Content Slide***
> * ***Level 3 - Level 6 & bullet points*** will become bullet points in the ***Content Slide***
> * All other text will be added to the slide notes
> * Images will be added in appendix slides (where possible)

<i class="fa fa-hand-o-right"></i> *See the [makeSlides web site](http://toketaware.com/makeslides/) for more information.*

Here's a simple markdown example:

```
# Google Slides With iOS Automation

## Method 1

* Drafts
* markdown
* makeSlides

## Method 2

* Workflow
* markdown
* makeSlides

```

<i class="fa fa-exclamation-circle"></i> ***In addition to [makeSlides](https://itunes.apple.com/us/app/makeslides/id596053822?mt=8), you'll need to have the [Google Slides](https://itunes.apple.com/us/app/google-slides/id879478102?mt=8) app installed.***

<br>

Once my markdown content has been created in **[Drafts](http://agiletortoise.com/drafts/)** or **[Workflow](https://workflow.is/)** *(see below)*, the **[makeSlides](https://itunes.apple.com/us/app/makeslides/id596053822?mt=8)** app is called and ***automatically*** creates a PowerPoint *.pptx* presentation with the passed markdown content.   

Here's how to ***easily*** save and convert the PowerPoint *.pptx* presentation to **[Google Slides](https://www.google.com/slides/about/)**.

<br>

***Save & Convert PowerPoint to Google Slides***

![Save Presentation]({{site.baseurl}}/images/2015-12-07-save-presentation.png)


1) From **[makeSlides](https://itunes.apple.com/us/app/makeslides/id596053822?mt=8)**, tap the **Share** button in the top right corner.

2) Locate and tap **Copy to Slides**.  *This will automatically open the [Google Slides](https://itunes.apple.com/us/app/google-slides/id879478102?mt=8) app.*  Tap **__Save to Drive__**.

3) Locate and open the newly created PowerPoint *.pptx* presentation in the [Google Slides](https://itunes.apple.com/us/app/google-slides/id879478102?mt=8) app.

4) In the top right, tap the **<i class="fa fa-ellipsis-v"></i>** icon.

5) Tap **<i class="fa fa-question-circle"></i>** next to **Office Compatibility Mode**.

6) Tap **Save as Google Slides** button to convert the PowerPoint presentation to the **[Google Slides](https://www.google.com/slides/about/)** format.

<i class="fa fa-pencil-square-o"></i>  *Use the __[Google Slides](https://itunes.apple.com/us/app/google-slides/id879478102?mt=8)__ app or the __[Google Slides web interface](https://docs.google.com/presentation)__ to edit, format, share & present the slides.*

---

### How To Create Google Slides

> ... *with [Drafts](http://agiletortoise.com/drafts/) and [makeSlides](http://toketaware.com/makeslides/)*


<br>

![Drafts]({{site.baseurl}}/images/2015-12-07-drafts.png)

<br>


**STEP 1**

Install the following apps on your iOS mobile device:

* [Drafts](https://itunes.apple.com/us/app/drafts-4-quickly-capture-notes/id905337691?mt=8)
* [makeSlides](https://itunes.apple.com/us/app/makeslides/id596053822?mt=8)
* [Google Slides](https://itunes.apple.com/us/app/google-slides/id879478102?mt=8) *(& [Google Drive](https://itunes.apple.com/us/app/google-drive-free-online-storage/id507874739?mt=8) )*


<i class="fa fa-hand-o-right"></i> *For more on __Drafts__ see [iOS Automation with Drafts](http://techstreams.github.io/2015/09/03/ios-automation-with-drafts/).*


`~~~`

**STEP 2**

After app installation:

* Install the **[GSlides Drafts Action](https://drafts4-actions.agiletortoise.com/a/1b2)** from the *[Drafts Action Directory](https://drafts4-actions.agiletortoise.com)*.

`~~~`

**STEP 3**

Enter presentation markdown content into **Drafts** using markdown. 

<i class="fa fa-exclamation-circle"></i> Be sure to follow the ***makeSlides Markdown Rules*** detailed above.

<i class="fa fa-hand-o-right"></i> *For more on editing in Drafts, see the [Basics of Navigating Drafts](https://agiletortoise.zendesk.com/hc/en-us/articles/203530077-Basics-Navigating-Drafts).*


`~~~`

**STEP 4**

In **Drafts**, run the installed **[GSlides Drafts Action](https://drafts4-actions.agiletortoise.com/a/1b2)** on the completed markdown content.


When the action runs, you'll be prompted for the **Presentation Title**.  *Enter the desired title or leave the default.*

The action will automatically open the **[makeSlides](https://itunes.apple.com/us/app/makeslides/id596053822?mt=8)** app and create a PowerPoint *.pptx* presentation.


`~~~`

**STEP 5**

Follow the ***Save & Convert PowerPoint to Google Slides*** section above to save and convert the presentation in **[Google Slides](https://www.google.com/slides/about/)**.


---

### How To Create Google Slides

> ... *with [Workflow](https://workflow.is/) and [makeSlides](http://toketaware.com/makeslides/)*

<br>

![Drafts]({{site.baseurl}}/images/2015-12-07-workflow.png)


<br>

**STEP 1**

Install the following apps on your iOS mobile device:

* [Workflow](https://itunes.apple.com/us/app/workflow-powerful-automation/id915249334?mt=8)
* [makeSlides](https://itunes.apple.com/us/app/makeslides/id596053822?mt=8)
* [Google Slides](https://itunes.apple.com/us/app/google-slides/id879478102?mt=8) *(& [Google Drive](https://itunes.apple.com/us/app/google-drive-free-online-storage/id507874739?mt=8) )*

<i class="fa fa-hand-o-right"></i> *For more on __Workflow__ see [iOS Automation with Workflow](http://techstreams.github.io/2015/04/06/ios-automation-with-workflow/).*

`~~~`

**STEP 2**

After app installation, install and run the **[GSlides](https://workflow.is/workflows/74367f2c5b95450b835810254a2f8754)** workflow.

You'll be prompted for presentation markdown content.  *Be sure to follow the __makeSlides Markdown Rules__ detailed above.*

Next, you'll be prompted for a **Presentation Title**.  *Enter the desired title or leave the default.*

The action will automatically open the **[makeSlides](https://itunes.apple.com/us/app/makeslides/id596053822?mt=8)** app and create a PowerPoint *.pptx* presentation.

`~~~`

**STEP 3**

Follow the ***Save & Convert PowerPoint to Google Slides*** section above to save and convert the presentation in **[Google Slides](https://www.google.com/slides/about/)**.








