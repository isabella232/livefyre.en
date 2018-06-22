---
description: Credentials required to enable Livefyre Social Sharing.
seo-description: Credentials required to enable Livefyre Social Sharing.
seo-title: Setting up Social Sharing
solution: Experience Manager
title: Setting up Social Sharing
---

# Setting up Social Sharing


>## Social Sharing {#c_social_sharing}
>Share your content or content from another user, to Facebook, Twitter or LinkedIn.

On this page:

* [](#c_social_sharing/section_t1q_mz2_wy)
* [](#c_social_sharing/section_blw_vy2_wy)
* [](#c_setting_up_social_sharing)
* [](#c_setting_up_social_sharing/section_dzq_1p1_21b)
* [](#c_setting_up_social_sharing/section_tch_gp1_21b)
* [](#c_setting_up_social_sharing/section_xkd_kp1_21b)
* [](#c_setting_up_social_sharing/section_tqh_mp1_21b)
* [](#c_setting_up_social_sharing/section_ur2_np1_21b)
Social Sharing allows your community to share their thoughts from your App to their friends on social networks, including Facebook, Twitter, and LinkedIn, and to share other users’ content to Facebook and Twitter. Enabling Social Sharing allows your community to spread the best response to your content, and to bring more traffic to your site.

## Sharing content to social networks {#section_t1q_mz2_wy}

You may configure your network to allow users to share to Twitter, Facebook, or LinkedIn when posting content to your Livefyre Apps. The default Livefyre `uicontrol Share Modal` includes links to all three sites. You may customize this modal using the Post To API to override the Livefyre default, and implement your own. For more information, see Advanced Topics &gt; Enabling Social Sharing.

When users click `uicontrol Share` to post their comment to social networks (Facebook, Twitter or LinkedIn), they are prompted to log in through the social app. (The list of available Share options may be customized. By default, Facebook and Twitter share checkboxes are shown on all Apps.) For custom networks, the social apps should be configured to be your social apps. As part of your integration process, add your app credentials through the Integration Settings page in Studio.

>[!NOTE]
>
>LinkedIn is included by default on Livefyre Community Comments. Custom networks must pass in the ‘li’ value when embedding the App to enable the LinkedIn button on the comment toolbar. (For more information, please see Enabling Social Sharing in the developer docs.)
## Sharing other users’ content to social networks {#section_blw_vy2_wy}

Clicking `uicontrol Share` on another user’s post opens the Share Comment pane, which includes an editable text field, your enabled share options, and a permalink to the post.

By clicking `uicontrol Share` for a post:

* Users can connect to their social networks by clicking the Twitter or Facebook Icons.
* After authorizing the page to post to the user’s social networks, the Twitter or Facebook buttons will light up to let the user know that they are active.
* Users may personalize the content within the sharing post box.
* Clicking `uicontrol Share` will send content to the user’s active social networks, with a link that will take others to the exact post that the user wants to share.
* Users may also choose to share a link to a specific comment by pasting the Permalink within an email, blog post, or social network.
>[!NOTE]
>
>During your integration, you can determine which social networks are available for sharing by your users. You may also integrate a custom Permalink to allow for uniformity with your current media links.

Clicking `uicontrol Share` on another user’s post opens the `uicontrol Share Comment` pane, which includes an editable text field, your enabled share options, and a permalink to the post.

By clicking `uicontrol Share` for a post:

* Users can connect to their social networks by clicking the Twitter or Facebook Icons.
* After authorizing the page to post to the user’s social networks, the Twitter or Facebook buttons will light up to let the user know that they are active.
* Users may personalize the content within the sharing post box.
* Clicking `uicontrol Share` will send content to the user’s active social networks, with a link that will take others to the exact post that the user wants to share.
* Users may also choose to share a link to a specific comment by pasting the Permalink within an email, blog post, or social network.
>[!NOTE]
>
>During your integration, you can determine which social networks are available for sharing by your users. You may also integrate a custom Permalink to allow for uniformity with your current media links.
Apps that use this feature:

* [Carousel](c_carousel_app.md#c_carousel_app)
* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](c_feature_card_app.md#c_feature_card_app)
* [Map](c_map_app.md#c_map_app)
* [Media Wall](c_media_wall_app.md#c_media_wall_app)
* [Mosaic](c_mosaic_app.md#c_mosaic_app)
* [Polls](c_polls_app.md#c_polls_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Sidenotes](c_sidenotes_app.md#c_sidenotes_app)
* [Storify 2](c_storify2.md#c_storify2)
* [Trending](c_trending_app.md#c_trending_app)

>## Setting up Social Sharing {#c_setting_up_social_sharing}
>Credentials required to enable Livefyre Social Sharing.

<!-- c_social_sharing.dita -->
Livefyre uses this information to connect to the listed social networks on behalf of your social App, and to post shared content for your users on their behalf. Enter these values to enable social integration. They may be edited at any time.

Settings available from this page will update to reflect your social sharing system, as defined during your Livefyre integration process. Those integrating using their own custom user identity systems, must supply social network credentials for Facebook, LinkedIn, and Twitter, if they wish to allow their end users to share to these platforms. Janrain Engage customers need only supply their Janrain credentials, and not Facebook, Twitter, or LinkedIn.

>[!NOTE]
>
>Only one app per Social Media site may be enabled for your Network. You may include these apps on multiple sites, but your Network may have only one Facebook, one Twitter, one LinkedIn, and one Bitly integration.
## Janrain Engage {#section_dzq_1p1_21b}

To enable Janrain Engage integration, enter the following credentials:

* `uicontrol Engage API Key:`the API key for your Janrain Engage account.
* `uicontrol Engage Domain:`your Janrain provided domain name.
## Facebook {#section_tch_gp1_21b}

To share to Facebook, enter the following Facebook app credentials:

* `uicontrol Client ID:` the Client ID provided with your Facebook app.
* `uicontrol Client Secret:` the client secret provided with your Facebook app.
* `uicontrol OAuth Proxy Redirect:` your redirect page for receiving Facebook requests.
## Twitter {#section_xkd_kp1_21b}

To share to Twitter, enter the following Twitter App credentials:

* `uicontrol Access Token:` your Twitter-provided token for making API requests.
* `uicontrol Access Token Secret:` your Twitter-provided secret for making API requests.
* `uicontrol API Key:` your Twitter-provided API key.
* `uicontrol API Secret:` your Twitter-provided API secret.
## LinkedIn {#section_tqh_mp1_21b}

To share to LinkedIn, enter the following credentials for your LinkedIn API requests:

* `uicontrol API Key:` your LinkedIn-provided API key.
* `uicontrol API Secret:` your LinkedIn-provided API secret.
## Bitly {#section_ur2_np1_21b}

To enable Bitly permalinks, enter the following information for your Bitly integration:

* `uicontrol Login:` your Bitly-provided end user username login.
* `uicontrol API Key:` your Bitly-provided API key.
<a id="section_blk_ccj_h1b"></a>

Apps that use this feature:

* [Carousel](c_carousel_app.md#c_carousel_app)
* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Feature Card](c_feature_card_app.md#c_feature_card_app)
* [Map](c_map_app.md#c_map_app)
* [Media Wall](c_media_wall_app.md#c_media_wall_app)
* [Mosaic](c_mosaic_app.md#c_mosaic_app)
* [Polls](c_polls_app.md#c_polls_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Sidenotes](c_sidenotes_app.md#c_sidenotes_app)
* [Storify 2](c_storify2.md#c_storify2)
* [Trending](c_trending_app.md#c_trending_app)
