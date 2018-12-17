---
description: Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.
seo-description: Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.
seo-title: Live Blog
solution: Experience Manager
title: Live Blog
uuid: 5ca373f1-2008-45ab-9ec2-1e295af4e368
index: y
internal: n
snippet: y
---

# Live Blog{#live-blog}

Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.

## Live Blog {#topic_574DEE2125A94B85BFB5C3D2C57C337E}

Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event.

## Integration {#c_live_blog_integration}

Live Blog allows you to feature real-time updates and images from your site’s own editors when covering a live event. 

To embed a Live Blog App, follow the procedure for Embedding an App. See [Embed an App](/help/implementation/c-livefyre-identity-comp/t-using-studio-to-connect-your-social-apps-to-your-livefyre-implementation.md). The following is an example of what an embedded Live Blog App looks like.

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

## NetworkConfig Object {#c_networkconfig_object}

The `NetworkConfig` object is a JSON object that customizes the authentication system for network users. 

The `NetworkConfig` object is a JSON object containing the following parameters: 

|  Parameter  | Type  | Description  |
|---|---|---|
|  *`authDelegate`* | Object *required*  | Used to customize the authentication system for custom network users.  |
|  *`network`* | String *required*  | A Livefyre-provided network name. For example: *yourname.fyre.co.* |
|  *`attachmentDelegate`* | Object (optional)  | Used to specify the types of media attachments visible in the App stream. For more information, see [Restricting Media](../c-app-customizations/c-restrict-media.md#c_restrict_media).  |
|  *`strings`* | Object (optional)  | Used to customize text strings of the HTML elements in any of the Livefyre Core Apps. For more information, see [String Customizations](/help/using/c-settings-other/c-translation-sets/c-localize-strings.md).  |

## ConvConfig Object {#c_convconfig_object}

The `convConfig` object is a JSON object used to specify the content that the Livefyre App renders on the page.

>[!NOTE]
>
>The `convConfig` object parameters listed here do not apply for the Reviews app. For integration information about the Reviews app using the `convConfig` object, see Reviews Integration.

The `ConvConfig` object contains the following required parameters: 

|Parameter|Type|Description|
|--- |--- |--- |
|articleId|String *required*|Uniquely identifies a Collection within your Site. Usually, this corresponds to a database primary key or Post ID within your CMS. For example: “post-42”. 255 character limit.  Note:  If you use the article URL as your articleId, make certain the string is MD5 or SHA-1 encoded.|
|collectionMeta|String *required*|JWT-encoded metadata about the Collection. See  CollectionMeta Object  for more information.|
|el|String *required*|The ID of a DOM element to which the content stream will render.|
|siteId|String *required*|The Livefyre-provided ID for the website or application to which the Collection belongs. For example: “303617”.|

>[!NOTE]
>
>The `app` parameter is not required for a Comments App implementation.

The `ConvConfig` object may also contain the following optional parameters: 

|Parameter|Type|Description|
|--- |--- |--- |
|actionButtons|Array (optional)|An array of custom action buttons to add to a piece of content next to the  Share  and  Flag  buttons. For more information, see Adding Custom Buttons.|
|animations|Boolean (optional)|Defines whether animations will run within the Livefyre App. Set to false to disable animations. Defaults to true.|
|anonymousFlaggingEnabled|Boolean (optional)|Defines whether guest users have the option to flag content. Default is true.|
|browserType|String (optional)|Defines the device for which display content should be generated. This will cause the CSS, and some functionality, to change to fit the input device type. Options are desktop, mobile, or tablet. (If left blank, will default to the Google Agent determination for the display format.)|
|checksum|String (recommended)|Identifies the current state of the CollectionMeta. Changing this value will cause Livefyre to update the data on the server with the new values in CollectionMeta.|
|datetimeFormat|(Optional)  String  Object  Function|Specifies the datetime format of streamed content. For more information, see Customizing Date and Time Stamps.|
|disableAvatars|Boolean (optional)|Prevents avatars from being rendered in the App stream, and thus reduces the number of items loaded into the browser. Default is false.|
|disableIE8Shim|Boolean (optional)|Disables the default shiv used by Livefyre to polyfill Internet Explorer 8 so that HTML5 elements are supported. Livefyre uses the following project:  [https://github.com/aFarkas/html5shiv](https://github.com/aFarkas/html5shiv) . Default is false.  Note:  If this value is false, polyfill of some sort must be used before Livefyre Chat is invoked for Internet Explorer 8 support.|
|disableThirdPartyAnalytics|Boolean (optional)|Disables third party analytics systems (Quantserve and Google Analytics) that Livefyre may use for internal measurements. Default is false.|
|editorCss|Object (optional)|Used to customize the comment editor styling. You may style the editor field background color as well as the font color, size, and family of the text that appears inside the editor.  For example: {background: ‘#ccc’, color: ‘red’, font: ’30px “Helvetica Neue”, Helvetica, Arial, Geneva, sans-serif’}|
|initialNumVisible|Integer (optional)|Allows you to set the default number of comments visible in your App upon load. This may be an integer from 1 to 50.|
|initialNumVisibleLegacy|integer (optional)|Allows you to set the default number of legacy content items visible in your App upon load. This may be an integer from 1 to 50. If this parameter is not specified, defaults to initialNumVisible.  For example: If your Collection includes 100 active and 100 legacy comments, set initalNumVisible:10, and initialNumVisibleLegacy:5, to display 10 active comments (with a  Show More  button) + 5 archive comments (with a  Show More  button).|
|maxVisible|Integer (optional)|Sets the maximum number of visible pieces of top-level content in the Chat App. If new pieces of content stream in, content at the bottom of the stream will be removed from the page. If the  Show more…  button is clicked, the parameter is ignored and the user is free to show as much content as desired. (Use this parameter to control the number of items that appear on the page in high velocity streams.)|
|postToButtons|Array (optional)|Used to configure which providers appear when embedding the Live Blog App. Available options are  tw  (Twitter),  fb  (Facebook), and  li  (LinkedIn). Defaults to [  tw ,  fb ].|
|readOnly|Boolean (optional)|Disables all interactivity for the Collection. When true, users will be unable to log into the stream, and unable to Post, Edit, Reply to, or Like content. When true, users will be able to Flag and Share content. Default is false.|
|stream|Object (optional)|Contains options to configure streaming of the App.|
|stream.catchup|Integer (optional)|Specifies the number of seconds previous to the present moment that the stream should load. By default, Livefyre loads 50 pieces of content, and then loads all content submitted between those and the present time. In very fast use cases, content may be posted too quickly to allow the App to ‘catch up’ to the present. Use this setting to define the number of seconds previous to now for which content will be posted (after the initial content load).|
|stream.delay|Integer (optional)|Specifies the number of seconds between streaming requests. Use this parameter to help control the flow of content and delay how often the DOM is updated.  Note:  If set too large, the stream may fall behind.|


>[!NOTE]
>
>You can pass one or more `convConfig` objects during App initialization to display multiple Apps on the same page. Be aware that extra Apps use browser resources and performance may degrade as the number increases.

## CollectionMeta Object {#c_collectionmeta_object}

The `CollectionMeta` object is a JSON object that specifies metadata to store within the Collection. 

`CollectionMeta` is always encoded before being passed to Livefyre for security. The encoded value is passed into the `ConvConfig` object shown above.

>[!NOTE]
>
>You must add server-side code to encode the `CollectionMeta` JSON object. See Building Server-side Tokens for more information.

|Parameter|Type|Description|
|--- |--- |--- |
|articleId|String *required*|A unique ID for the Collection.|
|title|String *required*|The title you wish to apply to the Collection. This often corresponds to the title of the page that displays the App.  For example: “Integration is So Much Fun!”  Note:  The max character length for the title is 255 characters. The title field does not support HTML entities. Please encode special characters using UTF-8.|
|url|String *required*|The canonical absolute URL you wish to attach to this Collection. This URL will be used to generate links back to the App from content shared on Facebook and Twitter, email notifications, and Livefyre Studio.  Note:  Livefyre requires the use of a fully qualified domain name; the port number or a callback to resolve the local setup is not required. If testing locally, be certain to use a valid base URL domain. (For example: `http://customer.com` is valid, while `http://localhost:5995` is not.) Once you have set up your local webserver to accept a fully qualified domain name, no callbacks or resolutions are needed, and local development can proceed as expected.|
|type|String *required*|The Collection type. Must be  livechat .|

The `CollectionMeta` object may also contain the following optional parameter: 

|  Parameter  | Type  | Description  |
|---|---|---|
|  *`tags`* | (optional) string  | A comma-separated list of single keywords or phrases. Search Collections by tags within Studio or with the search API. **Note:** While tags added through Studio may contain spaces, tags entered through the API cannot. Use underscores to define tags that will display spaces in the UI. (For example: use Monday_Quarterback to display Monday Quarterback in Studio.)  |

## Adding an Event Handler {#concept_D835C710A7214F6D921571E0770B6BC5}

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

