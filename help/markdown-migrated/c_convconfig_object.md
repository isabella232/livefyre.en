---
description: The convConfig object is a JSON object used to specify the content that the Livefyre App renders on the page.
seo-description: The convConfig object is a JSON object used to specify the content that the Livefyre App renders on the page.
seo-title: ConvConfig Object
solution: Experience Manager
title: ConvConfig Object
---

# ConvConfig Object

>[!NOTE]
>
>The`codeph convConfig` object parameters listed here do not apply for the Reviews app. For integration information about the Reviews app using the `codeph convConfig` object, see Reviews Integration.
The `codeph ConvConfig` object contains the following required parameters:

<table frame="all" rowsep="1" colsep="1" id="table_adq_qy5_nz"> 
 <tgroup cols="3"> 
  <colspec colname="c1" colnum="1" colwidth="1.0*" /> 
  <colspec colname="c2" colnum="2" colwidth="1.0*" /> 
  <colspec colname="c3" colnum="3" colwidth="1.0*" /> 
  <thead> 
   <tr> 
    <th class="entry">Parameter</th> 
    <th class="entry">Type</th> 
    <th class="entry">Description</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td><span class="varname">articleId</span></td> 
    <td>String (required)</td> 
    <td> <p>Uniquely identifies a Collection within your Site. Usually, this corresponds to a database primary key or Post ID within your CMS. For example: “post-42”. 255 character limit.</p> <p>Note: If you use the article URL as your articleId, make certain the string is MD5 or SHA-1 encoded.</p> </td> 
   </tr> 
   <tr> 
    <td><span class="codeph">authPageReload</span></td> 
    <td>(optional) Boolean</td> 
    <td>Applies to Comments App: Allows you to control whether a user’s comment is stored locally during the auth process. If true, if a user enters a comment, and then logs into the App, the comment will be stored locally, and will be re-entered in the content field after login and page refresh. If false, entered content will be wiped during the login process, and must be retyped.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">collectionMeta</span></td> 
    <td>String (required)</td> 
    <td>JWT-encoded metadata about the Collection. See CollectionMeta Object for more information.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">el</span></td> 
    <td>String (required)</td> 
    <td>The ID of a DOM element to which the content stream will render.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">siteId</span></td> 
    <td>String (required)</td> 
    <td>The Livefyre-provided ID for the website or application to which the Collection belongs. For example: “303617”.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

>[!NOTE]
>
>The`codeph app` parameter is not required for a Comments App implementation.
The `codeph ConvConfig` object may also contain the following optional parameters:

