---
layout: post
title: iOS Automation With Workflow And Google Apps Script
tags: [google-apps-script, workflow, markdown]
---

**[Workflow](https://workflow.is/)** is such an incredibly useful iOS app.  And by integrating ***[Google Apps Script](https://www.google.com/script/start/)*** ... I can **dynamically generate content** for my own workflows *OR* provide workflow automation content to a **group of users**.

---

## Workflow and Google Apps Script

<br>

![Workflows]({{site.baseurl}}/images/2015-12-16-workflows.png)

<br>

**Let's explore _three_ interesting ways** to integrate the **[Workflow](https://workflow.is/)** app with **[Google Apps Script](https://www.google.com/script/start/)**.

<i class="fa fa-hand-o-right"></i> *For more on the __Workflow__ app see [iOS Automation with Workflow](https://techstreams.github.io/2015/04/06/ios-automation-with-workflow/).*

<i class="fa fa-hand-o-right"></i> *See [Creating a standalone script](https://developers.google.com/apps-script/guides/standalone#creating_a_standalone_script) and  [Deploying a script as a web app](https://developers.google.com/apps-script/guides/web#deploying_a_script_as_a_web_app) for more on deploying these [Google Apps Script](https://www.google.com/script/start/) examples in your environment.*


`~~~`


**SIMPLE TEXT RESPONDER**

> An example Google Apps Script which supplies a set of commonly used responses to [Workflow](https://workflow.is/) to create a select list for quick messaging.
>
> *__Usage Example:__*
>
> * *Message repository for individuals or groups*
>
>  <i class="fa fa-exclamation-circle"></i> *__[Be sure to replace]({{site.baseurl}}/howto/replace-workflow-urls/)__ the __Google Apps Script URLs__ found in the following example workflow with your own.*

<br>


| Workflow |
| :--------: | 
| **[<i class="fa fa-refresh"></i> Simple Text Responder](https://workflow.is/workflows/396c0e1228f840c099080e34b079b129)** *(Click for workflow install page)*  |


***Google Apps Script code:***

<script src="https://gist.github.com/techstreams/ba6e8216cbc8ed1c4008.js"></script>

<br>

`~~~`

**MARKDOWN SERVER**

> An example Google Apps Script which supplies a set of markdown files to [Workflow](https://workflow.is/) to be converted into email or used to create PDFs.
>
> <i class="fa fa-hand-o-right"></i> *For an introductory markdown tutorial, see [Simplify Writing with Markdown](https://techstreams.github.io/2015/09/21/simplify-writing-with-markdown/).*
>
> *__Usage Examples:__*
> 
> * *Frequently used email responses*
> * *Simple self-help system for individuals or groups*
> * *FAQ repository for help-desk personnel*
>
>  <i class="fa fa-exclamation-circle"></i> *__[Be sure to replace]({{site.baseurl}}/howto/replace-workflow-urls/)__ the __Google Apps Script URLs__ found in the following example workflow with your own.*
>
> <i class="fa fa-exclamation-circle"></i> *The __second Google Apps Script URL__ in the following example workflow __requires a parameter__ to be sent back to the Google Apps Script.  __[Take care when replacing]({{site.baseurl}}/howto/replace-workflow-urls/)__ with your own URL.*

<br>

| Workflow |
| :--------: | 
| **[<i class="fa fa-refresh"></i> Markdown Server](https://workflow.is/workflows/2e84625a785744e2bd35e29c02bd7423)** *(Click for workflow install page)*  |


***Google Apps Script code:***

<script src="https://gist.github.com/techstreams/ed07d47d83cb5649ed59.js"></script>

<br>

***Example Markdown:*** 

<i class="fa fa-hand-o-right"></i>  *[Add to Google Apps Script](https://developers.google.com/apps-script/managing_projects#managing-files-in-a-project) project as an `html` file.*

<script src="https://gist.github.com/techstreams/320c77e7b9a6f003fb4a.js"></script>

<br>

`~~~`


**CUSTOM EMAILER**

> An example Google Apps Script which supplies custom templates to [Workflow](https://workflow.is/) to be converted into email after prompting for replacement fields.
>
> *__Usage Examples:__*  
> 
> * *Custom email response system for individuals or groups*
>
>  <i class="fa fa-exclamation-circle"></i> *__[Be sure to replace]({{site.baseurl}}/howto/replace-workflow-urls/)__ the __Google Apps Script URLs__ found in the following example workflow with your own.*
>
> <i class="fa fa-exclamation-circle"></i> *The __second Google Apps Script URL__ in the following example workflow __requires a parameter__ to be sent back to the Google Apps Script.  __[Take care when replacing]({{site.baseurl}}/howto/replace-workflow-urls/)__ with your own URL.*

<br>

| Workflow |
| :--------: | 
| **[<i class="fa fa-refresh"></i> Custom Emailer](https://workflow.is/workflows/cd4209d46a6a42ae901157b4b9699577)** *(Click for workflow install page)*  |


***Google Apps Script code:*** 

<script src="https://gist.github.com/techstreams/ed07d47d83cb5649ed59.js"></script>

<br>

***Example Email:***

<i class="fa fa-hand-o-right"></i> *[Add to Google Apps Script](https://developers.google.com/apps-script/managing_projects#managing-files-in-a-project) project as an `html` file.*

<i class="fa fa-hand-o-right"></i> *Note replacement values surrounded by double brackets  &#123; &#123; &nbsp;  &#125; &#125;.*

<script src="https://gist.github.com/techstreams/475710470e6a2ea98c13.js"></script>


`~~~`

<i class="fa fa-hand-o-right"></i> *In upcoming posts I'll describe more ways I integrate [Workflow](https://workflow.is/) with [Google Apps Script](https://www.google.com/script/start/).*
















