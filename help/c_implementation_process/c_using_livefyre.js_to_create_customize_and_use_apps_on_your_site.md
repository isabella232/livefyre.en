---
seo-title: Embed an App
solution: Experience Manager
title: Embed an App
uuid: 1c6ce724-ec6d-4e62-919b-849b4cd34709
index: y
internal: n
snippet: y
translate: y
---

# Embed an App

## Embed an App {#c_using_livefyre.js_to_create_customize_and_use_apps_on_your_site}
Add Livefyre Apps to your web pages using the Livefyre.js embed code structure.

This documentation is intended for a technical audience. For non-technical information about Apps, see [](c_about_apps.md#c_about_apps).

This section describes the code structure that you’ll need to include in your page template to embed Livefyre Apps on your site.

1. Create an .html file with a Livefyre placeholder.

   Create a new .html file in the text editor of your choice. Create a placeholder Livefyre ` <div>` element in which the App will be embedded.

   ```
   <html> 
      <head> </head> 
      <body> 
         <div id='livefyre'> </div> 
      </body> 
   </html>
   ```

1. Include the Livefyre.js Library.

   Then, include the Livefyre JS Library. Place the following reference in a ` <script>` element in your ` <head>` element. Then, open your page in a browser and use your browser’s web inspector to confirm that Livefyre is loaded.

   ```
   <head> 
      <script src='@{livefyre_js}'></script> 
   </head> 
   
   ```

1. Construct the Livefyre App.

   Use Livefyre.require to construct both Core and SDK Apps by passing in the Livefyre package(s) you plan to use.

    1. Build a Core App.

       To build a Core App (Comments, Live Blog, or Chat), use the following structure:
    
       ```
       Livefyre.require(['fyre.conv#@{fyre_conv_version_prod}'], function(Conv) { 
            new Conv(networkConfig, [convConfig], function(widget) {});  
       });  
       
       ```

    1. Build an SDK App.

       To build an SDK App such as Media Wall or Feed, use the following structure:
    
       ```
              Livefyre.require(['app#{version_number}'], 
          function (App, SDK) { 
             var app = new App({ 
             el: document.getElementById('app'), 
          }); 
          var collection = new SDK.Collection({ 
             network: "labs.fyre.co", 
             environment: "livefyre.com", 
             siteId: "315833", 
             articleId: 'livefyre-tweets' 
          }); 
          collection.pipe(feed); 
       }); 
       
       ```
       See [](c_about_apps.md#c_about_apps) for more information on specific Apps. It is recommended that you pin to the latest major version of the package (which can be found through [ Livefyre.require ](https://cdn.livefyre.com/packages.html)), to avoid unexpected broken integrations.


Next: Add authentication to your site to enable your users to post comments.
