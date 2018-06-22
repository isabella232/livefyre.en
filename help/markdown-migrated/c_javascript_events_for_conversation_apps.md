---
description: The events available to which you can bind JavaScript for conversation Apps (for example, Comments, Chat, Live Blog, Reviews, and Sidenotes).
seo-description: The events available to which you can bind JavaScript for conversation Apps (for example, Comments, Chat, Live Blog, Reviews, and Sidenotes).
seo-title: Javascript Events for Conversation Apps
solution: Experience Manager
title: Javascript Events for Conversation Apps
---

# Javascript Events for Conversation Apps

## Conversation Apps and Events Matrix {#section_y4j_x4m_ybb}

The following is a matrix of the events available for conversation apps. An X denotes that the event is available for the App, N/A indicates that the event does not apply to the App, and no marking means that the event is unavailable for that App:

<table frame="all" rowsep="1" colsep="1" id="table_rw4_x4m_ybb"> 
 <title>Conversation App Events</title> 
 <tgroup cols="8"> 
  <colspec colname="c1" colnum="1" colwidth="1.03*" /> 
  <colspec colname="c2" colnum="2" colwidth="1.03*" /> 
  <colspec colname="c3" colnum="3" colwidth="1.03*" /> 
  <colspec colname="c4" colnum="4" colwidth="1.06*" /> 
  <colspec colname="c5" colnum="5" colwidth="1*" /> 
  <colspec colname="c6" colnum="6" colwidth="1.04*" /> 
  <colspec colname="c7" colnum="7" colwidth="1.03*" /> 
  <colspec colname="c8" colnum="8" colwidth="1.1*" /> 
  <thead> 
   <tr> 
    <th class="entry">Events</th> 
    <th class="entry">Comments</th> 
    <th class="entry">Chat</th> 
    <th class="entry">Liveblog</th> 
    <th class="entry">Reviews</th> 
    <th class="entry">Sidenotes</th> 
    <th class="entry">Polls</th> 
    <th class="entry">Trending</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Init</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>Load</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>View</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>Post</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Posted</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Twitter Reply</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Twitter Like</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>LF like</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>LF Unlike</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Share On Post</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Share Button</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Share Twitter</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Share Facebook</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Share URL</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>ExpandReplies</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Collapse replies</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Flag Button</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Flag</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Flag Cancel</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Follow</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Unfollow</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>RequestMore</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>ModalView</td> 
    <td></td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Twitter Retweet</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Post button click</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Comment count updated</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>User logged in</td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>User logged out</td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Comment featured</td> 
    <td></td> 
    <td>N/A</td> 
    <td></td> 
    <td></td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Comment unfeatured</td> 
    <td></td> 
    <td>N/A</td> 
    <td></td> 
    <td></td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Comment voted</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>X</td> 
    <td>X</td> 
    <td>N/A</td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Poll selection</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td></td> 
    <td>N/A</td> 
   </tr> 
   <tr> 
    <td>Trending item selected</td> 
    <td>N/.A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td>N/A</td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>Network ID</td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>App ID</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>Context ID</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>App Type</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>Content Type</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td>X</td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>Published date to App</td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td>Logged in to end-user App</td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

