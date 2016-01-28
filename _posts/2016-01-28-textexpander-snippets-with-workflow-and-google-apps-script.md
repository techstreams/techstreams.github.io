---
layout: post
title: TextExpander Snippets with Workflow and Google Apps Script
tags: [google-apps-script, workflow]
---

Want to save time typing on iOS?  &nbsp; Use ***[TextExpander](https://smilesoftware.com/textexpander-ios)*** snippets.   &nbsp;&nbsp; Want an easy way to share and automate snippet creation?  &nbsp;Use ***[Workflow](https://workflow.is/)*** and ***[Google Apps Script](https://www.google.com/script/start/)***.

<br>

![Workflow]({{site.baseurl}}/images/2016-01-28-workflow.png)

---

<br>

## TextExpander Overview

> *Type more with less effort on your iPhone or iPad! &nbsp;Expand custom keyboard shortcuts into frequently-used text snippets.*

**[TextExpander](https://smilesoftware.com/textexpander-ios)** is a ***fantastic*** iOS typing shortcut app.  *([Download](https://itunes.apple.com/us/app/textexpander/id917416298) it on the App Store.)*

Common features include the ability to:

* Speed through email, texts, and tweets with the custom keyboard
* Expand formatted text
* Use fill-ins for standard replies
* Organize snippets into groups
* Access snippets in other *[TextExpander Enhanced Apps](https://smilesoftware.com/textexpander-ios/apps)*


Here's a short video overview:

<div class='embed-container'>
	<iframe src="https://www.youtube.com/embed/KXzWWsGMx_g" frameborder=0 allowfullscreen></iframe>
</div>

`~~~`

**[TextExpander](https://smilesoftware.com/textexpander-ios)** also provides the ability to ***[share snippet groups](https://smilesoftware.com/help/touch3/groups.html)***.  

Group sharing is usually accomplished through a local network or public URL ... but *[x-callback-url support](https://smilesoftware.com/textexpander/entry/textexpander-touch-3-5-adds-create-expand-xcallbackurl-support)* opens up other possibilities. 

Following is a **[Google Spreadsheet](https://www.google.com/sheets/about/)** with **[Google Apps Script](https://www.google.com/script/start/)** and an example workflow for the iOS **[Workflow](https://workflow.is/)** app which leverage the *x-callback-url* feature to share and automate snippet creation.

<i class="fa fa-hand-o-right"></i> *For more on __TextExpander__ for iOS, see the [Support Page](https://smilesoftware.com/textexpander-ios/support) and [User Guide](https://smilesoftware.com/help/touch3/index.html).*

<i class="fa fa-hand-o-right"></i> *For more on the __Workflow__ app see [iOS Automation with Workflow](https://techstreams.github.io/2015/04/06/ios-automation-with-workflow/).  &nbsp;(You can __[download](https://itunes.apple.com/app/workflow-powerful-automation/id915249334)__ it on the App Store.)*


---

<br>

![Workflow]({{site.baseurl}}/images/2016-01-28-snippet-server.png)

<br>

**TE Snippet Server**

> A [Google Apps Script](https://www.google.com/script/start/) which shares [TextExpander](https://smilesoftware.com/textexpander-ios) snippets from sheets in a [Google Spreadsheet](https://www.google.com/sheets/about/).  
>
> * Each sheet represents a snippet group 
> 
> * An integrated [Workflow](https://workflow.is/) app workflow accesses shared content and automates snippet creation on iOS
>
> <i class="fa fa-hand-o-right"></i> *Once the Google Apps Script is deployed ... just add new entries or sheets to the Google Spreadsheet to share new snippets!*
>
> `---`
>
> <i class="fa fa-exclamation-circle"></i> The ***Group Name*** in which to add the shared snippets ***must already exist*** in [TextExpander](https://smilesoftware.com/textexpander-ios) and is ***case sensitive***.  
>
> <i class="fa fa-exclamation-circle"></i> When prompted for the snippet ***Group Name*** in the running workflow, ***do not include leading or trailing spaces***.  *The workflow will fail on an invalid Group Name.*
>

<br>


| Workflow | Google Apps Script |
| :--------: | :---------------: |
| **[<i class="fa fa-refresh"></i> TE Snippet Server](https://workflow.is/workflows/5c443da149c748f2adda8338a2ff81b8)** *(Click for workflow install page)* | **[Snippet Server Spreadsheet & Script](https://docs.google.com/spreadsheets/d/1bh2eJEQ_pgqWI_dALaGxBNE585Yq45yliq_j_3Qf998/copy)** *(Click to make a copy of the spreadsheet w/ script in your Google account)* |

<br>

### To customize the Google Apps Script for your environment...

<br>

*  Remember to update the **`ssId`** variable in the Google Apps Script with ***your Google Spreadsheet ID*** before deploying.  *See the code comments for the location of the __`ssId`__ variable.* 

  * <i class="fa fa-hand-o-right"></i> *Execute the __`getSSId()`__ convenience method from the Google Apps Script Editor Run menu to get the Google Spreadsheet ID.*
  
* ***Do not use commas*** in the Google Spreadsheet sheet/tab names.

* See *[Deploying a script as a web app](https://developers.google.com/apps-script/guides/web#deploying_a_script_as_a_web_app)* for more on deploying the *[Google Apps Script](https://www.google.com/script/start/)*.

<br>


### To customize the example workflow for your environment...

<br>

* *[Be sure to replace]({{site.baseurl}}/howto/replace-workflow-urls/)* the ***Google Apps Script URLs*** found in the example workflow with your own.

* The **second Google Apps Script URL** in the example workflow ***requires one parameter*** to be sent back to the deployed Google Apps Script.  *[Take care when replacing]({{site.baseurl}}/howto/replace-workflow-urls/)* with your URL.  

  * <i class="fa fa-hand-o-right"></i>  *Format shoud be __`<your google apps script url>?name=`__ followed by the workflow __`GROUPNAME`__ variable.*


---

<br>

Here's the ***Google Apps Script code*** if you want to **[install the script](https://developers.google.com/apps-script/guides/standalone#creating_a_standalone_script)** manually.

{% gist techstreams/92cf9bdbef3f4e97af15 %}






























