---
description: Use the Moderation tab to set premoderation rules for incoming content, including profanity lists, flag rules, and banned IP addresses.
seo-description: Use the Moderation tab to set premoderation rules for incoming content, including profanity lists, flag rules, and banned IP addresses.
seo-title: Setting Up Moderation
solution: Experience Manager
title: Setting Up Moderation
---

# Setting Up Moderation

## How Moderation Works {#section_kyf_gvc_t1b}

You can moderate content in the following ways:

* Automatically premoderate content to filter out undesired content based on rules you set up before you publish the content.
* Manually delete or approve content that was flagged using the automatic premoderation using the ModQ or App Content in the Library.
* Identify site visitors that repeatedly post offensive content to keep them from posting by banning specific Livefyre users, social users, or IP addresses.
* Identify people and content that can always display by whitelisting users or turning off filters for specific streams, sites, or networks.
You can automatically premoderate content in the following ways:

* Set up rules to automatically flag certain types of content:
    * Set up flag rules for content that is flagged by site visitors flag using `uicontrol Settings &gt; Moderation &gt; Rules`
    * Set up SAFE rules using `uicontrol Settings &gt; Moderation &gt; Rules`
    * Ban specific Twitter users using `uicontrol Settings &gt; Streams`
    * Ban IP addresses using `uicontrol Settings &gt; Bans`
    * Ban IP regions by country code by request. Banned content will be marked as SPAM.
  
* Create a list of words that you consider profanity in the Profanity List under `uicontrol Settings &gt; Moderation &gt; Rules` for your Network or Site.
* Whitelist users (always allow content from these users to display) by using or turning off filters for specific streams, sites, or networks.
After you have set up your profanity lists, SAFE filters, and rules, you can choose whether to premoderate content and apply the SAFE filters in streams. For more information, see [](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules).

Livefyre marks content as `uicontrol Approved`, `uicontrol Pending`, `uicontrol Junk`, etc. depending on where the content comes from, where it will be published, and what rules you have set up in your system. The following table describes the actions Livefyre takes, depending on these factors, in detail.

