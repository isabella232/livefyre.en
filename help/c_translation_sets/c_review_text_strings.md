---
description: Customizing the text strings for Livefyre Reviews.
seo-description: Customizing the text strings for Livefyre Reviews.
seo-title: Review Text Strings
solution: Experience Manager
title: Review Text Strings
uuid: 89f7e87c-400a-491a-9f9f-15c6bc762fef
index: y
internal: n
snippet: y
translate: y
---

# Review Text Strings

Customizing the text strings for Livefyre Reviews.

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
 <thead> 
  <tr> 
   <th class="entry"> Element </th> 
   <th class="entry"> Key </th> 
   <th class="entry"> Default Text </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colspan="2"> <i>Buttons</i> </td> 
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
   <td> <a href="http://d.pr/i/QscA" format="html" scope="external"> Write review </a> </td> 
  </tr> 
  <tr> 
   <td></td> 
   <td> reviewsClosed </td> 
   <td> <a href="http://d.pr/i/zr7M" format="html" scope="external"> Reviews Closed </a> </td> 
  </tr> 
  <tr> 
   <td></td> 
   <td> showReviewBtn </td> 
   <td> <a href="http://d.pr/i/onxU" format="html" scope="external"> Show review </a> </td> 
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
   <td colspan="2"> <i>Rating tooltips</i> </td> 
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
   <td colspan="2"> <i>Rating subparts</i> </td> 
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
   <td colspan="2"> <i>Misc</i> </td> 
   <td></td> 
  </tr> 
  <tr> 
   <td></td> 
   <td> averageRating </td> 
   <td> <a href="http://d.pr/i/QscA" format="html" scope="external"> Average User Rating </a> </td> 
  </tr> 
  <tr> 
   <td></td> 
   <td> breakdownHeader </td> 
   <td> <a href="http://d.pr/i/QscA" format="html" scope="external"> Rating Breakdown </a> </td> 
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
</table>

## Stream Info {#section_wmv_yj4_xz}

Strings available for content stream information and display.

|  Element  | Key  | Default Text  |
|---|---|---|
|  *Sorting* | | |
|  | sortBy  | *Blank by default.* |
|  | sortHighestRated  | [Highest rating](http://d.pr/i/huTd)  |
|  | sortLowestRated  | [Lowest rating](http://d.pr/i/huTd)  |
|  | sortMostHelpful  | [Most helpful](http://d.pr/i/huTd)  |
|  *Stream misc.* | | |
|  | showMore  | Show More  |
|  *Stream high velocity* | | |
|  | newComment  | New Review  |
|  | newComments  | New Reviews  |
|  *Listener counts* | | |
|  | listenerCount  | person listening  |
|  | listenerCountPlural  | people listening  |
|  *Comment counts* | | |
|  | commentCountLabel  | LiveReviews<strong>|</strong>%s  |
|  | commentCountLabelPlural  | LiveReviews<strong>|</strong>%s  |
|  *Comment notifier counts* | | |
|  | commentNotifier  | New Review  |
|  | commentNotifierPlural  | New Reviews  |

## Author / Content Info {#section_osx_xj4_xz}

Stings available for author and individual content information.

|  Element  | Key  | Default Text  |
|---|---|---|
|  *Thread Breakout* | | |
|  | reviewsContentNotFoundMsg  | [This review is no longer visible](http://d.pr/i/svXs)  |
|  | backToComments  | Back to Reviews  |

## User Actions {#section_tlx_wj4_xz}

Strings available for user actions: flagging, sharing, and marking existing content as helpful.

|  Element  | Key  | Default Text  |
|---|---|---|
|  *Comment footer* | | |
|  | wasReviewHelpful  | [Helpful?](http://d.pr/i/Q0mA)  |
|  | wasReviewHelpfulMobile  | Helpful?  |
|  | ownWasReviewHelpful  | [Found helpful.](http://d.pr/i/Q0mA)  |
|  | reviewWasHelpful  | [Yes](http://d.pr/i/Q0mA)  |
|  | helpfulDivider  | [|](http://d.pr/i/Q0mA)  |
|  | reviewWasNotHelpful  | [No](http://d.pr/i/Q0mA)  |
|  *Vote modal* | | |
|  | voteTitle  | Was this review helpful?  |
|  | voteDownvote  | No  |
|  | voteReplyTitle  | Was this reply helpful?  |
|  | voteTitle  | Was this comment helpful?  |
|  | voteUpvote  | Yes  |
|  *Flag modal* | | |
|  | flagTitle  | Flag %s’s review  |
|  | flagSuccessMsg  | Review has been flagged.  |
|  *Flag Mobile* | | |
|  | flagConfirmationMessage  | Flag %s’s review as %s?  |
|  *Mention modal* | | |
|  | mentionDefaultText  | I mentioned you in a Livefyre review!  |
|  *Share modal* | | |
|  | shareTitle  | Share Review  |

## Post Functions {#section_yl1_wj4_xz}

Strings available for users posting reviews.

|  Element  | Key  | Default Text  |
|---|---|---|
|  *Editor* | | |
|  | bodyPlaceholder  | Write review…  |
|  | postEditButton  | Edit  |
|  | postEditCancelButton  | Cancel  |
|  | postAsButton  | Post review as…  |
|  | postButton  | Post review  |
|  | postReplyAsButton  | Post as…  |
|  | postReplyButton  | Post  |
|  | shareButton  | Share  |
|  | titlePlaceholder  | Title…  |

## Errors {#section_jbc_vj4_xz}

Strings available for general error messages.

|  Element  | Key  | Default Text  |
|---|---|---|
|  Errors  | | |
|  | errorAlreadyPosted  | You can only post one review.  |
|  | errorAuthError  | You’re not authorized to post a review on this conversation  |
|  | errorCommentsNotAllowed  | Reviews cannot be posted at this time  |
|  | errorDislikeOwnComment  | You cannot dislike your own review  |
|  | errorDuplicate  | As much as you liked your review, you’re not allowed to post it twice.  |
|  | errorEditDuplicate  | You must change the body of the review when you edit it.  |
|  | errorEditNotAllowed  | You’re not allowed to edit reviews on this conversation.  |
|  | errorEditTimeExceeded  | Sorry, your review editing period has expired.  |
|  | errorEmpty  | It seems you’re attempting to post an empty review.  |
|  | errorEmptyTitle  | It seems you’re attempting to post an empty title  |
|  | errorFieldRating  | star rating  |
|  | errorFieldReview  | review  |
|  | errorFieldTitle  | title  |
|  | errorMaxChars  | Sorry, your review is too long. Please edit and try again.  |
|  | errorMissingFields  | Please enter a  |
|  | errorRatingEmpty  | You cannot submit an empty rating  |
|  | errorRatingNotSet  | All ratings must be set  |
|  | errorRatingNotValid  | The rating must be an object  |
|  | errorShowMore  | There was an error loading more reviews.  |
|  | errorTitleMaxChars  | Sorry, your title is too long. Please edit and try again.  |
|  | errorVoteOwnComment  | You cannot vote on your own review  |

