---
---

<a id="section_bbp_g3y_ty"></a>

Custom strings are applied through an object injected into the Sidenotes constructor, and override default strings used through the application. These may be used to customize any part of the language to fit your style or language specifications. Strings will automatically merge with defaults.

```
var customStrings = { 
 'menuBackBtn': 'return' }; 
new Livefyre.Sidenotes({ 
 strings: customStrings, 
 ... 
});
```
<table id="table_j4j_15v_sy"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <span class="codeph"> appName </span> </td> 
    <td> Sidenotes </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentModeratorTag </span> </td> 
    <td> Mod </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentPendingTag </span> </td> 
    <td> Pending </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentReadMoreLink </span> </td> 
    <td> Read More </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentReplyLink </span> </td> 
    <td> See {number} replies </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentReplyLinkSing </span> </td> 
    <td> See reply </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentVoteCount </span> </td> 
    <td> votes </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> commentVoteCountSing </span> </td> 
    <td> vote </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> editorPlaceholder </span> </td> 
    <td> What do you think? </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> editorPostBtn </span> </td> 
    <td> Post Sidenote </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> editorPostBtnMobile </span> </td> 
    <td> Post </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> editorPosting </span> </td> 
    <td> Posting… </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> editorReplyBtn </span> </td> 
    <td> Post Reply </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> editorReplyTitle </span> </td> 
    <td> Write Reply </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> editorTitle </span> </td> 
    <td> Write Note </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> emptyImageBlockTxt </span> </td> 
    <td> What do you think? </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> emptyTextBlockTxt </span> </td> 
    <td> + </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> errorConnection </span> </td> 
    <td> Uh-oh. You don’t seem to have a good connection. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> errorDuplicate </span> </td> 
    <td> We like your note too, but you can’t post it twice. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> errorGeneral </span> </td> 
    <td> An error has occurred. Please try again. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> errorServer </span> </td> 
    <td> Something went wrong with our server. Try that again? </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> facebookShareCaption </span> </td> 
    <td> SideNotes on “{title}” </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuAuthSignedInMsg </span> </td> 
    <td> You must be signed in to {action} </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuAuthSignInBtn </span> </td> 
    <td> Sign in </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuBackBtn </span> </td> 
    <td> Back </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuConfirmAccept </span> </td> 
    <td> Yes, {action} </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuConfirmCancel </span> </td> 
    <td> Cancel </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuConfirmTitle </span> </td> 
    <td> Are you sure? </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuEtcOptionApprove </span> </td> 
    <td> Approve </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuEtcOptionDelete </span> </td> 
    <td> Delete </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuEtcOptionEdit </span> </td> 
    <td> Edit </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuEtcOptionFlag </span> </td> 
    <td> Flag </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuEtcOptionShare </span> </td> 
    <td> Share </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuEtcPostedAt </span> </td> 
    <td> Posted on {date} </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuEtcTitle </span> </td> 
    <td> More </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuFlagOptionDisagree </span> </td> 
    <td> Disagree </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuFlagOptionOffensive </span> </td> 
    <td> Offensive </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuFlagOptionOffTopic </span> </td> 
    <td> Off Topic </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuFlagOptionSpam </span> </td> 
    <td> Spam </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuFlagTitle </span> </td> 
    <td> Flag as… </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuInfoCopyright </span> </td> 
    <td> © Livefyre, Inc. 2014 </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuInfoHelp </span> </td> 
    <td> Help </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuInfoLivefyreLink </span> </td> 
    <td> Visit Livefyre.com </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuRepliesViewReply </span> </td> 
    <td> Reply to Conversation </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuRepliesViewTitle </span> </td> 
    <td> Details </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuShareOptionFacebook </span> </td> 
    <td> Facebook </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuShareOptionLink </span> </td> 
    <td> Copy Permalink </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuShareOptionLinkComplete </span> </td> 
    <td> Copied </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuShareOptionLinkFailed </span> </td> 
    <td> Copy Failed </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuShareOptionTwitter </span> </td> 
    <td> Twitter </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> menuShareTitle </span> </td> 
    <td> Share </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> notificationApproved </span> </td> 
    <td> Approved </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> notificationDeleted </span> </td> 
    <td> Deleted </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> notificationFlagged </span> </td> 
    <td> Flagged </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> permalinkBackBtn </span> </td> 
    <td> All </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> permalinkTitle </span> </td> 
    <td> Permalink </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> questionExplanation </span> </td> 
    <td> You can now read and write comments directly on sentences, paragraphs, images and quotes.&lt;br&gt;&lt;br&gt;&lt;span class=”lf-highlight-text”&gt;Highlight text&lt;/span&gt; and click the &lt;span class=”fycon-write”&gt;&lt;/span&gt; icon or click the &lt;span class=”fycon-action-view”&gt;&lt;/span&gt; icon at the end of each paragraph. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> questionMockText </span> </td> 
    <td> What is “familiarly known” is not properly known, just for the reason that it is “familiar”. </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> questionTitle </span> </td> 
    <td> What is a Sidenote? </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> queuedCommentsPlural </span> </td> 
    <td> {number} New Sidenotes </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> queuedCommentsSingular </span> </td> 
    <td> 1 New Sidenote </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> queuedRepliesPlural </span> </td> 
    <td> {number} New Replies </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> queuedRepliesSingular </span> </td> 
    <td> 1 New Reply </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> replyBtn </span> </td> 
    <td> Reply </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> signInToPost </span> </td> 
    <td> Sign in to write a sidenote </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> sliderCommentTally </span> </td> 
    <td> of </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> sliderInviteRead </span> </td> 
    <td> Read </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> sliderInviteWrite </span> </td> 
    <td> Write </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> sliderWriteText </span> </td> 
    <td> What do you think? Tap to write </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> threadCollapseBtn </span> </td> 
    <td> Collapse </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> threadExpandBtnPlural </span> </td> 
    <td> Expand {number} Replies </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> threadExpandBtnSingular </span> </td> 
    <td> Expand 1 Reply </td> 
   </tr> 
   <tr> 
    <td> <span class="codeph"> threadReplyBtn </span> </td> 
    <td> Reply to Conversation </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

