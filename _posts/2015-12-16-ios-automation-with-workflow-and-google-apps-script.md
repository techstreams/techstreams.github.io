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


***Example Workflow:*** &nbsp; **[<i class="fa fa-refresh"></i> Simple Text Responder](https://workflow.is/workflows/396c0e1228f840c099080e34b079b129)**


***Google Apps Script code:***

```javascript

/**
 * Copyright (c), Laura Taylor. (MIT Licensed)
 * https://techstreams.github.io
 */


/**
 * Simple Google Apps Script Content Server
 * @returns {string}
 */
function doGet() {
  
  // Comma separated list of responses
  var content = "Thank you very much," +
                "See you soon," +
                "Going to be late," +
                "Will call later," +
                "Have a nice day";
  
  return ContentService.createTextOutput(content);
  
}

```

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


***Example Workflow:*** &nbsp; **[<i class="fa fa-refresh"></i> Markdown Server](https://workflow.is/workflows/2e84625a785744e2bd35e29c02bd7423)**


***Google Apps Script code:***

```javascript

/**
 * Copyright (c), Laura Taylor. (MIT Licensed)
 * https://techstreams.github.io
 */


/**
 * Simple Google Apps Script Content Server
 * @param {string} e - Event object
 * @returns {string}
 */
function doGet(e) {
  
  var content;
  
  if (e.parameter.name) {
    // Get content of selected markdown file
    content = HtmlService
                 .createHtmlOutputFromFile(e.parameter.name.trim())
                 .getContent();
  } else {
    // Return a comma separated list of file names
    content = "Example1," +
              "Example2";
  }
  
  return ContentService.createTextOutput(content);
  
}


```

***Example Markdown:*** *([Add to Google Apps Script](https://developers.google.com/apps-script/managing_projects#managing-files-in-a-project) project as an `html` file)*

```

## How to Deploy Google Apps Script for the Workflow App

* **STEP 1:** Create a Google Apps Script Project

* **STEP 2:** Add Script Code

* **STEP 3:** Deploy Google Apps Script

* **STEP 4:** Copy Deployed Script URL for Use in [Workflow](https://workflow.is/) App

---

*See [techstreams.github.io](https://techstreams.github.io/2015/12/16/ios-automation-with-workflow-and-google-apps-script/) for more information.*


```

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


***Example Workflow:*** &nbsp; **[<i class="fa fa-refresh"></i> Custom Emailer](https://workflow.is/workflows/cd4209d46a6a42ae901157b4b9699577)**


***Google Apps Script code:***  *See code for __MARKDOWN SERVER__ example above.*


***Example Email:*** *([Add to Google Apps Script](https://developers.google.com/apps-script/managing_projects#managing-files-in-a-project) project as an `html` file)*

*Note replacement values surrounded by double brackets  &#123; &#123; &nbsp;  &#125; &#125;.*

```

Hello { { customer name } },

Thank you for your recent purchase. 

Please contact our customer service department if you need further assistance.

Best regards,

{ { email signature } }


```


`~~~`

<i class="fa fa-hand-o-right"></i> *In upcoming posts I'll describe more ways I integrate [Workflow](https://workflow.is/) with [Google Apps Script](https://www.google.com/script/start/).*
















