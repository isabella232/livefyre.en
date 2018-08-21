---
description: Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.
seo-description: Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.
seo-title: Live Blog
solution: Experience Manager
title: Live Blog
uuid: 84d4f078-e3eb-42a1-97db-cff953f6a321
index: y
internal: n
snippet: y
translate: y
---

# Live Blog

## Live Blog {#topic_574DEE2125A94B85BFB5C3D2C57C337E}
>Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.
>## Integration {#c_live_blog_integration}
>Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.To embed a Live Blog App, follow the procedure for Integrating a Conversation App. See [](c_implement_a_conversation_app.md#concept_zvy_c3c_tbb). The following is an example of what an embedded Live Blog App looks like. 

**Example:** 

```
<html> 
  <head> 
    <script src="//cdn.livefyre.com/Livefyre.js"> 
    </script> 
  </head> 
<body> 
    <script type="text/javascript"> 
    var networkConfig = { 
      network: "client-solutions.fyre.co" 
    }; 
    var convConfig = { 
      siteId: '347674', 
      articleId: '1', 
      el: 'livefyre', 
      collectionMeta: 'eyJ0eXAiOiJqd3QiLCJhbGciOiJIUzI1NiJ9.eyJ0aXRsZSI6IlRpdGxlIDEiLCJ1cmwiOiJodHRwOlwvXC9kZXYubGl2ZWZ5cmUuY29tIiwidGFncyI6InRhZzEsdGFnMiIsImNoZWNrc3VtIjoiY2Q0YTJjYWJkMTIxOTkyM2FjZGJhMjExOWY2NmYwNTUiLCJhcnRpY2xlSWQiOiIxIn0.Dq-ghi9KYmEPmagvCS1NPyYDRMGBujm735QaTRb7E7k', 
      checksum: '6e2e4faf7b95f896260fe695eafb34ba' 
    }; 
    
    Livefyre.require(['fyre.conv#3'], function(Conv) { 
        new Conv(networkConfig, [convConfig], function(blogWidget) {}); 
        auth.delegate({ 
          login: function (callback) { 
            callback(null,{livefyre:'<userauthtoken>'}); 
          }, 
        }); 
    }); 
  
    </script> 
    <div id="livefyre"> 
    </div> 
   </body> 
</html>
```
CollectionMeta is an encoded JSON object. In the above example, the JSON object takes the following format before it’s JWT encoded: 

```
{ 
"url": "http://dev.livefyre.com/articles/test.html",  
"articleId": "1",  
"type": "liveblog",  
"title": "Title 1" 
}
```
>## NetworkConfig Object {#c_networkconfig_object}
>The 
<codeph>
  NetworkConfig 
</codeph> object is a JSON object that customizes the authentication system for network users.The ` NetworkConfig` object is a JSON object containing the following parameters: 

|  Parameter  | Type  | Description  |
|---|---|---|
|  *` authDelegate`* | Object (required)  | Used to customize the authentication system for custom network users.  |
|  *` network`* | String (required)  | A Livefyre-provided network name. For example: *yourname.fyre.co.* |
|  *` attachmentDelegate`* | Object (optional)  | Used to specify the types of media attachments visible in the App stream. For more information, see [ Restricting Media ](c_restrict_media.md#c_restrict_media).  |
|  *` strings`* | Object (optional)  | Used to customize text strings of the HTML elements in any of the Livefyre Core Apps. For more information, see [ String Customizations ](c_translation_sets/c_localize_strings.md#c_localize_strings).  |

>## ConvConfig Object {#c_convconfig_object}
>The 
<codeph>
  convConfig 
</codeph> object is a JSON object used to specify the content that the Livefyre App renders on the page.
>[!NOTE]
>
>The ` convConfig` object parameters listed here do not apply for the Reviews app. For integration information about the Reviews app using the ` convConfig` object, see Reviews Integration. 

The ` ConvConfig` object contains the following required parameters: 

<table frame="all" rowsep="1" colsep="1" id="table_adq_qy5_nz"> 
 <thead> 
  <tr> 
   <th class="entry"> Parameter </th> 
   <th class="entry"> Type </th> 
   <th class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> <span class="varname"> articleId </span> </td> 
   <td> String (required) </td> 
   <td> <p>Uniquely identifies a Collection within your Site. Usually, this corresponds to a database primary key or Post ID within your CMS. For example: “post-42”. 255 character limit. </p> <p>Note:  If you use the article URL as your articleId, make certain the string is MD5 or SHA-1 encoded. </p> </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> collectionMeta </span> </td> 
   <td> String (required) </td> 
   <td> JWT-encoded metadata about the Collection. See <a href="c_collectionmeta_object.md#c_collectionmeta_object" format="dita" scope="local"> CollectionMeta Object </a> for more information. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> el </span> </td> 
   <td> String (required) </td> 
   <td> The ID of a DOM element to which the content stream will render. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> siteId </span> </td> 
   <td> String (required) </td> 
   <td> The Livefyre-provided ID for the website or application to which the Collection belongs. For example: “303617”. </td> 
  </tr> 
 </tbody> 
</table>


>[!NOTE]
>
>The ` app` parameter is not required for a Comments App implementation. 

The ` ConvConfig` object may also contain the following optional parameters: 

<table frame="all" rowsep="1" colsep="1" id="table_wlc_bz5_nz"> 
 <thead> 
  <tr> 
   <th class="entry"> Parameter </th> 
   <th class="entry"> Type </th> 
   <th class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> <span class="varname"> actionButtons </span> </td> 
   <td> Array (optional) </td> 
   <td> An array of custom action buttons to add to a piece of content next to the <span class="uicontrol"> Share </span> and <span class="uicontrol"> Flag </span> buttons. For more information, see Adding Custom Buttons. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> animations </span> </td> 
   <td> Boolean (optional) </td> 
   <td> Defines whether animations will run within the Livefyre App. Set to false to disable animations. Defaults to true. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> anonymousFlaggingEnabled </span> </td> 
   <td> Boolean (optional) </td> 
   <td> Defines whether guest users have the option to flag content. Default is true. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> browserType </span> </td> 
   <td> String (optional) </td> 
   <td> Defines the device for which display content should be generated. This will cause the CSS, and some functionality, to change to fit the input device type. Options are desktop, mobile, or tablet. (If left blank, will default to the Google Agent determination for the display format.) </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> checksum </span> </td> 
   <td> String (recommended) </td> 
   <td> Identifies the current state of the CollectionMeta. Changing this value will cause Livefyre to update the data on the server with the new values in CollectionMeta. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> datetimeFormat </span> </td> 
   <td> <p>(Optional) </p> <p>String </p> <p>Object </p> <p>Function </p> </td> 
   <td> Specifies the datetime format of streamed content. For more information, see Customizing Date and Time Stamps. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> disableAvatars </span> </td> 
   <td> Boolean (optional) </td> 
   <td> Prevents avatars from being rendered in the App stream, and thus reduces the number of items loaded into the browser. Default is false. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> disableIE8Shim </span> </td> 
   <td> Boolean (optional) </td> 
   <td> <p>Disables the default shiv used by Livefyre to polyfill Internet Explorer 8 so that HTML5 elements are supported. Livefyre uses the following project: <a href="https://github.com/aFarkas/html5shiv" format="html" scope="external"> https://github.com/aFarkas/html5shiv </a>. Default is false. </p> <p>Note:  If this value is false, polyfill of some sort must be used before Livefyre Chat is invoked for Internet Explorer 8 support. </p> </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> disableThirdPartyAnalytics </span> </td> 
   <td> Boolean (optional) </td> 
   <td> Disables third party analytics systems (Quantserve and Google Analytics) that Livefyre may use for internal measurements. Default is false. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> editorCss </span> </td> 
   <td> Object (optional) </td> 
   <td> <p>Used to customize the comment editor styling. You may style the editor field background color as well as the font color, size, and family of the text that appears inside the editor. </p> <p>For example: {background: ‘#ccc’, color: ‘red’, font: ’30px “Helvetica Neue”, Helvetica, Arial, Geneva, sans-serif’} </p> </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> initialNumVisible </span> </td> 
   <td> Integer (optional) </td> 
   <td> Allows you to set the default number of comments visible in your App upon load. This may be an integer from 1 to 50. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> initialNumVisibleLegacy </span> </td> 
   <td> integer (optional) </td> 
   <td> <p>Allows you to set the default number of legacy content items visible in your App upon load. This may be an integer from 1 to 50. If this parameter is not specified, defaults to initialNumVisible. </p> <p>For example: If your Collection includes 100 active and 100 legacy comments, set initalNumVisible:10, and initialNumVisibleLegacy:5, to display 10 active comments (with a <span class="uicontrol"> Show More </span> button) + 5 archive comments (with a <span class="uicontrol"> Show More </span> button). </p> </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> maxVisible </span> </td> 
   <td> Integer (optional) </td> 
   <td> Sets the maximum number of visible pieces of top-level content in the Chat App. If new pieces of content stream in, content at the bottom of the stream will be removed from the page. If the <span class="uicontrol"> Show more… </span> button is clicked, the parameter is ignored and the user is free to show as much content as desired. (Use this parameter to control the number of items that appear on the page in high velocity streams.) </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> postToButtons </span> </td> 
   <td> Array (optional) </td> 
   <td> Used to configure which providers appear when embedding the Live Blog App. Available options are <span class="codeph"> tw </span> (Twitter), <span class="codeph"> fb </span> (Facebook), and <span class="codeph"> li </span> (LinkedIn). Defaults to [ <span class="codeph"> tw </span>, <span class="codeph"> fb </span>]. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> readOnly </span> </td> 
   <td> Boolean (optional) </td> 
   <td> Disables all interactivity for the Collection. When true, users will be unable to log into the stream, and unable to Post, Edit, Reply to, or Like content. When true, users will be able to Flag and Share content. Default is false. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> stream </span> </td> 
   <td> Object (optional) </td> 
   <td> Contains options to configure streaming of the App. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> stream.catchup </span> </td> 
   <td> Integer (optional) </td> 
   <td> Specifies the number of seconds previous to the present moment that the stream should load. By default, Livefyre loads 50 pieces of content, and then loads all content submitted between those and the present time. In very fast use cases, content may be posted too quickly to allow the App to ‘catch up’ to the present. Use this setting to define the number of seconds previous to now for which content will be posted (after the initial content load). </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> stream.delay </span> </td> 
   <td> Integer (optional) </td> 
   <td> <p>Specifies the number of seconds between streaming requests. Use this parameter to help control the flow of content and delay how often the DOM is updated. </p> <p>Note:  If set too large, the stream may fall behind. </p> </td> 
  </tr> 
 </tbody> 
</table>


>[!NOTE]
>
>You can pass one or more ` convConfig` objects during App initialization to display multiple Apps on the same page. Be aware that extra Apps use browser resources and performance may degrade as the number increases. 

>## CollectionMeta Object {#c_collectionmeta_object}
>The 
<codeph>
  CollectionMeta 
</codeph> object is a JSON object that specifies metadata to store within the Collection.` CollectionMeta` is always encoded before being passed to Livefyre for security. The encoded value is passed into the ` ConvConfig` object shown above. 

>[!NOTE]
>
>You must add server-side code to encode the ` CollectionMeta` JSON object. See Building Server-side Tokens for more information. 


<table frame="all" rowsep="1" colsep="1" id="table_ibg_xc5_nz"> 
 <thead> 
  <tr> 
   <th class="entry"> Parameter </th> 
   <th class="entry"> Type </th> 
   <th class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> <span class="varname"> articleId </span> </td> 
   <td> String (required) </td> 
   <td> A unique ID for the Collection. </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> title </span> </td> 
   <td> String (required) </td> 
   <td> <p>The title you wish to apply to the Collection. This often corresponds to the title of the page that displays the App. </p> <p>For example: “Integration is So Much Fun!” </p> <p>Note:  The max character length for the title is 255 characters. The title field does not support HTML entities. Please encode special characters using UTF-8. </p> </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> url </span> </td> 
   <td> String (required) </td> 
   <td> <p>The canonical absolute URL you wish to attach to this Collection. This URL will be used to generate links back to the App from content shared on Facebook and Twitter, email notifications, and Livefyre Studio. </p> <p>Note:  Livefyre requires the use of a fully qualified domain name; the port number or a callback to resolve the local setup is not required. If testing locally, be certain to use a valid base URL domain. (For example: http://customer.com is valid, while http://localhost:5995 is not.) Once you have set up your local webserver to accept a fully qualified domain name, no callbacks or resolutions are needed, and local development can proceed as expected. </p> </td> 
  </tr> 
  <tr> 
   <td> <span class="varname"> type </span> </td> 
   <td> String (required) </td> 
   <td> The Collection type. Must be <span class="codeph"> livechat </span>. </td> 
  </tr> 
 </tbody> 
</table>

The ` CollectionMeta` object may also contain the following optional parameter: 

|  Parameter  | Type  | Description  |
|---|---|---|
|  *` tags`* | (optional) string  | A comma-separated list of single keywords or phrases. Search Collections by tags within Studio or with the search API. **Note: **While tags added through Studio may contain spaces, tags entered through the API cannot. Use underscores to define tags that will display spaces in the UI. (For example: use Monday_Quarterback to display Monday Quarterback in Studio.)  |

>## Adding an Event Handler {#concept_D835C710A7214F6D921571E0770B6BC5}
To register event handlers, use the widget.on call within the App’s callback function. 

For example: 

```
Livefyre.require(['fyre.conv#3'], function(Conv) { 
   new Conv(networkConfig, [convConfig], function(widget) { 
      widget.on('<strong><eventName></strong>', function (data) { 
         // Do something, perhaps using data 
      }); 
   }); 
});
```
