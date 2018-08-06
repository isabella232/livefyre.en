---
description: Define the settings for requesting rights for Instagram and Twitter posts.
seo-description: Define the settings for requesting rights for Instagram and Twitter posts.
seo-title: Set up Rights Management
solution: Experience Manager
title: Set up Rights Management
uuid: dc3239a3-ed5a-4a22-85bf-0c882520722a
index: y
internal: n
snippet: y
translate: y
---

# Set up Rights Management

Before you can define Rights Request Settings, you must configure one or more social accounts for Instagram or Twitter. For more information on how to configure a social account, see [](t_configure_social_accout_instagram.md#t_configure_social_accout_instagram).

>[!NOTE]
>
>You can configure rights management at the Network level only. You cannot configure site-specific rights management.


>1. Within Livefyre Studio, navigate to ** `Network` ** ** `Settings > Rights Management` **.

>   >[!NOTE]
>   >
>   >You will need Moderator or Administrator network-level permissions in order to set up Rights Management Accounts.
>
>1. Select ** `+Add New Account` ** if you do not have any Rights Management accounts set up.
>1. Click ** `Create New Setting` ** under the social network you want to use for Rights Management.

>   >[!NOTE]
>   >
>   >For Instagram accounts, you can add an Instagram personal account to manually request rights or an Instagram business account to request rights with partial automation. For more information on the different kinds of Instagram accounts and how to use them, see[](c_about_instagram_accounts.md#c_about_instagram_accounts).
>
>1. Fill in the displayed fields. All fields are required.
>    
>    * ** `Display name:` ** Enter a display name to identify the Twitter or Instagram account to use for your Rights Request account. This name is internal only.
>    * ** `Enabled:` **Set to on by default. Enables rights management for the account.
>    * ** `Approval hashtag:` ** The hashtag that the content owner will use to indicate that they consent to use their content.
>    * ** `Terms and conditions:` ** A link to your network’s Terms and Conditions for the reuse of content. This field is case sensitive.
>    * ** `Network and sites:` ** The network or site for which this account can request content reuse rights. To make this account available across your entire network, select the first item in the list, or limit to specific sites using the Command/CTRL key.
>    * ** `Default message:` ** A message to display with your Rights Request. You can override this message when you request rights.>    
>        * Livefyre presents one of the default messages to moderators when a moderator issues a request to a content author. Moderators can generate another default message or edit the message before sending. Messages must include the author’s Twitter or Instagram handle ({handle}), your approval hashtag ({grantTag}), and a link to your Terms and Conditions ({termsLink}).
>          ** `Note:` ** {handle}, {grantTag}, and {termsLink} are all case sensitive.
>          ** `Note:` ** To prevent malicious use, Twitter wraps any included URLs with [t.co](https://t.co/) formatting. To prevent your default message from exceeding 140 characters, Livefyre recommends against including URLs in your default message.

>        * Best practices for writing rights request messages:>        
>            * Create multiple default messages so you don’t sound like a robot. Save each default message prior to creating your next default message.
>            * Encourage your moderators to personalize this note before sending, to prevent your network’s requests from being tagged Spam.


>    
>1. Click ** `Save Settings` ** to add your Rights Request account.
