---
layout: howto
title: How to Replace Google Apps Script Workflow URLs
---

<br>

To use a different **[Google Apps Script](https://www.google.com/script/start/)** in a **[Workflow](https://workflow.is/)**, replace the script URL(s) with yours as shown below.

<i class="fa fa-hand-o-right"></i> *See [Deploying a script as a web app](https://developers.google.com/apps-script/guides/web#deploying_a_script_as_a_web_app) for more on how to locate your Google Apps Script URL.*

![Workflows]({{site.baseurl}}/images/workflow-replace-url.png)

`~~~`

If the Google Apps Script URL requires parameters, **append** the ***`?` character*** and any ***following parameter information from the original url*** to the end of your script URL.

![Workflows]({{site.baseurl}}/images/workflow-url-params.png)