---
description: 
seo-description: 
seo-title: Troubleshooting: Visualization Apps in WordPress Shortcode
solution: Experience Manager
title: Troubleshooting: Visualization Apps in WordPress Shortcode
---

# Troubleshooting: Visualization Apps in WordPress Shortcode


>## Livefyre Plugin for WordPress {#c_livefyre_for_wordpress}
>Use Livefyre on your WordPress pages by using the Livefyre for WordPress plugin.

On this page:

* [](#c_livefyre_for_wordpress/section_vqk_bbb_2cb)
* [](#c_livefyre_for_wordpress/section_jz3_1bb_2cb)
* [](#c_livefyre_for_wordpress/section_ktp_z1b_2cb)
* [](#c_livefyre_for_wordpress/section_z4w_y1b_2cb)
* [](#c_livefyre_for_wordpress/section_fc3_y1b_2cb)
* [](#c_livefyre_for_wordpress/section_usy_q1b_2cb)
* [](#c_livefyre_for_wordpress/section_rlm_l1b_2cb)
* [](#c_livefyre_for_wordpress/section_ogv_xz1_2cb)
* [](#c_livefyre_for_wordpress/section_u4d_vz1_2cb)
* [](#c_livefyre_for_wordpress/section_wlg_tz1_2cb)
* [](#t_embed_a_livefyre_app_inside_a_wordpress_page_or_post)
    * [](#t_install_livefyre_for_wordpress)
    * [](#c_troubleshooting_visualization_apps_in_wordpress_shortcode)
  
<!-- c_livefyre_for_wordpress.dita -->
The Livefyre WordPress Enterprise plugin allows you to add Livefyre Comments, Chat, Live Blog, or Sidenotes to your WordPress site.

This section describes the WordPress plugin installation process.

## Livefyre Credentials {#section_vqk_bbb_2cb}

To add Livefyre Apps to your WordPress sites, install the plugin, activate it, and add your Livefyre-provided credentials.

Required credentials include:

* Site ID
* Site Key
* Network Name
* Network Key
* User Auth Type (links to section Authentication Types)
* AuthDelegate Name
>[!NOTE]
>
>Multisite networks must install the plugin for each site. Multisite networks are configured on a per site basis. Each site will require its own Livefyre Apps settings entered on the site specific dashboard.
Enabled Apps will appear under Livefyre Apps in the side navigation panel. Click on the App type for more specific configuration information for each.

## User Auth Types {#section_jz3_1bb_2cb}

Select the user auth system to be used on your Livefyre App enabled WordPress sites:

* `uicontrol  Native WordPress:`The Livefyre Apps plugin will use the WordPress authentication/database to store user information for logging into and out of the App.
* `uicontrol  Custom/LFEP:`Used when you have specified your own Authentication system using Livefyre’s require module. Authentication will be found automatically by the Livefyre App if the authentication code with require.js is produced in the header of the page.
  *
  `uicontrol  Legacy Delegate:`Used with the Livefyre fyre.conv.RemoteAuthDelegate(); authentication delegate. Provide the name of the JavaScript authentication delegate you declared and Livefyre will link it to the new authentication code using Livefyre.require.
  
  >[!NOTE]
  >
  >This option is for clients who use the Livefyre.js library to construct auth.
  
## Environment {#section_ktp_z1b_2cb}

Select the Environment checkbox to specify that the credentials entered be used for your Livefyre production environment. Leave the box deselected to specify staging.

## App Settings {#section_z4w_y1b_2cb}

Once enabled, click on an App in the sidebar menu to settings options for the App. Available options vary by App, and may include the following.

* **Settings: **Allows you to control the types of pages for which the App will be enabled, and provides a link to a description of the configuration options available for the App. Configuration options are available for all Livefyre Apps, and are set using the ConvConfig object. Add the listed script to your theme’s header, and pass in options as a comma separated array.
* **Status: **Lists conflicting plugins and setting status for the App, if available.
* **Shortcode: **Some Livefyre Apps (Comments, Live Blog and Chat) can be applied with shortcodes to give users more flexibility with where they can produce Livefyre products. To use them, follow the structure on the settings page pertaining to that particular app.
## Customizations {#section_fc3_y1b_2cb}

The Livefyre Apps Plugin for WordPress can be customized in two ways: through Collection customizations and string customizations.

**Collection Customizations**

Collections can be customized by passing in a script code to your theme’s header. For example, for Comments, the following script may be used:

```
&lt;script&gt; var liveCommentsConfig = { 'readOnly': true } &lt;/script&gt; 

```
Each example is on the App’s specific settings page, reachable through WordPress’s sidebar menu.

**String Customizations**

String customizations are built using the [ WordPress filters functionality ](https://codex.wordpress.org/Function_Reference/add_filter). Each Livefyre App will bind to a particular filter name and expects a PHP associative array returned in order to build the customized strings. This filter should be registered on all posts/pages on which your specific Livefyre App will appear. The 4 filter names are:

For example, to apply a filter for a Comments App:

```
add_filter('livefyre_custom_comments_strings', 
 'my_comments_strings_filter'); function my_comments_strings_filter() { 
 $strings['postAsButton'] = "New Post As"; 
 $strings['postEditBtton'] = "New Post Edit"; 
 ... 
 return $strings; 
} 

```
By replacing the filter with the corresponding names, the App will use those strings to replace normal widget defaults. A complete list of string customization keys can be found at the String Customizations page.

**Collection Information Customizations**

Use the [ WordPress filters functionality ](https://codex.wordpress.org/Function_Reference/add_filter) to override Collection information (articleId, Collection title, or Collection URL).

To implement the customization, apply any of these filters:

For example, to implement an articleId filter:

```
add_filter('livefyre_article_id', 'my_articleId_filter'); 
 function my_articleId_filter() { 
 return 'NewArticleId-74929'; 
}
```
When implemented, Collection information customizations will change the information associated with the Collection. This feature may be used to map new URLs to a Collection, using different mappings in the database to identify Collections.

## Comments {#section_usy_q1b_2cb}

Enabling Comments will replace your default WordPress comments with Livefyre’s. Use the Comments page to select whether Comments will be enabled on Posts or Pages, to view any conflicting plugin information, and to review the shortcode format.

>[!NOTE]
>
>Only Chat or Comments may be enabled for each of these options. While you may select Chat for one, and Comments for the other, you cannot select both Apps for either posts or pages.
**Comments Settings**

Use the **post** and **page** checkboxes to select the types of posts for which Comments will be enabled. Once enabled, you may set different Comments configuration variables using the ConvConfig object with your theme.

**Comments Status**

* **Conflicting Plugins: **Lists enabled plugins that have been known to cause issues with Comments.
* **Allow Comments/Chat Status: **Lists posts and pages that have **Allow Comments** disabled. Comments will not appear on these posts/pages.
**Comments Shortcode**

While Comments will automatically replace your default WordPress Comments, you may also add it directly within your content using a shortcode.

To generate a Comments stream inside post content, enter the following syntax within the content editor:

```
[livefyre_comments] 

```
Comments streams are separated by the Article ID, and, if not specified, Livefyre will use the current post ID. Define the Article ID manually using the following format:

```
[livefyre_comments article_id="123"] 

```
## Chat {#section_rlm_l1b_2cb}

Enabling Chat will replace your default WordPress comments with Chat. Use the Chat page to select whether Chat will be enabled on Posts or Pages, to view any conflicting plugin information, and to review the shortcode format. (Chat differs from Comments in that Chat does not allow content threading.)

>[!NOTE]
>
>Only Chat or Comments may be enabled for each of these options. While you may select Chat for one, and Comments for the other, you cannot select both Apps for either posts or pages.
**Chat Settings**

Use the `uicontrol  post` and `uicontrol  page` checkboxes to select the types of posts for which Chat will be enabled. Once enabled, you may set different Chat configuration variables using the ConvConfig object with your theme.

**Chat Status**

* **Conflicting Plugins: **Lists enabled plugins that have been known to cause issues with Chat.
* **Allow Comments/Chat Status: **Lists posts and pages that have ‘Allow Comments’ turned off. Chat will not appear on these posts/pages.
**Chat Shortcode**

While Chat will automatically replace your default WordPress Comments, you may also add it directly within your content using a shortcode.

To generate a Chat stream inside post content, enter the following syntax within the content editor:

```
[livefyre_chat] 

```
Chat streams are separated by the Article ID, and, if not specified, Livefyre will use the current post ID. Define the Article ID manually using the following format:

```
[livefyre_chat article_id="123"] 

```
## Live Blog {#section_ogv_xz1_2cb}

Enabling Live Blog allows you to include Live Blogs on your site. Use the Live Blog page to review configuration and shortcode options.

>[!NOTE]
>
>Unlike Chat or Comments, Live Blog may be enabled only by using a shortcode.
**Live Blog Settings**

Use the Live Blog ConvConfig object to set different Live Blog configuration variables.

**Live Blog Shortcode**

To enable Live Blog, you must embed a shortcode in your content. Once enabled, you may set different Live Blog configuration variables using the ConvConfig object with your theme.

To generate a Live Blog inside post content, enter the following syntax within the content editor:

```
[livefyre_liveblog] 

```
Live Blog streams are separated by the Article ID, and, if not specified, Livefyre will use the current post ID. Define the Article ID manually using the following format:

```
[livefyre_liveblog article_id="123"] 

```
## Sidenotes {#section_u4d_vz1_2cb}

Enabling Sidenotes allows your users to sidenote your content. Use the Sidenotes page to select whether Sidenotes will be enabled on posts or pages, to define which sorts of content may be sidenoted and to review configuration options.

**Sidenotes Settings**

Use the **post** and **page** checkboxes to select the types of posts for which Sidenotes will be enabled. Once enabled, you may set different Sidenotes configuration variables using the ConvConfig object with your theme.

Use the Selectors field to specify the type of content to be sidenoted. This field is prepopulated with a string which follows the Livefyre Sidenotes jQuery/CSS based selectors format. For more information, see App Integrations &gt; Sidenotes.

Once enabled, you may set different Chat configuration variables using the ConvConfig object with your theme.

## Visualization Apps {#section_wlg_tz1_2cb}

The Visualization Apps plugin allows you to automatically add any Livefyre App to a WordPress page or post using shortcode.

To enable Visualization Apps, embed shortcode in your post or page.


>## Embed a Livefyre App Inside a Wordpress Page or Post {#t_embed_a_livefyre_app_inside_a_wordpress_page_or_post}

<!-- t_embed_a_livefyre_app_inside_a_wordpress_page_or_post.dita -->
>1. Create an App in Livefyre.
>   
>1. In Livefyre, click on the App to embed in your WordPress page or post.
>   
>1. Find the App ID of the App.
>   
>1. In WordPress, enter the following shortcode, replacing appID with the App ID:
>   `codeph  [livefyre_designer app_id=”appID”]`
>   
>   

>## Install Livefyre for WordPress {#t_install_livefyre_for_wordpress}

<!-- t_install_livefyre_for_wordpress.dita -->
>1. Search for the `uicontrol  Livefyre Apps` plugin in WordPress.org.
>   
>1. Follow the WordPress instructions to install the plugin.
>   
>1. Deactivate all previous Livefyre plugins (Livefyre Comments, Livefyre Sidenotes).
>   
>1. Activate the `uicontrol  Livefyre Apps` plugin.
>   
>1. From the WordPress navigation panel, go to `uicontrol  Livefyre Apps &gt; General`.
>   
>1. From the top right pane, select `uicontrol  Environment Type &gt; Enterprise`.
>   
>1. Enter your Site information ( `uicontrol  Livefyre Access Details`).
>   
>1. Use the `uicontrol  Livefyre App Management` panel to enable the Apps you wish to include on your site.
>   
>   

>## Troubleshooting: Visualization Apps in WordPress Shortcode {#c_troubleshooting_visualization_apps_in_wordpress_shortcode}

<table id="table_xqd_grm_5z"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> <b>Problem</b> </th> 
    <th class="entry"> <b>Solution</b> </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <span class="uicontrol"> App not displaying </span> </td> 
    <td> Check that you have the correct App ID </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> If you use more than one network, check that you are using the correct network. </td> 
   </tr> 
   <tr> 
    <td></td> 
    <td> Check that you are using the correct credentials. </td> 
   </tr> 
   <tr> 
    <td> <span class="uicontrol"> Can’t find App ID </span> </td> 
    <td> The App ID is an alphanumeric string that Livefyre generates. You can find it within the Livefyre Application in the App you want to display in WordPress. For more help finding the App ID, contact Livefyre support at https://livefyre.zendesk.com/hc/en-us. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<!-- c_troubleshooting_visualization_apps_in_wordpress_shortcode.dita -->
