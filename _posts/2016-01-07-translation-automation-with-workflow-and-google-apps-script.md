---
layout: post
title: Translation Automation With Workflow And Google Apps Script
tags: [google-apps-script, workflow]
---

As described in the *[previous post](https://techstreams.github.io/2015/12/16/ios-automation-with-workflow-and-google-apps-script/)*, I'm discovering interesting ways to combine **[Workflow](https://workflow.is/)** and **[Google Apps Script](https://www.google.com/script/start/)**.  

Here's another engaging integration utilizing *[Google Translate](https://translate.google.com/)* to automatically generate *[localized](https://en.wikipedia.org/wiki/Internationalization_and_localization)* content to send as email or share as a PDF from an iOS device.

<i class="fa fa-hand-o-right"></i> *For more on the __Workflow__ app see [iOS Automation with Workflow](https://techstreams.github.io/2015/04/06/ios-automation-with-workflow/).*

<i class="fa fa-hand-o-right"></i> *For more on using [localization](https://en.wikipedia.org/wiki/Internationalization_and_localization) with a [Google Form](https://www.google.com/forms/about/) see [TSFormTranslator](https://techstreams.github.io/2015/04/14/tsformtranslator-overview/).*

---

## Localize Content with Workflow and Google Apps Script

<br>

![Workflows]({{site.baseurl}}/images/2016-01-07-workflows.png)

<br>

The **[Workflow](https://workflow.is/)** app already provides fantastic translation capabilities.  

Here's a simple *standalone* workflow which ...

* Prompts the user for text input
* Detects the origin language
* Translates the text into the selected language
* Prompts the user to share the content as a message, email or share as a PDF  

| Workflow |
| :--------: | 
| **[<i class="fa fa-refresh"></i> Text Translator](https://workflow.is/workflows/3f43d9bc1dca43a1a4b9115a96b9a0f2)** *(Click for install page)*  |

<br>

`~~~`

<br>

With the integration of **[Google Apps Script](https://www.google.com/script/start/)**, I'm able to provide *rich text* localized content to a ***distributed set of [Workflow](https://workflow.is/) users***.


<br>

**CUSTOM TRANSLATOR**

> An example Google Apps Script which supplies localized rich text content to the iOS [Workflow](https://workflow.is/) app to be sent as email or shared as a PDF after prompting for the translation language.
>
> <i class="fa fa-hand-o-right"></i> *Content can include [html](https://en.wikipedia.org/wiki/HTML) for rich text.*
>
> *__Usage Example:__*  
> 
> * *Localized rich text content system for individuals or groups*
>
>  <i class="fa fa-exclamation-circle"></i> *Be sure to replace the __Google Apps Script URLs__ found in the following example workflow with your own.*
>
> <i class="fa fa-exclamation-circle"></i> *The __second Google Apps Script URL__ in the following example workflow requires two parameters to be sent back to the Google Apps Script.  __Take care__ when replacing with your own URL.*
>
> <i class="fa fa-exclamation-circle"></i> *Some inter-language translations may not be supported.*
>

<br>

| Workflow | Google Apps Script |
| :--------: | :---------------: |
| **[<i class="fa fa-refresh"></i> Custom Translator](https://workflow.is/workflows/ad520fad30484a3fa8d63adbf3337d9c)** *(Click for install page)* | **[Custom Translator Script](https://script.google.com/d/1lRVhoir1brlYnXfW70fR6inCwNBr_SjBjmHnl3cmtSansD051lkGmWPI/edit?usp=sharing)** *(Click to make a copy of script)* |

<br>


<i class="fa fa-hand-o-right"></i> *See [Deploying a script as a web app](https://developers.google.com/apps-script/guides/web#deploying_a_script_as_a_web_app) for more on deploying this [Google Apps Script](https://www.google.com/script/start/) example in your environment.*

<br>

---

Here's the ***Google Apps Script code*** if you want to install the script manually.

{% gist techstreams/c99f4f0c88f9c62eadee %}

<br>

<i class="fa fa-hand-o-right"></i> *__Add content__ to the Google Apps Script project as `html` files.  See the __[Custom Translator Script](https://script.google.com/d/1lRVhoir1brlYnXfW70fR6inCwNBr_SjBjmHnl3cmtSansD051lkGmWPI/edit?usp=sharing)__ for examples.*




























