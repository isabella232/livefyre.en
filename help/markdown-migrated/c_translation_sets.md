---
description: Customizing the text strings for Livefyre Sidenotes
seo-description: Customizing the text strings for Livefyre Sidenotes
seo-title: Sidenotes Text Strings
solution: Experience Manager
title: Sidenotes Text Strings
---

# Sidenotes Text Strings


>## Translation Sets {#c_translation_sets}
>Translation Sets allow you to specify alternate language for Apps.

<!-- c_translation_sets.dita -->
Use translation settings to localize Apps in various languages or to specify alternate text for several Apps from one location in Studio. For example, you can ensure all Spanish-language sites use Spanish language for all App fields. You can also modify the text so that all fields match the voice and feel of your site or network.

You can specify translation settings for all Apps, except Storify 2. For more information about what fields you can localize, see [ Localize Strings ](c_localize_strings.md#c_localize_strings).

Comments, Live Blog, and Chat share the same set of strings within a translation set.

Specify a translation set for a network, site, app, or using an API.

The translation sets at different levels override each other following this pattern:

* API translation set overrides any translation sets at any level (App, network, and site)
* App translation set overrides network-level and site-level translation sets.
* Site-level translation sets override network-level translation sets.

>## <draft-comment author="ind14750" otherprops="merge">
 
    c_review_text_strings.dita
   
</draft-comment>Review Text Strings {#c_review_text_strings}
>Customizing the text strings for Livefyre Reviews.

This page lists and describes the strings available for customization in Review apps. The strings listed here are in addition to and overrides for the default strings for Livefyre core apps, listed in String Customizations. Where duplicates are listed, the strings listed in these tables are the default for Reviews apps.

* Implementation
* Review / Rating Interface
* Stream Info
* Author / Content Info
* User Actions
* Post Functions
* Errors
## Implementation {#section_vsy_1k4_xz}

To implement this feature, pass in a 1-1 object mapping of the strings you wish to override to the Javascript configuration object. If you don’t provide a field, the default text will be used.

Example:

```
var customStrings = { 
 postAsButton: "New Post As Text", 
 postEditButton: "New Post Edit Text" }; 
networkConfig["strings"] = customStrings; fyre.conv.load( 
 networkConfig, 
 [convConfig], 
 function(){} 
);
```
## Review / Rating Interface {#section_iyv_zj4_xz}

Strings available for the Review and Rating user interface.

<table id="table_jrv_snl_wz"> 
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
    <td namest="col1" nameend="col2"> <i>Buttons</i> </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> editReviewBtn </td> 
    <td> Edit review </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> reviewBtn </td> 
    <td> <a href="https://d.pr/i/QscA" format="html" scope="external"> Write review </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> reviewsClosed </td> 
    <td> <a href="https://d.pr/i/zr7M" format="html" scope="external"> Reviews Closed </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> showReviewBtn </td> 
    <td> <a href="https://d.pr/i/onxU" format="html" scope="external"> Show review </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> follow </td> 
    <td> I’m interested </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareText </td> 
    <td> I just wrote a review. Check it out! </td> 
   </tr> 
   <tr> 
    <td namest="col1" nameend="col2"> <i>Rating tooltips</i> </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> ratingValues </td> 
    <td> <i>An array. Default = </i>[‘Poor’, ‘Poor’, ‘Fair’, ‘Fair’, ‘Average’, ‘Average’, ‘Good’, ‘Good’, ‘Excellent’, ‘Excellent’]; 
     <ul id="ul_krv_snl_wz"> 
      <li><b>Note: </b>Values in the array must be duplicated to assign both the left and the right half of each star the same name.</li> 
     </ul> </td> 
   </tr> 
   <tr> 
    <td namest="col1" nameend="col2"> <i>Rating subparts</i> </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> ratingSubpartPlaceholders </td> 
    <td> <i>An array. Default = </i>[] </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> ratingSubpartTitles </td> 
    <td> <i>An array. Default = </i>[] </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> reviewStreamTitle </td> 
    <td> <i>Blank by default. Title of the summary section of the review.</i> </td> 
   </tr> 
   <tr> 
    <td namest="col1" nameend="col2"> <i>Misc</i> </td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> averageRating </td> 
    <td> <a href="https://d.pr/i/QscA" format="html" scope="external"> Average User Rating </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> breakdownHeader </td> 
    <td> <a href="https://d.pr/i/QscA" format="html" scope="external"> Rating Breakdown </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> helpful </td> 
    <td> %s of %s found helpful </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> helpfulPlural </td> 
    <td> %s of %s found helpful </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> outOf </td> 
    <td> / </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> ratingType </td> 
    <td> star </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Stream Info {#section_wmv_yj4_xz}

Strings available for content stream information and display.

<table id="table_lrv_snl_wz"> 
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
    <td> <i>Sorting</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sortBy </td> 
    <td> <i>Blank by default.</i> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sortHighestRated </td> 
    <td> <a href="https://d.pr/i/huTd" format="html" scope="external"> Highest rating </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sortLowestRated </td> 
    <td> <a href="https://d.pr/i/huTd" format="html" scope="external"> Lowest rating </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> sortMostHelpful </td> 
    <td> <a href="https://d.pr/i/huTd" format="html" scope="external"> Most helpful </a> </td> 
   </tr> 
   <tr> 
    <td> <i>Stream misc.</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> showMore </td> 
    <td> Show More </td> 
   </tr> 
   <tr> 
    <td> <i>Stream high velocity</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> newComment </td> 
    <td> New Review </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> newComments </td> 
    <td> New Reviews </td> 
   </tr> 
   <tr> 
    <td> <i>Listener counts</i> </td> 
    <td></td> 
    <td></td> 
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
    <td> <i>Comment counts</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentCountLabel </td> 
    <td> LiveReviews&lt;strong&gt;|&lt;/strong&gt;%s </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentCountLabelPlural </td> 
    <td> LiveReviews&lt;strong&gt;|&lt;/strong&gt;%s </td> 
   </tr> 
   <tr> 
    <td> <i>Comment notifier counts</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentNotifier </td> 
    <td> New Review </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> commentNotifierPlural </td> 
    <td> New Reviews </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Author / Content Info {#section_osx_xj4_xz}

Stings available for author and individual content information.

<table id="table_mrv_snl_wz"> 
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
    <td> <i>Thread Breakout</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> reviewsContentNotFoundMsg </td> 
    <td> <a href="https://d.pr/i/svXs" format="html" scope="external"> This review is no longer visible </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> backToComments </td> 
    <td> Back to Reviews </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## User Actions {#section_tlx_wj4_xz}

Strings available for user actions: flagging, sharing, and marking existing content as helpful.

<table id="table_nrv_snl_wz"> 
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
    <td> <i>Comment footer</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> wasReviewHelpful </td> 
    <td> <a href="https://d.pr/i/Q0mA" format="html" scope="external"> Helpful? </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> wasReviewHelpfulMobile </td> 
    <td> Helpful? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> ownWasReviewHelpful </td> 
    <td> <a href="https://d.pr/i/Q0mA" format="html" scope="external"> Found helpful. </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> reviewWasHelpful </td> 
    <td> <a href="https://d.pr/i/Q0mA" format="html" scope="external"> Yes </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> helpfulDivider </td> 
    <td> <a href="https://d.pr/i/Q0mA" format="html" scope="external"> | </a> </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> reviewWasNotHelpful </td> 
    <td> <a href="https://d.pr/i/Q0mA" format="html" scope="external"> No </a> </td> 
   </tr> 
   <tr> 
    <td> <i>Vote modal</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> voteTitle </td> 
    <td> Was this review helpful? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> voteDownvote </td> 
    <td> No </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> voteReplyTitle </td> 
    <td> Was this reply helpful? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> voteTitle </td> 
    <td> Was this comment helpful? </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> voteUpvote </td> 
    <td> Yes </td> 
   </tr> 
   <tr> 
    <td> <i>Flag modal</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagTitle </td> 
    <td> Flag %s’s review </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagSuccessMsg </td> 
    <td> Review has been flagged. </td> 
   </tr> 
   <tr> 
    <td> <i>Flag Mobile</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> flagConfirmationMessage </td> 
    <td> Flag %s’s review as %s? </td> 
   </tr> 
   <tr> 
    <td> <i>Mention modal</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> mentionDefaultText </td> 
    <td> I mentioned you in a Livefyre review! </td> 
   </tr> 
   <tr> 
    <td> <i>Share modal</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareTitle </td> 
    <td> Share Review </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Post Functions {#section_yl1_wj4_xz}

Strings available for users posting reviews.

<table id="table_orv_snl_wz"> 
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
    <td> <i>Editor</i> </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> bodyPlaceholder </td> 
    <td> Write review… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postEditButton </td> 
    <td> Edit </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postEditCancelButton </td> 
    <td> Cancel </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postAsButton </td> 
    <td> Post review as… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postButton </td> 
    <td> Post review </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postReplyAsButton </td> 
    <td> Post as… </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> postReplyButton </td> 
    <td> Post </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> shareButton </td> 
    <td> Share </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> titlePlaceholder </td> 
    <td> Title… </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Errors {#section_jbc_vj4_xz}

Strings available for general error messages.

<table id="table_prv_snl_wz"> 
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
    <td> Errors </td> 
    <td></td> 
    <td></td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorAlreadyPosted </td> 
    <td> You can only post one review. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorAuthError </td> 
    <td> You’re not authorized to post a review on this conversation </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorCommentsNotAllowed </td> 
    <td> Reviews cannot be posted at this time </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorDislikeOwnComment </td> 
    <td> You cannot dislike your own review </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorDuplicate </td> 
    <td> As much as you liked your review, you’re not allowed to post it twice. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorEditDuplicate </td> 
    <td> You must change the body of the review when you edit it. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorEditNotAllowed </td> 
    <td> You’re not allowed to edit reviews on this conversation. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorEditTimeExceeded </td> 
    <td> Sorry, your review editing period has expired. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorEmpty </td> 
    <td> It seems you’re attempting to post an empty review. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorEmptyTitle </td> 
    <td> It seems you’re attempting to post an empty title </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorFieldRating </td> 
    <td> star rating </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorFieldReview </td> 
    <td> review </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorFieldTitle </td> 
    <td> title </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorMaxChars </td> 
    <td> Sorry, your review is too long. Please edit and try again. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorMissingFields </td> 
    <td> Please enter a </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorRatingEmpty </td> 
    <td> You cannot submit an empty rating </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorRatingNotSet </td> 
    <td> All ratings must be set </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorRatingNotValid </td> 
    <td> The rating must be an object </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorShowMore </td> 
    <td> There was an error loading more reviews. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorTitleMaxChars </td> 
    <td> Sorry, your title is too long. Please edit and try again. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> errorVoteOwnComment </td> 
    <td> You cannot vote on your own review </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>


>## Sidenotes Text Strings {#c_sidenotes_text_strings}
>Customizing the text strings for Livefyre Sidenotes

<!-- c_sidenotes_text_strings.dita -->
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
    <td> <i>An array. Default = </i>[ ‘January’, ‘February’, ‘March’, ‘April’, ‘May’, ‘June’, ‘July’, ‘August’, ‘September’, ‘October’, ‘November’, ‘December’ ] </td> 
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

