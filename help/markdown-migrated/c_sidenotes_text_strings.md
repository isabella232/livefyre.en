---
description: Customizing the text strings for Livefyre Sidenotes
seo-description: Customizing the text strings for Livefyre Sidenotes
seo-title: Sidenotes Text Strings
solution: Experience Manager
title: Sidenotes Text Strings
---

# Sidenotes Text Strings

This page lists and describes all strings available for customization in Sidenotes apps. For information on strings available for the core Livefyre apps, please see String Customizations.

* Implementation
* Auth
* Stream Info
* Author / Content Info
* User Actions
* Post Functions
* Moderator Interface
* Errors
## Implementation {#section_wp2_ql4_xz}

To implement this feature, pass in a 1-1 object mapping of the strings you wish to override to the Javascript configuration object. If you don’t provide a field, then the default text will be used.

Example:

```
var customStrings = { 
 postAsButton: "New Post As Text", 
 postEditButton: "New Post Edit Text" 
}; 
networkConfig["strings"] = customStrings; fyre.conv.load( 
 networkConfig, 
 [convConfig], 
 function(){} 
);
```
## Authentication {#section_pqf_3l4_xz}

Strings available for the Authentication process, and from the authenticated user menus.

<table id="table_vfk_vnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Element </th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <i>Auth menu strings</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuAuthSignInBtn </td> 
    <td> Sign in </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuAuthSignedInMsg </td> 
    <td> You must be signed in to {action} </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuUserEditProfile </td> 
    <td> Edit Profile </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuUserAdmin </td> 
    <td> Admin Console </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuUserLogout </td> 
    <td> Sign Out </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuUserBackBtn </td> 
    <td> All </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Stream Info {#section_wpy_gl4_xz}

Strings available for content stream information and display.

<table id="table_wfk_vnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Element </th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <i>Info menu options</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuInfoCopyright </td> 
    <td> &amp;copy; Livefyre, Inc. 2014 </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuInfoHelp </td> 
    <td> Help </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuInfoLivefyreLink </td> 
    <td> Visit Livefyre.com </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Author / Content Info {#section_dhb_gl4_xz}

Stings available for author and individual content information.

<table id="table_xfk_vnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Element </th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td></td> 
    <td> commentModeratorTag </td> 
    <td> Mod </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentPendingTag </td> 
    <td> Pending </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentReadMoreLink </td> 
    <td> Read More </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentReplyLink </td> 
    <td> See {number} replies </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentReplyLinkSing </td> 
    <td> See reply </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentVoteCount </td> 
    <td> votes </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentVoteCountSing </td> 
    <td> vote </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> datetimeMinutePrefix </td> 
    <td> m </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> datetimeMonths </td> 
    <td> <i>An array. Default =</i>[ ‘January’, ‘February’, ‘March’, ‘April’, ‘May’, ‘June’, ‘July’, ‘August’, ‘September’, ‘October’, ‘November’, ‘December’ ] </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> questionExplanation </td> 
    <td> You can now read and write comments directly on sentences, paragraphs, images and quotes.&lt;br&gt;&lt;br&gt;&lt;span class=”lf-highlight-text”&gt;Highlight text&lt;/span&gt; and click the &lt;span class=”fycon-write”&gt;&lt;/span&gt; icon or click the &lt;span class=”fycon-action-view”&gt;&lt;/span&gt; icon at the end of each paragraph. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> questionMockText </td> 
    <td> What is “familiarly known” is not properly known, just for the reason that it is “familiar”. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> questionTitle </td> 
    <td> What is a Sidenote? </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## User Actions {#section_qxd_fl4_xz}

Strings available for user actions: flagging, sharing, and liking existing content.

<table id="table_yfk_vnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Element </th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <i>Reply menu options</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuRepliesViewTitle </td> 
    <td> Details </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuRepliesViewReply </td> 
    <td> Reply to Conversation </td> 
   </tr> 
   <tr> 
    <td> <i>Share menu options</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuShareOptionFacebook </td> 
    <td> Facebook </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuShareOptionTwitter </td> 
    <td> Twitter </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuShareTitle </td> 
    <td> Share </td> 
   </tr> 
   <tr> 
    <td> <i>Flag menu options</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuFlagOptionDisagree </td> 
    <td> Disagree </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuFlagOptionOffensive </td> 
    <td> Offensive </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuFlagOptionOffTopic </td> 
    <td> Off Topic </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuFlagOptionSpam </td> 
    <td> Spam </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuFlagTitle </td> 
    <td> Flag as… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> facebookShareCaption </td> 
    <td> Sidenotes on “{title}” </td> 
   </tr> 
   <tr> 
    <td> <i>Mobile user options</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sliderCommentTally </td> 
    <td> of </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sliderInviteRead </td> 
    <td> Read </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sliderInviteWrite </td> 
    <td> Write </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sliderLoading </td> 
    <td> Loading… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sliderWriteText </td> 
    <td> What do you think? Tap to write. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Post Functions {#section_xzf_2l4_xz}

Strings available for users posting content.

<table id="table_zfk_vnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Element </th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td></td> 
    <td> editorEditBtn </td> 
    <td> Save </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorEditPosting </td> 
    <td> Saving… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorEditReplyTitle </td> 
    <td> Edit Reply </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorEditTitle </td> 
    <td> Edit Sidenote </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorPlaceholder </td> 
    <td> What do you think? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorPostBtn </td> 
    <td> Post Sidenote </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorPostBtnMobile </td> 
    <td> Post </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorPosting </td> 
    <td> Posting… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorReplyBtn </td> 
    <td> Post Reply </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorReplyTitle </td> 
    <td> Write Reply </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorTitle </td> 
    <td> Write Sidenote </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> emptyImageBlockTxt </td> 
    <td> What do you think? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> emptyTextBlockTxt </td> 
    <td> + </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> replyBtn </td> 
    <td> Reply </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> threadReplyBtn </td> 
    <td> Reply to Conversation </td> 
   </tr> 
   <tr> 
    <td> <i>Delete menu options</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuConfirmAccept </td> 
    <td> Yes, {action} </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuConfirmCancel </td> 
    <td> Cancel </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuConfirmTitle </td> 
    <td> Are you sure? </td> 
   </tr> 
   <tr> 
    <td> <i>Etc menu options</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuEtcOptionApprove </td> 
    <td> Approve </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuEtcOptionDelete </td> 
    <td> Delete </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuEtcOptionEdit </td> 
    <td> Edit </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuEtcOptionFlag </td> 
    <td> Flag </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuEtcOptionShare </td> 
    <td> Share </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuEtcPostedAt </td> 
    <td> Posted on {date} </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> menuEtcTitle </td> 
    <td> More </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Moderator Interface {#section_o5f_dl4_xz}

Strings available to the user-authenticated moderator interface.

<table id="table_agk_vnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Element </th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <i>Confirmation messages from the More menu</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> notificationApproved </td> 
    <td> Approved </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> notificationDeleted </td> 
    <td> Deleted </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> notificationFlagged </td> 
    <td> Flagged </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Errors {#section_gtk_cl4_xz}

Strings available for general error messages.

<table id="table_bgk_vnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Element </th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td></td> 
    <td> errorConnection </td> 
    <td> Uh-oh. You don’t seem to have a good connection. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorDuplicate </td> 
    <td> We like your note too, but you can’t post it twice. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorGeneral </td> 
    <td> An error has occurred. Please try again. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorServer </td> 
    <td> Something went wrong with our server. Try that again? </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

