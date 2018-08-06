---
description: Use this reference for information about configuring the Adobe Livefyre extension and the options available when using this extension to build a rule.
keywords: Launch;extension;Livefyre;rule
seo-description: Use this reference for information about configuring the Adobe Livefyre extension and the options available when using this extension to build a rule.
seo-title: Configure the Adobe Livefyre Extension
solution: Analytics,Marketing Cloud,Launch
title: Configure the Adobe Livefyre Extension
uuid: 5c4e6f45-7115-4356-af07-cf5646b1b903
index: y
internal: n
snippet: y
translate: y
---

# Configure the Adobe Livefyre Extension

If the Adobe Livefyre Launch extension is not yet installed, open your property, then click ** ` Extensions > Catalog` **, hover over the Livefyre extension, and click ** ` Install` **.
To configure the extension:

1. Open the ** ` Extensions` ** tab
1. Hover over the extension
1. Click ** ` Configure` **.
![](images/launch_lf_extension.png) To use the Adobe Livefyre Launch extension, you must have:

* Livefyre license
* networkId
**Settings**
** ` Livefyre network` **. Enter your ` networkId` in the Network in the form: . This enables other sections within the extension to process properly.
** ` Exclude specific paths.` ** Enter the name of any paths you want to exclude from using the Livefyre extension. 
Set up a rule for Livefyre.

1. In the Adobe Launch Livefyre extension, click **Rules**.
1. Add a new rule or click on an existing one to edit it.
1. Enter one or more events in the **If** portion of the rule. For a list of events you can use, see Events.Add the event that will kick off this rule workflow. This will cause the rule to run once the library is loaded on the page.
   Load an app on a page with the Livefyre extension without Adobe Analytics.
   Choose ** ` Core > Library Loaded (Page Top)` **.
   <!-- Need to link to the events listed in this document. hrk 5/21/18 -->
1. Do not add any exceptions to the rule.
1. Add the page path condition to determine which page is being targeted: 
    * Choose ** ` Extension:` **Core
    * Choose ** ` Condition Type:` ** Path And Query String.
    * Add the path of the page where the App will be loaded in the ** ` Path` ** field.

1. Set up the Livefyre Load App action which will handle loading the App on the page.
Choose ** ` Adobe Livefyre > Load App` **.
**EVENTS:**
This section describes the event types available in the Livefyre extension.
The Livefyre extension provides the following events in the If portion of a rule:

* **App Initialized.** When an App is included on a page.
* **App Loaded.** When an App was loaded on a page regardless of position.
* **All User Interactions.** A consolidation of all the events in the list that are actions users perform.
* **Show Modal.** When user clicks to view Media Wall content in a larger modal window.
* **Request More Content.** When user loads more content in an App.
* **Share Button Click.** Any time a user clicks on the share button on an App card.
* **Twitter Retweet Click.** When a user clicks the Twitter Retweet button from an App.
* **Share to Twitter.** When a user clicks the Twitter Like/Favorite button from an App.
* **Share URL.** When Share to URL text area is selected/copied from an App.
* **Twitter Like Click.** When a user clicks the Twitter Like/Favorite button from an App.
* **Twitter Reply Click.** When a user clicks the Twitter Reply button from an App.
* **Share to Facebook.** When Share to Facebook is clicked from an App.
**ACTIONS:**
The Livefyre extension provides the following actions in the Then portion of a rule:
App ID: The ID of the App to load. To get or create an App, navigate to the ** ` Apps` ** section in Livefyre. Here is the documentation for managing Apps: https://marketing.adobe.com/resources/help/en_US/livefyre/c_create_an_app.html. Once you have created an App, navigate to the App and you will see App ID under the ** ` Developer Info` ** section on the right.
Selector: A CSS selector that chooses an element within the destination page where the app will be loaded.
Use with new/existing embeds on a page
Supporting new/existing embeds is extremely easy. Once you add the Launch JavaScript to the page, all embeds that currently exist will continue to work and new ones will be able to be easily added.
Here is an example of an existing App embed:

```
<script type="text/javascript" src="https://cdn.livefyre.com/Livefyre.js"> 
</script><div class="lf-app-embed" data-lf-app="ae260092-4239-43d9-b403- 
08b923136701/tagged/published" data-lf-env="qa" data-lf-read-only=""></div> 
<script>Livefyre.require(["https://livefyre-cdn- 
qa.s3.amazonaws.com/libs/app-embed/v1.0.10/app-embed.min.js"], function  
(appEmbed) {appEmbed.loadAll().done(function(embed) {embed = embed[0];if  
(embed.el.onload &amp;&amp; embed.getConfig)  
{embed.el.onload(embed.getConfig());}});});</script>
```
With the Livefyre Launch extension, this can be simplified to:

```
<div class="lf-app-embed" data-lf-app="ae260092-4239-43d9-b403- 
08b923136701/tagged/published" data-lf-env="prod" data-lf-read-only=""> 
</div>
```
The Livefyre.js script is included in the extension. The Livefyre.js script can find all of the embed elements on the page and instantiate the Apps for them.
For information on how to create an App in Adobe Livefyre, see [](c_create_an_app.md#concept_isg_4jt_bbb).
Enable an Adobe Analytics Tracking Rule

1. Add an App to a page. For more on how to do this, see [](c_create_an_app.md#concept_isg_4jt_bbb).
1. Choose or create a rule for your ** ` Property` ** in the Adobe Launch Livefyre extension to enable Adobe Analytics tracking.
1. Add an event that kicks off the rule workflow.
1. Choose ** ` Adobe Analytics > Set Variables` ** to set up the Adobe Analytics actions that happen after the events are fired. For more about how to set up Adobe Analytics with DTM and how to set up eVars and events, see .
1. Set the values to use for eVars and events to determine how you want the reports to work. You can see a list of all of attributes within the event object here.
1. Set the Action to ** ` Adobe Analytics > Send Beacon` **.Choose ` s.tl()` to not treat each triggered action as a page view and incorrectly count page views in reports.

Events:
Choose ** ` Adobe Livefyre > All User Interactions` ** to track all user interaction events in Adobe Analytics. 
you don't have to set up all of the event types, but if you want more control, that is definitely possible.
