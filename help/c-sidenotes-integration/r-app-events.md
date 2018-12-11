---
description: You can listen to events on an instance of Sidenotes.
seo-description: You can listen to events on an instance of Sidenotes.
seo-title: Sidenotes App Events
solution: Experience Manager
title: Sidenotes App Events
uuid: c4d16486-1d93-4ba5-9c81-55166a5b3762
index: y
internal: n
snippet: y
---

# Sidenotes App Events{#sidenotes-app-events}

You can listen to events on an instance of Sidenotes.

<a id="section_e31_5jy_ty"></a>

Callbacks can be registered with the `onmethod` and unregistered with the `removeListener` method. A `once` method is available for convenience if the callback is to be called only once and then unregistered.

```
var app = Livefyre.Sidenotes(convConfig); 
   app.once('sidenotes.initialized', function () { 
     // Sidenotes initialized!  
});
```

(For more information on Livefyre events, see the JavaScript Events page in the Reference section.)

<table id="table_syj_stv_sy"> 
 <thead> 
  <tr> 
   <th class="entry"> Key </th> 
   <th class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> <span class="codeph"> sidenotes.initialized </span> </td> 
   <td> Fired when the App is instantiated, has data, and is on the page. </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> sidenotes.commentFlagged </span> </td> 
   <td> Fired when a comment has been flagged. Data contains: 
    <ul id="ul_gxt_pky_ty"> 
     <li><b>targetId</b>: id of the comment that was flagged</li> 
     <li><b>type</b>: flag type string (offensive, off-topic, spam, disagree)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> sidenotes.commentPosted </span> </td> 
   <td> Fired when a comment has been posted. Data contains: 
    <ul id="ul_dxr_rky_ty"> 
     <li><b>authorId</b>: id of the author of the comment</li> 
     <li><b>bodyHtml</b>: body of the comment</li> 
     <li><b>parent</b>: id of the comment’s parent, or null</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> sidenotes.commentShared </span> </td> 
   <td> Fired when a comment has been shared. Data contains: 
    <ul id="ul_gg5_tky_ty"> 
     <li><b>targetId</b>: id of the comment that was shared</li> 
     <li><b>sharedToFacebook</b>: whether the comment was shared to Facebook</li> 
     <li><b>sharedToTwitter</b>: whether the comment was shared to Twitter</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> sidenotes.commentVoted </span> </td> 
   <td> Fired when a comment has been voted on. Data contains: 
    <ul id="ul_nc1_3py_ty"> 
     <li><b>targetId</b>: id of the comment that was voted on</li> 
     <li><b>targetAuthorId</b>: id of the author whose comment was voted on</li> 
     <li><b>type</b>: numerical vote type: 0: ‘clear’, 1: ‘upvote’, or 2: ‘downvote’</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> sidenotes.userLoggedIn </span> </td> 
   <td> Fired when a user logs in. Data contains: 
    <ul id="ul_gpc_lpy_ty"> 
     <li><b>avatar</b>: avatar url for the user</li> 
     <li><b>displayName</b>: display name of the user</li> 
     <li><b>id</b>: id of the user</li> 
     <li><b>isModerator</b>: whether the user is a moderator of the current collection</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> sidenotes.userLoggedOut </span> </td> 
   <td> Fired when a user logs out </td> 
  </tr> 
 </tbody> 
</table>

