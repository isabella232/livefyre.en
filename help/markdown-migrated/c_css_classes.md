---
description: Use available CSS classes to customize your Apps’ display.
seo-description: Use available CSS classes to customize your Apps’ display.
seo-title: CSS Classes
solution: Experience Manager
title: CSS Classes
---

# CSS Classes

Available for Chat, Comments, Live Blog, Reviews, and Sidenotes.

Use CSS to customize your Livefyre Apps for a more complete integration with your page, by simply overriding the default App CSS with your own stylesheet. This section describes available CSS customizations.

* [ Editor CSS ](#c_css_classes/section_edx_prh_xz)
* [ Sorting Options CSS ](#c_css_classes/section_btq_4rh_xz)
* [ Comment CSS ](#c_css_classes/section_mlv_nrh_xz)
* [ Featured Comments CSS ](#c_css_classes/section_m2v_mrh_xz)
* [ Archived Comments CSS ](#c_css_classes/section_bs5_lrh_xz)
* [ Comment Notifier CSS ](#c_css_classes/section_dy4_krh_xz)
* [ Storify CSS Classes ](c_storify_css_classes.md#c_storify_css_classes)
## Editor CSS {#section_edx_prh_xz}

Use these classes to change the post editor interface.

<table id="table_a1m_bnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Class </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> .fyre-comment-count </td> 
    <td> The text displaying the number of comments. </td> 
   </tr> 
   <tr> 
    <td> .fyre-login-bar </td> 
    <td> The bounding box that contains the login bar and options. </td> 
   </tr> 
   <tr> 
    <td> .fyre-live-container </td> 
    <td> The bounding box around the number of people listening and their avatars. </td> 
   </tr> 
   <tr> 
    <td> .fyre-editor </td> 
    <td> The bounding box around the .fyre-login-bar, .fyre-live-container and the text area where users write their comments. </td> 
   </tr> 
   <tr> 
    <td> .fyre-stream-sort </td> 
    <td> The bounding box around the sorting options. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

You can also edit styles in the App configuration itself, including the editor field background color, and the font color, size, and family of the text that appears inside the editor.

To customize the comment editor, add the editorCss:{} object to fyre.conv.load() and include your desired styling. For example, to update the editor with your custom CSS:

```
fyre.conv.load(networkConfig, [{ 
 siteId: LF_siteId, 
 el: 'livefyre', 
 articleId: LF_articleId, 
 collectionMeta: #CollectionMeta 
 editorCss: { 
 background: '#ccc', 
 color: 'red', 
 font: '30px "Helvetica Neue", Helvetica, Arial, Geneva, sans-serif' 
 } 
}]);
```
## Sorting Options CSS {#section_btq_4rh_xz}

<table id="table_c1m_bnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Class </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> .fyre-stream-sort </td> 
    <td> The entire sorting options div. </td> 
   </tr> 
   <tr> 
    <td> .fyre-stream-sort-newest </td> 
    <td> The option “Newest”. </td> 
   </tr> 
   <tr> 
    <td> .fyre-stream-sort-oldest </td> 
    <td> The option “Oldest”. </td> 
   </tr> 
   <tr> 
    <td> .fyre-stream-sort-bar </td> 
    <td> The separator bar between the options. </td> 
   </tr> 
   <tr> 
    <td> .fyre-stream-sort-selected </td> 
    <td> The currently selected sorting option. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

HTML Structure:

```
&lt;div class="fyre-stream-sort"&gt; 
 &lt;a href="#" class="fyre-stream-sort-newest fyre-stream-sort-selected"&gt;Newest&lt;/a&gt; 
 &lt;span class="fyre-stream-sort-bar"&gt; | &lt;/span&gt; 
 &lt;a href="#" class="fyre-stream-sort-oldest"&gt;Oldest&lt;/a&gt; 
&lt;/div&gt;
```
Hide the ‘|’ separating the sorting options.

```
.fyre-stream-sort .fyre-stream-sort-bar { 
 display: none !important; 
}
```
## Comment CSS {#section_mlv_nrh_xz}

<table id="table_f1m_bnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Class </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> .fyre-comment-author-tag- <i>&lt;custom tag name&gt;</i> </td> 
    <td> Livefyre will create a CSS class in this format for each user tag added through Livefyre’s <a href="http://350.df9.mwp.accessdomain.com/product/studio/users/#CreatingUserGroups" format="html" scope="external"> Studio </a>, <a href="http://350.df9.mwp.accessdomain.com/developers/identity-integration/your-identity/#PingForPull" format="html" scope="external"> Profile Sync </a>, or <a href="http://350.df9.mwp.accessdomain.com/developers/imports/" format="html" scope="external"> data import </a>. This class may be used to style the background for any content posted by user accounts including that tag. </td> 
   </tr> 
   <tr> 
    <td> .fyre-tag-content-icon- <i>&lt;tag name&gt;</i> </td> 
    <td> Livefyre will create a CSS class in this format for each content tag added through Livefyre <a href="http://350.df9.mwp.accessdomain.com/product/studio/users/#CreatingUserGroups" format="html" scope="external"> Studio </a>. This class may be used to style any content to which you have added the tag. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment-user </td> 
    <td> The bounding box that contains the user profile picture. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment-username </td> 
    <td> The username. </td> 
   </tr> 
   <tr> 
    <td> .fyre-moderator </td> 
    <td> The moderator bounding box. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment </td> 
    <td> Bounding box around the comment text/link. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment-article </td> 
    <td> The bounding box for the entire comment content. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment-date </td> 
    <td> The tag attached to the “time since posted” element. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment-media </td> 
    <td> The bounding box around the media content. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment-actions </td> 
    <td> The bounding box around the available actions to take on a comment. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment-like </td> 
    <td> The bounding box around the “Like” link. </td> 
   </tr> 
   <tr> 
    <td> .fyre-comment-reply </td> 
    <td> The bounding box around the “Reply” link. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Featured Comments CSS {#section_m2v_mrh_xz}

>[!NOTE]
>
>All Comment CSS classes may also be applied to Featured Content.
<table id="table_g1m_bnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Class </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> .fyre-featured-content-wrapper </td> 
    <td> The container div for the reader. </td> 
   </tr> 
   <tr> 
    <td> .fyre-featured-header </td> 
    <td> The leading title bar. </td> 
   </tr> 
   <tr> 
    <td> .fyre-featured-header-icon </td> 
    <td> The header’s quill icon. </td> 
   </tr> 
   <tr> 
    <td> .fyre-featured-title </td> 
    <td> The header text. </td> 
   </tr> 
   <tr> 
    <td> .fyre-featured-body </td> 
    <td> The container div for featured content in the reader. </td> 
   </tr> 
   <tr> 
    <td> .fyre-featured-quote </td> 
    <td> The quote icon that begins each content item. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Archived Comments CSS {#section_bs5_lrh_xz}

>[!NOTE]
>
>All content CSS classes may also be applied to archived content.
<table id="table_i1m_bnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Class </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> .fyre-archive-stream-title </td> 
    <td> The “From the Archive” text. </td> 
   </tr> 
   <tr> 
    <td> .fyre-archive-stream-title-icon </td> 
    <td> The logo for the “From the Archive” header. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Comment Notifier CSS {#section_dy4_krh_xz}

These classes allow you to customize the Livefyre Comment Notifier.

<table id="table_k1m_bnl_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Class </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> .fyre-notification </td> 
    <td> The div for the list item (both new and archive content). </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier </td> 
    <td> The wrapper for the contents of the Notifier. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-archive </td> 
    <td> The wrapper for all new content other than the most recent post. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-avatar </td> 
    <td> The image for the avatar. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-avatar-container </td> 
    <td> The container div for the user avatar. Allows you to define positioning. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-avatar-shading </td> 
    <td> The shading for the avatar div. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-banner </td> 
    <td> The container for the Notifier’s preview content, which displays the user avatar and a content snippet for the most recently posted item. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-base </td> 
    <td> The container for the information part of the Notifier, which lists the number of new comments, the Notifier caption, and the close button. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-base-close </td> 
    <td> The container div for the close button (x) for the Notifier. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-base-shadow </td> 
    <td> The shading for the Notifier base. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-caption </td> 
    <td> The text displayed for the notifier. ‘New Comment(s)’ by default. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-close </td> 
    <td> A button which closes the notifier. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-container </td> 
    <td> The container for the Notifier, includes both the banner and the base. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-counter </td> 
    <td> The container for the number listed in the Notifier. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-list </td> 
    <td> The container for the most recent piece of content. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-message </td> 
    <td> The first ~30 characters of the content displayed. </td> 
   </tr> 
   <tr> 
    <td> .fyre-notifier-message-container </td> 
    <td> The container div for the header message. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

