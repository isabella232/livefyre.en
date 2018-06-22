---
description: Configure a Social Account in Settings to gather content from Instagram or Twitter to use in Livefyre Apps.
seo-description: Configure a Social Account in Settings to gather content from Instagram or Twitter to use in Livefyre Apps.
seo-title: c_social_accounts.ditaSocial Accounts
title: c_social_accounts.ditaSocial Accounts
---

# c_social_accounts.ditaSocial Accounts


>## Settings {#c_settings}
><draft-comment author="ind14750" otherprops="merge">
  c_settings.dita 
</draft-comment>Use Network and Site Settings to set moderation, filtering, and other settings.

With settings you can set up credentials, localize text for a site, and perform administrator tasks.


>## <draft-comment author="ind14750" otherprops="merge">
 
    c_how_requesting_rights_works.dita
   
</draft-comment>How Requesting Rights Works {#c_how_requesting_rights_works}
>When you bring user-generated content (UGC) into a Livefyre App, the content includes tacit permission for reuse. You cannot use content from Twitter or Instagram for other purposes without the author’s permission.

The following rights statuses are available from Library Assets, App Content, ModQ, and AEM Commerce:

* `uicontrol  Granted`. When the author grants you the right to reuse their content, the status of the asset changes to `uicontrol  Granted`.
  *
  `uicontrol  Expired`. Livefyre monitors the Instagram and Twitter stream for the author’s reply for 14 days. After 14 days, the request expires, the rights request status changes to `uicontrol  Expired`, and you can send a second request or remove the item from your Library.
  
  
  *
  `uicontrol  Requested`. Request permission for content from the Library. You can do this for one or more assets at a time. After you request permission, Livefyre sets the asset status to `uicontrol  Requested`.
  
  
* `uicontrol  Needs Review`. If the author replies with a note that does not include your #approvalHashtag, the status of the asset changes to `uicontrol  Needs Review`.
* `uicontrol  Request Failed`. Request failed to be sent (due to expired token, etc.).
* `uicontrol  Request Pending`. Queues the Rights Request so that not too many are sent at one time.
## Managing Rights Requests {#section_iy1_dhx_cbb}

You can manage Rights Requests in the following ways:

* Request Rights from the Library. For more information on how to request rights from the Library, see [](#c_how_requesting_rights_works/section_npr_qmn_bbb).
* Request Rights from App Content. For more information on how to request rights from the App Content, see [](#c_how_requesting_rights_works/section_cdp_hzl_dbb).
* Request Rights from ModQ. For more information on how to request rights from the ModQ, see [](#c_how_requesting_rights_works/section_ays_qrn_bbb)
* Request Rights from AEM Commerce. For more information on how to request rights from AEM Commerce. See [](t_request_rights_using_aem_assets.md#t_request_rights_using_aem_assets).
* Search for content with a specific rights status in the Library or App Content to follow-up on previous rights requests. For more on how to manage content with previous rights requests, see [](#c_how_requesting_rights_works/section_vd3_cnn_bbb).
* View the rights request history for a piece of content. For more information on how to view the history of rights requests for a piece of content, see [](#c_how_requesting_rights_works/section_cj5_nxl_dbb).
  *
  Manually override the rights for one or more assets at a time. For more on how to manually grant rights, see [](#c_how_requesting_rights_works/section_gpx_gnn_bbb).
  
  >[!NOTE]
  >
  >Overriding a rights request is stating that you own the content. Do not override a rights request without verifying that you own the content.
  
## Set up Rights Management {#section_xzk_bmn_bbb}

Before you can define Rights Request Settings, you must configure one or more social accounts for Instagram or Twitter. For more information on how to configure a social account, see [ Social Accounts ](c_social_accounts.md#c_social_accounts).

>[!NOTE]
>
>You can configure rights management at the Network level only. You cannot configure site-specific rights management.
1. Within Livefyre Studio, navigate to `uicontrol  Network` `uicontrol  Settings &gt; Rights Management`.
   >[!NOTE]
   >
   >You will need Moderator or Administrator network-level permissions in order to set up Rights Management Accounts.
   
1. Select `uicontrol  +Add New Account` if you do not have any Rights Management accounts set up.
1. Click `uicontrol  Create New Setting`.
1. Fill in the displayed fields. All fields are required.
    * `uicontrol  Display name:` Enter a display name to identify the Twitter or Instagram account to use for your Rights Request account. This name is internal only.
    * `uicontrol  Enabled:`Set to on by default. Enables rights management for the account.
    * `uicontrol  Approval hashtag:` The hashtag that the content owner will use to indicate that they consent to use their content.
    * `uicontrol  Terms and conditions:` A link to your network’s Terms and Conditions for the reuse of content. This field is case sensitive.
    * `uicontrol  Network and sites:` The network or site for which this account can request content reuse rights. To make this account available across your entire network, select the first item in the list, or limit to specific sites using the Command/CTRL key.
    * `uicontrol  Default message:` A message to display with your Rights Request. You can override this message when you request rights.
          *
          Livefyre presents one of the default messages to moderators when a moderator issues a request to a content author. Moderators can generate another default message or edit the message before sending. Messages must include the author’s Twitter or Instagram handle ({handle}), your approval hashtag ({grantTag}), and a link to your Terms and Conditions ({termsLink}).
          
          `uicontrol  Note:` {handle}, {grantTag}, and {termsLink} are all case sensitive.
          
          `uicontrol  Note:` To prevent malicious use, Twitter wraps any included URLs with [ t.co ](http://t.co/) formatting. To prevent your default message from exceeding 140 characters, Livefyre recommends against including URLs in your default message.
          
          
        * Best practices for writing rights request messages:
            * Create multiple default messages so you don’t sound like a robot. Save each default message prior to creating your next default message.
            * Encourage your moderators to personalize this note before sending, to prevent your network’s requests from being tagged Spam.
          
      
   
1. Click `uicontrol  Save Settings` to add your Rights Request account.
## Send a Rights Request from the Library {#section_npr_qmn_bbb}

You can request the right to reuse the item for your commercial purposes from the Library.

Before you can send a rights request you must:

* Add an Instagram or Twitter social account. For more information on how to configure a social account, see [ Social Accounts ](c_social_accounts.md#c_social_accounts).
* Set up Rights Management. For more information on how to set up rights management, see [](#c_how_requesting_rights_works/section_xzk_bmn_bbb).
1. Click on `uicontrol  Library` to access the Asset Library.
1. (Optional) Add content to folders using the Social Search.
1. Open a folder and click on a piece of content that you saved from Twitter or Instagram. You can see where the content originated by looking at the icon on the piece of content. For example, a piece of content from Twitter has the Twitter logo on it.
1. Click on the ellipsis icon that displays when you hover over the content card for `uicontrol  More Options`.
1. Click `uicontrol  Rights` to open the `uicontrol  Rights options` window.
1. Select the account to use to request rights.
1. (Optional) Edit the request message. If the message is missing an element or a required element is misspelled, an error message displays that specifies the incorrect or missing information.
1. Click `uicontrol  Send` to send the request to the owner of the content.
## View Rights Activity History {#section_cj5_nxl_dbb}

Livefyre keeps an audit trail of your rights activity. Specifically, Livefyre tracks:

* Requests sent to a social network user.
* Replies from a social network user on rights requests.
* Content status changes. Livefyre tracks which user changed the status and when they changed the status.
* Notes entered by a user on a rights management request.
* System error messages.
1. Click on `uicontrol  Library` to access the Asset Library.
1. (Optional) Add content to folders using the Social Search.
1. Open a folder and click on a piece of content that you saved from Twitter or Instagram. You can see where the content originated by looking at the icon on the piece of content. For example, a piece of content from Twitter has the Twitter logo on it.
1. Click on the ellipsis icon that displays when you hover over the content card for `uicontrol  More Options`.
1. Click `uicontrol  Rights` to open the `uicontrol  Rights options` window.
1. View the history under `uicontrol  Activity History`.
## Send Rights Request from App Content {#section_cdp_hzl_dbb}


1. Click on `uicontrol  Library`, then `uicontrol  App Content`.
1. Click on a piece of content.
1. Click `uicontrol  Actions` to open the `uicontrol  Actions` menu.
1. Click `uicontrol  Advanced`.
1. Click `uicontrol  OK` to save the content as an asset.
1. Click the checkbox next to `uicontrol  Request Rights` in the `uicontrol  Advanced Options` window.
1. Click `uicontrol  Save and Continue`.
1. Select the account to use to request rights.
1. (Optional) Edit the request message. If the message is missing an element or a required element is misspelled, an error message displays that specifies the incorrect or missing information.
1. Click `uicontrol  Send` to send the request to the owner of the content.

## Send Rights Request from ModQ {#section_ays_qrn_bbb}

1. Open `uicontrol  ModQ`.
1. Click on the `uicontrol  Streams Premoderation` tab.
1. Click the down arrow for `uicontrol  More Options` for a piece of content.
1. Select the account to use to request rights.
1. (Optional) Edit the request message.
1. Click `uicontrol  Send Request` to send the request to the owner of the content.
## Manage Content with a Pending Rights Request from the Asset Library {#section_vd3_cnn_bbb}

See and modify the assets in Livefyre with a pending rights request.

1. Click on `uicontrol  Library` to access `uicontrol  All Assets`.
1. Use the options in the `uicontrol  Rights` filter to choose a pending rights request status ( `uicontrol  Requested`, `uicontrol  Needs Review`) for specific assets.
1. Change the Rights Request status. See [](#c_how_requesting_rights_works/section_npr_qmn_bbb) for more on how to change Rights Request statuses in `uicontrol  All Assets`.
## Manage Content with a Pending Rights Request from App Content {#section_ymr_zdk_fbb}

See and modify the assets in Livefyre with a pending rights request.

1. Click on `uicontrol  Library` to access `uicontrol  App Content`.
1. Use the options in the `uicontrol  Rights` filter to choose a pending rights request status ( `uicontrol  Requested`, `uicontrol  Needs Review`) for specific assets.
1. Change the Rights Request status. See [](#c_how_requesting_rights_works/section_cdp_hzl_dbb) for more on how to change Rights Request statuses in `uicontrol  App Content`.
## Manually Grant or Revoke Rights for an Asset from the Asset Library {#section_gpx_gnn_bbb}

>[!NOTE]
>
>Manually granting rights on a piece of content is stating that you own the content. Do not manually grant rights without verifying that you own the content.
1. Click on `uicontrol  Library` to access the `uicontrol  Asset Library`.
1. Open a folder and click on a piece of content that you saved from Twitter or Instagram. You can see where the content originated by looking at the icon on the piece of content. For example, a piece of content from Twitter has the Twitter logo on it.
1. Click on the ellipsis icon that displays when you hover over the content card for `uicontrol  More Options`.
1. Click `uicontrol  Rights` to open the `uicontrol  Rights options` window.
1. Click `uicontrol  Manually Grant Rights`.
## Manually Grant or Revoke Rights for an Asset from App Content {#section_vbt_12k_fbb}

>[!NOTE]
>
>Manually granting rights on a piece of content is stating that you own the content. Do not manually grant rights without verifying that you own the content.
1. Click on `uicontrol  Library` to access `uicontrol  App Content`.
1. Click on a piece of content from Twitter or Instagram. You can see where the content originated by looking at the icon on the piece of content. For example, a piece of content from Twitter has the Twitter logo on it.
1. Click `uicontrol  Advanced`.
1. Click the checkbox next to `uicontrol  Request Rights` in the `uicontrol  Advanced Options` window.
1. Click `uicontrol  Save and Continue`.
1. Select Manually Grant Rights and enter a note explaining why you are manually granting rights.
1. Click `uicontrol  Grant` to manually grant rights.

>## <draft-comment author="ind14750" otherprops="merge">
 
    t_set_up_network_email.dita
   
</draft-comment>Set up Network Email {#t_set_up_network_email}
>Customize available email notification fields.

**Email Notification Setup**

  *
* **Logo for Email: **select the file that will be used as the logo in customer email notifications.
* **Email From: **enter the email address that will appear in the From field. (**Note: **If this field is blank, no email notifications will be sent.)
* **Email Display Name: **enter the name that will appear in place of your email address in comment email notifications.

>## <draft-comment author="ind14750" otherprops="merge">
 
    t_set_up_bans.dita
   
</draft-comment>Ban
      IP Addresses {#t_set_up_bans}
>You can ban IP addresses if a malicious user creates multiple accounts from the same IP address.

![](https://answers.livefyre.com/wp-content/uploads/2015/11/Bans-1024x239.png)

If a banned user begins to realize that no one is seeing their comments, they may decide to create a new user account, with a different username and avatar, and begin posting inappropriate or spam comments from this new, unbanned account. Your moderators may recognize the content as the same user, and verify this assumption by checking the IP address of the user posting the comments (from the Account Details page).

>1. Click `uicontrol  + IP Address` in the Banned IPs panel.
>   
>1. Enter the IP Address in the field. To Ban a range of IP addresses, enter the range in the format “192.168.0.1 - 192.168.0.10” (separate the IP addresses by spaces and a dash all in quotes) and click `uicontrol  Save`.
>   
>1. Select an action from the pulldown menu (Trash, Premoderate, or Bozo content).
>   
>1. Click the checkmark to save.
>   
>   

>## <draft-comment author="ind14750" otherprops="merge">
 
    t_set_up_user_sync.dita
   
</draft-comment>User Sync {#t_set_up_user_sync}
>User Sync allows you to enter the endpoint used to fetch user profile data from your user management system.

See Identity Integration &gt; Your Identity Service for more information on how Livefyre uses this URL to sync your user data with Livefyre through Ping for Pull.

**Custom User Profile Sync**

  *
  **Profile Sync URL:** enter the URL from which Livefyre will fetch your updated user profile information.
  
  For example: https://example.yoursite.com/some_path/?id={***id***}
  
  

>## <draft-comment author="ind14750" otherprops="merge">
 
    t_add_a_site.dita
   
</draft-comment>Add
      a Site to a Network {#t_add_a_site}
>You can add new sites to your network for domains and subdomains that share the same user profiles.

You can add and display up to 1,200 sites in Studio. Sites are listed alphabetically.

To add a new site to your network:

>1. click the `uicontrol  Network` item from the Studio menu bar to open the `uicontrol  Select Network or Site` panel.
>   
>1. Use the search field to search for sites, or click `uicontrol  Add new site` to add a new one.
>   This panel lists all sites included within the selected network.
>   
>   
>   
>1. Enter a `uicontrol  Name` and `uicontrol  URL` in the fields provided, and click `uicontrol  Add Site`.
>   
>   

>## <draft-comment author="ind14750" otherprops="merge">
 
    t_set_up_credentials.dita
   
</draft-comment>Set up Credentials {#t_set_up_credentials}

**Credentials**
The Credentials panel displays your Livefyre Network and Site Credentials. These fields will be populated by Livefyre during your integration process, and are available here for your reference. New Sites added through Studio will also be included in this page. These values are read-only.

**Network Credentials**
**Note: **Your Network Key is used **only** to generate userAuth tokens and is not used for any other API calls. When constructing collectionMeta tokens, the Site Key is used. For more information, see Developers &gt; Getting Started &gt; [ Building a User Auth Token ](https://answers.livefyre.com/developers/getting-started/tokens/auth/).

* Network Domain
* Network Key
**Site Credentials (per site)**
**Note: **Enter your site in the Search field to populate these fields.

* Site Name
* Site URL
* Site ID
* Site Key

>## <draft-comment author="ind14750" otherprops="merge">
 
    c_social_accounts.dita
   
</draft-comment>Social Accounts {#c_social_accounts}
>Configure a Social Account in Settings to gather content from Instagram or Twitter to use in Livefyre Apps.

Configure social accounts to:

* Perform social search on Instagram
* Create stream rules on Instagram
* Send rights requests to users on Twitter and Instagram.
