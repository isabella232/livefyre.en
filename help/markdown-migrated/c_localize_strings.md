---
description: Customizing the strings of the Livefyre Apps.
seo-description: Customizing the strings of the Livefyre Apps.
seo-title: Localize Strings
solution: Experience Manager
title: Localize Strings
---

# Localize Strings

The text strings for most HTML elements in any Livefyre App may be customized. This provides the flexibility to change the text of rendered HTML elements, such as the “Post As” button, the “Comment Count” text, or the “Sign In” button, to any valid UTF-8 string. Use this feature to add personality to your implementation of the stream, or to localize the language in the app for your user base.

* Comments, Chat, and Live Blog
    * [](#c_localize_strings/section_im4_224_xz)
    * [](#c_localize_strings/section_cm3_d24_xz)
    * [ Stream Info ](#c_localize_strings/section_wx1_c24_xz)
    * [ Stream Sorting ](#c_localize_strings/section_ih2_124_xz)
    * [ Content Info ](#c_localize_strings/section_llv_yd4_xz)
    * [ Featured Content ](#c_localize_strings/section_gmw_vd4_xz)
    * [ Text Editor ](#c_localize_strings/section_ky5_td4_xz)
    * [ Response Options ](#c_localize_strings/section_zvt_qd4_xz)
    * [ Comment Notifier ](#c_localize_strings/section_qqt_pd4_xz)
    * [ Error Messages ](#c_localize_strings/section_omz_jxn_xz)
  
* [ Time and Date Format ](#c_localize_strings/section_yz4_g5n_xz)
* [ Media Wall ](#c_localize_strings/section_vwt_d5n_xz)
* [ Map ](#c_localize_strings/section_fxv_c5n_xz)
* [ Mosaic ](#c_localize_strings/section_e2s_b5n_xz)
* [ Carousel ](#c_localize_strings/section_l2z_hkn_xz)
* [ Feature Card ](#c_localize_strings/section_mw2_hkn_xz)
* [](#c_localize_strings/section_grc_gkn_xz)
* [ Poll ](#c_localize_strings/section_pdg_fwh_xz)
* [ Livefyre Identity ](#c_localize_strings/section_zc3_xvh_xz)
* More:
    * [](c_review_text_strings.md#c_review_text_strings)
    * [ Sidenotes ](c_sidenotes_text_strings.md#c_sidenotes_text_strings)
  
## Implementation {#section_im4_224_xz}

To implement this feature, pass in a 1-1 object mapping of the strings you wish to override to the JavaScript configuration object. If you don’t provide a field, then the default text will be used.

Example:

```
var customStrings = { 
 postAsButton: "New Post As Text", 
 postEditButton: "New Post Edit Text" 
}; 
 convConfig["strings"] = customStrings; fyre.conv.load( 
 networkConfig, 
 [convConfig], 
 function(){} 
);
```
This page lists all text strings which may be customized for the Livefyre Core Apps.

## Account Access {#section_cm3_d24_xz}

Strings available for the Authentication process, and from the authenticated user menus.

<table id="table_icg_pnl_wz"> 
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
    <td> displayName </td> 
    <td> %s </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editProfile </td> 
    <td> Edit profile </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> notificationSettings </td> 
    <td> Notification settings </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> siteAdmin </td> 
    <td> Admin Console (links to Studio) </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> signOut </td> 
    <td> Sign out </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

![](images/strings_threadheader-150x40.png)
## Stream Info {#section_wx1_c24_xz}

Strings available for content stream information and display. Lists the number of people listening, the number of posts to the App, and allows users to sign in, or access their account information.

<table id="table_kcg_pnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
    <th class="entry"> Stream data </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td></td> 
    <td> commentCountLabelZero </td> 
    <td> %s comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentCountLabel </td> 
    <td> %s comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentCountLabelPlural </td> 
    <td> %s comments </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> listenerCount </td> 
    <td> person listening </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> listenerCountPlural </td> 
    <td> people listening </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> liveblogPostCountLabelZero </td> 
    <td> post </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> liveblogPostCountLabel </td> 
    <td> post </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> liveblogPostCountLabelPlural </td> 
    <td> posts </td> 
   </tr> 
   <tr> 
    <td> <b>Thread options</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> threadBreakoutButton </td> 
    <td> Show entire Thread </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> toggleCollapse </td> 
    <td> Toggle Collapse </td> 
   </tr> 
   <tr> 
    <td> <b>High velocity / queued comments</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> refresh </td> 
    <td> Refresh </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> newComment </td> 
    <td> New Comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> newComments </td> 
    <td> New Comments </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> newReply </td> 
    <td> new reply </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> newReplies </td> 
    <td> new replies </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Stream Sorting {#section_ih2_124_xz}

Allows uses to sort returned content by age or popularity.

<table id="table_lcg_pnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
    <th class="entry"> Header options </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td></td> 
    <td> sortNewest </td> 
    <td> Newest </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sortOldest </td> 
    <td> Oldest </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sortTopComments </td> 
    <td> Top Comments </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sortHotThreads </td> 
    <td> Hot Threads </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sortSeparator </td> 
    <td> | </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> streamSorting </td> 
    <td> Loading </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> topCommentsContentNotFoundMsg </td> 
    <td> There are not enough likes yet. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> hotThreadsContentNotFoundMsg </td> 
    <td> There are not enough threads yet. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> streamRefreshMsg </td> 
    <td> See what’s new. </td> 
   </tr> 
   <tr> 
    <td> <b>Footer options</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> archiveHeaderTitle </td> 
    <td> From the Archive </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> archiveShowMore </td> 
    <td> Show More </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> showMore </td> 
    <td> Show More Comments </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> showMoreLiveblog </td> 
    <td> Show More Posts </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

![](images/strings_newestoldesttop-1-150x56.png)  ![](images/strings_threadend-150x47.png)
## Content Info {#section_llv_yd4_xz}

Lists post information: user name, any applied user tags, and post time.

<table id="table_ocg_pnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
    <th class="entry"> Author </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td></td> 
    <td> moderator </td> 
    <td> moderator </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> hovercardViewProfile </td> 
    <td> View Full Profile </td> 
   </tr> 
   <tr> 
    <td> <b>Post info</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> timeJustNow </td> 
    <td> just now </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> timeMinutesAgo </td> 
    <td> minute ago </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> timeMinutesAgoPlural </td> 
    <td> minutes ago </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> timeHoursAgo </td> 
    <td> hour ago </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> timeHoursAgoPlural </td> 
    <td> hours ago </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> timeDaysAgo </td> 
    <td> day ago </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> timeDaysAgoPlural </td> 
    <td> days ago </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> likesPlural </td> 
    <td> Likes </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> likesSingular </td> 
    <td> Like </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> moderatorEditTimestamp </td> 
    <td> Edited by a Moderator </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentTombstone </td> 
    <td> This comment has been deleted </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> permalinkNotFoundMsg </td> 
    <td> This comment is no longer visible. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> quickProfileTooltip </td> 
    <td> Quick Profile </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

![](images/strings_authorinfo-150x52.png) ![](images/strings_posttime-150x45.png)
## Featured Content {#section_gmw_vd4_xz}

If enabled, featured content is listed at the top of the stream.

<table id="table_rcg_pnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"></th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <b>Featured labels</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_featuredcontent-150x40.png" id="image_tq1_5cd_12b" /> </td> 
    <td> featuredCommentsTag </td> 
    <td> Featured </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> featuredCommentsTitlePlural </td> 
    <td> Featured Comments </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Text Editor {#section_ky5_td4_xz}

By default, available at the top of the page for all users.

<table id="table_tcg_pnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"></th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <b>Editor buttons</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_texteditor-1-150x77.png" id="image_vgp_vcd_12b" /> </td> 
    <td> follow </td> 
    <td> + Follow </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> unfollow </td> 
    <td> - Unfollow </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> liveblogFollow </td> 
    <td> Follow Live Blog </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> liveblogUnfollow </td> 
    <td> Unfollow Live Blog </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postButton(Available for logged in users.) </td> 
    <td> Post comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postAsButton(Available for unauthenticated users.) </td> 
    <td> Post comment as… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postEditButton </td> 
    <td> Edit comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postEditAsButton </td> 
    <td> Edit comment as… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postEditCancelButton </td> 
    <td> Cancel </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editorDisabled </td> 
    <td> This conversation is currently closed to new comments. </td> 
   </tr> 
   <tr> 
    <td> <b>Chat options</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> livechatPostButtonLabel </td> 
    <td> Post </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> livechatPostEditButton </td> 
    <td> Edit </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> livechatWindowsInstruction </td> 
    <td> Press control+enter to post </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> livechatOtherInstruction </td> 
    <td> Press command+enter to post </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Response Options {#section_zvt_qd4_xz}

Unless otherwise noted, available to all logged in users. Mouse over a content panel to access.

<table id="table_vcg_pnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
    <th class="entry"></th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <b>User Response Options</b> </td> 
    <td> Available for end users. </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_banusermodal-150x36.png" id="image_cdr_ycd_12b" /> </td> 
    <td> flagButton </td> 
    <td> Flag </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagCommentTooltip </td> 
    <td> Flag </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editButton(Available only for authors and moderators, if enabled.) </td> 
    <td> Edit </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> deleteButton(Available only for authors and moderators, if enabled.) </td> 
    <td> Delete </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> deleteCommentTooltip </td> 
    <td> Delete </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareButton </td> 
    <td> Share </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareCommentTooltip </td> 
    <td> Share </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> likeButton </td> 
    <td> Like </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> unlikeButton </td> 
    <td> Unlike </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> replyButton </td> 
    <td> Reply </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> replyButtonSingular(Available for Chat and Live Blog.) </td> 
    <td> Reply </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> replyButtonPlural(Available for Chat and Live Blog.) </td> 
    <td> Replies </td> 
   </tr> 
   <tr> 
    <td> <b>Flag Modal</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_responseoptions-150x35.png" id="image_kh3_1dd_12b" /> </td> 
    <td> flagTitle </td> 
    <td> Flag %s’s comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagSubtitle </td> 
    <td> Flag as </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagDefaultSelectOption </td> 
    <td> Select </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagSpam </td> 
    <td> Spam </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagSpamButton </td> 
    <td> Spam </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagSpamCommentTooltip </td> 
    <td> Spam </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagOffensive </td> 
    <td> Offensive </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagOffensiveButton </td> 
    <td> Offensive </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagOffensiveCommentTooltip </td> 
    <td> Offensive </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagDisagree </td> 
    <td> Disagree </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagDisagreeButton </td> 
    <td> Disagree </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagDisagreeCommentTooltip </td> 
    <td> Disagree </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagOffTopic </td> 
    <td> Off Topic </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagOfftopicButton </td> 
    <td> Off Topic </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagOfftopicCommentTooltip </td> 
    <td> Off Topic </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagEmail </td> 
    <td> Email </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagEmailPlaceholder </td> 
    <td> you@example.com </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagNotes </td> 
    <td> Notes </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagNotesPlaceholder </td> 
    <td> Start typing here… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagConfirmButton </td> 
    <td> OK </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagCancelButton </td> 
    <td> Cancel </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagConfirmationMessage </td> 
    <td> Flag %s’s comment as %s? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagSuccessMsg </td> 
    <td> Comment has been flagged. </td> 
   </tr> 
   <tr> 
    <td> <b>Share Modal</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_flagmodal-150x87.png" id="image_mty_cdd_12b" /> </td> 
    <td> shareTitle </td> 
    <td> Share Comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sharePlaceholderText </td> 
    <td> What do you think? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareLabel </td> 
    <td> Share on: </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareTextTwitter </td> 
    <td> blank </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareTextFacebook </td> 
    <td> blank </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareTextLinkedin </td> 
    <td> blank </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareButtonText </td> 
    <td> Share </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sharePermalink </td> 
    <td> Permalink </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> loadingPermalink </td> 
    <td> Loading short url… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareText </td> 
    <td> I just posted a comment. Check it out! </td> 
   </tr> 
   <tr> 
    <td> <b>Reply Modal</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_sharemodal-150x59.png" id="image_qwp_2dd_12b" /> </td> 
    <td> postReplyAsButton </td> 
    <td> Post comment as… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postReplyButton(Available for logged in users.) </td> 
    <td> Post comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> backToHotThreads </td> 
    <td> Back to Hot Threads </td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_replymodal-150x64.png" id="image_ocy_fdd_12b" /> </td> 
    <td> backToComments(Appears above reply modal for featured content.) </td> 
    <td> Back to Newest </td> 
   </tr> 
   <tr> 
    <td> <b>Twitter @mention modal</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_backto-150x48.png" id="image_osk_hdd_12b" /> </td> 
    <td> mentionTitle </td> 
    <td> Share Mention </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionSubtitleTwitter </td> 
    <td> Share Tweet to: </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionDefaultText </td> 
    <td> I mentioned you in a Livefyre comment! </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionConfirmButton </td> 
    <td> OK </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionCancelButton </td> 
    <td> Cancel </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionErrorGeneral </td> 
    <td> Oops! Something went wrong! Livefyre has been alerted. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionErrorNoneSelected </td> 
    <td> You must have at least one mention enabled. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionMenuTitle </td> 
    <td> To see and mention your friends </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionTwitterConnect </td> 
    <td> Connect to Twitter </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionTwitterFetching </td> 
    <td> Fetching Friends… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionSuccessMsg </td> 
    <td> Mentions have been successfully sent. </td> 
   </tr> 
   <tr> 
    <td> <b>Edit Modal</b> </td> 
    <td> Available to Studio Admins, User Managers or Moderators </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_sharemention-150x60.png" id="image_xyy_3dd_12b" /> </td> 
    <td> @(@mention.) </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> &lt;/&gt;(Opens the custom html window.) </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> customHtmlDialogTitle(Appears as the header for the modal.) </td> 
    <td> Add Custom HTML </td> 
   </tr> 
   <tr> 
    <td> <b>Moderator Response Options</b> </td> 
    <td> Available to Studio Admins, User Managers or Moderators. </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_moderatoreditmodal-150x49.png" id="image_zhb_kdd_12b" /> </td> 
    <td> pendingComment </td> 
    <td> pending </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> banUserButton </td> 
    <td> Ban user </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> banUserTooltip </td> 
    <td> Ban User </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> bozoButton </td> 
    <td> Bozo </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> bozoCommentTooltip </td> 
    <td> Bozo </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> featureButton </td> 
    <td> Feature </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> featureCommentTooltip </td> 
    <td> Feature </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> unfeatureButton </td> 
    <td> Unfeature </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> featuredCommentTooltip </td> 
    <td> Unfeature </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <b>Ban User modal</b> </td> 
    <td> Available to Studio Admins, User Managers or Moderators. </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_adminoptions-150x33.png" id="image_a2h_ldd_12b" /> </td> 
    <td> banTitle </td> 
    <td> Ban User </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> banConfirmation </td> 
    <td> Are you sure you want to ban this user? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> banConfirmButton </td> 
    <td> OK </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> banCancelButton </td> 
    <td> Cancel </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Comment Notifier {#section_qqt_pd4_xz}

If enabled, available at the bottom of the page for all Livefyre conversation Apps.

<table id="table_fdg_pnl_wz"> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"></th> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <b>Notifier labels</b> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> <img href="images/strings_notifier-150x112.png" id="image_rhq_mdd_12b" /> </td> 
    <td> commentNotifier </td> 
    <td> New Comment </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentNotifierPlural </td> 
    <td> New Comments </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> liveblogNotifier </td> 
    <td> New Post </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> liveblogNotifierPlural </td> 
    <td> New Posts </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Error Messages {#section_omz_jxn_xz}

Strings available for customizable error messages.

<table id="table_hdg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> errorAuthError </td> 
    <td> You’re not authorized to post a comment on this conversation </td> 
   </tr> 
   <tr> 
    <td> errorCommentsNotAllowed </td> 
    <td> Comments are not allowed on this conversation </td> 
   </tr> 
   <tr> 
    <td> errorDefault </td> 
    <td> An error has occurred. Please try again. </td> 
   </tr> 
   <tr> 
    <td> errorDuplicate </td> 
    <td> As much as you liked your comment, you’re not allowed to post it twice. </td> 
   </tr> 
   <tr> 
    <td> errorEditDuplicate </td> 
    <td> You must change the body of the comment when you edit it. </td> 
   </tr> 
   <tr> 
    <td> errorEditNotAllowed </td> 
    <td> You’re not allowed to edit comments on this conversation. </td> 
   </tr> 
   <tr> 
    <td> errorEditTimeExceeded </td> 
    <td> Sorry, your comment editing period has expired. </td> 
   </tr> 
   <tr> 
    <td> errorEmpty </td> 
    <td> It seems you’re attempting to post an empty comment. </td> 
   </tr> 
   <tr> 
    <td> errorExpired </td> 
    <td> Your session has expired. Please reload the page. </td> 
   </tr> 
   <tr> 
    <td> errorFlagNotSelected </td> 
    <td> Please select a flag type. </td> 
   </tr> 
   <tr> 
    <td> errorGuestLiked </td> 
    <td> Sorry, only those with accounts can like content. </td> 
   </tr> 
   <tr> 
    <td> errorInsufficientPermissions </td> 
    <td> Insufficient Permissions </td> 
   </tr> 
   <tr> 
    <td> errorInvalidChar </td> 
    <td> It seems you’re attempting to post an invalid character. </td> 
   </tr> 
   <tr> 
    <td> errorLikeOwnComment </td> 
    <td> You cannot like your own comment </td> 
   </tr> 
   <tr> 
    <td> errorMalformed </td> 
    <td> It seems you’re attempting to post malformed content. </td> 
   </tr> 
   <tr> 
    <td> errorMaxChars </td> 
    <td> Sorry, your comment is too long. Please edit and try again. </td> 
   </tr> 
   <tr> 
    <td> errorMediaNotAvailable </td> 
    <td> Media is no longer visible. </td> 
   </tr> 
   <tr> 
    <td> errorShowMore </td> 
    <td> There was an error loading more comments. </td> 
   </tr> 
   <tr> 
    <td> MultipleMediaNotAllowedError </td> 
    <td> Your permissions only grant you one media attachment at a time. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Time and Date Format {#section_yz4_g5n_xz}

Translate and customize how dates appear on content cards within visualization apps.

<table id="table_idg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> hoursAgo </td> 
    <td> {number}h </td> 
   </tr> 
   <tr> 
    <td> hoursAgoSingular </td> 
    <td> {number}h </td> 
   </tr> 
   <tr> 
    <td> justNow </td> 
    <td> 1s </td> 
   </tr> 
   <tr> 
    <td> minutesAgo </td> 
    <td> {number}m </td> 
   </tr> 
   <tr> 
    <td> minutesAgoSingular </td> 
    <td> {number}m </td> 
   </tr> 
   <tr> 
    <td> monthDayFormat </td> 
    <td> {day} {monthAbbrev} </td> 
   </tr> 
   <tr> 
    <td> monthDayYearFormat </td> 
    <td> {day} {monthAbbrev} {year} </td> 
   </tr> 
   <tr> 
    <td> monthNames </td> 
    <td> January, February, March, April, May, June, July, August, September, October, November, December </td> 
   </tr> 
   <tr> 
    <td> monthNamesAbbrev </td> 
    <td> Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec </td> 
   </tr> 
   <tr> 
    <td> secondsAgo </td> 
    <td> {number}s </td> 
   </tr> 
   <tr> 
    <td> secondsAgoSingular </td> 
    <td> {number}s </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Media Wall {#section_vwt_d5n_xz}

Strings available for the Media Wall App.

<table id="table_w1r_yyh_xz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> featuredText </td> 
    <td> Featured </td> 
   </tr> 
   <tr> 
    <td> shareButtonText </td> 
    <td> Share </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<table id="table_jdg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> postButtonText </td> 
    <td> What’s on your mind? </td> 
   </tr> 
   <tr> 
    <td> postModalTitle </td> 
    <td> Post Your Comment </td> 
   </tr> 
   <tr> 
    <td> postModalButton </td> 
    <td> Post Your Comment </td> 
   </tr> 
   <tr> 
    <td> postModalPlaceholder </td> 
    <td> What would you like to say? </td> 
   </tr> 
   <tr> 
    <td> showMoreButtonText </td> 
    <td> Load More </td> 
   </tr> 
   <tr> 
    <td> shareButtonText </td> 
    <td> Share </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Map {#section_fxv_c5n_xz}

Strings available for Maps.

<table id="table_kdg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> featuredText </td> 
    <td> Featured </td> 
   </tr> 
   <tr> 
    <td> shareButtonText </td> 
    <td> Share </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Mosaic {#section_e2s_b5n_xz}

Strings available for Mosaics.

<table id="table_ldg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> featuredText </td> 
    <td> Featured </td> 
   </tr> 
   <tr> 
    <td> shareButtonText </td> 
    <td> Share </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Carousel {#section_l2z_hkn_xz}

Strings available for Carousel.

<table id="table_mdg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> featuredText </td> 
    <td> Featured </td> 
   </tr> 
   <tr> 
    <td> shareButtonText </td> 
    <td> Share </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Feature Card {#section_mw2_hkn_xz}

Strings available for the Feature Card.

<table id="table_ndg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> featuredText </td> 
    <td> Featured </td> 
   </tr> 
   <tr> 
    <td> shareButtonText </td> 
    <td> Share </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Upload App {#section_grc_gkn_xz}

Strings available for the Upload App.

<table id="table_odg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> postButtonText </td> 
    <td> What’s on your mind? </td> 
   </tr> 
   <tr> 
    <td> postModalTitle </td> 
    <td> Post Your Comment </td> 
   </tr> 
   <tr> 
    <td> postModalButton </td> 
    <td> Post Your Comment </td> 
   </tr> 
   <tr> 
    <td> postModalTitlePlaceholder </td> 
    <td> Enter a title </td> 
   </tr> 
   <tr> 
    <td> postModalPlaceholder </td> 
    <td> What would you like to say? </td> 
   </tr> 
   <tr> 
    <td> postModalConfirationTitle </td> 
    <td> Thank you for posting! </td> 
   </tr> 
   <tr> 
    <td> postModalConfirmationMessage </td> 
    <td> Your post is being reviewed. </td> 
   </tr> 
   <tr> 
    <td> postModalConfirmationButton </td> 
    <td> Done </td> 
   </tr> 
   <tr> 
    <td> title </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> message </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td> editorErrorAttachmentsRequired </td> 
    <td> An attachment is required </td> 
   </tr> 
   <tr> 
    <td> editorErrorBody </td> 
    <td> Please add a message </td> 
   </tr> 
   <tr> 
    <td> editorErrorDuplicate </td> 
    <td> As much as you like your note, you cannot post it twice </td> 
   </tr> 
   <tr> 
    <td> editorErrorGeneric </td> 
    <td> There was an error </td> 
   </tr> 
   <tr> 
    <td> editorErrorTitleRequired </td> 
    <td> A title is required </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Poll {#section_pdg_fwh_xz}

Strings available for Polls.

<table id="table_pdg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> totalVotesLabel </td> 
    <td> %s total votes </td> 
   </tr> 
   <tr> 
    <td> shareStringText </td> 
    <td> I just voted on %s what’s your vote? </td> 
   </tr> 
   <tr> 
    <td> pollClosedLabel </td> 
    <td> This poll is currently closed </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Livefyre Identity {#section_zc3_xvh_xz}

Strings available for Livefyre Identity.

<table id="table_qdg_pnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Key </th> 
    <th class="entry"> Default Text </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> automaticallyFollowConversations </td> 
    <td> Automatically follow conversations I join </td> 
   </tr> 
   <tr> 
    <td> back </td> 
    <td> Back </td> 
   </tr> 
   <tr> 
    <td> bio </td> 
    <td> Bio </td> 
   </tr> 
   <tr> 
    <td> create </td> 
    <td> Create </td> 
   </tr> 
   <tr> 
    <td> createANewAccount </td> 
    <td> Create New Account </td> 
   </tr> 
   <tr> 
    <td> createNewAccountWithEmail </td> 
    <td> Create a new account with email </td> 
   </tr> 
   <tr> 
    <td> changeAvatar </td> 
    <td> Change Avatar </td> 
   </tr> 
   <tr> 
    <td> chooseFile </td> 
    <td> Choose File </td> 
   </tr> 
   <tr> 
    <td> completeAccount </td> 
    <td> Complete account </td> 
   </tr> 
   <tr> 
    <td> emailWhenSomeoneReplies </td> 
    <td> Email when someone replies to me </td> 
   </tr> 
   <tr> 
    <td> emailCommentsIFollow </td> 
    <td> Email comments in conversations I follow </td> 
   </tr> 
   <tr> 
    <td> emailSenttoResetPassword </td> 
    <td> Email sent! Check your inbox for a link to reset your password </td> 
   </tr> 
   <tr> 
    <td> emailVerificationSent </td> 
    <td> Email Verification Sent </td> 
   </tr> 
   <tr> 
    <td> firstName </td> 
    <td> First name </td> 
   </tr> 
   <tr> 
    <td> forgotPassword </td> 
    <td> Forgot password? </td> 
   </tr> 
   <tr> 
    <td> forgotYourPassword </td> 
    <td> Forgot your password? </td> 
   </tr> 
   <tr> 
    <td> forgotYourPasswordInstructions </td> 
    <td> Enter your username or email address below, and we’ll send you a link to change your password. </td> 
   </tr> 
   <tr> 
    <td> formInputCloseButtonText </td> 
    <td> Close </td> 
   </tr> 
   <tr> 
    <td> formInputCancelButtonText </td> 
    <td> Cancel </td> 
   </tr> 
   <tr> 
    <td> formInputSaveButtonText </td> 
    <td> Save </td> 
   </tr> 
   <tr> 
    <td> hasNotLeftAnyComments </td> 
    <td> hasn’t left any comments </td> 
   </tr> 
   <tr> 
    <td> locationIsFrom </td> 
    <td> is from </td> 
   </tr> 
   <tr> 
    <td> labelAvatar </td> 
    <td> Avatar </td> 
   </tr> 
   <tr> 
    <td> labelComments </td> 
    <td> Comments </td> 
   </tr> 
   <tr> 
    <td> labelConfirmNewPassword </td> 
    <td> Confirm New Password </td> 
   </tr> 
   <tr> 
    <td> labelConfirmPassword </td> 
    <td> Confirm Password </td> 
   </tr> 
   <tr> 
    <td> labelEmail </td> 
    <td> Email Address </td> 
   </tr> 
   <tr> 
    <td> labelLikes </td> 
    <td> Likes </td> 
   </tr> 
   <tr> 
    <td> labelLoading </td> 
    <td> Loading </td> 
   </tr> 
   <tr> 
    <td> labelNewPassword </td> 
    <td> New Password </td> 
   </tr> 
   <tr> 
    <td> labelNotification </td> 
    <td> Notifications </td> 
   </tr> 
   <tr> 
    <td> labelPassword </td> 
    <td> Password </td> 
   </tr> 
   <tr> 
    <td> labelProfile </td> 
    <td> Profile </td> 
   </tr> 
   <tr> 
    <td> labelUsername </td> 
    <td> Username </td> 
   </tr> 
   <tr> 
    <td> labelUsernameOrEmail </td> 
    <td> Username or email </td> 
   </tr> 
   <tr> 
    <td> lastName </td> 
    <td> Last name </td> 
   </tr> 
   <tr> 
    <td> livefyreAccount </td> 
    <td> Livefyre Account </td> 
   </tr> 
   <tr> 
    <td> location </td> 
    <td> Location </td> 
   </tr> 
   <tr> 
    <td> loadingProfile </td> 
    <td> Loading Profile </td> 
   </tr> 
   <tr> 
    <td> newPassword </td> 
    <td> New Password </td> 
   </tr> 
   <tr> 
    <td> oldPassword </td> 
    <td> Old Password </td> 
   </tr> 
   <tr> 
    <td> on </td> 
    <td> on </td> 
   </tr> 
   <tr> 
    <td> or </td> 
    <td> or </td> 
   </tr> 
   <tr> 
    <td> passwordLinkExpired </td> 
    <td> The link you clicked to reset your password has expired. Reset your password again, and we’ll send you a new link. </td> 
   </tr> 
   <tr> 
    <td> pleasecheckEmailToComplete </td> 
    <td> Please check your email to complete your registration. </td> 
   </tr> 
   <tr> 
    <td> posted </td> 
    <td> Posted </td> 
   </tr> 
   <tr> 
    <td> poweredBy </td> 
    <td> powered by </td> 
   </tr> 
   <tr> 
    <td> profileNotificationImmediate </td> 
    <td> immediate </td> 
   </tr> 
   <tr> 
    <td> profileNotificationHourly </td> 
    <td> hourly </td> 
   </tr> 
   <tr> 
    <td> profileNotificationNever </td> 
    <td> never </td> 
   </tr> 
   <tr> 
    <td> recentComments </td> 
    <td> Recent Comments </td> 
   </tr> 
   <tr> 
    <td> reset </td> 
    <td> Reset </td> 
   </tr> 
   <tr> 
    <td> resetPassword </td> 
    <td> Reset Password </td> 
   </tr> 
   <tr> 
    <td> signIn </td> 
    <td> Sign In </td> 
   </tr> 
   <tr> 
    <td> signInWith </td> 
    <td> Sign In With </td> 
   </tr> 
   <tr> 
    <td> signInWithEmail </td> 
    <td> Sign In With Email </td> 
   </tr> 
   <tr> 
    <td> signUp </td> 
    <td> Sign Up </td> 
   </tr> 
   <tr> 
    <td> socialAccount </td> 
    <td> Social Account </td> 
   </tr> 
   <tr> 
    <td> successPasswordChanged </td> 
    <td> Success! Your password has been changed, and you are now logged in </td> 
   </tr> 
   <tr> 
    <td> termsAndConditions </td> 
    <td> Terms &amp; Conditions </td> 
   </tr> 
   <tr> 
    <td> termsAndConditionsIntro </td> 
    <td> By signing up you accept the </td> 
   </tr> 
   <tr> 
    <td> termsOfUse </td> 
    <td> Terms of Use </td> 
   </tr> 
   <tr> 
    <td> termsOfUseIntro </td> 
    <td> By logging in, you agree to </td> 
   </tr> 
   <tr> 
    <td> thisUser </td> 
    <td> This user </td> 
   </tr> 
   <tr> 
    <td> verifyPassword </td> 
    <td> Verify Password </td> 
   </tr> 
   <tr> 
    <td> fileSizeLimit </td> 
    <td> 2MB max </td> 
   </tr> 
   <tr> 
    <td> accountnotfound </td> 
    <td> Account not found </td> 
   </tr> 
   <tr> 
    <td> avatarImageExceedSize </td> 
    <td> Your avatar image has exceed the 2mb file limit </td> 
   </tr> 
   <tr> 
    <td> fieldisrequired </td> 
    <td> Field only accepts an integer </td> 
   </tr> 
   <tr> 
    <td> fieldonlyacceptsavalidemail </td> 
    <td> Field only accept a valid email </td> 
   </tr> 
   <tr> 
    <td> fieldonlyacceptsletters </td> 
    <td> Field only accepts letters </td> 
   </tr> 
   <tr> 
    <td> filesizemustbelessthanMB </td> 
    <td> File size must be less than {#}MB </td> 
   </tr> 
   <tr> 
    <td> invalidusernameorpassword </td> 
    <td> Invalid username or password </td> 
   </tr> 
   <tr> 
    <td> minimumlengthofcharacters </td> 
    <td> Minimum Length of {#} characters </td> 
   </tr> 
   <tr> 
    <td> maximumlengthofcharacters </td> 
    <td> Maximum length of {#} characters </td> 
   </tr> 
   <tr> 
    <td> therewasanerror </td> 
    <td> There was an error </td> 
   </tr> 
   <tr> 
    <td> thisfieldisrequired </td> 
    <td> This field is required. </td> 
   </tr> 
   <tr> 
    <td> validfileextensions </td> 
    <td> Valid file extensions </td> 
   </tr> 
   <tr> 
    <td> valuemustmatch </td> 
    <td> Value must match </td> 
   </tr> 
   <tr> 
    <td> passwordLength </td> 
    <td> be 6 to 32 character long. </td> 
   </tr> 
   <tr> 
    <td> passwordCharacters </td> 
    <td> include both lower and upper case characters. </td> 
   </tr> 
   <tr> 
    <td> passwordSymbols </td> 
    <td> include at least one number and one symbol. </td> 
   </tr> 
   <tr> 
    <td> passwordUsername </td> 
    <td> not contain your username. </td> 
   </tr> 
   <tr> 
    <td> passwordPopoverTitle </td> 
    <td> Your password needs to: </td> 
   </tr> 
   <tr> 
    <td> passwordErrorContainsFirstName </td> 
    <td> The password you entered contains either your username, first name or last name. For security reasons, please enter a password that does not contain your username, first name or last name. <p>Please also remember that your password needs to contain:</p> <p>6 to 32 characters</p> <p>An uppercase character</p> <p>A lowercase character</p> <p>A symbol</p> </td> 
   </tr> 
   <tr> 
    <td> passwordErrorContainsLastName </td> 
    <td> The password you entered contains either your username, first name or last name. For security reasons, please enter a password that does not contain your username, first name or last name. <p>Please also remember that your password needs to contain:</p> <p>6 to 32 characters</p> <p>An uppercase character</p> <p>A lowercase character</p> <p>A symbol</p> </td> 
   </tr> 
   <tr> 
    <td> passwordErrorContainsUsername </td> 
    <td> The password you entered contains either your username, first name or last name. For security reasons, please enter a password that does not contain your username, first name or last name. <p>Please also remember that your password needs to contain:</p> <p>6 to 32 characters</p> <p>An uppercase character</p> <p>A lowercase character</p> <p>A symbol</p> </td> 
   </tr> 
   <tr> 
    <td> passwordErrorTooShort </td> 
    <td> Minimum of 6 characters for pasword </td> 
   </tr> 
   <tr> 
    <td> passwordErrorTooLong </td> 
    <td> Maximum of 32 characters for password </td> 
   </tr> 
   <tr> 
    <td> passwordErrorMissingUppercase </td> 
    <td> Password should contain at least one uppercase character </td> 
   </tr> 
   <tr> 
    <td> passwordErrorMissingLowercase </td> 
    <td> Passsword should contain at least one lowercase character </td> 
   </tr> 
   <tr> 
    <td> passwordErrorMissingSymbol </td> 
    <td> Password should contain at least one symbol in the set !@#$%^&amp;*()?.,&lt;&gt;\’;:”[]{}| </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

