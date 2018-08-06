---
description: Allow users to select their notification frequency and content.
seo-description: Allow users to select their notification frequency and content.
seo-title: Email Notifications
title: Email Notifications
uuid: 195da78d-0e49-46e1-9f44-4367771cbea0
index: y
internal: n
snippet: y
translate: y
---

# Email Notifications

**Enable email notifications for your users and moderators.**
Livefyre Apps allow you to enable email notifications for your users and moderators, based on specific actions. Notifications are based upon the time when content is posted to the stream, allowing your users to remain engaged in conversations that they care about, and to be notified when someone likes or replies to one of their comments.
Users and Moderators may opt in or out of email notification, and may set the frequency with which emails are received. This section describes how to configure and customize these email notifications.

* User Email Options: available user notification options.
* Moderator Email Options: available moderator notification options.
* Livefyre Identity Emails Options: emails sent as part of Livefyre Identity. These emails are only relevant for Livefyre Identity Customers.
* Data Sync with Livefyre: maintaining preferences sync with Livefyre.
* Customizing Emails: available email customizations.
Use the Settings &gt; Integration Settings &gt; Email Notification Setup options to customize email notifications for your network.

>[!NOTE]
>
>To ensure that your end users do not receive unintended mail, no email notifications are sent from the Livefyre UAT environment.

**User Email Options**
Livefyre allows you to enable users to receive email notifications of site activity. Use the Livefyre-provided User Profile integration settings to allow users to select their preferences for notification schedules.

>[!NOTE]
>
>Emails are sent only for content posted manually into the stream, and not for content pulled from SocialSync or Curate.

To allow users to set their notification preferences, include an Email Notification section in the User Settings for your user profile system. Add the corresponding fields to your user profile database schema, then manage your user settings using Ping for Pull. (Work with your Technical Integration Manager to define default frequencies for your network. If you are an Enterprise Profiles customer, pass your selected defaults to your Livefyre delivery team for configuration in the Livefyre database.)
Users on your site can then follow a conversation and begin receiving email notifications by clicking the ** `+Follow` ** button on the comment editor. Notification preferences are defined at the Livefyre network level. Any user settings will apply to all sites and conversations across your network.
**Recommended Defaults**

* Someone comments in a conversation I’m following: **hourly digest**
* Someone likes one of my comments: **hourly digest**
* Someone replies to one of my comments: **immediately**
* Auto-follow conversations when I leave a comment: **off** (unchecked)
**Note**: Email notifications are based upon the time content is approved for inclusion in the stream.
Livefyre offers two email frequency options:

* Immediately
* Hourly Digest
**Immediately**
Emails sent immediately display the post’s text, article title, author’s username, and a **Reply** link which takes the user to the content on the page. These emails also include an **unsubscribe** link in the footer, allowing users to unsubscribe from email notifications for that Collection. Clicking **unsubscribe**will take them to a confirmation page letting them know that they have been unsubscribed from the Collection.
**Hourly Digest**
Emails sent in an hourly digest display all content, replies to content, and likes on the content within the last hour (or so) per Collection that the user is following. If the user is following multiple Collections across your network, they will receive one digest email for each Collection.

>[!NOTE]
>
>In conversations without new content for more than several hours, users with hourly digest enabled will receive notice immediately upon a new content post.

**Moderator Email Options**
Moderators can opt in to receive emails for content posted in a Collection they are following, and for comments flagged Spam or Offensive in a Collection they are moderating. **Note:**No emails will be sent when users flag a comment with Disagree or Off-Topic, as these categories are not deemed important for moderator notification.
The moderator_comments and moderator_flags fields should also be added to your moderator user profile settings page database schema to allow your moderators to update the frequency of their email notifications, and opt out if they wish. Livefyre recommends that you set these two moderator email notification fields to **never**. Options include **never** (default), **immediately**, and **often**.
**Moderator Email (flagged content):**
When content is flagged in a moderated Collection, the email sent to the moderator will display the content that was flagged, the username who flagged the content, and a link back to the content page.
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
