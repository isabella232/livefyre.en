---
description: 
seo-description: 
seo-title: Livefyre Analytics Events
solution: Experience Manager
title: Livefyre Analytics Events
---

# Livefyre Analytics Events

## Event Object Definition {#section_dh1_yhn_pdb}

The following code defines the fields in the event object that get received by the analytics handler on a page.

```
{
 evars: {
 appId : string : URN ID of the app
 appType : string : Type of the app
 contentType : string : Type of the content that this event pertains to
 contextId : string : URN ID of the contextual item that this event pertains to
 environment : string : Environment that this app is using
 networkId : string : Network that this app is using
 publishedDate : number : Epoch time when the app was published
 userLoggedIn : boolean : If a user is logged in
 },
 generator: {
 env : string: Environment that this app is using
 id : string: URN ID of the app
 name : string: Name of the app
 networkId : string: Network that this app is using
 source : string: URN of the collection
 version : string: Semver version of the app
 },
 startTime : number: Epoch time when event was created
 type : string: Event type (Table 1)
}

```
## Livefyre Analytics Events and eVars {#section_u3k_tft_mcb}

The following Livefyre events to map to custom events to use in reports using the Report Suite Manager. For more information about Report Suites in Adobe Analytics, see [Report Suite Manager](https://marketing.adobe.com/resources/help/en_US/reference/report_suites_admin.html). For more on how to use Livefyre events with Report Suite Manager, see [](c_use_livefyre_with_adobe_analytics.md#c_use_livefyre_with_adobe_analytics/section_iks_kgd_4cb).

<table id="table_n24_1kd_4cb"> 
 <title>Livefyre Analytics Events</title> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry">Event</th> 
    <th class="entry">Description</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Init</td> 
    <td>When a page that includes at least one Livefyre app is loaded</td> 
   </tr> 
   <tr> 
    <td>Load</td> 
    <td>Any time an app was loaded on a page regardless of user view</td> 
   </tr> 
   <tr> 
    <td>View</td> 
    <td>When an app entered the viewport for the first time.</td> 
   </tr> 
   <tr> 
    <td>Post</td> 
    <td>Any time a user posts a comment or a piece of content including ex: top level post, replies, reviews, media wall uploads </td> 
   </tr> 
   <tr> 
    <td>Posted</td> 
    <td>When a post was successsful.</td> 
   </tr> 
   <tr> 
    <td>Twitter_Reply</td> 
    <td>Any time a user replied on Twitter</td> 
   </tr> 
   <tr> 
    <td>Twitter_Like</td> 
    <td>Where content was shared to: Retweet</td> 
   </tr> 
   <tr> 
    <td>Livefyre_Like</td> 
    <td>Any time the livefyre like feature is used in an app</td> 
   </tr> 
   <tr> 
    <td>Livefyre_Unlike</td> 
    <td>Any time a user unlikes a livefyre like </td> 
   </tr> 
   <tr> 
    <td>ShareOnPost</td> 
    <td>Anytime a user posts content and uses the share on post feature</td> 
   </tr> 
   <tr> 
    <td>ShareButtonClick</td> 
    <td>Any time a user clicks on the share button on a comment</td> 
   </tr> 
   <tr> 
    <td>ShareTwitter</td> 
    <td>When Share to Twitter is clicked</td> 
   </tr> 
   <tr> 
    <td>ShareFacebook</td> 
    <td>When Share to Facebook is clicked</td> 
   </tr> 
   <tr> 
    <td>ShareURL</td> 
    <td>When Share to URL text area is selected/copied.</td> 
   </tr> 
   <tr> 
    <td>ExpandReplies </td> 
    <td>When a user clicks on the + or Expand link to view all replies on a top level post</td> 
   </tr> 
   <tr> 
    <td>CollapseReplies </td> 
    <td>When a user clicks on the - or Collapse link to view all replies on a top level post</td> 
   </tr> 
   <tr> 
    <td>FlagClick</td> 
    <td>Any time a user opens the Flag Modal</td> 
   </tr> 
   <tr> 
    <td>FlagSpam</td> 
    <td>When a user flags content as spam</td> 
   </tr> 
   <tr> 
    <td>FlagDisagree</td> 
    <td>When a user flags content as disagree</td> 
   </tr> 
   <tr> 
    <td>FlagOffensive</td> 
    <td>When a user flags content as offensive</td> 
   </tr> 
   <tr> 
    <td>FlagOffTopic</td> 
    <td>When a user flags content as off topic</td> 
   </tr> 
   <tr> 
    <td>FlagCancel </td> 
    <td>Any time a user clicks X or "cancel" when submitting a flag</td> 
   </tr> 
   <tr> 
    <td>FollowCollection</td> 
    <td>Any time a conversation is followed ("I'm interested" in Reviews) </td> 
   </tr> 
   <tr> 
    <td>UnfollowCollection</td> 
    <td>When a conversation is unfollowed</td> 
   </tr> 
   <tr> 
    <td>RequestMore</td> 
    <td>Any time a user loaded more content in an app (needs to be for high velocity too) </td> 
   </tr> 
   <tr> 
    <td>ModalView</td> 
    <td>Any time a user clicks to view content in a modal</td> 
   </tr> 
   <tr> 
    <td>TwitterRetweetClick</td> 
    <td>Where content was shared to: Retweet</td> 
   </tr> 
   <tr> 
    <td>PostButtonClick</td> 
    <td>When a user clicks on the post ("Whats on your mind?") button</td> 
   </tr> 
   <tr> 
    <td>Login</td> 
    <td>Any time a user logged in</td> 
   </tr> 
   <tr> 
    <td>Logout</td> 
    <td>Any time a user logged out</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

The following is a list of conversion variables (eVars) that Livefyre provides.

<table id="table_dvm_pkd_4cb"> 
 <title>Conversion Variables (eVars) </title> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry">Event</th> 
    <th class="entry">Description</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Network ID</td> 
    <td>Network ID/Name in Livefyre</td> 
   </tr> 
   <tr> 
    <td>App ID</td> 
    <td>The URN of the app</td> 
   </tr> 
   <tr> 
    <td>Context ID</td> 
    <td>Content ID in Livefyre</td> 
   </tr> 
   <tr> 
    <td>App Type</td> 
    <td> <p>Livefyre App Type. Options:</p> 
     <ul id="ul_sxl_h1y_12b"> 
      <li> <p>Live Blog</p> <p></p> </li> 
      <li> <p>Feature Card</p> </li> 
      <li> <p>Carousel</p> </li> 
      <li> <p>Chat</p> </li> 
      <li> <p>Comments</p> </li> 
      <li> <p>Filmstrip</p> </li> 
      <li> <p>Storify 2</p> </li> 
      <li> <p>Map</p> </li> 
      <li> <p>Upload Button</p> </li> 
      <li> <p>Mosaic</p> </li> 
      <li> <p>Poll</p> </li> 
      <li> <p>Media Wall</p> </li> 
      <li> <p>Trending</p> </li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td>Content Type</td> 
    <td>Instagram, Twitter, Facebook, LiveFyre, YouTube, etc</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## More Info {#section_b3d_4yl_pdb}

For more information on the topics discussed on this page, see:

* [Report Suite Manager](https://marketing.adobe.com/resources/help/en_US/reference/report_suites_admin.html)
  [DTM](https://marketing.adobe.com/resources/help/en_US/livefyre/c_filmstrip_app.html)
  
  
* [Rules](https://marketing.adobe.com/resources/help/en_US/dtm/rules.html)
  *
  [Livefyre.js](c_reference_livefyre.js_comp.md#topic_hcz_ppx_2cb)
  
  
