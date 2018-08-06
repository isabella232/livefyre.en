---
description: Installing and configuring the WordPress Plugin.
seo-description: Installing and configuring the WordPress Plugin.
seo-title: Livefyre for WordPress
title: Livefyre for WordPress
uuid: c2c301f5-4cab-49d8-a907-c7d2663a6e45
index: y
internal: n
snippet: y
translate: y
---

# Livefyre for WordPress

The Livefyre WordPress Enterprise plugin allows you to add Livefyre Comments, Chat, Live Blog, or Sidenotes to your WordPress site.
This section describes the WordPress plugin installation process.

* Livefyre Credentials
* Installation
* Customizations
* Comments
* Chat
* Live Blog
* Sidenotes
**Livefyre Credentials**
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
**User Auth Types** 
Select the user auth system to be used on your Livefyre App enabled WordPress sites:

* ** ` Native WordPress:` **The Livefyre Apps plugin will use the WordPress authentication/database to store user information for logging into and out of the App.
* ** ` Custom/LFEP:` **Used when you have specified your own Authentication system using Livefyre’s require module. Authentication will be found automatically by the Livefyre App if the authentication code with require.js is produced in the header of the page.
* ** ` Legacy Delegate:` **Used with the Livefyre fyre.conv.RemoteAuthDelegate(); authentication delegate. Provide the name of the JavaScript authentication delegate you declared and Livefyre will link it to the new authentication code using Livefyre.require.

  >[!NOTE]
  >
  >This option is for clients who use the Livefyre.js library to construct auth.

**Environment**
Select the Environment checkbox to specify that the credentials entered be used for your Livefyre production environment. Leave the box deselected to specify staging.
**App Settings**
Once enabled, click on an App in the sidebar menu to settings options for the App. Available options vary by App, and may include the following.

* **Settings:**Allows you to control the types of pages for which the App will be enabled, and provides a link to a description of the configuration options available for the App. Configuration options are available for all Livefyre Apps, and are set using the ConvConfig object. Add the listed script to your theme’s header, and pass in options as a comma separated array.
* **Status:**Lists conflicting plugins and setting status for the App, if available.
* **Shortcode:**Some Livefyre Apps (Comments, Live Blog and Chat) can be applied with shortcodes to give users more flexibility with where they can produce Livefyre products. To use them, follow the structure on the settings page pertaining to that particular app.
**Customizations**
The Livefyre Apps Plugin for WordPress can be customized in two ways: through Collection customizations and string customizations.
**Collection Customizations**
Collections can be customized by passing in a script code to your theme’s header. For example, for Comments, the following script may be used:

```
<script> var liveCommentsConfig = { 'readOnly': true } </script> 

```
Each example is on the App’s specific settings page, reachable through WordPress’s sidebar menu.
**String Customizations**
String customizations are built using the [ WordPress filters functionality ](http://codex.wordpress.org/Function_Reference/add_filter). Each Livefyre App will bind to a particular filter name and expects a PHP associative array returned in order to build the customized strings. This filter should be registered on all posts/pages on which your specific Livefyre App will appear. The 4 filter names are:
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
Use the [ WordPress filters functionality ](http://codex.wordpress.org/Function_Reference/add_filter) to override Collection information (articleId, Collection title, or Collection URL).
To implement the customization, apply any of these filters:
For example, to implement an articleId filter:

```
add_filter('livefyre_article_id', 'my_articleId_filter'); 
 function my_articleId_filter() { 
     return 'NewArticleId-74929'; 
}
```
When implemented, Collection information customizations will change the information associated with the Collection. This feature may be used to map new URLs to a Collection, using different mappings in the database to identify Collections.
**Comments**
Enabling Comments will replace your default WordPress comments with Livefyre’s. Use the Comments page to select whether Comments will be enabled on Posts or Pages, to view any conflicting plugin information, and to review the shortcode format.

>[!NOTE]
>
>Only Chat or Comments may be enabled for each of these options. While you may select Chat for one, and Comments for the other, you cannot select both Apps for either posts or pages.

**Comments Settings**
Use the **post** and **page** checkboxes to select the types of posts for which Comments will be enabled. Once enabled, you may set different Comments configuration variables using the ConvConfig object with your theme.
**Comments Status** 

* **Conflicting Plugins:**Lists enabled plugins that have been known to cause issues with Comments.
* **Allow Comments/Chat Status:**Lists posts and pages that have **Allow Comments** disabled. Comments will not appear on these posts/pages.

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
**Chat**
Enabling Chat will replace your default WordPress comments with Chat. Use the Chat page to select whether Chat will be enabled on Posts or Pages, to view any conflicting plugin information, and to review the shortcode format. (Chat differs from Comments in that Chat does not allow content threading.)

>[!NOTE]
>
>Only Chat or Comments may be enabled for each of these options. While you may select Chat for one, and Comments for the other, you cannot select both Apps for either posts or pages.

**Chat Settings** 
Use the ** ` post` ** and ** ` page` ** checkboxes to select the types of posts for which Chat will be enabled. Once enabled, you may set different Chat configuration variables using the ConvConfig object with your theme.
**Chat Status**

* **Conflicting Plugins:**Lists enabled plugins that have been known to cause issues with Chat.
* **Allow Comments/Chat Status:**Lists posts and pages that have ‘Allow Comments’ turned off. Chat will not appear on these posts/pages.
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
**Live Blog**
Enabling Live Blog allows you to include Live Blogs on your site. Use the Live Blog page to review configuration and shortcode options.
**Note:**Unlike Chat or Comments, Live Blog may be enabled only by using a shortcode.
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
**Sidenotes**
Enabling Sidenotes allows your users to sidenote your content. Use the Sidenotes page to select whether Sidenotes will be enabled on posts or pages, to define which sorts of content may be sidenoted and to review configuration options.
**Sidenotes Settings**
Use the **post** and **page** checkboxes to select the types of posts for which Sidenotes will be enabled. Once enabled, you may set different Sidenotes configuration variables using the ConvConfig object with your theme.
Use the Selectors field to specify the type of content to be sidenoted. This field is prepopulated with a string which follows the Livefyre Sidenotes jQuery/CSS based selectors format. For more information, see App Integrations &gt; Sidenotes.
Once enabled, you may set different Chat configuration variables using the ConvConfig object with your theme.
**Visualization Apps**
The Visualization Apps plugin allows you to automatically add any Livefyre App to a WordPress page or post using shortcode.
To enable Visualization Apps, embed shortcode in your post or page.
