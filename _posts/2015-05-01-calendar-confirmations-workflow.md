---
layout: post
title: Calendar Confirmations with Workflow
tags: [workflow]
---

I often want to confirm scheduled meetings from my mobile device.  Depending upon the number, this can take more time than it should ... until now.

Using [Workflow](https://workflow.is/) app automation I built an ***email calendar confirmations workflow*** which speeds up my confirmation processing.

![Workflow Image]({{site.baseurl}}/images/2015-05-01-workflow.png)

<p class="message">

<strong>IMPORTANT!</strong> 
<br><br>
You must install the <a href="https://workflow.is/">Workflow</a> app for iOS before installing the following workflow.  
<br><br>
<em>Read more about the <a href="https://workflow.is/">Workflow</a> app in my <a href="{{ site.baseurl }}/2015/04/06/ios-automation-with-workflow/">previous post</a>.</em>
</p>

**Overview**

1. The **[<i class="fa fa-refresh"></i> email calendar confirmations workflow](https://workflow.is/workflows/dbb3567098d64658ab1b62e0408218dc)** begins by asking for the number of days to search your calendar.  Enter a *number* at the prompt.

1. The workflow continues by searching calendar events matching the date range and displays an event list which matches the criteria.  Select one or more events and click *Done* at the top of the selection dialog.  

1. The workflow will loop through the selected events, composing an email confirmation for each.  If there are participants on the event, their email addresses will display in a selection dialog.  Select one or more recipients from the list to have them automatically added in the ***to*** field of the email and click *Done* to continue.  The calendar event title will be automatically entered as the email subject line.  

1. After the email has been composed it will display for a final inspection.  Modify the email as needed and send.  

1. The processing loop will continue for each selected event until complete.

Click this **[<i class="fa fa-refresh"></i> email calendar confirmations workflow](https://workflow.is/workflows/dbb3567098d64658ab1b62e0408218dc)** link from your iOS device to install the workflow.

**Additional Notes:**

* If you have multiple email accounts configured on your device, remember to select the correct ***from*** sender address in the email dialog.
* Canceling the send of any email in the loop will stop the workflow.
* The [Workflow](https://workflow.is/) app may need authorization to access workflow elements such as your calendar if you've not previously granted premission.

---

**Workflow Variations:**

The previous workflow removes the calendar event's ***year*** value from the confirmation message.  If you need to include it install **[<i class="fa fa-refresh"></i> this workflow](https://workflow.is/workflows/9c8772b340b14feda785c031fc588745)**.

Sometimes I want to highlight the meeting information in **bold** to make sure it stands out in my email.  I've added the capability in **[<i class="fa fa-refresh"></i> this workflow](https://workflow.is/workflows/ff3fcc48fcc64c18953eac6a0350260c)**.

