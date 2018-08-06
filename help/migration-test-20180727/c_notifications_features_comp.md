---
description: You can set up several different types of notifications for site visitors and Livefyre Moderators to use to interact with the end user.
seo-description: You can set up several different types of notifications for site visitors and Livefyre Moderators to use to interact with the end user.
seo-title: Notifications Features
solution: Experience Manager
title: Notifications Features
uuid: c1d2d944-d5f3-4584-8249-640769a9ebb5
index: y
internal: n
snippet: y
translate: y
---

# Notifications Features

## Notifications Features {#c_notifications_features}You can set up several different types of notifications for site visitors and Livefyre Moderators to use to interact with the end user.<!-- c_notifications_features.dita --> On this page:
* [](#c_comment_notifier)
* [](#c_email_notifications)
* [](#c_email_notifications/section_jxb_c5k_yy)
* [](#t_set_up_network_email)

>## Comment Notifier {#c_comment_notifier}Allows you to enable a small pop-up on the page to notify users when a comment has been added.<!-- c_comment_notifier.dita --> The Comment Notifier is a small pop-up at the bottom right of the page, that notifies users on the page of new activity in the stream by displaying the first few words of the comment with the Avatar for its author. (Notifiers are not available for Top Comments, Hot Threads, or Queued Comments.)

## Comment Notifier Features {#section_ut2_lvx_vy}

The comment notifier increases user engagement by surfacing activity happening on the page, no matter where on the page the user is currently engaged, encouraging them to click on new comments, and respond.
The notifier includes a preview of the latest comment, and the user’s avatar to the left of text. The total count of new comments is displayed in the toolbar underneath, and this number increments with more posts in the stream. If there are two or more new comments above or below the user’s current view of the stream, a scroll bar will appear within the notifier, allowing the user to scroll and view snippets of all other new comments.
Click the preview of a new comment to jump to the location of that comment in the stream. Click the number of new comments to expand the pane to show a preview of each unread comment.
The notifier disappears after all new comments have been viewed, and reappears when a new comment appears above or below the user’s current view of the stream.

## Hiding the Comment Notifier {#section_cmy_cvx_vy}

Click the ** `x` ** in the right corner of the ** `New Comments` ** bar to close the notifier for the page. Refresh the page, and the notifier will reappear.
Hide the notifier widget across your entire network using CSS Customizations.

>[!NOTE]
>
>The comment notifier is not available on mobile devices.


<a id="section_blk_ccj_h1b"></a>

Apps that use this feature:

* [Comments](c_comments_app.md#c_comments_app)
>## Email Notifications {#c_email_notifications}Allow users to select their notification frequency and content.<!-- c_email_notifications.dita --> **Enable email notifications for your users and moderators.** 
Livefyre Apps allow you to enable email notifications for your users and moderators, based on specific actions. Notifications are based upon the time when content is posted to the App, allowing your users to remain engaged in conversations that they care about, and to be notified when someone likes or replies to one of their comments.
Users and Moderators may opt in or out of email notification, and may set the frequency with which emails are received. This section describes how to configure and customize these email notifications.

* User Email Options: available user notification options.
* Moderator Email Options: available moderator notification options.
* Livefyre Identity Emails Options: emails sent as part of Livefyre Identity. These emails are only relevant for Livefyre Identity Customers.
* Data Sync with Livefyre: maintaining preferences sync with Livefyre.
* Customizing Emails: available email customizations.
Use the **Settings &gt; Integration Settings &gt; Email Notification Setup** options to customize email notifications for your network.

>[!NOTE]
>
>To ensure that your end users do not receive unintended mail, no email notifications are sent from the Livefyre UAT environment.

**User Email Options** 
Livefyre allows you to enable users to receive email notifications of site activity. Use the Livefyre-provided User Profile integration settings to allow users to select their preferences for notification schedules.

>[!NOTE]
>
>Emails are sent only for content posted manually into the stream, and not for content pulled from SocialSync.

To allow users to set their notification preferences, include an Email Notification section in the User Settings for your user profile system. Add the corresponding fields to your user profile database schema, then manage your user settings using Ping for Pull. (Work with your Technical Integration Manager to define default frequencies for your network. If you are an Enterprise Profiles customer, pass your selected defaults to your Livefyre delivery team for configuration in the Livefyre database.)
Users on your site can then follow a conversation and begin receiving email notifications by clicking the ** `+Follow` ** button on the comment editor. Notification preferences are defined at the Livefyre network level. Any user settings will apply to all sites and conversations across your network.
**Recommended Defaults** 

* Someone comments in a conversation I’m following: **hourly digest**
* Someone likes one of my comments: **hourly digest**
* Someone replies to one of my comments: **immediately**
* Auto-follow conversations when I leave a comment: **off** (unchecked)
**Note**: Email notifications are based upon the time content is approved for inclusion in the App.
Livefyre offers two email frequency options:

* Immediately
* Hourly Digest
**Immediately** 
Emails sent immediately display the post’s text, article title, author’s username, and a **Reply** link which takes the user to the content on the page. These emails also include an **unsubscribe** link in the footer, allowing users to unsubscribe from email notifications for that App. Clicking **unsubscribe**will take them to a confirmation page letting them know that they have been unsubscribed from the App.
**Hourly Digest** 
Emails sent in an hourly digest display all content, replies to content, and likes on the content within the last hour (or so) per App that the user is following. If the user is following multiple Apps across your network, they will receive one digest email for each App.

>[!NOTE]
>
>In conversations without new content for more than several hours, users with hourly digest enabled will receive notice immediately upon a new content post.

**Moderator Email Options** 
Moderators can opt in to receive emails for content posted in an App they are following, and for comments flagged Spam or Offensive in an App they are moderating. **Note:**No emails will be sent when users flag a comment with Disagree or Off-Topic, as these categories are not deemed important for moderator notification.
The moderator_comments and moderator_flags fields should also be added to your moderator user profile settings page database schema to allow your moderators to update the frequency of their email notifications, and opt out if they wish. Livefyre recommends that you set these two moderator email notification fields to **never**. Options include **never** (default), **immediately**, and **often**.
**Moderator Email (flagged content):** 
When content is flagged in a moderated App, the email sent to the moderator will display the content that was flagged, the username who flagged the content, and a link back to the content page.
When a user changes their email notification preferences on your site in your profile system, sync the update to the Livefyre remote profile system using Livefyre’s Ping for Pull.
**Data Sync with Livefyre** 

## Customizing Emails {#section_jxb_c5k_yy}

Several fields in the email notification templates may be changed to fit your style and brand.

* ** `From Email Address` ** 
  The “from email address” for all email notifications may be customized to be consistent with your brand. Livefyre recommends **noreply@customerdomain.com**, replacing **customerdomain**with your domain name. (The default is **noreply@livefyre.com**.) Please pass your preferred “from email address” to your Technical Integration Manager for configuration in the Livefyre database for your network.

  >[!NOTE]
  >
  >Leave this field blank to disable email notifications for your network

* ** `Email Logo` ** 
  The logo displayed in email notifications may be customized to display your company logo, rather than the default Livefyre logo, using the Branding tab of the **Network Settings** page of Studio. This customization is available only at the network level, not the site level, and is available only for paid Livefyre customers.

* ** `Custom Templates` ** 
  It is possible to implement a fully customized email template if you wish. However, this will require some development effort and may incur professional services costs. Please contact your Account Manager for details.


<a id="section_blk_ccj_h1b"></a>

Apps that use this feature:

* [Carousel](c_carousel_app.md#c_carousel_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](c_feature_card_app.md#c_feature_card_app)
* [Media Wall](c_media_wall_app.md#c_media_wall_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
>## Set up Network Email {#t_set_up_network_email}Customize available email notification fields.<!-- t_set_up_network_email.dita --> **Email Notification Setup** 

* **Logo for Email:**select the file that will be used as the logo in customer email notifications.
* **Email From:**enter the email address that will appear in the From field. (**Note:**If this field is blank, no email notifications will be sent.)
* **Email Display Name:**enter the name that will appear in place of your email address in comment email notifications.
