---
description: Use Javascript events to listen for events that occur in a Media Wall and send them to the analytics tool of your choice.
seo-description: Use Javascript events to listen for events that occur in a Media Wall and send them to the analytics tool of your choice.
seo-title: Javascript Events for Media Wall
solution: Experience Manager
title: Javascript Events for Media Wall
---

# Javascript Events for Media Wall

Livefyre provides JavaScript events to track user activity in your Livefyre Apps. For example, you may wish to update the page when users like or share content to Twitter or Facebook, or when new content is posted.

Here is an example of how to receive the events. Replace `codeph  console.log` with your code to map and send the event to your analytics integration (Dynamic Tag Management, Adobe Analytics JS, Google Analytics, etc.):

```
document.body.addEventListener('insights', function (data) { 
 console.log('Received:', data.detail.type, data); 
});
```
List of supported Media Wall events:

<table frame="all" rowsep="1" colsep="1" id="table_kvk_w5g_n1b"> 
 <title>Media Wall Events</title> 
 <tgroup cols="2"> 
  <colspec colname="c1" colnum="1" colwidth="1.0*" /> 
  <colspec colname="c2" colnum="2" colwidth="1.0*" /> 
  <thead> 
   <tr> 
    <th class="entry"> Event </th> 
    <th class="entry"> Definition </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <span class="codeph"> Init </span> </td> 
    <td> When a Media Wall is included on a page. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> Load </span> </td> 
    <td> When the Media Wall was loaded on a page regardless of position. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> PostButtonClick </span> </td> 
    <td> When a user clicks on an Upload Button on a Media Wall. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> RequestMore </span> </td> 
    <td> When user loads more content in a Media Wall. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> TwitterReplyClick </span> </td> 
    <td> When a user clicks the Twitter Reply button from the Media Wall. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> TwitterRetweetClick </span> </td> 
    <td> When a user clicks the Twitter Retweet button from the Media Wall. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> TwitterLikeClick </span> </td> 
    <td> When a user clicks the Twitter Like/Favorite button from the Media Wall. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> ModalView </span> </td> 
    <td> When user clicks to view Media Wall content in a larger modal window. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> Like </span> </td> 
    <td> When a user clicks the Like button from the Media Wall. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> ShareButtonClick </span> </td> 
    <td> Any time a user clicks on the share button on a Media Wall card. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> ShareURL </span> </td> 
    <td> When Share to URL text area is selected/copied from the Media Wall. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> ShareFacebook </span> </td> 
    <td> When Share to Facebook is clicked from the Media Wall. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> ShareTwitter </span> </td> 
    <td> When Share to Twitter is clicked from the Media Wall. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