<table frame="all" rowsep="1" colsep="1" id="table_wlc_bz5_nz"> 
 <tgroup cols="3"> 
  <colspec colname="c1" colnum="1" colwidth="1.0*" /> 
  <colspec colname="c2" colnum="2" colwidth="1.0*" /> 
  <colspec colname="c3" colnum="3" colwidth="1.0*" /> 
  <thead> 
   <tr> 
    <th class="entry">Parameter</th> 
    <th class="entry">Type</th> 
    <th class="entry">Description</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td><span class="varname">actionButtons</span></td> 
    <td>Array (optional)</td> 
    <td>An array of custom action buttons to add to a piece of content next to the <span class="uicontrol">Share</span> and <span class="uicontrol">Flag</span> buttons. For more information, see Adding Custom Buttons.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">animations</span></td> 
    <td>Boolean (optional)</td> 
    <td>Defines whether animations will run within the Livefyre App. Set to false to disable animations. Defaults to true.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">anonymousFlaggingEnabled</span></td> 
    <td>Boolean (optional)</td> 
    <td>Defines whether guest users have the option to flag content. Default is true.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">browserType</span></td> 
    <td>String (optional)</td> 
    <td>Defines the device for which display content should be generated. This will cause the CSS, and some functionality, to change to fit the input device type. Options are desktop, mobile, or tablet. (If left blank, will default to the Google Agent determination for the display format.)</td> 
   </tr> 
   <tr> 
    <td><span class="varname">checksum</span></td> 
    <td>String (recommended)</td> 
    <td>Identifies the current state of the CollectionMeta. Changing this value will cause Livefyre to update the data on the server with the new values in CollectionMeta.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">datetimeFormat</span></td> 
    <td> <p>(Optional)</p> <p>String</p> <p>Object</p> <p>Function</p> </td> 
    <td>Specifies the datetime format of streamed content. For more information, see Customizing Date and Time Stamps.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">disableAvatars</span></td> 
    <td>Boolean (optional)</td> 
    <td>Prevents avatars from being rendered in the App stream, and thus reduces the number of items loaded into the browser. Default is false.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">disableIE8Shim</span></td> 
    <td>Boolean (optional)</td> 
    <td> <p>Disables the default shiv used by Livefyre to polyfill Internet Explorer 8 so that HTML5 elements are supported. Livefyre uses the following project: <a href="https://github.com/aFarkas/html5shiv" format="html" scope="external">https://github.com/aFarkas/html5shiv</a>. Default is false.</p> <p>Note: If this value is false, polyfill of some sort must be used before Livefyre Chat is invoked for Internet Explorer 8 support.</p> </td> 
   </tr> 
   <tr> 
    <td><span class="varname">disableThirdPartyAnalytics</span></td> 
    <td>Boolean (optional)</td> 
    <td>Disables third party analytics systems (Quantserve and Google Analytics) that Livefyre may use for internal measurements. Default is false.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">editorCss</span></td> 
    <td>Object (optional)</td> 
    <td> <p>Used to customize the comment editor styling. You may style the editor field background color as well as the font color, size, and family of the text that appears inside the editor.</p> <p>For example: {background: ‘#ccc’, color: ‘red’, font: ’30px “Helvetica Neue”, Helvetica, Arial, Geneva, sans-serif’}</p> </td> 
   </tr> 
   <tr> 
    <td><span class="varname">initialNumVisible</span></td> 
    <td>Integer (optional)</td> 
    <td>Allows you to set the default number of comments visible in your App upon load. This may be an integer from 1 to 50.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">initialNumVisibleLegacy</span></td> 
    <td>integer (optional)</td> 
    <td> <p>Allows you to set the default number of legacy content items visible in your App upon load. This may be an integer from 1 to 50. If this parameter is not specified, defaults to initialNumVisible.</p> <p>For example: If your Collection includes 100 active and 100 legacy comments, set initalNumVisible:10, and initialNumVisibleLegacy:5, to display 10 active comments (with a <span class="uicontrol">Show More</span> button) + 5 archive comments (with a <span class="uicontrol">Show More</span> button).</p> </td> 
   </tr> 
   <tr> 
    <td><span class="varname">maxVisible</span></td> 
    <td>Integer (optional)</td> 
    <td>Sets the maximum number of visible pieces of top-level content in the Chat App. If new pieces of content stream in, content at the bottom of the stream will be removed from the page. If the <span class="uicontrol">Show more…</span> button is clicked, the parameter is ignored and the user is free to show as much content as desired. (Use this parameter to control the number of items that appear on the page in high velocity streams.)</td> 
   </tr> 
   <tr> 
    <td><span class="varname">postToButtons</span></td> 
    <td>Array (optional)</td> 
    <td>Used to configure which providers appear when embedding the Live Blog App. Available options are <span class="codeph">tw</span> (Twitter), <span class="codeph">fb</span> (Facebook), and <span class="codeph">li</span> (LinkedIn). Defaults to [<span class="codeph">tw</span>, <span class="codeph">fb</span>].</td> 
   </tr> 
   <tr> 
    <td><span class="varname">readOnly</span></td> 
    <td>Boolean (optional)</td> 
    <td>Disables all interactivity for the Collection. When true, users will be unable to log into the stream, and unable to Post, Edit, Reply to, or Like content. When true, users will be able to Flag and Share content. Default is false.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">stream</span></td> 
    <td>Object (optional)</td> 
    <td>Contains options to configure streaming of the App.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">stream.catchup</span></td> 
    <td>Integer (optional)</td> 
    <td>Specifies the number of seconds previous to the present moment that the stream should load. By default, Livefyre loads 50 pieces of content, and then loads all content submitted between those and the present time. In very fast use cases, content may be posted too quickly to allow the App to ‘catch up’ to the present. Use this setting to define the number of seconds previous to now for which content will be posted (after the initial content load).</td> 
   </tr> 
   <tr> 
    <td><span class="varname">stream.delay</span></td> 
    <td>Integer (optional)</td> 
    <td> <p>Specifies the number of seconds between streaming requests. Use this parameter to help control the flow of content and delay how often the DOM is updated.</p> <p>Note: If set too large, the stream may fall behind.</p> </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

>[!NOTE]
>
>You can pass one or more`codeph convConfig` objects during App initialization to display multiple Apps on the same page. Be aware that extra Apps use browser resources and performance may degrade as the number increases.
