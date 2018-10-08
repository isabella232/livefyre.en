---
description: Embedding the Comments App follows the process for embedding a Core App.
seo-description: Embedding the Comments App follows the process for embedding a Core App.
seo-title: Embed a Comments App
solution: Experience Manager
title: Embed a Comments App
uuid: 369b9222-36a8-46b3-a933-b50c73544b59
index: y
internal: n
snippet: y
translate: y
---

# Embed a Comments App

Embedding the Comments App follows the process for embedding a Core App.

Embedding the Comments App follows the process for embedding a Core App described in [](t_embed_an_app_on_your_site_using_livefyre.js.md#embed_an_app_on_your_site_using_livefyre.js)

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
      network: 'domainName' 
    }; 
    var convConfig = { 
      siteId: 'siteId', 
      articleId: 'articleId', 
      el: 'livefyre', 
      collectionMeta: 'collectionMeta', 
      checksum: 'checksum' 
    }; 
    
    Livefyre.require(['fyre.conv#3', 'auth'], function(Conv, auth) { 
        new Conv(networkConfig, [convConfig], function(commentsWidget) {}); 
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

As noted in the Building CollectionMeta section, CollectionMeta is an encoded JSON object. In the above example, the JSON object takes the following format before it’s JWT encoded:

```
{ 
"url": "articleUrl",  
"articleId": "articleId",  
"type": "livecomments",  
"title": "articleTitle" 
}
```

