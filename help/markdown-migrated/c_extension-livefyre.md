---
description: Use this reference for information about the options available when using this extension to build a rule.
keywords: Launch;extension;Livefyre;rule
seo-description: Use this reference for information about the options available when using this extension to build a rule.
seo-title: Adobe Livefyre Extension
solution: Analytics,Marketing Cloud,Launch
title: Adobe Livefyre Extension
---

# Adobe Livefyre Extension

Use Adobe Analytics:

Now that apps have been added to pages, we need to create a rule to enable Adobe Analytics tracking. In order to do this, you will need to use the rule system:

EVENTS:

Add the event that will kick off this rule workflow.

Choose "Adobe Livefyre" -&gt; "All User Interactions"

This will track all user interaction events in a similar way within Adobe Analytics. This is useful so that you don't have to set up all of the event types, but if you want more control, that is definitely possible.

ACTIONS:

Now we need to set up the Adobe Analytics actions that will happen once the events are fired.

Choose "Adobe Analytics" -&gt; "Set Variables"

View our documentation about setting up Adobe Analytics with DTM to learn how to set up eVars and events.

The values to use for eVars and events should be determined by how you want the reports to work. You can see a list of all of attributes within the event object here.

Choose "Adobe Analytics" -&gt; "Send Beacon"

Choose the s.tl() option because we don't want to treat every triggered action as a page view. This would incorrectly count page views and would cause reporting problems.

