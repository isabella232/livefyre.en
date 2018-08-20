---
description: Customizing the strings of the Livefyre Apps.
seo-description: Customizing the strings of the Livefyre Apps.
seo-title: Localize Strings
solution: Experience Manager
title: Localize Strings
uuid: 1902ab89-fa69-4955-9d0f-6ce26a2fc58e
index: y
internal: n
snippet: y
translate: y
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
    * [](../c_translation_sets/c_review_text_strings.md#c_review_text_strings)
    * [ Sidenotes ](../c_translation_sets/c_sidenotes_text_strings.md#c_sidenotes_text_strings)


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
![](assets/strings_threadheader-150x40.png) 
|  Element  | Key  | Default Text  |
|---|---|---|
|  | displayName  | %s  |
|  | editProfile  | Edit profile  |
|  | notificationSettings  | Notification settings  |
|  | siteAdmin  | Admin Console (links to Studio)  |
|  | signOut  | Sign out  |


## Stream Info {#section_wx1_c24_xz}

Strings available for content stream information and display. Lists the number of people listening, the number of posts to the App, and allows users to sign in, or access their account information.

|  Key  | Default Text  | Stream data  |
|---|---|---|
|  | commentCountLabelZero  | %s comment  |
|  | commentCountLabel  | %s comment  |
|  | commentCountLabelPlural  | %s comments  |
|  | listenerCount  | person listening  |
|  | listenerCountPlural  | people listening  |
|  | liveblogPostCountLabelZero  | post  |
|  | liveblogPostCountLabel  | post  |
|  | liveblogPostCountLabelPlural  | posts  |
|  **Thread options** | | |
|  | threadBreakoutButton  | Show entire Thread  |
|  | toggleCollapse  | Toggle Collapse  |
|  **High velocity / queued comments** | | |
|  | refresh  | Refresh  |
|  | newComment  | New Comment  |
|  | newComments  | New Comments  |
|  | newReply  | new reply  |
|  | newReplies  | new replies  |


## Stream Sorting {#section_ih2_124_xz}

Allows uses to sort returned content by age or popularity.
![](assets/strings_newestoldesttop-1-150x56.png) 
|  Key  | Default Text  | Header options  |
|---|---|---|
|  | sortNewest  | Newest  |
|  | sortOldest  | Oldest  |
|  | sortTopComments  | Top Comments  |
|  | sortHotThreads  | Hot Threads  |
|  | sortSeparator  | |  |
|  | streamSorting  | Loading  |
|  | topCommentsContentNotFoundMsg  | There are not enough likes yet.  |
|  | hotThreadsContentNotFoundMsg  | There are not enough threads yet.  |
|  | streamRefreshMsg  | See what’s new.  |
|  **Footer options** | | |
|  | archiveHeaderTitle  | From the Archive  |
|  | archiveShowMore  | Show More  |
|  | showMore  | Show More Comments  |
|  | showMoreLiveblog  | Show More Posts  |

![](assets/strings_threadend-150x47.png) 
## Content Info {#section_llv_yd4_xz}

Lists post information: user name, any applied user tags, and post time.
![](assets/strings_authorinfo-150x52.png)  ![](assets/strings_posttime-150x45.png) 
|  Key  | Default Text  | Author  |
|---|---|---|
|  | moderator  | moderator  |
|  | hovercardViewProfile  | View Full Profile  |
|  **Post info** | | |
|  | timeJustNow  | just now  |
|  | timeMinutesAgo  | minute ago  |
|  | timeMinutesAgoPlural  | minutes ago  |
|  | timeHoursAgo  | hour ago  |
|  | timeHoursAgoPlural  | hours ago  |
|  | timeDaysAgo  | day ago  |
|  | timeDaysAgoPlural  | days ago  |
|  | likesPlural  | Likes  |
|  | likesSingular  | Like  |
|  | moderatorEditTimestamp  | Edited by a Moderator  |
|  | commentTombstone  | This comment has been deleted  |
|  | permalinkNotFoundMsg  | This comment is no longer visible.  |
|  | quickProfileTooltip  | Quick Profile  |


## Featured Content {#section_gmw_vd4_xz}

If enabled, featured content is listed at the top of the stream.

|  | Key  | Default Text  |
|---|---|---|
|  **Featured labels** | | |
|   ![](assets/strings_featuredcontent-150x40.png)  | featuredCommentsTag  | Featured  |
|  | featuredCommentsTitlePlural  | Featured Comments  |


## Text Editor {#section_ky5_td4_xz}

By default, available at the top of the page for all users.

|  | Key  | Default Text  |
|---|---|---|
|  **Editor buttons** | | |
|   ![](assets/strings_texteditor-1-150x77.png)  | follow  | + Follow  |
|  | unfollow  | - Unfollow  |
|  | liveblogFollow  | Follow Live Blog  |
|  | liveblogUnfollow  | Unfollow Live Blog  |
|  | postButton(Available for logged in users.)  | Post comment  |
|  | postAsButton(Available for unauthenticated users.)  | Post comment as…  |
|  | postEditButton  | Edit comment  |
|  | postEditAsButton  | Edit comment as…  |
|  | postEditCancelButton  | Cancel  |
|  | editorDisabled  | This conversation is currently closed to new comments.  |
|  **Chat options** | | |
|  | livechatPostButtonLabel  | Post  |
|  | livechatPostEditButton  | Edit  |
|  | livechatWindowsInstruction  | Press control+enter to post  |
|  | livechatOtherInstruction  | Press command+enter to post  |


## Response Options {#section_zvt_qd4_xz}

Unless otherwise noted, available to all logged in users. Mouse over a content panel to access.

|  Key  | Default Text  | |
|---|---|---|
|  **User Response Options** | Available for end users.  | |
|   ![](assets/strings_banusermodal-150x36.png)  | flagButton  | Flag  |
|  | flagCommentTooltip  | Flag  |
|  | editButton(Available only for authors and moderators, if enabled.)  | Edit  |
|  | deleteButton(Available only for authors and moderators, if enabled.)  | Delete  |
|  | deleteCommentTooltip  | Delete  |
|  | shareButton  | Share  |
|  | shareCommentTooltip  | Share  |
|  | likeButton  | Like  |
|  | unlikeButton  | Unlike  |
|  | replyButton  | Reply  |
|  | replyButtonSingular(Available for Chat and Live Blog.)  | Reply  |
|  | replyButtonPlural(Available for Chat and Live Blog.)  | Replies  |
|  **Flag Modal** | | |
|   ![](assets/strings_responseoptions-150x35.png)  | flagTitle  | Flag %s’s comment  |
|  | flagSubtitle  | Flag as  |
|  | flagDefaultSelectOption  | Select  |
|  | flagSpam  | Spam  |
|  | flagSpamButton  | Spam  |
|  | flagSpamCommentTooltip  | Spam  |
|  | flagOffensive  | Offensive  |
|  | flagOffensiveButton  | Offensive  |
|  | flagOffensiveCommentTooltip  | Offensive  |
|  | flagDisagree  | Disagree  |
|  | flagDisagreeButton  | Disagree  |
|  | flagDisagreeCommentTooltip  | Disagree  |
|  | flagOffTopic  | Off Topic  |
|  | flagOfftopicButton  | Off Topic  |
|  | flagOfftopicCommentTooltip  | Off Topic  |
|  | flagEmail  | Email  |
|  | flagEmailPlaceholder  | you@example.com  |
|  | flagNotes  | Notes  |
|  | flagNotesPlaceholder  | Start typing here…  |
|  | flagConfirmButton  | OK  |
|  | flagCancelButton  | Cancel  |
|  | flagConfirmationMessage  | Flag %s’s comment as %s?  |
|  | flagSuccessMsg  | Comment has been flagged.  |
|  **Share Modal** | | |
|   ![](assets/strings_flagmodal-150x87.png)  | shareTitle  | Share Comment  |
|  | sharePlaceholderText  | What do you think?  |
|  | shareLabel  | Share on:  |
|  | shareTextTwitter  | blank  |
|  | shareTextFacebook  | blank  |
|  | shareTextLinkedin  | blank  |
|  | shareButtonText  | Share  |
|  | sharePermalink  | Permalink  |
|  | loadingPermalink  | Loading short url…  |
|  | shareText  | I just posted a comment. Check it out!  |
|  **Reply Modal** | | |
|   ![](assets/strings_sharemodal-150x59.png)  | postReplyAsButton  | Post comment as…  |
|  | postReplyButton(Available for logged in users.)  | Post comment  |
|  | backToHotThreads  | Back to Hot Threads  |
|   ![](assets/strings_replymodal-150x64.png)  | backToComments(Appears above reply modal for featured content.)  | Back to Newest  |
|  **Twitter @mention modal** | | |
|   ![](assets/strings_backto-150x48.png)  | mentionTitle  | Share Mention  |
|  | mentionSubtitleTwitter  | Share Tweet to:  |
|  | mentionDefaultText  | I mentioned you in a Livefyre comment!  |
|  | mentionConfirmButton  | OK  |
|  | mentionCancelButton  | Cancel  |
|  | mentionErrorGeneral  | Oops! Something went wrong! Livefyre has been alerted.  |
|  | mentionErrorNoneSelected  | You must have at least one mention enabled.  |
|  | mentionMenuTitle  | To see and mention your friends  |
|  | mentionTwitterConnect  | Connect to Twitter  |
|  | mentionTwitterFetching  | Fetching Friends…  |
|  | mentionSuccessMsg  | Mentions have been successfully sent.  |
|  **Edit Modal** | Available to Studio Admins, User Managers or Moderators  | |
|   ![](assets/strings_sharemention-150x60.png)  | @(@mention.)  | |
|  | &amp;lt;/&amp;gt;(Opens the custom html window.)  | |
|  | customHtmlDialogTitle(Appears as the header for the modal.)  | Add Custom HTML  |
|  **Moderator Response Options** | Available to Studio Admins, User Managers or Moderators.  | |
|   ![](assets/strings_moderatoreditmodal-150x49.png)  | pendingComment  | pending  |
|  | banUserButton  | Ban user  |
|  | banUserTooltip  | Ban User  |
|  | bozoButton  | Bozo  |
|  | bozoCommentTooltip  | Bozo  |
|  | featureButton  | Feature  |
|  | featureCommentTooltip  | Feature  |
|  | unfeatureButton  | Unfeature  |
|  | featuredCommentTooltip  | Unfeature  |
|  | | |
|  **Ban User modal** | Available to Studio Admins, User Managers or Moderators.  | |
|   ![](assets/strings_adminoptions-150x33.png)  | banTitle  | Ban User  |
|  | banConfirmation  | Are you sure you want to ban this user?  |
|  | banConfirmButton  | OK  |
|  | banCancelButton  | Cancel  |


## Comment Notifier {#section_qqt_pd4_xz}

If enabled, available at the bottom of the page for all Livefyre conversation Apps.

|  | Key  | Default Text  |
|---|---|---|
|  **Notifier labels** | | |
|   ![](assets/strings_notifier-150x112.png)  | commentNotifier  | New Comment  |
|  | commentNotifierPlural  | New Comments  |
|  | liveblogNotifier  | New Post  |
|  | liveblogNotifierPlural  | New Posts  |


## Error Messages {#section_omz_jxn_xz}

Strings available for customizable error messages.

|  Key  | Default Text  |
|---|---|
|  errorAuthError  | You’re not authorized to post a comment on this conversation  |
|  errorCommentsNotAllowed  | Comments are not allowed on this conversation  |
|  errorDefault  | An error has occurred. Please try again.  |
|  errorDuplicate  | As much as you liked your comment, you’re not allowed to post it twice.  |
|  errorEditDuplicate  | You must change the body of the comment when you edit it.  |
|  errorEditNotAllowed  | You’re not allowed to edit comments on this conversation.  |
|  errorEditTimeExceeded  | Sorry, your comment editing period has expired.  |
|  errorEmpty  | It seems you’re attempting to post an empty comment.  |
|  errorExpired  | Your session has expired. Please reload the page.  |
|  errorFlagNotSelected  | Please select a flag type.  |
|  errorGuestLiked  | Sorry, only those with accounts can like content.  |
|  errorInsufficientPermissions  | Insufficient Permissions  |
|  errorInvalidChar  | It seems you’re attempting to post an invalid character.  |
|  errorLikeOwnComment  | You cannot like your own comment  |
|  errorMalformed  | It seems you’re attempting to post malformed content.  |
|  errorMaxChars  | Sorry, your comment is too long. Please edit and try again.  |
|  errorMediaNotAvailable  | Media is no longer visible.  |
|  errorShowMore  | There was an error loading more comments.  |
|  MultipleMediaNotAllowedError  | Your permissions only grant you one media attachment at a time.  |


## Time and Date Format {#section_yz4_g5n_xz}

Translate and customize how dates appear on content cards within visualization apps.

|  Key  | Default Text  |
|---|---|
|  hoursAgo  | {number}h  |
|  hoursAgoSingular  | {number}h  |
|  justNow  | 1s  |
|  minutesAgo  | {number}m  |
|  minutesAgoSingular  | {number}m  |
|  monthDayFormat  | {day} {monthAbbrev}  |
|  monthDayYearFormat  | {day} {monthAbbrev} {year}  |
|  monthNames  | January, February, March, April, May, June, July, August, September, October, November, December  |
|  monthNamesAbbrev  | Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec  |
|  secondsAgo  | {number}s  |
|  secondsAgoSingular  | {number}s  |


## Media Wall {#section_vwt_d5n_xz}

Strings available for the Media Wall App.

|  Key  | Default Text  |
|---|---|
|  featuredText  | Featured  |
|  shareButtonText  | Share  |


|  Key  | Default Text  |
|---|---|
|  postButtonText  | What’s on your mind?  |
|  postModalTitle  | Post Your Comment  |
|  postModalButton  | Post Your Comment  |
|  postModalPlaceholder  | What would you like to say?  |
|  showMoreButtonText  | Load More  |
|  shareButtonText  | Share  |


## Map {#section_fxv_c5n_xz}

Strings available for Maps.

|  Key  | Default Text  |
|---|---|
|  featuredText  | Featured  |
|  shareButtonText  | Share  |


## Mosaic {#section_e2s_b5n_xz}

Strings available for Mosaics.

|  Key  | Default Text  |
|---|---|
|  featuredText  | Featured  |
|  shareButtonText  | Share  |


## Carousel {#section_l2z_hkn_xz}

Strings available for Carousel.

|  Key  | Default Text  |
|---|---|
|  featuredText  | Featured  |
|  shareButtonText  | Share  |


## Feature Card {#section_mw2_hkn_xz}

Strings available for the Feature Card.

|  Key  | Default Text  |
|---|---|
|  featuredText  | Featured  |
|  shareButtonText  | Share  |


## Upload App {#section_grc_gkn_xz}

Strings available for the Upload App.

|  Key  | Default Text  |
|---|---|
|  postButtonText  | What’s on your mind?  |
|  postModalTitle  | Post Your Comment  |
|  postModalButton  | Post Your Comment  |
|  postModalTitlePlaceholder  | Enter a title  |
|  postModalPlaceholder  | What would you like to say?  |
|  postModalConfirationTitle  | Thank you for posting!  |
|  postModalConfirmationMessage  | Your post is being reviewed.  |
|  postModalConfirmationButton  | Done  |
|  title  | |
|  message  | |
|  editorErrorAttachmentsRequired  | An attachment is required  |
|  editorErrorBody  | Please add a message  |
|  editorErrorDuplicate  | As much as you like your note, you cannot post it twice  |
|  editorErrorGeneric  | There was an error  |
|  editorErrorTitleRequired  | A title is required  |


## Poll {#section_pdg_fwh_xz}

Strings available for Polls.

|  Key  | Default Text  |
|---|---|
|  totalVotesLabel  | %s total votes  |
|  shareStringText  | I just voted on %s what’s your vote?  |
|  pollClosedLabel  | This poll is currently closed  |


## Livefyre Identity {#section_zc3_xvh_xz}

Strings available for Livefyre Identity.

<table id="table_qdg_pnl_wz"> 
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
   <td> Terms &amp;amp; Conditions </td> 
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
   <td> Password should contain at least one symbol in the set !@#$%^&amp;amp;*()?.,&amp;lt;&amp;gt;\’;:”[]{}| </td> 
  </tr> 
 </tbody> 
</table>

