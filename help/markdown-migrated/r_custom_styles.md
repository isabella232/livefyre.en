---
---

<a id="section_thp_wtv_sy"></a>

The “keys” are object keys which represent DOM elements, while “properties” are supported CSS properties for the particular key. For example, to customize the style of the blockBtn (which is the button that launches the Sidenotes popover), one would construct an object such as:

```
var styles = { 
 'blockBtn': { 
 'fontColor': '#555', 
 'fontSize': '18px' 
 } 
}; 
new Livefyre.Sidenotes({ 
 customStyles: styles, 
 ... 
})
```
<table id="table_jjd_xtv_sy"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> <b>Key</b> </th> 
    <th class="entry"> <b>Properties</b> </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <span class="codeph"> anonymousAvatar </span> </td> 
    <td> ‘height’, ‘width’ </td> 
    <td> Anonymous avatar image, to left of text area editor. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> blockBtn </span> </td> 
    <td> ‘fontColor’, ‘fontSize’, ‘left’, ‘position’, ‘right’, ‘top’ </td> 
    <td> The “Launcher icon” placed next to elements specified as sidenote-able. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> blockBtnActive </span> </td> 
    <td> ‘fontColor’, ‘fontSize’, ‘left’, ‘position’, ‘right’, ‘top’ </td> 
    <td> Launcher icon when in an active state. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentAvatar </span> </td> 
    <td> ‘height’, ‘width’ </td> 
    <td> Avatar image to the left of top level notes. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentBody </span> </td> 
    <td> ‘fontColor’, ‘fontFamily’, ‘fontSize’, ‘fontWeight’, ‘lineHeight’ </td> 
    <td> Text body of threaded notes. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentDisplayName </span> </td> 
    <td> ‘fontColor’, ‘fontFamily’, ‘fontSize’, ‘fontWeight’, ‘lineHeight’ </td> 
    <td> Display name of user who has left a note. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentDownvote </span> </td> 
    <td> ‘fontColor’, ‘fontSize’ </td> 
    <td> Downvote button on a note. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentReplyExpand </span> </td> 
    <td> ‘backgroundColor’, ‘borderColor’, ‘borderWidth’, ‘fontColor’, ‘fontFamily’, ‘fontSize’, ‘fontWeight’, ‘lineHeight’ </td> 
    <td> Button for expanding threads with a large number of replies. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentTags </span> </td> 
    <td> ‘fontColor’, ‘fontFamily’, ‘fontSize’, ‘fontWeight’, ‘lineHeight’ </td> 
    <td> Tags about a user on a note. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentUpvote </span> </td> 
    <td> ‘fontColor’, ‘fontSize’ </td> 
    <td> Upvote button on a note. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> editorTextarea </span> </td> 
    <td> ‘height’, ‘width’, ‘fontColor’, ‘fontFamily’, ‘fontSize’, ‘fontWeight’, ‘lineHeight’ </td> 
    <td> Textarea input box for leaving notes. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> mediaBlockBtn </span> </td> 
    <td> ‘fontColor’, ‘fontSize’, ‘left’, ‘position’, ‘right’, ‘top’ </td> 
    <td> Media launcher icon when on top of a media item (img, video). </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> mediaBlockBtnActive </span> </td> 
    <td> ‘fontColor’, ‘fontSize’, ‘left’, ‘position’, ‘right’, ‘top’ </td> 
    <td> Media launcher icon in an active state. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> numSidenotes </span> </td> 
    <td> ‘fontColor’, ‘fontFamily’, ‘fontSize’, ‘fontWeight’, ‘lineHeight’, ‘backgroundColor’, ‘borderColor’, ‘borderWidth’, ‘height’, ‘width’ </td> 
    <td> Clickable button that shows the number of Sidenotes in the collection. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> numSidenotesPopover </span> </td> 
    <td> ‘fontColor’, ‘fontFamily’, ‘fontSize’, ‘fontWeight’, ‘lineHeight’, ‘backgroundColor’, ‘borderColor’, ‘borderWidth’, ‘height’, ‘width’ </td> 
    <td> Popover with a brief explanation of Sidenotes for the user. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> popover </span> </td> 
    <td> ‘backgroundColor’ </td> 
    <td> Popover that is brought up when launcher icon invoked. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> popoverArrowLeft </span> </td> 
    <td> ‘backgroundImage’, ‘height’, ‘left’, ‘right’, ‘top’, ‘width’ </td> 
    <td> Left arrow element on the popover that points to the DOM element containing a launcher icon. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> popoverArrorRight </span> </td> 
    <td> ‘backgroundImage’, ‘height’, ‘left’, ‘right’, ‘top’, ‘width’ </td> 
    <td> Right arrow element on the popover that points to the DOM element containing a launcher icon. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> popoverArrowTop </span> </td> 
    <td> ‘backgroundImage’, ‘height’, ‘left’, ‘right’, ‘top’, ‘width’ </td> 
    <td> Top arrow element on the popover that points to the DOM element containing a launcher icon. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> replyAvatar </span> </td> 
    <td> ‘height’, ‘width’ </td> 
    <td> Avatar image to the left of reply level notes. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> streamPoweredBy </span> </td> 
    <td> ‘backgroundColor’, ‘borderColor’, ‘lineHeight’ </td> 
    <td> “Powered by” footer on the popover. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> streamQueueButton </span> </td> 
    <td> ‘backgroundColor’, ‘borderColor’, ‘borderWidth’, ‘fontColor’, ‘fontFamily’, ‘fontSize’, ‘fontWeight’, ‘lineHeight’ </td> 
    <td> Button to indicate when new notes stream into an open popover. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> userAvatar </span> </td> 
    <td> ‘height’, ‘width’ </td> 
    <td> Authenticated user’s avatar image, to the left of the text area editor. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

