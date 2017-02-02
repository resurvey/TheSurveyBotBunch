Build your own Brady Bunch-like Feed of Ongoing Surveys
===================

Using [SurveyBot Webhooks](https://golive.gosurveybot.com/webhooks "SurveyBot Webhooks") you can easily enable features and integrations only limited by your imagination. This step-by-step guide shows you how you can have a Hollywood Squares-like live feed of all your group's ongoing surveys, as they happen. Let’s get to mashing.

----------


What we are building:
-------------
![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image02.png "what we are building")



Prerequisites:
---------

 - A SurveyBot account ([sign up here](https://gosurveybot.com/)) 

Services we will leverage:
--------------------------

 - SurveyBot Webhooks
 - [WebhookInbox](http://webhookInbox.com) "WebhookInbox receives HTTP requests and
captures the data for later inspection."


Steps
-----

1) Goto http://webhookinbox.com and click “create an inbox”

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image07.png)

2) Once you are taken to your inbox, leave the page open to:
http://webhookinbox.com/view/YOUR_INBOX_ID/

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image04.png)

3) Copy the URL provided:
http://api.webhookinbox.com/i/YOUR_INBOX_ID/in/

4) Login to the SurveyBot, and navigate to the [webhooks page](https://golive.gosurveybot.com/webhooks)

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image01.png)

5) Add the WebhookInbox.com URL from earlier into a new webhook for your group. 

> **Note:** This will add the webhook subscription for any events where the selected group is a group collaborator. This action also fires a test event to the WebhookInbox we setup earlier. 

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image05.png)

6) The SurveyBot portal tells us the attempt to post to the webhook was successful. 

> **Tip:** A click on the spinner may be required to reload the list of webhooks if the page does not auto-update itself. 

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image03.png)

7) The WebHookInbox.com page tells us that the test webhook was received.

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image00.png)

8) Since you are loading HTML iframe tags of pages that require authentication, it is required that you keep another tab open that has an active login to the [SurveyBot portal](https://golive.gosurveybot.com), or that you select "remember me" when you login, thus enabling cookies to maintain your authenticated session even when tabs are closed. **This is required.** 

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image06.png)

9) Download “The SurveyBot Bunch” HTML file to your desktop.
https://github.com/resurvey/TheSurveyBotBunch/archive/master.zip

10) Open the HTML file with a WebRTC capable browser (i.e Chrome or Firefox).

11) Paste in your WebhookInbox Link and press the "Subscribe" button

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image08.png)

12) In SurveyBot, jump into a survey for this group

13) Did you see a new live feed appear in one of the squares? *Should appear in less than a minute.*

14) Now have 8 more friends jump into surveys in your group, and you have a bunch.


> **Tip:** Check out [the SurveyBot blog](https://gosurveybot.com/blog/) for more mash-ups ideas and sample code 

What Next?
------

This is a pointed example of what an organization could do with webhooks to expand what is going on in SurveyBot, with their surveys, into systems and workflow external to SurveyBot. We could and probably will build such a feature into SurveyBot at some point, with some internal APIs and it will be sleeker, but... *this was built with tools that are available to all users*, and that is the power of webhooks were trying to convey. If you were looking for suggestions on where to go from here, we might suggest the following:

A) [Open the HTML file source](https://github.com/resurvey/TheSurveyBotBunch/blob/master/surveybotbunch.htm) and modify the javascript it to consume and drive new workflows off different events


> **Note:** This was the original intent of the exercise, to show folks how little javascript was required, ... but it was hard to not just start making it into a copy and paste solution. Because it was fun to do so, and because there are a demographic of non-developers we wanted to speak to as well. 

B) Combine the use of SurveyBot webhooks w/ the [SurveyBot API](https://golive.gosurveybot.com/apis).
