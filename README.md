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
 - [WebhookInbox](http://webhookInbox.com)


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

*(This will add the webhook subscription for any events where the selected group is a group collaborator. This action also fires a test event to the WebhookInbox we setup earlier.)*

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image05.png)

6) The SurveyBot portal tells us the attempt to post to the webhook was successful

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image03.png)

7) The WebHookInbox.com page tells us that the test webhook was received.

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image00.png)

8) Since you are loading iframes of pages that require authentication, is it required that you open another tab and ensure you have an active login to the [SurveyBot portal](https://golive.gosurveybot.com). **This is required.** 

![enter image description here](https://cdn.gosurveybot.com/Content/img/thesurveybotbunch/image06.png)

9) Download “The SurveyBot Bunch” HTML file.
https://raw.githubusercontent.com/resurvey/TheSurveyBotBunch/master/surveybotbunch.htm

10) Double click top run it from your desktop.

11) Paste in your WebhookInbox Link and press the "Subscribe" button

12) In SurveyBot, jump into a survey for this group

13) Did you see a new live feed appear in one the squares? *Should appear in less than a minute.*

14) Now have 8 more friends jump into surveys in your group, and you have a bunch.


> **Tip:** Check out [the SurveyBot blog](https://gosurveybot.com/blog/) for more mash-ups ideas and sample code 