<table frame="all" rowsep="1" colsep="1" id="table_jcs_wnd_t1b"> 
 <title>How Moderation Works</title> 
 <tgroup cols="3"> 
  <colspec colname="c1" colnum="1" colwidth="1.0*" /> 
  <colspec colname="c2" colnum="2" colwidth="1.0*" /> 
  <colspec colname="c3" colnum="3" colwidth="1.0*" /> 
  <thead> 
   <tr> 
    <th class="entry">Content Comes From:</th> 
    <th class="entry">Sending Content To:</th> 
    <th class="entry">Approval Status</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Library</td> 
    <td>App</td> 
    <td>Content Approved</td> 
   </tr> 
   <tr> 
    <td>Social Search</td> 
    <td>App</td> 
    <td>Content Approved</td> 
   </tr> 
   <tr> 
    <td>Stream Rule</td> 
    <td>App</td> 
    <td> <p>Is content marked as Junk by SAFE filter?</p> 
     <ul id="ul_s4m_r4d_t1b"> 
      <li>No - <a href="#c_setting_up_moderation/section_z5z_w4d_t1b" format="dita">Stream-to-App Moderation Workflow</a></li> 
      <li>Yes - Content Trashed</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td>Library</td> 
    <td>Folder</td> 
    <td>No status (in folder, not published, not trashed)</td> 
   </tr> 
   <tr> 
    <td>Social Search</td> 
    <td>Folder</td> 
    <td>No status (in folder, not published, not trashed)</td> 
   </tr> 
   <tr> 
    <td>Stream Rule</td> 
    <td>Folder</td> 
    <td> <p>Is content marked as Junk by SAFE filter?</p> 
     <ul id="ul_h1n_p4d_t1b"> 
      <li>No - No status (in folder, not published, not trashed)</li> 
      <li>Yes - Content Trashed</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td>App Post</td> 
    <td>App</td> 
    <td> <p>Is content marked as Junk by SAFE filter?</p> 
     <ul id="ul_mkf_t4d_t1b"> 
      <li>No - <a href="#c_setting_up_moderation/section_fwn_w4d_t1b" format="dita">Post-to-App Moderation Workflow</a></li> 
      <li>Yes - Content Trashed</li> 
     </ul> </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Stream-to-App Moderation Workflow {#section_z5z_w4d_t1b}

![](images/stream_to_app_workflow.png)
Before the content from a Stream is published to an App, Livefyre performs the following checks to determine what to do with the content:

1. If SAFE flags the content as junk or drop, Livefyre trashes the content.
1. If SAFE does not flag the content as junk, Livefyre checks to see if premoderation is on.
1. If premoderation is on, Livefyre marks the content as pending.
1. If you set up ModQ rules, then Livefyre sends the content to ModQ.
1. If premoderation is not on, Livefyre checks to see if SAFE flagged the content.
1. If SAFE flagged the content, Livefyre approves the content and publishes the content to the App.
1. If SAFE flags the content and you did not set up SAFE rules, then Livefyre approves the content and publishes the content to the App.
1. If SAFE flags the content and you set up SAFE rules, Livefyre checks if you set up SAFE rules for the Stream.
1. If you set up SAFE rules for the stream, Livefyre approves the content and publishes the content to the App. If you did not set up SAFE rules for the stream, Livefyre uses the moderation SAFE rules to determine how to handle the content (send to ModQ, trash, etc.).
## Post-to-App Moderation Workflow {#section_fwn_w4d_t1b}

![](images/post_to_app_workflow.png)
Before the content from an App post is published to an App, Livefyre performs the following checks to determine what to do with the content:

1. If the SAFE filter flags the content as drop, Livefyre drops the content.
1. If SAFE does not flag the content as drop, Livefyre checks to see if premoderation is on. If premoderation is on, Livefyre marks the content as pending. If you set up ModQ rules, then Livefyre sends the content to ModQ as pending. If not, the content remains in a pending status in App Content in the Library.
1. If premoderation is not on, Livefyre checks to see if SAFE flagged the content. If not, Livefyre approves the content and publishes the content to the App.
1. If SAFE flags the content and you set up SAFE rules, Livefyre uses the SAFE rule to determine how to handle the content (send to ModQ, trash, etc.). If SAFE flags the content and you did not set up SAFE rules, then Livefyre approves the content and publishes the content to the App.
## Bulk Filters {#section_lyk_ktx_vy}

The Bulk Filter looks for repetitive content posted across all Livefyre networks within a short timeframe. If detected, this content is flagged as Bulk, and then trashed by default. While bulk content may be user-generated (such as “Touchdown!” posted repeatedly in a Chat during a popular football game), most originates with spam campaigns. This filter is language-independent, and works with any language. To customize the bulk filter, you must contact Livefyre support.

## Rules {#section_gqz_ksk_f1b}

Use the Rules section to create pre-moderation rules, based on SAFE and user applied flags. This panel offers two types of rules:

* `uicontrol Flag Rules:` specify an action that should be taken on a comment flagged by users a defined number of times.
* `uicontrol SAFE Rules:`combine SAFE flags with actions to take on the flagged content.
To create Flag Rules, select the flag (Offensive, Off Topic, Disagree, or Spam), enter the number of times it must be applied to a piece of content, and select the action to take. You can set one Flag Rule for each flag option (Offensive, Off Topic, Disagree, or Spam).

You can create rules at the Network, Site, and Stream levels. Site level rules inherit network rules, unless you configure Site rules differently. Stream rules inherit Site rules unless you configure them differently.

Available actions:

* `uicontrol Trash it:`sends the flagged comment to the trash.
* `uicontrol Bozo it:` hides the flagged comment from all users, except its writer, to whom it remains visible.
* `uicontrol Pending:` sets the content as pending. If you set Premoderation to ON under `uicontrol Settings &gt; ModQ`, then it will be in the ModQ. Otherwise it will be in App Content only.
>[!NOTE]
>
>Livefyre recommends that you create rules to Bozo comments that are flagged as Spam or Offensive by five users.
## Moderation Recommendations {#section_ec3_vr3_2cb}

You can use moderation recommendations to help you determine how to moderate content posted by site visitors in Livefyre Apps. The Moderation Recommendation Indicator recommends when a piece of content is likely to be trashed, based on what actions you took previously on similar content. To use Moderation Recommendations:
1. Turn on the Moderation Recommendations functionality by contacting your Adobe Livefyre support professional.
   1.
   Set up moderation recommendations in Network Settings.
   
   Set up moderation recommendations using the `uicontrol Livefyre Recommends Trash` setting under `uicontrol Network Settings`.
   
   ![](images/image_mod_reco_trash.png)
   1.
   Set up a SAFE rule to tell Livefyre what to do with content that the moderation recommendation identifies as content that is likely to be trashed. For more information on how to set up a SAFE rule for the `uicontrol Livefyre Recommends Trash` option, see [](c_moderation.md#c_moderation).
   
   
1. Use the `uicontrol Moderation Recommendation Indicator` in the ModQ or in App Content to filter content that the moderation recommendation identifies as likely to be trashed. For more information on how to use Moderation Recommendations to moderate content in ModQ, see [](c_modq.md#c_modq). For more information on how to use Moderation Recommendations in App Content, see [](c_moderate_content_using_app_content.md#c_moderate_content_using_app_content).

